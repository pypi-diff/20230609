# Comparing `tmp/sqlite_dataset-0.3.0.tar.gz` & `tmp/sqlite_dataset-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_dataset-0.3.0.tar", max compression
+gzip compressed data, was "sqlite_dataset-0.4.0.tar", max compression
```

## Comparing `sqlite_dataset-0.3.0.tar` & `sqlite_dataset-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1089 2023-03-27 15:03:36.310226 sqlite_dataset-0.3.0/LICENSE
--rw-r--r--   0        0        0      465 2023-03-27 15:30:03.123496 sqlite_dataset-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4353 2023-03-27 14:49:17.613963 sqlite_dataset-0.3.0/README.md
--rw-r--r--   0        0        0       35 2023-03-27 11:15:18.536322 sqlite_dataset-0.3.0/sqlite_dataset/__init__.py
--rw-r--r--   0        0        0     4215 2023-03-27 14:07:57.540847 sqlite_dataset-0.3.0/sqlite_dataset/dataset.py
--rw-r--r--   0        0        0     1296 2023-03-27 14:47:49.612007 sqlite_dataset-0.3.0/sqlite_dataset/test.py
--rw-r--r--   0        0        0      308 2023-03-27 09:27:16.270611 sqlite_dataset-0.3.0/sqlite_dataset/utils.py
--rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 sqlite_dataset-0.3.0/setup.py
--rw-r--r--   0        0        0     4951 1970-01-01 00:00:00.000000 sqlite_dataset-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-09 11:39:25.599908 sqlite_dataset-0.4.0/LICENSE
+-rw-r--r--   0        0        0      528 2023-06-09 15:07:34.828133 sqlite_dataset-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5374 2023-06-09 15:11:27.339707 sqlite_dataset-0.4.0/README.md
+-rw-r--r--   0        0        0       89 2023-06-09 13:45:27.347401 sqlite_dataset-0.4.0/sqlite_dataset/__init__.py
+-rw-r--r--   0        0        0     5064 2023-06-09 14:52:12.604865 sqlite_dataset-0.4.0/sqlite_dataset/dataset.py
+-rw-r--r--   0        0        0      440 2023-06-09 13:34:22.954170 sqlite_dataset-0.4.0/sqlite_dataset/fields.py
+-rw-r--r--   0        0        0     1471 2023-06-09 13:45:56.787610 sqlite_dataset-0.4.0/sqlite_dataset/test.py
+-rw-r--r--   0        0        0      308 2023-03-27 09:27:16.270611 sqlite_dataset-0.4.0/sqlite_dataset/utils.py
+-rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 sqlite_dataset-0.4.0/setup.py
+-rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 sqlite_dataset-0.4.0/PKG-INFO
```

### Comparing `sqlite_dataset-0.3.0/LICENSE` & `sqlite_dataset-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_dataset-0.3.0/sqlite_dataset/dataset.py` & `sqlite_dataset-0.4.0/sqlite_dataset/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,86 @@
-import os.path
+import inspect
+import os
 import warnings
+from collections import OrderedDict
 
 from sqlalchemy import MetaData, Table, insert, Column, select, text
 
+from sqlite_dataset.fields import Field
 from sqlite_dataset.utils import create_sqlite_db_engine
 
 
-class SQLiteDataset(object):
-    schema = None
+def _get_fields_by_mro(klass):
+    mro = inspect.getmro(klass)
+    return sum(
+        (
+            _get_fields(
+                getattr(base, "_declared_fields", base.__dict__)
+            )
+            for base in mro[:0:-1]
+        ),
+        [],
+    )
+
+
+def is_field_class(val):
+    try:
+        return issubclass(val, Field)
+    except TypeError:
+        return isinstance(val, Field)
+
+
+def _get_fields(attrs):
+    fields = [
+        (field_name, field_value)
+        for field_name, field_value in attrs.items()
+        if is_field_class(field_value)
+    ]
+    return fields
+
+
+class DatasetMeta(type):
+
+    def __new__(mcs, name, bases, attrs):
+        cls_fields = _get_fields(attrs)
+        for field_name, _ in cls_fields:
+            del attrs[field_name]
+        klass = super().__new__(mcs, name, bases, attrs)
+        inherited_fields = _get_fields_by_mro(klass)
+        klass._declared_fields = mcs.get_declared_fields(
+            cls_fields=cls_fields,
+            inherited_fields=inherited_fields,
+        )
+        return klass
 
     @classmethod
