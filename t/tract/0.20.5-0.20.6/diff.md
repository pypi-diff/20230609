# Comparing `tmp/tract-0.20.5.tar.gz` & `tmp/tract-0.20.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tract-0.20.5.tar", last modified: Fri May 26 07:15:54 2023, max compression
+gzip compressed data, was "tract-0.20.6.tar", last modified: Fri Jun  9 08:58:35 2023, max compression
```

## Comparing `tract-0.20.5.tar` & `tract-0.20.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:54.178110 tract-0.20.5/
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-26 07:15:54.178110 tract-0.20.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-26 07:15:43.000000 tract-0.20.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:15:54.178110 tract-0.20.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 07:15:43.000000 tract-0.20.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:54.178110 tract-0.20.5/tract/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-26 07:15:43.000000 tract-0.20.5/tract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-26 07:15:43.000000 tract-0.20.5/tract/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-26 07:15:43.000000 tract-0.20.5/tract/fact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-26 07:15:43.000000 tract-0.20.5/tract/inference_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-05-26 07:15:43.000000 tract-0.20.5/tract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-26 07:15:43.000000 tract-0.20.5/tract/nnef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-26 07:15:43.000000 tract-0.20.5/tract/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-26 07:15:43.000000 tract-0.20.5/tract/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-26 07:15:43.000000 tract-0.20.5/tract/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:54.178110 tract-0.20.5/tract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-26 07:15:54.000000 tract-0.20.5/tract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 07:15:54.000000 tract-0.20.5/tract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:15:54.000000 tract-0.20.5/tract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:15:53.000000 tract-0.20.5/tract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 07:15:54.000000 tract-0.20.5/tract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 07:15:54.000000 tract-0.20.5/tract.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:58:35.416003 tract-0.20.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-06-09 08:58:35.416003 tract-0.20.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-09 08:58:24.000000 tract-0.20.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:58:35.416003 tract-0.20.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-09 08:58:24.000000 tract-0.20.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:58:35.416003 tract-0.20.6/tract/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-09 08:58:24.000000 tract-0.20.6/tract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-09 08:58:24.000000 tract-0.20.6/tract/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-09 08:58:24.000000 tract-0.20.6/tract/fact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-09 08:58:24.000000 tract-0.20.6/tract/inference_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-09 08:58:24.000000 tract-0.20.6/tract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-09 08:58:24.000000 tract-0.20.6/tract/nnef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-09 08:58:24.000000 tract-0.20.6/tract/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-09 08:58:24.000000 tract-0.20.6/tract/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-09 08:58:24.000000 tract-0.20.6/tract/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:58:35.416003 tract-0.20.6/tract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-06-09 08:58:35.000000 tract-0.20.6/tract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-09 08:58:35.000000 tract-0.20.6/tract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:58:35.000000 tract-0.20.6/tract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:58:35.000000 tract-0.20.6/tract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 08:58:35.000000 tract-0.20.6/tract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 08:58:35.000000 tract-0.20.6/tract.egg-info/top_level.txt
```

### Comparing `tract-0.20.5/PKG-INFO` & `tract-0.20.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tract
-Version: 0.20.5
+Version: 0.20.6
 Summary: Python bindings for tract, a neural network inference engine
 Author: Mathieu Poumeyrol, Sonos, and tract contributors
 Author-email: mathieu@poumeyrol.fr
 License: Apache License, Version 2.0 OR MIT
 Project-URL: Documentation, https://github.com/sonos/tract
 Project-URL: Source, https://github.com/sonos/tract
 Keywords: onnx tensorflow nnef runtime neural network
```

### Comparing `tract-0.20.5/pyproject.toml` & `tract-0.20.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/setup.py` & `tract-0.20.6/setup.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/__init__.py` & `tract-0.20.6/tract/__init__.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/bindings.py` & `tract-0.20.6/tract/bindings.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/fact.py` & `tract-0.20.6/tract/fact.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/inference_model.py` & `tract-0.20.6/tract/inference_model.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/model.py` & `tract-0.20.6/tract/model.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/nnef.py` & `tract-0.20.6/tract/nnef.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/onnx.py` & `tract-0.20.6/tract/onnx.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/runnable.py` & `tract-0.20.6/tract/runnable.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract/value.py` & `tract-0.20.6/tract/value.py`

 * *Files identical despite different names*

### Comparing `tract-0.20.5/tract.egg-info/PKG-INFO` & `tract-0.20.6/tract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tract
-Version: 0.20.5
+Version: 0.20.6
 Summary: Python bindings for tract, a neural network inference engine
 Author: Mathieu Poumeyrol, Sonos, and tract contributors
 Author-email: mathieu@poumeyrol.fr
 License: Apache License, Version 2.0 OR MIT
 Project-URL: Documentation, https://github.com/sonos/tract
 Project-URL: Source, https://github.com/sonos/tract
 Keywords: onnx tensorflow nnef runtime neural network
```

