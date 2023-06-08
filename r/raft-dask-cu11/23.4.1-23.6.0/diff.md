# Comparing `tmp/raft_dask_cu11-23.4.1.tar.gz` & `tmp/raft-dask-cu11-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raft_dask_cu11-23.4.1.tar", last modified: Fri Apr 21 19:10:55 2023, max compression
+gzip compressed data, was "raft-dask-cu11-23.6.0.tar", last modified: Thu Jun  8 22:32:55 2023, max compression
```

## Comparing `raft_dask_cu11-23.4.1.tar` & `raft-dask-cu11-23.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 19:10:55.949380 raft_dask_cu11-23.4.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-12 18:02:21.000000 raft_dask_cu11-23.4.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-04-21 19:10:55.949380 raft_dask_cu11-23.4.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-21 19:10:55.949380 raft_dask_cu11-23.4.1/raft_dask_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/raft_dask_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/raft_dask_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/raft_dask_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-21 19:10:55.000000 raft_dask_cu11-23.4.1/raft_dask_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-21 19:10:55.949380 raft_dask_cu11-23.4.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-12 18:02:21.000000 raft_dask_cu11-23.4.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-08 22:32:55.349664 raft-dask-cu11-23.6.0/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-06-08 22:32:55.000000 raft-dask-cu11-23.6.0/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:19:03.000000 raft-dask-cu11-23.6.0/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-06-08 22:32:54.000000 raft-dask-cu11-23.6.0/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-08 22:32:55.347664 raft-dask-cu11-23.6.0/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-06-08 22:32:55.000000 raft-dask-cu11-23.6.0/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-08 22:32:55.347664 raft-dask-cu11-23.6.0/raft_dask_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-08 22:32:55.000000 raft-dask-cu11-23.6.0/raft_dask_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-06-08 22:32:55.000000 raft-dask-cu11-23.6.0/raft_dask_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-08 22:32:55.000000 raft-dask-cu11-23.6.0/raft_dask_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-08 22:32:55.000000 raft-dask-cu11-23.6.0/raft_dask_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-08 22:32:55.349664 raft-dask-cu11-23.6.0/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:19:03.000000 raft-dask-cu11-23.6.0/setup.py
```

### Comparing `raft_dask_cu11-23.4.1/LICENSE.md` & `raft-dask-cu11-23.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `raft_dask_cu11-23.4.1/PKG-INFO` & `raft-dask-cu11-23.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: raft_dask_cu11
-Version: 23.4.1
+Name: raft-dask-cu11
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
 
-RAFT_DASK_CU11
+RAFT-DASK-CU11
 ==============
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com raft_dask_cu11
+    pip install --extra-index-url https://pypi.nvidia.com raft-dask-cu11
```

### Comparing `raft_dask_cu11-23.4.1/raft_dask_cu11.egg-info/PKG-INFO` & `raft-dask-cu11-23.6.0/raft_dask_cu11.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raft-dask-cu11
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
 
-RAFT_DASK_CU11
+RAFT-DASK-CU11
 ==============
 
 **WARNING:** This project is not functional and is a placeholder from NVIDIA.
 To install, please execute the following:
 
 .. code-block:: bash
 
-    pip install --extra-index-url https://pypi.nvidia.com raft_dask_cu11
+    pip install --extra-index-url https://pypi.nvidia.com raft-dask-cu11
```

### Comparing `raft_dask_cu11-23.4.1/setup.py` & `raft-dask-cu11-23.6.0/setup.py`

 * *Files identical despite different names*

