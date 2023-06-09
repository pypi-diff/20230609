# Comparing `tmp/gaohn-common-utils-0.0.29.tar.gz` & `tmp/gaohn-common-utils-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.29.tar", last modified: Fri Jun  9 04:09:44 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.30.tar", last modified: Fri Jun  9 04:13:03 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.29.tar` & `gaohn-common-utils-0.0.30.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.617959 gaohn-common-utils-0.0.29/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:09:44.617959 gaohn-common-utils-0.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.613959 gaohn-common-utils-0.0.29/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.613959 gaohn-common-utils-0.0.29/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.613959 gaohn-common-utils-0.0.29/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.613959 gaohn-common-utils-0.0.29/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.617959 gaohn-common-utils-0.0.29/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.613959 gaohn-common-utils-0.0.29/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.617959 gaohn-common-utils-0.0.29/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:09:44.617959 gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:09:44.000000 gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 04:09:44.000000 gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:09:44.000000 gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 04:09:44.000000 gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 04:09:44.000000 gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 04:09:17.000000 gaohn-common-utils-0.0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:09:44.617959 gaohn-common-utils-0.0.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.186067 gaohn-common-utils-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:13:03.186067 gaohn-common-utils-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.182067 gaohn-common-utils-0.0.30/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.182067 gaohn-common-utils-0.0.30/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.182067 gaohn-common-utils-0.0.30/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.182067 gaohn-common-utils-0.0.30/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.182067 gaohn-common-utils-0.0.30/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.182067 gaohn-common-utils-0.0.30/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.186067 gaohn-common-utils-0.0.30/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:03.186067 gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:13:03.000000 gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 04:13:03.000000 gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:13:03.000000 gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 04:13:03.000000 gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 04:13:03.000000 gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 04:12:38.000000 gaohn-common-utils-0.0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:13:03.186067 gaohn-common-utils-0.0.30/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.29/LICENSE` & `gaohn-common-utils-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/PKG-INFO` & `gaohn-common-utils-0.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.29
+Version: 0.0.30
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.29/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.30/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.30/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.30/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.30/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/core/common.py` & `gaohn-common-utils-0.0.30/common_utils/core/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,8 +168,13 @@
         Path to the root directory of the project.
     """
     root_dir_env = os.getenv(env_var)
     if root_dir_env is None:
         logger.warning("Environment variable %s is not set.", env_var)
         logger.warning("Using default value %s", root_dir)
         return Path(root_dir)
+    logger.info(
+        "Using environment variable %s and discarding default value %s",
+        env_var,
+        root_dir,
+    )
     return Path(root_dir_env)
```

### Comparing `gaohn-common-utils-0.0.29/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.30/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.30/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/core/logger.py` & `gaohn-common-utils-0.0.30/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.30/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.29
+Version: 0.0.30
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.29/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.30/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.29/pyproject.toml` & `gaohn-common-utils-0.0.30/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.29"
+version = "0.0.30"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

