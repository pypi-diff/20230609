# Comparing `tmp/cuml_cu11-23.4.1.tar.gz` & `tmp/cuml-cu11-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuml_cu11-23.4.1.tar", last modified: Fri Apr 21 21:02:11 2023, max compression
+gzip compressed data, was "cuml-cu11-23.6.0.tar", last modified: Fri Jun  9 15:16:42 2023, max compression
```

## Comparing `cuml_cu11-23.4.1.tar` & `cuml-cu11-23.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:02:11.629010 cuml_cu11-23.4.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:16:23.000000 cuml_cu11-23.4.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-04-21 21:02:11.629010 cuml_cu11-23.4.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 21:02:11.628010 cuml_cu11-23.4.1/cuml_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/cuml_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/cuml_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/cuml_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 21:02:11.000000 cuml_cu11-23.4.1/cuml_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 21:02:11.629010 cuml_cu11-23.4.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:16:23.000000 cuml_cu11-23.4.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:16:42.948654 cuml-cu11-23.6.0/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 18:23:22.000000 cuml-cu11-23.6.0/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-06-09 15:16:42.948654 cuml-cu11-23.6.0/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:16:42.948654 cuml-cu11-23.6.0/cuml_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/cuml_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/cuml_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/cuml_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-09 15:16:42.000000 cuml-cu11-23.6.0/cuml_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-09 15:16:42.948654 cuml-cu11-23.6.0/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 18:23:22.000000 cuml-cu11-23.6.0/setup.py
```

### Comparing `cuml_cu11-23.4.1/LICENSE.md` & `cuml-cu11-23.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cuml_cu11-23.4.1/PKG-INFO` & `cuml-cu11-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cuml_cu11
-Version: 23.4.1
+Name: cuml-cu11
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
 
-CUML_CU11
+CUML-CU11
 =========
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com cuml_cu11
+    pip install --extra-index-url https://pypi.nvidia.com cuml-cu11
```

### Comparing `cuml_cu11-23.4.1/cuml_cu11.egg-info/PKG-INFO` & `cuml-cu11-23.6.0/cuml_cu11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuml-cu11
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
 
-CUML_CU11
+CUML-CU11
 =========
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com cuml_cu11
+    pip install --extra-index-url https://pypi.nvidia.com cuml-cu11
```

### Comparing `cuml_cu11-23.4.1/setup.py` & `cuml-cu11-23.6.0/setup.py`

 * *Files identical despite different names*

