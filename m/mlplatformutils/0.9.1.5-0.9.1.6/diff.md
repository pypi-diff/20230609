# Comparing `tmp/mlplatformutils-0.9.1.5.tar.gz` & `tmp/mlplatformutils-0.9.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.1.5.tar", last modified: Fri Jun  9 05:01:53 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.1.6.tar", last modified: Fri Jun  9 06:59:28 2023, max compression
```

## Comparing `mlplatformutils-0.9.1.5.tar` & `mlplatformutils-0.9.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 05:01:53.965514 mlplatformutils-0.9.1.5/
--rw-rw-rw-   0        0        0     4744 2023-06-09 05:01:53.965514 mlplatformutils-0.9.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.5/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-09 05:01:53.968508 mlplatformutils-0.9.1.5/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-06-09 05:00:47.000000 mlplatformutils-0.9.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 05:01:53.728052 mlplatformutils-0.9.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 05:01:53.754058 mlplatformutils-0.9.1.5/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 05:01:53.963512 mlplatformutils-0.9.1.5/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    12631 2023-06-09 05:00:32.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-08 21:43:42.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-09 05:00:52.000000 mlplatformutils-0.9.1.5/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-09 05:01:53.793224 mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     4744 2023-06-09 05:01:53.000000 mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-09 05:01:53.000000 mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 05:01:53.000000 mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-09 05:01:53.000000 mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 05:01:53.000000 mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:59:28.235931 mlplatformutils-0.9.1.6/
+-rw-rw-rw-   0        0        0     4744 2023-06-09 06:59:28.241948 mlplatformutils-0.9.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.6/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-09 06:59:28.267935 mlplatformutils-0.9.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-09 06:59:17.000000 mlplatformutils-0.9.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:59:27.969299 mlplatformutils-0.9.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:59:27.998307 mlplatformutils-0.9.1.6/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:59:28.232931 mlplatformutils-0.9.1.6/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    13410 2023-06-09 06:58:53.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-08 21:43:42.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-09 06:59:02.000000 mlplatformutils-0.9.1.6/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:59:28.039830 mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     4744 2023-06-09 06:59:27.000000 mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-09 06:59:27.000000 mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:59:27.000000 mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-09 06:59:27.000000 mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 06:59:27.000000 mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.1.5/PKG-INFO` & `mlplatformutils-0.9.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.5
+Version: 0.9.1.6
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.5/setup.py` & `mlplatformutils-0.9.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.1.5',
+    version='0.9.1.6',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/pandasutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,27 +32,27 @@
         client_secret=SOURCE_READ_SPNKEY_VALUE,\
         tenant_id=tenant_id
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
-
     if dataprop is None:
-        dataprop = {"DataReadSource": str({"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
+        dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                        "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})}
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
-        dataprop = {"DataReadSource": str({**dataprop, **{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
-                                                       "Type":"ADLS",\
-                                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}})}
-
-    LineageLogger.update_vertex(documentId, {**{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
+        dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+    
+    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("delta"),\
-                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
+                                             "DataReadSource":str(dataprop)})
     return pandas_df
 
 def read_parquet_file_from_adlsgen2_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
@@ -76,25 +76,26 @@
     #pandas_df = pd.read_parquet(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs , engine="pyarrow")
     #pandas_df = pq.read_table(source=AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs, use_legacy_dataset= True).to_pandas()
     pandas_df = pq.ParquetDataset(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,filesystem=fs).read().to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
-        dataprop = {"DataReadSource": str({"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+        dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})}
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
-        dataprop = {"DataReadSource": str({**dataprop, **{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                                       "Type":"ADLS",\
-                                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}})}
-
-    LineageLogger.update_vertex(documentId, {**{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+        dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+    
+    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
-                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
+                                             "DataReadSource":str(dataprop)})
 
     return pandas_df
 
 def list_directory_contents(storage_account_name,\
                             tenant_id,client_id,\
                             client_secret,\
                             directory_path):
@@ -149,25 +150,26 @@
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     pandas_df = pq.ParquetDataset(parquet_files_from_path_list,filesystem=fs).read().to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
-        dataprop = {"DataReadSource": str({"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+        dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})}
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
-        dataprop = {"DataReadSource": str({**dataprop, **{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                                       "Type":"ADLS",\
-                                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}})}
+        dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     
-    LineageLogger.update_vertex(documentId, {**{"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
-                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
+                                             "DataReadSource":str(dataprop)})
     return pandas_df
 
 def write_pandas_as_parquet_file_to_adlsgen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
@@ -202,22 +204,24 @@
         AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,
         format='parquet',
         filesystem=pyarrow.fs.PyFileSystem(handler)
     )
     """
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataWriteColumns","DataWriteTarget",LineageLogger)
+
     if dataprop is None:
-        dataprop = {"DataWriteTarget": str({"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+        dataprop = str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
-                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})}
+                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
-        dataprop = {"DataWriteTarget": str({**dataprop, **{"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                                       "Type":"ADLS",\
-                                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"}})}
-
-    LineageLogger.update_vertex(documentId, {**{"DataWriteTarget_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                             "FileFormat_"+sourcePostfix:str("parquet"),\
-                                             "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"},**dataprop})
+        dataprop = str(dataprop)+str(",")+str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                       "Type":"ADLS",\
+                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     
+    LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                             "FileFormat_"+sourcePostfix:str("parquet"),\
+                                             "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
+                                             "DataWriteTarget":str(dataprop)})
+
     print("File Write Successful at "+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH+" !")
     return
```

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.1.6/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.5
+Version: 0.9.1.6
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.5/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.1.6/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

