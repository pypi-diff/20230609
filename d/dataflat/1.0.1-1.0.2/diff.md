# Comparing `tmp/dataflat-1.0.1.tar.gz` & `tmp/dataflat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflat-1.0.1.tar", last modified: Thu Mar 23 05:12:06 2023, max compression
+gzip compressed data, was "dataflat-1.0.2.tar", last modified: Fri Jun  9 17:07:20 2023, max compression
```

## Comparing `dataflat-1.0.1.tar` & `dataflat-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:12:06.695997 dataflat-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-23 05:11:49.000000 dataflat-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-23 05:12:06.691997 dataflat-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-23 05:11:49.000000 dataflat-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:12:06.691997 dataflat-1.0.1/dataflat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:12:06.691997 dataflat-1.0.1/dataflat/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/dictionary/flattener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/flattener_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:12:06.691997 dataflat-1.0.1/dataflat/pandas_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/pandas_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/pandas_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:12:06.691997 dataflat-1.0.1/dataflat/spark_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/spark_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-03-23 05:11:49.000000 dataflat-1.0.1/dataflat/spark_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 05:12:06.691997 dataflat-1.0.1/dataflat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-23 05:12:06.000000 dataflat-1.0.1/dataflat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-23 05:12:06.000000 dataflat-1.0.1/dataflat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 05:12:06.000000 dataflat-1.0.1/dataflat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 05:12:06.000000 dataflat-1.0.1/dataflat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 05:12:06.000000 dataflat-1.0.1/dataflat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 05:12:06.695997 dataflat-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-23 05:11:49.000000 dataflat-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 17:07:01.000000 dataflat-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 17:07:20.704804 dataflat-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 17:07:01.000000 dataflat-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.700804 dataflat-1.0.2/dataflat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/dictionary/flattener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/flattener_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat/pandas_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/pandas_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/pandas_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat/spark_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/spark_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-09 17:07:01.000000 dataflat-1.0.2/dataflat/spark_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:07:20.704804 dataflat-1.0.2/dataflat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 17:07:20.000000 dataflat-1.0.2/dataflat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:07:20.704804 dataflat-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-09 17:07:01.000000 dataflat-1.0.2/setup.py
```

### Comparing `dataflat-1.0.1/LICENSE` & `dataflat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.1/PKG-INFO` & `dataflat-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -39,24 +39,26 @@
 
 id_key = 'id'
 black_list = ['keys','or','columns','to','skip']
 
 #The following variables have the default values for each transform function
 to_snake_case = False
 replace_dots = False
-dict_name = 'dct'
-chunk_size = 500
-dataframe_name = 'df'
 
 # Instantiate a Dictionary Flattener
+dict_name = 'dct'
 flattener_dict = Flattener().handler(Options.DICTIONARY)
-flattener.transform(dictionary, id_key, black_list, dict_name, to_snake_case, replace_dots)
+flattener_dict.transform(dictionary, id_key, black_list, dict_name, to_snake_case, replace_dots)
 
 
 # Instantiate a Pandas Dataframe Flattener
+##Default chunk size = 500
+dataframe_name = 'df'
+chunk_size = 500
 flattener_pd = Flattener().handler(Options.PANDAS_DF)
-transform(dataframe, id_key, black_list, dataframe_name, chunk_size, to_snake_case, replace_dots)
+flattener_pd.transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots, chunk_size)
 
 # Instantiate a Spark Dataframe Flattener
+dataframe_name = 'df'
 flattener_sp = Flattener().handler(Options.SPARK_DF)
-transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots)
+flattener_sp.transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots)
 ```
```

### Comparing `dataflat-1.0.1/README.md` & `dataflat-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 
 id_key = 'id'
 black_list = ['keys','or','columns','to','skip']
 
 #The following variables have the default values for each transform function
 to_snake_case = False
 replace_dots = False
-dict_name = 'dct'
-chunk_size = 500
-dataframe_name = 'df'
 
 # Instantiate a Dictionary Flattener
+dict_name = 'dct'
 flattener_dict = Flattener().handler(Options.DICTIONARY)
-flattener.transform(dictionary, id_key, black_list, dict_name, to_snake_case, replace_dots)
+flattener_dict.transform(dictionary, id_key, black_list, dict_name, to_snake_case, replace_dots)
 
 
 # Instantiate a Pandas Dataframe Flattener
+##Default chunk size = 500
+dataframe_name = 'df'
+chunk_size = 500
 flattener_pd = Flattener().handler(Options.PANDAS_DF)
