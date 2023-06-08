# Comparing `tmp/pylibcugraph_cu11-23.4.1.tar.gz` & `tmp/pylibcugraph-cu11-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibcugraph_cu11-23.4.1.tar", last modified: Fri Apr 21 19:13:25 2023, max compression
+gzip compressed data, was "pylibcugraph-cu11-23.6.0.tar", last modified: Thu Jun  8 22:14:30 2023, max compression
```

## Comparing `pylibcugraph_cu11-23.4.1.tar` & `pylibcugraph-cu11-23.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 19:13:25.971079 pylibcugraph_cu11-23.4.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 03:15:24.000000 pylibcugraph_cu11-23.4.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-04-21 19:13:25.971079 pylibcugraph_cu11-23.4.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 19:13:25.971079 pylibcugraph_cu11-23.4.1/pylibcugraph_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/pylibcugraph_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/pylibcugraph_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/pylibcugraph_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 19:13:25.000000 pylibcugraph_cu11-23.4.1/pylibcugraph_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 19:13:25.971079 pylibcugraph_cu11-23.4.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 03:15:24.000000 pylibcugraph_cu11-23.4.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-08 22:14:30.145284 pylibcugraph-cu11-23.6.0/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:12:21.000000 pylibcugraph-cu11-23.6.0/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-08 22:14:30.145284 pylibcugraph-cu11-23.6.0/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-08 22:14:30.145284 pylibcugraph-cu11-23.6.0/pylibcugraph_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/pylibcugraph_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/pylibcugraph_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/pylibcugraph_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-08 22:14:30.000000 pylibcugraph-cu11-23.6.0/pylibcugraph_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-08 22:14:30.145284 pylibcugraph-cu11-23.6.0/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:12:21.000000 pylibcugraph-cu11-23.6.0/setup.py
```

### Comparing `pylibcugraph_cu11-23.4.1/LICENSE.md` & `pylibcugraph-cu11-23.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylibcugraph_cu11-23.4.1/PKG-INFO` & `pylibcugraph-cu11-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pylibcugraph_cu11
-Version: 23.4.1
+Name: pylibcugraph-cu11
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
 
-PYLIBCUGRAPH_CU11
+PYLIBCUGRAPH-CU11
 =================
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com pylibcugraph_cu11
+    pip install --extra-index-url https://pypi.nvidia.com pylibcugraph-cu11
```

### Comparing `pylibcugraph_cu11-23.4.1/pylibcugraph_cu11.egg-info/PKG-INFO` & `pylibcugraph-cu11-23.6.0/pylibcugraph_cu11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibcugraph-cu11
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
 
-PYLIBCUGRAPH_CU11
+PYLIBCUGRAPH-CU11
 =================
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com pylibcugraph_cu11
+    pip install --extra-index-url https://pypi.nvidia.com pylibcugraph-cu11
```

### Comparing `pylibcugraph_cu11-23.4.1/setup.py` & `pylibcugraph-cu11-23.6.0/setup.py`

 * *Files identical despite different names*

