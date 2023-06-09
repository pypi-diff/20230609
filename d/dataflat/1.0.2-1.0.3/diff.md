# Comparing `tmp/dataflat-1.0.2.tar.gz` & `tmp/dataflat-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflat-1.0.2.tar", last modified: Fri Jun  9 17:07:20 2023, max compression
+gzip compressed data, was "dataflat-1.0.3.tar", last modified: Fri Jun  9 18:47:54 2023, max compression
```

## Comparing `dataflat-1.0.2.tar` & `dataflat-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 17:07:01.000000 dataflat-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 17:07:20.704804 dataflat-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 17:07:01.000000 dataflat-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.700804 dataflat-1.0.2/dataflat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/dictionary/flattener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/flattener_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat/pandas_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/pandas_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/pandas_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat/spark_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/spark_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/spark_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:07:20.704804 dataflat-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-09 17:07:01.000000 dataflat-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:54.072298 dataflat-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 18:47:42.000000 dataflat-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 18:47:54.072298 dataflat-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 18:47:42.000000 dataflat-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:54.068298 dataflat-1.0.3/dataflat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:54.072298 dataflat-1.0.3/dataflat/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/dictionary/flattener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/flattener_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:54.072298 dataflat-1.0.3/dataflat/pandas_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/pandas_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/pandas_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:54.072298 dataflat-1.0.3/dataflat/spark_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/spark_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-09 18:47:42.000000 dataflat-1.0.3/dataflat/spark_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:47:54.068298 dataflat-1.0.3/dataflat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 18:47:54.000000 dataflat-1.0.3/dataflat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 18:47:54.000000 dataflat-1.0.3/dataflat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:47:54.000000 dataflat-1.0.3/dataflat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 18:47:54.000000 dataflat-1.0.3/dataflat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 18:47:54.000000 dataflat-1.0.3/dataflat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:47:54.072298 dataflat-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-09 18:47:42.000000 dataflat-1.0.3/setup.py
```

### Comparing `dataflat-1.0.2/LICENSE` & `dataflat-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/PKG-INFO` & `dataflat-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dataflat-1.0.2/README.md` & `dataflat-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/dataflat/commons.py` & `dataflat-1.0.3/dataflat/commons.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/dataflat/dictionary/flattener.py` & `dataflat-1.0.3/dataflat/dictionary/flattener.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/dataflat/exceptions.py` & `dataflat-1.0.3/dataflat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/dataflat/flattener_handler.py` & `dataflat-1.0.3/dataflat/flattener_handler.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/dataflat/pandas_df/flattener.py` & `dataflat-1.0.3/dataflat/pandas_df/flattener.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.2/dataflat/spark_df/flattener.py` & `dataflat-1.0.3/dataflat/spark_df/flattener.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 logger = init_logger(__name__)
 
 @typechecked
 class CustomFlattener():
     def __init__(self):
         logger.info("CustomFlattener for PySpark Dataframes has been initiated")
 
-    def _to_snake_case(process_col:bool, col_name:str):
+    def _to_snake_case(self, process_col:bool, col_name:str):
         if process_col:
             pattern = re.compile(r'(?<!^)(?=[A-Z])')
             return pattern.sub('_', col_name).lower().replace("__", "_").replace("._", ".")
         return col_name
     
-    def _replace_dots(process_col:bool, col_name:str):
+    def _replace_dots(self, process_col:bool, col_name:str):
         if process_col:
             return col_name.replace(".", "_")
         return col_name
 
     def _process_column_name(self, dataframe:DataFrame, to_snake_case:bool, replace_dots:bool):
         """Receive a Spark Dataframe and return a snake_case columns like dataframe.
         If replace_dots is True, then all the subcolumns like "Column.SubColumn" will be
@@ -61,15 +61,16 @@
         Returns
         -------
         dataframe: pyspark.Dataframe
         """
         for col in dataframe.columns:
             sc_col = self._to_snake_case(to_snake_case, col)
             sc_col = self._replace_dots(replace_dots, sc_col)
-            dataframe = dataframe.withColumnRenamed(col, sc_col)
+            if to_snake_case | replace_dots:
+                dataframe = dataframe.withColumnRenamed(col, sc_col)
         return dataframe
 
     def _get_schema_struct(self, dataframe_schema:dict, id_key:str, black_list:List[str], dataframe_name:str, _ref:str = "", named_struct:dict = {}):
         """Receive Spark Dataframe Schema in dictionary format, and return 
         a dictionary[str, str] with the all required named_struct expressions
         to flatten de Dataframe.
 
@@ -133,15 +134,15 @@
         processed_data : dict[str, pyspark.DataFrame]
             A dictionary with all the resulting Dataframes from the flattening process.
             Each ArrayType column will be flattened and added as a Dataframe inside the
             processed_data return.
         """
         processed_data = {}
         schema = json.loads(dataframe.schema.json())
-        ns = self._get_schema_struct(schema, id_key, black_list, dataframe_name, ns={})
+        ns = self._get_schema_struct(schema, id_key, black_list, dataframe_name, _ref="", named_struct={})
         for df_name, struct in ns.items():
             selectExpr = f"named_struct( {struct[:-1]} ) as Item"
             aux_df = dataframe.selectExpr( selectExpr ).select("Item.*")
             if df_name != dataframe_name:
                 expld_col = aux_df.columns[1]
                 expld_expr = expld_col if "." not in expld_col else f"`{expld_col}`"
                 aux_df = aux_df.select(id_key, posexplode(expld_expr).alias('pos', expld_col))
```

### Comparing `dataflat-1.0.2/dataflat.egg-info/PKG-INFO` & `dataflat-1.0.3/dataflat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dataflat-1.0.2/setup.py` & `dataflat-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 PATH = path.abspath(path.dirname(__file__))
 
 with open(path.join(PATH, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
  
 setuptools.setup(
     name="dataflat",
-    version="1.0.2",
+    version="1.0.3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/JuanARojasA/dataflat',
     author="Juan Rojas",
     author_email="jarojasa97@gmail.com",
     license='Apache License 2.0',
     platforms='any',
```

