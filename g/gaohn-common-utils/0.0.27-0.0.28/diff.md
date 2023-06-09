# Comparing `tmp/gaohn-common-utils-0.0.27.tar.gz` & `tmp/gaohn-common-utils-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.27.tar", last modified: Fri Jun  9 04:00:01 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.28.tar", last modified: Fri Jun  9 04:06:36 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.27.tar` & `gaohn-common-utils-0.0.28.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.430704 gaohn-common-utils-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:00:01.430704 gaohn-common-utils-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.426705 gaohn-common-utils-0.0.27/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.426705 gaohn-common-utils-0.0.27/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.422705 gaohn-common-utils-0.0.27/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.426705 gaohn-common-utils-0.0.27/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.430704 gaohn-common-utils-0.0.27/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.426705 gaohn-common-utils-0.0.27/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.430704 gaohn-common-utils-0.0.27/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:00:01.430704 gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:00:01.000000 gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 04:00:01.000000 gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:00:01.000000 gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 04:00:01.000000 gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 04:00:01.000000 gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 03:59:44.000000 gaohn-common-utils-0.0.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:00:01.430704 gaohn-common-utils-0.0.27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.907804 gaohn-common-utils-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:06:36.907804 gaohn-common-utils-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.903804 gaohn-common-utils-0.0.28/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:06:36.907804 gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 04:06:36.000000 gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 04:06:36.000000 gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:06:36.000000 gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 04:06:36.000000 gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 04:06:36.000000 gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 04:06:14.000000 gaohn-common-utils-0.0.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:06:36.907804 gaohn-common-utils-0.0.28/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.27/LICENSE` & `gaohn-common-utils-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/PKG-INFO` & `gaohn-common-utils-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.27
+Version: 0.0.28
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.27/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.28/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.28/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.28/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.28/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/core/common.py` & `gaohn-common-utils-0.0.28/common_utils/core/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 """
 common_utils/core/common.py
 
 This module contains common utility functions for various purposes.
 """
 import json
+import logging
 import os
 import random
-from typing import Any, Dict, Optional, Union
 from pathlib import Path
+from typing import Any, Dict, Optional, Union
 
 import numpy as np
 import rich
 import torch
 import yaml
 from dotenv import load_dotenv
+from rich.logging import RichHandler
 from yaml import FullLoader
 
 from common_utils.core.base import DictPersistence
 
+# Setup logging
+logging.basicConfig(
+    level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler()]
+)
+
+logger = logging.getLogger("rich")
+
 
 class JsonAdapter(DictPersistence):
     def save_as_dict(
         self, data: Dict[str, Any], filepath: str, **kwargs: Dict[str, Any]
     ) -> None:
         """
         Save a dictionary to a specific location.
@@ -154,8 +163,13 @@
         Default value to use if the environment variable is not set. Defaults to ".".
 
     Returns
     -------
     Path
         Path to the root directory of the project.
     """
-    return Path(os.getenv(env_var, root_dir))
+    root_dir_env = os.getenv(env_var)
+    if root_dir_env is None:
+        logger.warning("Environment variable %s is not set.", env_var)
+        logger.warning("Using default value %s.", root_dir)
+        return Path(root_dir)
+    return Path(root_dir_env)
```

### Comparing `gaohn-common-utils-0.0.27/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.28/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.28/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/core/logger.py` & `gaohn-common-utils-0.0.28/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.28/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.27
+Version: 0.0.28
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.27/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.28/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.27/pyproject.toml` & `gaohn-common-utils-0.0.28/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.27"
+version = "0.0.28"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

