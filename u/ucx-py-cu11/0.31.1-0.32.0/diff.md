# Comparing `tmp/ucx_py_cu11-0.31.1.tar.gz` & `tmp/ucx-py-cu11-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucx_py_cu11-0.31.1.tar", last modified: Fri Apr 21 21:01:43 2023, max compression
+gzip compressed data, was "ucx-py-cu11-0.32.0.tar", last modified: Fri Jun  9 15:17:28 2023, max compression
```

## Comparing `ucx_py_cu11-0.31.1.tar` & `ucx-py-cu11-0.32.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      443 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 03:15:24.000000 ucx_py_cu11-0.31.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       11 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      238 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 03:15:24.000000 ucx_py_cu11-0.31.1/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:01:43.496640 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      193 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:01:43.000000 ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:17:28.103159 ucx-py-cu11-0.32.0/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      443 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 04:47:43.000000 ucx-py-cu11-0.32.0/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       11 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-06-09 15:17:28.103159 ucx-py-cu11-0.32.0/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      238 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-09 15:17:28.103159 ucx-py-cu11-0.32.0/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 04:47:43.000000 ucx-py-cu11-0.32.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:17:28.103159 ucx-py-cu11-0.32.0/ucx_py_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/ucx_py_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      193 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/ucx_py_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/ucx_py_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-09 15:17:28.000000 ucx-py-cu11-0.32.0/ucx_py_cu11.egg-info/top_level.txt
```

### Comparing `ucx_py_cu11-0.31.1/LICENSE.md` & `ucx-py-cu11-0.32.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ucx_py_cu11-0.31.1/PKG-INFO` & `ucx-py-cu11-0.32.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ucx_py_cu11
-Version: 0.31.1
+Name: ucx-py-cu11
+Version: 0.32.0
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
@@ -26,16 +26,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.md
 
-UCX_PY_CU11
+UCX-PY-CU11
 ===========
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com ucx_py_cu11
+    pip install --extra-index-url https://pypi.nvidia.com ucx-py-cu11
```

### Comparing `ucx_py_cu11-0.31.1/setup.py` & `ucx-py-cu11-0.32.0/setup.py`

 * *Files identical despite different names*

### Comparing `ucx_py_cu11-0.31.1/ucx_py_cu11.egg-info/PKG-INFO` & `ucx-py-cu11-0.32.0/ucx_py_cu11.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucx-py-cu11
-Version: 0.31.1
+Version: 0.32.0
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
@@ -26,16 +26,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.md
 
-UCX_PY_CU11
+UCX-PY-CU11
 ===========
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com ucx_py_cu11
+    pip install --extra-index-url https://pypi.nvidia.com ucx-py-cu11
```