-    def create(cls, db_path, schema=None):
-        if cls.schema is None and schema is None:
-            raise ValueError(
-                'Schema not found. To create a dataset, either override the schema field or pass in a schema when '
-                'calling create(db_path, schema=schema). To load an existing dataset without specifying schema, '
-                'or create an empty dataset to use with pandas, instantiate SQLiteDataset(db_path) directly.'
-            )
-        db = cls(db_path, schema=schema)
-        db.build()
-        return db
+    def get_declared_fields(
+            mcs,
+            cls_fields: list,
+            inherited_fields: list
+    ):
+        return OrderedDict(inherited_fields + cls_fields)
+
 
-    def __init__(self, db_path, schema=None):
+class SQLiteDataset(object, metaclass=DatasetMeta):
+
+    def __init__(self, db_path):
         self.db_path = db_path
         self.engine = create_sqlite_db_engine(db_path)
         self.metadata = MetaData()
-        if schema is not None:
-            self.schema = schema
-        if self.schema is not None:
+        self.schema = {}
+
+        if self._declared_fields:
+            for name, field in self._declared_fields.items():
+                if not self.schema.get(field.tablename):
+                    self.schema[field.tablename] = []
+                self.schema[field.tablename].append(field.new_column(name=name))
             self.add_tables(self.schema)
-        elif not os.path.exists(self.db_path):
-            warnings.warn(
-                'Database file does not exist. To to create a dataset, call create(db_path). '
-                'Refer to documentation for more details.'
-            )
+            if not os.path.exists(self.db_path):
+                self.build()
         else:
             self.reflect()
         self.db_connection = None
 
     @property
     def connection(self):
         if self.db_connection is None:
@@ -102,15 +145,15 @@
 
     def read_data(self, table, return_tuple=False, cols=None, chunk=None, limit=None):
         if cols:
             stmt = select(*[self.get_column(table, col) for col in cols])
         else:
             stmt = select(self.get_table(table))
         if type(limit) == int and limit > 0:
-            stmt.limit(limit)
+            stmt = stmt.limit(limit)
 
         if chunk:
             def iterator(chk, itr, rt=False):
                 while data := itr.fetchmany(chk):
                     if rt:
                         yield [r.tuple() for r in data]
                     else:
