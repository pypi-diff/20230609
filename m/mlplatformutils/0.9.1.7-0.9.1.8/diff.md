# Comparing `tmp/mlplatformutils-0.9.1.7.tar.gz` & `tmp/mlplatformutils-0.9.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.1.7.tar", last modified: Fri Jun  9 07:39:55 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.1.8.tar", last modified: Fri Jun  9 20:27:23 2023, max compression
```

## Comparing `mlplatformutils-0.9.1.7.tar` & `mlplatformutils-0.9.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:39:55.824625 mlplatformutils-0.9.1.7/
--rw-rw-rw-   0        0        0     4744 2023-06-09 07:39:55.824625 mlplatformutils-0.9.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.7/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-09 07:39:55.826624 mlplatformutils-0.9.1.7/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-06-09 07:39:49.000000 mlplatformutils-0.9.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:39:55.623030 mlplatformutils-0.9.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 07:39:55.646031 mlplatformutils-0.9.1.7/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:39:55.821631 mlplatformutils-0.9.1.7/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    13418 2023-06-09 07:39:32.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-08 21:43:42.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-09 07:39:41.000000 mlplatformutils-0.9.1.7/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:39:55.686251 mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     4744 2023-06-09 07:39:55.000000 mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-09 07:39:55.000000 mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 07:39:55.000000 mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-09 07:39:55.000000 mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 07:39:55.000000 mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 20:27:23.921650 mlplatformutils-0.9.1.8/
+-rw-rw-rw-   0        0        0     4744 2023-06-09 20:27:23.921650 mlplatformutils-0.9.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.8/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-09 20:27:23.930160 mlplatformutils-0.9.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-09 20:27:16.000000 mlplatformutils-0.9.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:27:23.485195 mlplatformutils-0.9.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 20:27:23.530448 mlplatformutils-0.9.1.8/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:27:23.918636 mlplatformutils-0.9.1.8/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    13534 2023-06-09 20:27:01.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-08 21:43:42.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-09 20:27:09.000000 mlplatformutils-0.9.1.8/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:27:23.589962 mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     4744 2023-06-09 20:27:23.000000 mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-09 20:27:23.000000 mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:27:23.000000 mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-09 20:27:23.000000 mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 20:27:23.000000 mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.1.7/PKG-INFO` & `mlplatformutils-0.9.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.7
+Version: 0.9.1.8
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.7/setup.py` & `mlplatformutils-0.9.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.1.7',
+    version='0.9.1.8',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/pandasutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,19 @@
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
-    
+    dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("delta"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
-                                             "DataReadSource":{str(dataprop)}})
+                                             "DataReadSource":dataprop})
     return pandas_df
 
 def read_parquet_file_from_adlsgen2_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
@@ -83,19 +83,19 @@
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
-    
+    dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
-                                             "DataReadSource":{str(dataprop)}})
+                                             "DataReadSource":dataprop})
 
     return pandas_df
 
 def list_directory_contents(storage_account_name,\
                             tenant_id,client_id,\
                             client_secret,\
                             directory_path):
@@ -157,19 +157,19 @@
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
-    
+    dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
-                                             "DataReadSource":{str(dataprop)}})
+                                             "DataReadSource":dataprop})
     return pandas_df
 
 def write_pandas_as_parquet_file_to_adlsgen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
@@ -213,15 +213,15 @@
         dataprop = str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS",\
                                         "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
-    
+    dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
-                                             "DataWriteTarget":{str(dataprop)}})
+                                             "DataWriteTarget":dataprop})
 
     print("File Write Successful at "+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH+" !")
     return
```

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.1.8/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.7
+Version: 0.9.1.8
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.7/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.1.8/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

