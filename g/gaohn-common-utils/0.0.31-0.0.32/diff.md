# Comparing `tmp/gaohn-common-utils-0.0.31.tar.gz` & `tmp/gaohn-common-utils-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.31.tar", last modified: Fri Jun  9 06:42:23 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.32.tar", last modified: Fri Jun  9 06:47:15 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.31.tar` & `gaohn-common-utils-0.0.32.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.867566 gaohn-common-utils-0.0.31/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.867566 gaohn-common-utils-0.0.31/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 06:42:23.000000 gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 06:42:23.000000 gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:42:23.000000 gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 06:42:23.000000 gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 06:42:23.000000 gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 06:42:03.000000 gaohn-common-utils-0.0.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:42:23.871566 gaohn-common-utils-0.0.31/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.333285 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.333285 gaohn-common-utils-0.0.32/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.31/LICENSE` & `gaohn-common-utils-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/PKG-INFO` & `gaohn-common-utils-0.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.31
+Version: 0.0.32
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.31/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.32/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from google.cloud.exceptions import NotFound
 from rich.logging import RichHandler
 
 from common_utils.cloud.base import GCPConnector
 
 # Setup logging
 logging.basicConfig(
-    level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler()]
+    level="INFO",
+    format="%(asctime)s [%(levelname)s]: %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+    handlers=[RichHandler()],
 )
 
 logger = logging.getLogger("rich")
 
 
 @dataclass
 class BigQuery(GCPConnector):
```

### Comparing `gaohn-common-utils-0.0.31/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/gcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from google.cloud.exceptions import NotFound
 from rich.logging import RichHandler
 
 from common_utils.cloud.base import GCPConnector
 
 # Setup logging
 logging.basicConfig(
-    level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler()]
+    level="INFO",
+    format="%(asctime)s [%(levelname)s]: %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+    handlers=[RichHandler()],
 )
 
 logger = logging.getLogger("rich")
 
 
 @dataclass
 class GCS(GCPConnector):
```

### Comparing `gaohn-common-utils-0.0.31/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.32/common_utils/core/artifacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import subprocess
 from typing import Optional
 
 from rich.logging import RichHandler
 
 # Setup logging
 logging.basicConfig(
-    level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler()]
+    level="INFO",
+    format="%(asctime)s [%(levelname)s]: %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+    handlers=[RichHandler()],
 )
 
 logger = logging.getLogger("rich")
 
 
 def get_git_commit_hash(working_dir: Optional[str] = None) -> str:
     """
```

### Comparing `gaohn-common-utils-0.0.31/common_utils/core/common.py` & `gaohn-common-utils-0.0.32/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.32/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.32/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/common_utils/core/logger.py` & `gaohn-common-utils-0.0.32/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.32/common_utils/versioning/dvc/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 import hashlib
 import json
+import logging
 import os
 from datetime import datetime
 
 import pandas as pd
+from rich.logging import RichHandler
+
+# Setup logging
+logging.basicConfig(
+    level="INFO",
+    format="%(asctime)s [%(levelname)s]: %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+    handlers=[RichHandler()],
+)
+
+logger = logging.getLogger("rich")
+
 
 DATA_DIR = "data_versions"
 CODE_DIR = "code_versions"
 METADATA_FILE = "metadata.json"
 
 
 def hash_file(filepath):
```

### Comparing `gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.31
+Version: 0.0.32
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.31/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.31/pyproject.toml` & `gaohn-common-utils-0.0.32/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

