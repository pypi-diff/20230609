# Comparing `tmp/nvidia-dali-nightly-cuda110-1.27.0.dev20230607.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.27.0.dev20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.27.0.dev20230607.tar", last modified: Wed Jun  7 10:04:59 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.27.0.dev20230608.tar", last modified: Thu Jun  8 18:26:44 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.27.0.dev20230607.tar` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230608.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-07 10:04:59.153589 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-05-24 10:07:51.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-07 10:04:59.153589 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-07 10:04:59.153589 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-07 10:04:59.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-07 10:04:59.153589 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-05-24 10:07:51.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230607/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-08 18:26:44.571639 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 04:47:43.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-08 18:26:44.571639 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-08 18:26:44.571639 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-08 18:26:44.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-08 18:26:44.571639 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 04:47:43.000000 nvidia-dali-nightly-cuda110-1.27.0.dev20230608/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.27.0.dev20230607/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230608/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.27.0.dev20230607/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230608/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.27.0.dev20230607
+Version: 1.27.0.dev20230608
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.27.0.dev20230607/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230608/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.27.0.dev20230607
+Version: 1.27.0.dev20230608
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.27.0.dev20230607/setup.py` & `nvidia-dali-nightly-cuda110-1.27.0.dev20230608/setup.py`

 * *Files identical despite different names*