```

### Comparing `sqlite_dataset-0.3.0/sqlite_dataset/test.py` & `sqlite_dataset-0.4.0/sqlite_dataset/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 import pandas as pd
-from sqlalchemy import Column, String, Float
-#
-from sqlite_dataset import SQLiteDataset
-#
-#
-class MyIrisDataset(SQLiteDataset):
-    schema = {
-        'iris': [
-            Column('sepal_length_cm', String),
-            Column('sepal_width_cm', Float),
-            Column('petal_length_cm', Float),
-            Column('petal_width_cm', Float),
-            Column('class', String),
-        ]
+
+from sqlite_dataset import SQLiteDataset, Field, String, Float
+
+
+class MyBaseIrisDataset(SQLiteDataset):
+    text = Field(String, tablename='sentence')
+    sepal_length_cm = Field(String, tablename='iris')
+
+
+class MyIrisDataset(MyBaseIrisDataset):
+    sepal_width_cm = Field(Float, tablename='iris')
+    petal_length_cm = Field(Float, tablename='iris')
+    petal_width_cm = Field(Float, tablename='iris')
+    class_field = Field(String, name='class', tablename='iris')
+
+data = [
+    {
+        'sepal_length_cm': '5.1',
+        'sepal_width_cm': '3.5',
+        'petal_length_cm': '1.4',
+        'petal_width_cm': '0.2',
+        'class': 'setosa'
+    },
+    {
+        'sepal_length_cm': '4.9',
+        'sepal_width_cm': '3.0',
+        'petal_length_cm': '1.4',
+        'petal_width_cm': '0.2',
+        'class': 'setosa'
     }
-#
-# # ds = MyIrisDataset.create('iris.db')
-#
-# data = [
-#     {
-#         'sepal_length_cm': '5.1',
-#         'sepal_width_cm': '3.5',
-#         'petal_length_cm': '1.4',
-#         'petal_width_cm': '0.2',
-#         'class': 'setosa'
-#     },
-#     {
-#         'sepal_length_cm': '4.9',
-#         'sepal_width_cm': '3.0',
-#         'petal_length_cm': '1.4',
-#         'petal_width_cm': '0.2',
-#         'class': 'setosa'
-#     }
-# ]
-#
-# with MyIrisDataset('iris.db') as ds:
-#     # ds.insert_data('iris', data)
-#     res = ds.read_data('iris')
-#     print(res)
+]
 
-import seaborn as sns
+with MyIrisDataset('iris.db') as ds:
+    ds.insert_data('iris', data)
+    # res = ds.read_data('iris')
+    # print(res)
+
+with MyIrisDataset('iris11.db') as ds:
+    ds.insert_data('iris', data)
 
-df = sns.load_dataset('iris')
-with SQLiteDataset('iris11.db') as ds:
-    # df.to_sql('iris', ds.connection)
-    # ds.connection.commit()
-    res = pd.read_sql(
-        ds.get_table('iris').select(),
-        ds.connection
-    )
+with MyIrisDataset('iris.db') as ds:
+    res = ds.read_data('iris')
     print(res)
+
+import seaborn as sns
+
+# df = sns.load_dataset('iris')
+# with MyIrisDataset('iris11.db') as ds:
+#     df.to_sql('iris', ds.connection)
+#     ds.connection.commit()
+#     # res = pd.read_sql(
+#     #     ds.get_table('iris').select(),
+#     #     ds.connection
+#     # )
+#     # print(res)
```

### Comparing `sqlite_dataset-0.3.0/setup.py` & `sqlite_dataset-0.4.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['sqlite_dataset']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['sqlalchemy>=2.0,<3.0']
+['sqlalchemy>=1.3.0']
 
 setup_kwargs = {
     'name': 'sqlite-dataset',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Use SQLite database to store datasets.',
-    'long_description': "# SQLite Dataset\n\nUse [SQLite](https://sqlite.org/index.html) database to store datasets. Based on [SQLAlchemy core](https://docs.sqlalchemy.org/en/20/core/).\n\n## Structure\n\nThe core of sqlite-dataset is the Class **SQLiteDataset**, which wraps a SQLAlchemy connection to a SQLite database.\n\n## Usage\n\n### Create a new dataset\n\nA **schema** is required to create a new dataset. The **schema** should be a dictionary where each item is a column.\n\nThere are two ways to specify the schema:\n\n1. Extend the base **SQLiteDataset** class and override the **schema** field.\n\n```python\nfrom sqlite_dataset import SQLiteDataset\nfrom sqlalchemy import Column, String, Float\n\nclass MyIrisDataset(SQLiteDataset):\n    schema = {\n        'iris': [\n            Column('sepal_length_cm', String),\n            Column('sepal_width_cm', Float),\n            Column('petal_length_cm', Float),\n            Column('petal_width_cm', Float),\n            Column('class', String),\n        ]\n    }\n\nds = MyIrisDataset.create('test.db')\n```\n\n2. Pass schema to `SQLiteDataset.create()`\n\n```python\nschema = {\n    'iris': [\n        Column('sepal_length_cm', String),\n        Column('sepal_width_cm', Float),\n        Column('petal_length_cm', Float),\n        Column('petal_width_cm', Float),\n        Column('class', String),\n    ]\n}\nds = SQLiteDataset.create('test.db', schema=schema)\n```\n\nBe aware that the schema passed to `SQLiteDataset.create()` will override the class field schema.\n\n### Connect to an existing dataset\n\nAn existing dataset could be one created by calling `SQLiteDataset.create()` as shown above, or could be any SQLite database file.\n\nTo connect to a dataset, call the `connect()` method and `close()` after complete all tasks.\n\n```python\nds = SQLiteDataset('test.db')\nds.connect()\n# do something\nds.close()\n```\n\nOr the dataset can be used as a context manager\n\n```python\nwith SQLiteDataset('test.db') as ds:\n    # do something\n    pass\n```\n\n### Schema for existing dataset\n\n**SQLiteDataset** object uses SQLAlchemy connection under the hood, soa schema is required to make any database queries or operations.\n\nThe way to specify schema for an existing dataset is similar to *create a new dataset*.\n\nIf it's a class extending the base SQLiteDataset class, and overrides the schema field, then this schema will be used.\n\n```python\nwith MyIrisDataset('test.db') as ds:\n    pass\n```\n\nOr a schema can be passed into the class constructor. The schema passed into the constructor will always override the class field schema.\n\n```python\nwith MyIrisDataset('test.db', schema=schema) as ds:\n    pass\n\nwith SQLiteDataset('test.db', schema=schema) as ds:\n    pass\n```\n\nIf no schema provided by either of the above, a [SQLAlchemy **reflection**](https://docs.sqlalchemy.org/en/13/core/reflection.html) is performed to load and parse schema from the existing database.\n\n```python\nwith SQLiteDataset('test.db') as ds:\n    pass\n```\n\nIt is recommended to explicitly define the schema as **reflection** may have performance issue in some cases if the schema is very large and complex.\n\n## Add and read data\n\n```python\ndata = [\n    {\n        'sepal_length_cm': '5.1',\n        'sepal_width_cm': '3.5',\n        'petal_length_cm': '1.4',\n        'petal_width_cm': '0.2',\n        'class': 'setosa'\n    },\n    {\n        'sepal_length_cm': '4.9',\n        'sepal_width_cm': '3.0',\n        'petal_length_cm': '1.4',\n        'petal_width_cm': '0.2',\n        'class': 'setosa'\n    }\n]\n\nwith MyIrisDataset('test.db') as ds:\n    ds.insert_data('iris', data)\n```\n\n```python\nwith MyIrisDataset('test.db') as ds:\n    res = ds.read_data('iris')\n```\n\n\n### Use with pandas\n\nA pandas DataFrame can be inserted into a dataset by utilizing the `to_sql()` function, and read from the dataset using `read_sql` function.\n\nBe aware that in this case, `SQLiteDataset()` should be used without specifying the schema.\n\n```python\nimport seaborn as sns\nimport pandas as pd\n\ndf = sns.load_dataset('iris')\nwith SQLiteDataset('iris11.db') as ds:\n    df.to_sql('iris', ds.connection)\n    ds.connection.commit()\n```\n\n```python\nwith SQLiteDataset('iris11.db') as ds:\n    res = pd.read_sql(\n        ds.get_table('iris').select(),\n        ds.connection\n    )\n```",
+    'long_description': "# SQLite Dataset\n\nUse [SQLite](https://sqlite.org/index.html) database to store datasets. Based on [SQLAlchemy core](https://docs.sqlalchemy.org/en/20/core/).\n\n## Structure\n\nThe core of sqlite-dataset is the Class **SQLiteDataset**, which wraps a SQLAlchemy connection to a SQLite database.\n\n## Usage\n\n### Declare a dataset\n\nTo declare a dataset, extend the base **SQLiteDataset** class and specify fields.\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String, Float\n\nclass MyIrisDataset(SQLiteDataset):\n    \n    sepal_length_cm = Field(String, tablename='iris')\n    sepal_width_cm = Field(Float, tablename='iris')\n    petal_length_cm = Field(Float, tablename='iris')\n    petal_width_cm = Field(Float, tablename='iris')\n    class_field = Field(String, tablename='iris', name='class')\n\nds = MyIrisDataset('my_iris_dataset.db')\n```\n\nThis will create a sqlite database file on the specified path. If a dataset already exists, it will then be loaded. \n\n#### The *Field* object\n\n`Field` can be seen as a factory that can create a SQLAlchemy's Column object.\n\nThe `Field` object's constructor takes same arguments as `sqlalchemy.schema.Column` with the difference that `Field` does not take positional name argument and has an extra keyword argument `tablename`.\n\nDeclare a Column using sqlalchemy.Column:\n\n```python\nfrom sqlalchemy import Column, String\n\nColumn('sepal_length_cm', String)\nColumn(name='sepal_length_cm', type_=String)\n```\n\nDeclare a sqlite_dataset.Field:\n\n```python\nfrom sqlite_dataset import Field, String\n\nsepal_length_cm = Field(String)\n```\n\nThe variable name will be automatically used as the column name.\n\nColumn name can also be specified using `name` argument, which is useful if the column name is a Python preserved keyword:\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String\n\nclass MyDataset(SQLiteDataset):\n    class_field = Field(String, name='class')\n    type_field = Field(String, name='type')\n```\n\nTable name can be specified using `tablename` keyword argument:\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String\n\nclass MyDataset(SQLiteDataset):\n    class_field = Field(String, name='class', tablename='table1')\n    type_field = Field(String, name='type', tablename='table2')\n```\n\nThis will create two tables: table1, table2.\n\nIf tablename is not specified, the column will be created in default table **data**. \n\n#### Field type and keyword arguments\n\nThe field type is the sqlalchemy column type. All sqlalchemy members were imported into sqlite_dataset.\n\n```python\nfrom sqlalchemy import String, Integer\n```\n\nis exactly the same as:\n\n```python\nfrom sqlite_dataset import String, Integer\n```\n\n### Inheritance\n\nDataset can be inherited.\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String, Float\n\nclass BaseDataset(SQLiteDataset):\n    class_field = Field(String, tablename='iris', name='class')\n    example_field = Field(String, tablename='example_table')\n\nclass ChildDataset(BaseDataset): \n    sepal_length_cm = Field(String, tablename='iris')\n    sepal_width_cm = Field(Float, tablename='iris')\n    petal_length_cm = Field(Float, tablename='iris')\n    petal_width_cm = Field(Float, tablename='iris')\n```\n\n### Connect to an existing dataset\n\nTo connect to a dataset, call the `connect()` method. Call `close()` to close it.\n\n```python\nds = SQLiteDataset('test.db')\nds.connect()\n# do something\nds.close()\n```\n\nOr the dataset can be used as a context manager\n\n```python\nwith SQLiteDataset('test.db') as ds:\n    # do something\n    pass\n```\n\n### Schema for existing dataset\n\n**SQLiteDataset** object uses SQLAlchemy connection under the hood, so a schema is required to make any database queries or operations.\n\nIf no schema provided by either of the above, a [SQLAlchemy **reflection**](https://docs.sqlalchemy.org/en/13/core/reflection.html) is performed to load and parse schema from the existing database.\n\nIt is recommended to explicitly define the schema as **reflection** may have performance issue in some cases if the schema is very large and complex.\n\n## Add and read data\n\n```python\ndata = [\n    {\n        'sepal_length_cm': '5.1',\n        'sepal_width_cm': '3.5',\n        'petal_length_cm': '1.4',\n        'petal_width_cm': '0.2',\n        'class': 'setosa'\n    },\n    {\n        'sepal_length_cm': '4.9',\n        'sepal_width_cm': '3.0',\n        'petal_length_cm': '1.4',\n        'petal_width_cm': '0.2',\n        'class': 'setosa'\n    }\n]\n\nwith MyIrisDataset('test.db') as ds:\n    ds.insert_data('iris', data)\n```\n\n```python\nwith MyIrisDataset('test.db') as ds:\n    res = ds.read_data('iris')\n```\n\n\n### Use with pandas\n\nA pandas DataFrame can be inserted into a dataset by utilizing the `to_sql()` function, and read from the dataset using `read_sql` function.\n\nBe aware that in this case, `SQLiteDataset()` should be used without specifying the schema.\n\n```python\nimport seaborn as sns\nimport pandas as pd\n\ndf = sns.load_dataset('iris')\nwith SQLiteDataset('iris11.db') as ds:\n    df.to_sql('iris', ds.connection)\n    ds.connection.commit()\n```\n\n```python\nwith SQLiteDataset('iris11.db') as ds:\n    res = pd.read_sql(\n        ds.get_table('iris').select(),\n        ds.connection\n    )\n```",
     'author': 'Jinshuai Ma',
     'author_email': 'mayazureee@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Mayazure/sqlite-dataset',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sqlite_dataset-0.3.0/PKG-INFO` & `sqlite_dataset-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,163 @@
 Metadata-Version: 2.1
 Name: sqlite-dataset
-Version: 0.3.0
+Version: 0.4.0
 Summary: Use SQLite database to store datasets.
 Home-page: https://github.com/Mayazure/sqlite-dataset
 License: MIT
 Author: Jinshuai Ma
 Author-email: mayazureee@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sqlalchemy (>=2.0,<3.0)
+Requires-Dist: sqlalchemy (>=1.3.0)
 Project-URL: Repository, https://github.com/Mayazure/sqlite-dataset
 Description-Content-Type: text/markdown
 
 # SQLite Dataset
 
 Use [SQLite](https://sqlite.org/index.html) database to store datasets. Based on [SQLAlchemy core](https://docs.sqlalchemy.org/en/20/core/).
 
 ## Structure
 
 The core of sqlite-dataset is the Class **SQLiteDataset**, which wraps a SQLAlchemy connection to a SQLite database.
 
 ## Usage
 
-### Create a new dataset
+### Declare a dataset
 
-A **schema** is required to create a new dataset. The **schema** should be a dictionary where each item is a column.
+To declare a dataset, extend the base **SQLiteDataset** class and specify fields.
 
-There are two ways to specify the schema:
+```python
+from sqlite_dataset import SQLiteDataset, Field, String, Float
+
+class MyIrisDataset(SQLiteDataset):
+    
+    sepal_length_cm = Field(String, tablename='iris')
+    sepal_width_cm = Field(Float, tablename='iris')
+    petal_length_cm = Field(Float, tablename='iris')
+    petal_width_cm = Field(Float, tablename='iris')
+    class_field = Field(String, tablename='iris', name='class')
+
+ds = MyIrisDataset('my_iris_dataset.db')
+```
+
+This will create a sqlite database file on the specified path. If a dataset already exists, it will then be loaded. 
+
+#### The *Field* object
 
-1. Extend the base **SQLiteDataset** class and override the **schema** field.
+`Field` can be seen as a factory that can create a SQLAlchemy's Column object.
+
+The `Field` object's constructor takes same arguments as `sqlalchemy.schema.Column` with the difference that `Field` does not take positional name argument and has an extra keyword argument `tablename`.
+
+Declare a Column using sqlalchemy.Column:
 
 ```python
-from sqlite_dataset import SQLiteDataset
-from sqlalchemy import Column, String, Float
+from sqlalchemy import Column, String
 
-class MyIrisDataset(SQLiteDataset):
-    schema = {
-        'iris': [
-            Column('sepal_length_cm', String),
-            Column('sepal_width_cm', Float),
-            Column('petal_length_cm', Float),
-            Column('petal_width_cm', Float),
-            Column('class', String),
-        ]
-    }
-
-ds = MyIrisDataset.create('test.db')
-```
-
-2. Pass schema to `SQLiteDataset.create()`
-
-```python
-schema = {
-    'iris': [
-        Column('sepal_length_cm', String),
-        Column('sepal_width_cm', Float),
-        Column('petal_length_cm', Float),
-        Column('petal_width_cm', Float),
-        Column('class', String),
-    ]
-}
-ds = SQLiteDataset.create('test.db', schema=schema)
+Column('sepal_length_cm', String)
+Column(name='sepal_length_cm', type_=String)
 ```
 
-Be aware that the schema passed to `SQLiteDataset.create()` will override the class field schema.
+Declare a sqlite_dataset.Field:
 
-### Connect to an existing dataset
+```python
+from sqlite_dataset import Field, String
+
+sepal_length_cm = Field(String)
+```
 
-An existing dataset could be one created by calling `SQLiteDataset.create()` as shown above, or could be any SQLite database file.
+The variable name will be automatically used as the column name.
 
-To connect to a dataset, call the `connect()` method and `close()` after complete all tasks.
+Column name can also be specified using `name` argument, which is useful if the column name is a Python preserved keyword:
 
 ```python
-ds = SQLiteDataset('test.db')
-ds.connect()
-# do something
-ds.close()
+from sqlite_dataset import SQLiteDataset, Field, String
+
+class MyDataset(SQLiteDataset):
+    class_field = Field(String, name='class')
+    type_field = Field(String, name='type')
 ```
 
-Or the dataset can be used as a context manager
+Table name can be specified using `tablename` keyword argument:
 
 ```python
-with SQLiteDataset('test.db') as ds:
-    # do something
-    pass
+from sqlite_dataset import SQLiteDataset, Field, String
+
+class MyDataset(SQLiteDataset):
+    class_field = Field(String, name='class', tablename='table1')
+    type_field = Field(String, name='type', tablename='table2')
 ```
 
-### Schema for existing dataset
+This will create two tables: table1, table2.
 
-**SQLiteDataset** object uses SQLAlchemy connection under the hood, soa schema is required to make any database queries or operations.
+If tablename is not specified, the column will be created in default table **data**. 
 
-The way to specify schema for an existing dataset is similar to *create a new dataset*.
+#### Field type and keyword arguments
 
-If it's a class extending the base SQLiteDataset class, and overrides the schema field, then this schema will be used.
+The field type is the sqlalchemy column type. All sqlalchemy members were imported into sqlite_dataset.
 
 ```python
-with MyIrisDataset('test.db') as ds:
-    pass
+from sqlalchemy import String, Integer
 ```
 
-Or a schema can be passed into the class constructor. The schema passed into the constructor will always override the class field schema.
+is exactly the same as:
 
 ```python
-with MyIrisDataset('test.db', schema=schema) as ds:
-    pass
+from sqlite_dataset import String, Integer
+```
 
-with SQLiteDataset('test.db', schema=schema) as ds:
-    pass
+### Inheritance
+
+Dataset can be inherited.
+
+```python
+from sqlite_dataset import SQLiteDataset, Field, String, Float
+
+class BaseDataset(SQLiteDataset):
+    class_field = Field(String, tablename='iris', name='class')
+    example_field = Field(String, tablename='example_table')
+
+class ChildDataset(BaseDataset): 
+    sepal_length_cm = Field(String, tablename='iris')
+    sepal_width_cm = Field(Float, tablename='iris')
+    petal_length_cm = Field(Float, tablename='iris')
+    petal_width_cm = Field(Float, tablename='iris')
 ```
 
-If no schema provided by either of the above, a [SQLAlchemy **reflection**](https://docs.sqlalchemy.org/en/13/core/reflection.html) is performed to load and parse schema from the existing database.
+### Connect to an existing dataset
+
+To connect to a dataset, call the `connect()` method. Call `close()` to close it.
+
+```python
+ds = SQLiteDataset('test.db')
+ds.connect()
+# do something
+ds.close()
+```
+
+Or the dataset can be used as a context manager
 
 ```python
 with SQLiteDataset('test.db') as ds:
+    # do something
     pass
 ```
 
+### Schema for existing dataset
+
+**SQLiteDataset** object uses SQLAlchemy connection under the hood, so a schema is required to make any database queries or operations.
+
+If no schema provided by either of the above, a [SQLAlchemy **reflection**](https://docs.sqlalchemy.org/en/13/core/reflection.html) is performed to load and parse schema from the existing database.
+
 It is recommended to explicitly define the schema as **reflection** may have performance issue in some cases if the schema is very large and complex.
 
 ## Add and read data
 
 ```python
 data = [
     {
```