-transform(dataframe, id_key, black_list, dataframe_name, chunk_size, to_snake_case, replace_dots)
+flattener_pd.transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots, chunk_size)
 
 # Instantiate a Spark Dataframe Flattener
+dataframe_name = 'df'
 flattener_sp = Flattener().handler(Options.SPARK_DF)
-transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots)
+flattener_sp.transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots)
 ```
```

### Comparing `dataflat-1.0.1/dataflat/commons.py` & `dataflat-1.0.2/dataflat/commons.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.1/dataflat/dictionary/flattener.py` & `dataflat-1.0.2/dataflat/dictionary/flattener.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Authors:
     Juan ROJAS <jarojasa97@gmail.com>
 '''
 
 import re
 from typeguard import typechecked
-from typing import Tuple, List, Union
+from typing import Tuple, List, Union, Any
 from dataflat.commons import init_logger
 from dataflat.exceptions import FlatteningException
 
 
 logger = init_logger(__name__)
 
 @typechecked
@@ -194,15 +194,15 @@
                                                                   super_dict_ref_id = dict_ref_id,
                                                                   processed_data = processed_data)
                 else:
                     flat_dict.update({f"{dict_ref}{key}": value})
         return flat_dict, processed_data
 
 
-    def transform(self, dictionary:dict, id_key:str, black_list:List[str] = [], dict_name:str = "dct", to_snake_case:bool = False, replace_dots:bool = False) -> dict:
+    def transform(self, dictionary:dict, id_key:Any, black_list:List[str] = [], dict_name:str = "dct", to_snake_case:bool = False, replace_dots:bool = False) -> dict:
         """Receive a dictionary to flatten and a id_key used as 
         reference key under all the resulting flattened dictionaries.
         Receive a dictionary and an id_key to start processing.
         If a black_list is provided then all the keys inside the black_list will
         be skipped. Notice that if ['name'] is provided as black list, then 
         all the 'name' keys will be skipped, even if they are under a nested
         dictionary or list.
```

### Comparing `dataflat-1.0.1/dataflat/exceptions.py` & `dataflat-1.0.2/dataflat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.1/dataflat/flattener_handler.py` & `dataflat-1.0.2/dataflat/flattener_handler.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.1/dataflat/pandas_df/flattener.py` & `dataflat-1.0.2/dataflat/pandas_df/flattener.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 @typechecked
 class CustomFlattener():
     def __init__(self):
         logger.info("CustomFlattener for Pandas Dataframes has been initiated")
 
 
-    def transform(self, dataframe:pd.DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df", chunk_size:int = 500, to_snake_case:bool = False, replace_dots:bool = False) -> dict:
+    def transform(self, dataframe:pd.DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df", to_snake_case:bool = False, replace_dots:bool = False, chunk_size:int = 500) -> dict:
         """Receive a pandas Dataframe, and return a dictionary with the
         flattenend pandas Dataframes.
         If a black_list is provided then all the column names inside the black_list will
         be skipped. Notice that if ['name'] is provided as black list, then 
         all the 'name' columns will be skipped, even if they are under a nested
         column.
         The dataframe_name will be used to reference each resulting flattened dataframe
@@ -54,22 +54,22 @@
         id_key: str
             The id key to be used as reference to the parent dataframe.
         black_list: List[str], (default [])
             A list of keys to ignore and not to add to the resulting flattened dictionary.
         dataframe_name: str, (default 'df')
             A reference name for the dataframe, used to difference each
             resulting dataframe in the processed_dataframes return.
-        chunk_size: int, (default 500)
-            The chunk size used to process the dataframe in batches. 
-            i.e. If dataframe size is 2000, and chunk_size is 500,
-            then the dataframe will be processed in 4 batches.
         to_snake_case: bool
             If True process the column name to Snake Case.
         replace_dots: bool
             If True replace the column name dots with underscores.
+        chunk_size: int, (default 500)
+            The chunk size used to process the dataframe in batches. 
+            i.e. If dataframe size is 2000, and chunk_size is 500,
+            then the dataframe will be processed in 4 batches.
 
         Returns
         -------
         processed_dicts : dict
         """
         dataframe_len = len(dataframe)
         if dataframe_len == 0:
```

### Comparing `dataflat-1.0.1/dataflat/spark_df/flattener.py` & `dataflat-1.0.2/dataflat/spark_df/flattener.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,24 @@
 logger = init_logger(__name__)
 
 @typechecked
 class CustomFlattener():
     def __init__(self):
         logger.info("CustomFlattener for PySpark Dataframes has been initiated")
 
+    def _to_snake_case(process_col:bool, col_name:str):
+        if process_col:
+            pattern = re.compile(r'(?<!^)(?=[A-Z])')
+            return pattern.sub('_', col_name).lower().replace("__", "_").replace("._", ".")
+        return col_name
+    
+    def _replace_dots(process_col:bool, col_name:str):
+        if process_col:
+            return col_name.replace(".", "_")
+        return col_name
 
     def _process_column_name(self, dataframe:DataFrame, to_snake_case:bool, replace_dots:bool):
         """Receive a Spark Dataframe and return a snake_case columns like dataframe.
         If replace_dots is True, then all the subcolumns like "Column.SubColumn" will be
         renamed as "Column_SubColumn".
 
         Parameters
@@ -48,20 +58,17 @@
         replace_dots: bool
             If True replace the column name dots with underscores.
 
         Returns
         -------
         dataframe: pyspark.Dataframe
         """
-        pattern = re.compile(r'(?<!^)(?=[A-Z])')
         for col in dataframe.columns:
-            if to_snake_case:
-                sc_col = pattern.sub('_', col).lower().replace("__", "_").replace("._", ".")
-            if replace_dots:
-                sc_col = sc_col.replace(".", "_")
+            sc_col = self._to_snake_case(to_snake_case, col)
+            sc_col = self._replace_dots(replace_dots, sc_col)
             dataframe = dataframe.withColumnRenamed(col, sc_col)
         return dataframe
 
     def _get_schema_struct(self, dataframe_schema:dict, id_key:str, black_list:List[str], dataframe_name:str, _ref:str = "", named_struct:dict = {}):
         """Receive Spark Dataframe Schema in dictionary format, and return 
         a dictionary[str, str] with the all required named_struct expressions
         to flatten de Dataframe.
@@ -176,14 +183,14 @@
         Returns
         -------
         processed_data : dict[str, pyspark.DataFrame]
             A dictionary with all the resulting Dataframes from the flattening process.
             Each ArrayType column will be flattened and added as a Dataframe inside the
             processed_data return.
         """
-        if len(dataframe.head(1)) > 0:
+        if len(dataframe.head(1)) == 0:
             raise FlatteningException("The provided dataframe is empty.")
         processed_data = {}
         processed_data = self._processor(dataframe, id_key, black_list, dataframe_name)
         for processed_df_name, processed_df in processed_data.items():
             processed_data[processed_df_name] = self._process_column_name(processed_df, to_snake_case, replace_dots)
         return processed_data
```

### Comparing `dataflat-1.0.1/dataflat.egg-info/PKG-INFO` & `dataflat-1.0.2/dataflat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -39,24 +39,26 @@
 
 id_key = 'id'
 black_list = ['keys','or','columns','to','skip']
 
 #The following variables have the default values for each transform function
 to_snake_case = False
 replace_dots = False
-dict_name = 'dct'
-chunk_size = 500
-dataframe_name = 'df'
 
 # Instantiate a Dictionary Flattener
+dict_name = 'dct'
 flattener_dict = Flattener().handler(Options.DICTIONARY)
-flattener.transform(dictionary, id_key, black_list, dict_name, to_snake_case, replace_dots)
+flattener_dict.transform(dictionary, id_key, black_list, dict_name, to_snake_case, replace_dots)
 
 
 # Instantiate a Pandas Dataframe Flattener
+##Default chunk size = 500
+dataframe_name = 'df'
+chunk_size = 500
 flattener_pd = Flattener().handler(Options.PANDAS_DF)
-transform(dataframe, id_key, black_list, dataframe_name, chunk_size, to_snake_case, replace_dots)
+flattener_pd.transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots, chunk_size)
 
 # Instantiate a Spark Dataframe Flattener
+dataframe_name = 'df'
 flattener_sp = Flattener().handler(Options.SPARK_DF)
-transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots)
+flattener_sp.transform(dataframe, id_key, black_list, dataframe_name, to_snake_case, replace_dots)
 ```
```

### Comparing `dataflat-1.0.1/setup.py` & `dataflat-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 PATH = path.abspath(path.dirname(__file__))
 
 with open(path.join(PATH, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
  
 setuptools.setup(
     name="dataflat",
-    version="1.0.1",
+    version="1.0.2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/JuanARojasA/dataflat',
     author="Juan Rojas",
     author_email="jarojasa97@gmail.com",
     license='Apache License 2.0',
     platforms='any',
```

