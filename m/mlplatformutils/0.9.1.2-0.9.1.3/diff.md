# Comparing `tmp/mlplatformutils-0.9.1.2.tar.gz` & `tmp/mlplatformutils-0.9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.1.2.tar", last modified: Wed Jun  7 03:35:14 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.1.3.tar", last modified: Fri Jun  9 03:38:59 2023, max compression
```

## Comparing `mlplatformutils-0.9.1.2.tar` & `mlplatformutils-0.9.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.833687 mlplatformutils-0.9.1.2/
--rw-rw-rw-   0        0        0     3470 2023-06-07 03:35:14.833687 mlplatformutils-0.9.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.2/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-07 03:35:14.836690 mlplatformutils-0.9.1.2/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-06-07 03:35:10.000000 mlplatformutils-0.9.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.756849 mlplatformutils-0.9.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.770110 mlplatformutils-0.9.1.2/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.830689 mlplatformutils-0.9.1.2/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     9560 2023-06-07 03:21:53.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-07 03:35:03.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.801161 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3470 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 03:38:59.739078 mlplatformutils-0.9.1.3/
+-rw-rw-rw-   0        0        0     3470 2023-06-09 03:38:59.739078 mlplatformutils-0.9.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.3/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-09 03:38:59.739078 mlplatformutils-0.9.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-09 03:38:04.000000 mlplatformutils-0.9.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:38:59.550710 mlplatformutils-0.9.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 03:38:59.566730 mlplatformutils-0.9.1.3/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:38:59.723447 mlplatformutils-0.9.1.3/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12560 2023-06-09 03:37:41.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-08 21:43:42.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-09 03:38:20.000000 mlplatformutils-0.9.1.3/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:38:59.629243 mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3470 2023-06-09 03:38:59.000000 mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-09 03:38:59.000000 mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:38:59.000000 mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-09 03:38:59.000000 mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 03:38:59.000000 mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.1.2/PKG-INFO` & `mlplatformutils-0.9.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.2
+Version: 0.9.1.3
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.2/setup.py` & `mlplatformutils-0.9.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.1.2',
+    version='0.9.1.3',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.1.3/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.1.3/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.1.3/src/mlplatformutils/core/pandasutils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
-def get_max_properties_starting_with(id, prefix,LineageLogger):
+def get_max_properties_starting_with(id, prefix,dataprop,LineageLogger):
 
     document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
         max_val = max(int(prop) for prop in matching_props) if matching_props else 0
+        datapropval = properties.get(dataprop)[0].get('value') if properties.get(dataprop) else None
     else:
         max_val = 0
-    return str(max_val+1)
+    return str(max_val+1),datapropval
 
 def read_from_delta_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                               SOURCE_READ_SPN_VALUE,\
                               SOURCE_READ_SPNKEY_VALUE,\
                               tenant_id,\
                               AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH,\
                               RUN_ID,\
@@ -30,18 +31,28 @@
         client_id=SOURCE_READ_SPN_VALUE,\
         client_secret=SOURCE_READ_SPNKEY_VALUE,\
         tenant_id=tenant_id
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
-    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
+    sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
+
+    if dataprop is None:
+        dataprop = {"DataReadSource": {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}
+    else:
+        dataprop = {"DataReadSource": {**dataprop, **{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
+                                                       "Type":"ADLS",\
+                                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}}
+
+    LineageLogger.update_vertex(documentId, {**{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("delta"),\
-                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
     return pandas_df
 
 def read_parquet_file_from_adlsgen2_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
@@ -63,18 +74,27 @@
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     #pandas_df = pd.read_parquet(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs , engine="pyarrow")
     #pandas_df = pq.read_table(source=AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs, use_legacy_dataset= True).to_pandas()
     pandas_df = pq.ParquetDataset(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,filesystem=fs).read().to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
-    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
+    if dataprop is None:
+        dataprop = {"DataReadSource": {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}
+    else:
+        dataprop = {"DataReadSource": {**dataprop, **{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                                       "Type":"ADLS",\
+                                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}}
+
+    LineageLogger.update_vertex(documentId, {**{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
-                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
 
     return pandas_df
 
 def list_directory_contents(storage_account_name,\
                             tenant_id,client_id,\
                             client_secret,\
                             directory_path):
@@ -127,18 +147,27 @@
     client_secret=SOURCE_READ_SPNKEY_VALUE)
 
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     pandas_df = pq.ParquetDataset(parquet_files_from_path_list,filesystem=fs).read().to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
-    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
+    if dataprop is None:
+        dataprop = {"DataReadSource": {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}
+    else:
+        dataprop = {"DataReadSource": {**dataprop, **{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                                       "Type":"ADLS",\
+                                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}}
+
+    LineageLogger.update_vertex(documentId, {**{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
-                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
     return pandas_df
 
 def write_pandas_as_parquet_file_to_adlsgen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
@@ -172,13 +201,23 @@
         pyarrow_table,
         AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,
         format='parquet',
         filesystem=pyarrow.fs.PyFileSystem(handler)
     )
     """
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataWriteColumns",LineageLogger)
-    LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataWriteColumns","DataWriteTarget",LineageLogger)
+    if dataprop is None:
+        dataprop = {"DataWriteTarget": {"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}
+    else:
+        dataprop = {"DataWriteTarget": {**dataprop, **{"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                                       "Type":"ADLS",\
+                                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}}}
+
+    LineageLogger.update_vertex(documentId, {**{"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
-                                             "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                             "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
+    
     print("File Write Successful at "+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH+" !")
     return
```

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.1.3/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.1.3/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.2
+Version: 0.9.1.3
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.1.3/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,11 +6,13 @@
 src/mlplatformutils.egg-info/SOURCES.txt
 src/mlplatformutils.egg-info/dependency_links.txt
 src/mlplatformutils.egg-info/requires.txt
 src/mlplatformutils.egg-info/top_level.txt
 src/mlplatformutils/core/__init__.py
 src/mlplatformutils/core/app_insights_logger.py
 src/mlplatformutils/core/lineagegraph.py
+src/mlplatformutils/core/pandascoreutils.py
 src/mlplatformutils/core/pandasutils.py
 src/mlplatformutils/core/platformutils.py
+src/mlplatformutils/core/sparkcoreutils.py
 src/mlplatformutils/core/sparkutils.py
 src/mlplatformutils/core/version.py
```

