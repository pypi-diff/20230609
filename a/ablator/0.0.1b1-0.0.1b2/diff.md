# Comparing `tmp/ablator-0.0.1b1.tar.gz` & `tmp/ablator-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablator-0.0.1b1.tar", last modified: Wed Jun  7 00:57:45 2023, max compression
+gzip compressed data, was "ablator-0.0.1b2.tar", last modified: Thu Jun  8 22:43:04 2023, max compression
```

## Comparing `ablator-0.0.1b1.tar` & `ablator-0.0.1b2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.136830 ablator-0.0.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 00:57:35.000000 ablator-0.0.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-07 00:57:45.136830 ablator-0.0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-07 00:57:35.000000 ablator-0.0.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.128830 ablator-0.0.1b1/ablator/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.128830 ablator-0.0.1b1/ablator/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/analysis/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/plot/cat_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/plot/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/plot/num_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/analysis/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18493 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/config/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/main/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/model/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/model/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)    32475 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/main/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/modules/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/loggers/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/loggers/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/modules/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18609 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/metrics/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/metrics/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.132830 ablator-0.0.1b1/ablator/modules/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/storage/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/modules/storage/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.136830 ablator-0.0.1b1/ablator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-07 00:57:35.000000 ablator-0.0.1b1/ablator/utils/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:57:45.128830 ablator-0.0.1b1/ablator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-07 00:57:45.000000 ablator-0.0.1b1/ablator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-07 00:57:45.000000 ablator-0.0.1b1/ablator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:57:45.000000 ablator-0.0.1b1/ablator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 00:57:45.000000 ablator-0.0.1b1/ablator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 00:57:45.000000 ablator-0.0.1b1/ablator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:57:45.136830 ablator-0.0.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-07 00:57:35.000000 ablator-0.0.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.547041 ablator-0.0.1b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 22:42:49.000000 ablator-0.0.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-08 22:43:04.547041 ablator-0.0.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-08 22:42:49.000000 ablator-0.0.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.535041 ablator-0.0.1b2/ablator/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.535041 ablator-0.0.1b2/ablator/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.539041 ablator-0.0.1b2/ablator/analysis/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/plot/cat_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/plot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/plot/num_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/analysis/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.539041 ablator-0.0.1b2/ablator/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18493 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.543041 ablator-0.0.1b2/ablator/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.543041 ablator-0.0.1b2/ablator/main/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/model/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/model/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32475 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/main/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.543041 ablator-0.0.1b2/ablator/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.543041 ablator-0.0.1b2/ablator/modules/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/loggers/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/loggers/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.543041 ablator-0.0.1b2/ablator/modules/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18609 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/metrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/metrics/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.543041 ablator-0.0.1b2/ablator/modules/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/storage/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/modules/storage/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.547041 ablator-0.0.1b2/ablator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-08 22:42:49.000000 ablator-0.0.1b2/ablator/utils/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:43:04.535041 ablator-0.0.1b2/ablator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-08 22:43:04.000000 ablator-0.0.1b2/ablator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-08 22:43:04.000000 ablator-0.0.1b2/ablator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:43:04.000000 ablator-0.0.1b2/ablator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 22:43:04.000000 ablator-0.0.1b2/ablator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 22:43:04.000000 ablator-0.0.1b2/ablator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:43:04.547041 ablator-0.0.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-08 22:42:49.000000 ablator-0.0.1b2/setup.py
```

### Comparing `ablator-0.0.1b1/LICENSE` & `ablator-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/PKG-INFO` & `ablator-0.0.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablator
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Model Ablation Tool-Kit
 Home-page: https://iordanis.xyz
 Author: Iordanis Fostiropoulos
 Author-email: dev@iordanis.xyz
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ablator-0.0.1b1/README.md` & `ablator-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/__init__.py` & `ablator-0.0.1b2/ablator/__init__.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/main.py` & `ablator-0.0.1b2/ablator/analysis/main.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/plot/__init__.py` & `ablator-0.0.1b2/ablator/analysis/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/plot/cat_plot.py` & `ablator-0.0.1b2/ablator/analysis/plot/cat_plot.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/plot/main.py` & `ablator-0.0.1b2/ablator/analysis/plot/main.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/plot/num_plot.py` & `ablator-0.0.1b2/ablator/analysis/plot/num_plot.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/plot/utils.py` & `ablator-0.0.1b2/ablator/analysis/plot/utils.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/analysis/results.py` & `ablator-0.0.1b2/ablator/analysis/results.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/config/main.py` & `ablator-0.0.1b2/ablator/config/main.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/config/types.py` & `ablator-0.0.1b2/ablator/config/types.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/config/utils.py` & `ablator-0.0.1b2/ablator/config/utils.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/main/configs.py` & `ablator-0.0.1b2/ablator/main/configs.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/main/model/main.py` & `ablator-0.0.1b2/ablator/main/model/main.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/main/model/wrapper.py` & `ablator-0.0.1b2/ablator/main/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/main/mp.py` & `ablator-0.0.1b2/ablator/main/mp.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/main/proto.py` & `ablator-0.0.1b2/ablator/main/proto.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/main/state.py` & `ablator-0.0.1b2/ablator/main/state.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/loggers/__init__.py` & `ablator-0.0.1b2/ablator/modules/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/loggers/file.py` & `ablator-0.0.1b2/ablator/modules/loggers/file.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/loggers/main.py` & `ablator-0.0.1b2/ablator/modules/loggers/main.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/loggers/tensor.py` & `ablator-0.0.1b2/ablator/modules/loggers/tensor.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/metrics/main.py` & `ablator-0.0.1b2/ablator/modules/metrics/main.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/metrics/stores.py` & `ablator-0.0.1b2/ablator/modules/metrics/stores.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/optimizer.py` & `ablator-0.0.1b2/ablator/modules/optimizer.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/scheduler.py` & `ablator-0.0.1b2/ablator/modules/scheduler.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/storage/cloud.py` & `ablator-0.0.1b2/ablator/modules/storage/cloud.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/modules/storage/remote.py` & `ablator-0.0.1b2/ablator/modules/storage/remote.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/utils/base.py` & `ablator-0.0.1b2/ablator/utils/base.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator/utils/file.py` & `ablator-0.0.1b2/ablator/utils/file.py`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/ablator.egg-info/PKG-INFO` & `ablator-0.0.1b2/ablator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablator
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Model Ablation Tool-Kit
 Home-page: https://iordanis.xyz
 Author: Iordanis Fostiropoulos
 Author-email: dev@iordanis.xyz
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ablator-0.0.1b1/ablator.egg-info/SOURCES.txt` & `ablator-0.0.1b2/ablator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablator-0.0.1b1/setup.py` & `ablator-0.0.1b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 package_path = __file__
 setup(
     name="ablator",
-    version="0.0.1b1",
+    version="0.0.1b2",
     author="Iordanis Fostiropoulos",
     author_email="dev@iordanis.xyz",
     url="https://iordanis.xyz",
     packages=find_packages(),
     description="Model Ablation Tool-Kit",
     python_requires=">3.10",
     long_description=Path(package_path).parent.joinpath("README.md").read_text(),
@@ -21,15 +21,15 @@
         "torchvision==0.14.1",
         "tqdm==4.64.1",
         "tensorboardX==2.6",
         "matplotlib==3.7.1",
         "omegaconf==2.2.3",
         "scipy==1.10.1",
         "setproctitle==1.3.2",
-        "ray==2.1.0",
+        "ray>=2.1.0,<=2.2.0",
         "pynvml==11.5.0",
         "optuna==3.1.1",
         "tabulate==0.9.0",
         "seaborn==0.12.2",
         "numpydoc==1.5.0"
     ],
     extras_require={
```

