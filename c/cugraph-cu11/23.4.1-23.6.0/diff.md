# Comparing `tmp/cugraph_cu11-23.4.1.tar.gz` & `tmp/cugraph-cu11-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cugraph_cu11-23.4.1.tar", last modified: Fri Apr 21 21:02:22 2023, max compression
+gzip compressed data, was "cugraph-cu11-23.6.0.tar", last modified: Fri Jun  9 15:17:28 2023, max compression
```

## Comparing `cugraph_cu11-23.4.1.tar` & `cugraph-cu11-23.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      444 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 02:54:55.000000 cugraph_cu11-23.4.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       12 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      241 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      197 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:02:22.000000 cugraph_cu11-23.4.1/cugraph_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 21:02:22.570909 cugraph_cu11-23.4.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 02:54:55.000000 cugraph_cu11-23.4.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:17:28.082435 cugraph-cu11-23.6.0/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      444 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:12:21.000000 cugraph-cu11-23.6.0/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       12 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-06-09 15:17:28.082435 cugraph-cu11-23.6.0/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      241 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:17:28.081435 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      197 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-09 15:17:28.082435 cugraph-cu11-23.6.0/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:12:21.000000 cugraph-cu11-23.6.0/setup.py
```

### Comparing `cugraph_cu11-23.4.1/LICENSE.md` & `cugraph-cu11-23.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cugraph_cu11-23.4.1/PKG-INFO` & `cugraph-cu11-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cugraph_cu11
-Version: 23.4.1
+Name: cugraph-cu11
+Version: 23.6.0
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
 
-CUGRAPH_CU11
+CUGRAPH-CU11
 ============
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com cugraph_cu11
+    pip install --extra-index-url https://pypi.nvidia.com cugraph-cu11
```

### Comparing `cugraph_cu11-23.4.1/cugraph_cu11.egg-info/PKG-INFO` & `cugraph-cu11-23.6.0/cugraph_cu11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cugraph-cu11
-Version: 23.4.1
+Version: 23.6.0
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
 
-CUGRAPH_CU11
+CUGRAPH-CU11
 ============
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com cugraph_cu11
+    pip install --extra-index-url https://pypi.nvidia.com cugraph-cu11
```

### Comparing `cugraph_cu11-23.4.1/setup.py` & `cugraph-cu11-23.6.0/setup.py`

 * *Files identical despite different names*

