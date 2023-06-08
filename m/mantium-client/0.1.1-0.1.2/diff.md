# Comparing `tmp/mantium_client-0.1.1.tar.gz` & `tmp/mantium_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantium_client-0.1.1.tar", max compression
+gzip compressed data, was "mantium_client-0.1.2.tar", max compression
```

## Comparing `mantium_client-0.1.1.tar` & `mantium_client-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-08 21:18:14.058797 mantium_client-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1023 2023-06-08 21:18:14.058797 mantium_client-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-08 21:18:14.058797 mantium_client-0.1.1/mantium/client/__init__.py
--rw-r--r--   0        0        0      894 2023-06-08 21:18:14.058797 mantium_client-0.1.1/mantium/client/invoke_tasks/__init__.py
--rw-r--r--   0        0        0     1446 2023-06-08 21:18:14.058797 mantium_client-0.1.1/mantium/client/invoke_tasks/build.py
--rw-r--r--   0        0        0      176 2023-06-08 21:18:14.058797 mantium_client-0.1.1/mantium/client/invoke_tasks/test.py
--rw-r--r--   0        0        0     1324 2023-06-08 21:18:14.058797 mantium_client-0.1.1/mantium/client/invoke_tasks/utils.py
--rw-r--r--   0        0        0     1665 2023-06-08 21:18:14.058797 mantium_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 mantium_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 22:23:13.931547 mantium_client-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1030 2023-06-08 22:23:13.931547 mantium_client-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/__init__.py
+-rw-r--r--   0        0        0      894 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/__init__.py
+-rw-r--r--   0        0        0     1446 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/build.py
+-rw-r--r--   0        0        0      176 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/test.py
+-rw-r--r--   0        0        0     1324 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/utils.py
+-rw-r--r--   0        0        0     1665 2023-06-08 22:23:13.931547 mantium_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 mantium_client-0.1.2/PKG-INFO
```

### Comparing `mantium_client-0.1.1/LICENSE.txt` & `mantium_client-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.1/README.md` & `mantium_client-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 A Python client library for [Mantium services](https://mantiumai.com/).
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install this client.
 
 ```bash
-pip install mantium
+pip install mantium-client
 ```
 
 ## Usage
 
 ```python
 from mantium import ApiClient
 from mantium.openapi_client.api.applications_api import ApplicationsApi
```

### Comparing `mantium_client-0.1.1/mantium/client/invoke_tasks/__init__.py` & `mantium_client-0.1.2/mantium/client/invoke_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.1/mantium/client/invoke_tasks/build.py` & `mantium_client-0.1.2/mantium/client/invoke_tasks/build.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.1/mantium/client/invoke_tasks/utils.py` & `mantium_client-0.1.2/mantium/client/invoke_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.1/pyproject.toml` & `mantium_client-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mantium-client"
-version = "0.1.1"
+version = "0.1.2"
 license = "Apache-2.0"
 description = "Python client for the Mantium API"
 authors = ["Mantium <support@mantiumai.com>"]
 readme = "README.md"
 packages = [{include = "mantium"}]
 repository = "https://github.com/mantiumai/mantium-client-py"
 homepage = "https://github.com/mantiumai/mantium-client-py"
```

### Comparing `mantium_client-0.1.1/PKG-INFO` & `mantium_client-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantium-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Mantium API
 Home-page: https://github.com/mantiumai/mantium-client-py
 License: Apache-2.0
 Keywords: mantium,ChatGPT,AI
 Author: Mantium
 Author-email: support@mantiumai.com
 Requires-Python: >=3.10,<4.0
@@ -36,15 +36,15 @@
 A Python client library for [Mantium services](https://mantiumai.com/).
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install this client.
 
 ```bash
-pip install mantium
+pip install mantium-client
 ```
 
 ## Usage
 
 ```python
 from mantium import ApiClient
 from mantium.openapi_client.api.applications_api import ApplicationsApi
```

