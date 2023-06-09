# Comparing `tmp/geolibs-0.0.7.tar.gz` & `tmp/geolibs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolibs-0.0.7.tar", max compression
+gzip compressed data, was "geolibs-0.0.8.tar", max compression
```

## Comparing `geolibs-0.0.7.tar` & `geolibs-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.7/README.rst
--rwxr-xr-x   0        0        0      512 2023-05-15 23:28:10.304224 geolibs-0.0.7/geolibs/__init__.py
--rwxr-xr-x   0        0        0    12311 2023-05-15 23:27:54.339092 geolibs-0.0.7/geolibs/engine_cocoext.py
--rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.7/geolibs/engine_cocometric.py
--rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.7/geolibs/engine_csv.py
--rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.7/geolibs/enginelogger_hook.py
--rwxr-xr-x   0        0        0    12195 2023-05-15 22:23:50.825583 geolibs-0.0.7/geolibs/loading.py
--rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.7/geolibs/misc.py
--rwxr-xr-x   0        0        0     1066 2023-05-15 23:28:10.298099 geolibs-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.8/README.rst
+-rwxr-xr-x   0        0        0      512 2023-05-16 14:51:22.214266 geolibs-0.0.8/geolibs/__init__.py
+-rwxr-xr-x   0        0        0    15831 2023-05-16 13:41:13.691179 geolibs-0.0.8/geolibs/engine_cocoext.py
+-rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.8/geolibs/engine_cocometric.py
+-rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.8/geolibs/engine_csv.py
+-rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.8/geolibs/enginelogger_hook.py
+-rwxr-xr-x   0        0        0    12195 2023-05-15 22:23:50.825583 geolibs-0.0.8/geolibs/loading.py
+-rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.8/geolibs/misc.py
+-rwxr-xr-x   0        0        0     1066 2023-05-16 14:51:22.206745 geolibs-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.8/PKG-INFO
```

### Comparing `geolibs-0.0.7/README.rst` & `geolibs-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.7/geolibs/__init__.py` & `geolibs-0.0.8/geolibs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from .engine_cocoext import EngineCocoExt
 from .engine_csv import EngineCSV
 from .loading import LoadBandsFromFile, LoadVariableSizedBandsFromFile, LoadMasks
 from .engine_cocometric import EngineCocoMetric
 
 __author__ = """Sagar Verma"""
 __email__ = 'sagar@granular.ai'
-__version__ = 'v0.0.7'
+__version__ = 'v0.0.8'
 
 __all__ = ["EngineLoggerHook", "EngineCocoExt", "EngineCocoMetric",
            "EngineCSV", "LoadBandsFromFile", "LoadVariableSizedBandsFromFile",
            "LoadMasks"]
```

### Comparing `geolibs-0.0.7/geolibs/engine_cocometric.py` & `geolibs-0.0.8/geolibs/engine_cocometric.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.7/geolibs/engine_csv.py` & `geolibs-0.0.8/geolibs/engine_csv.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.7/geolibs/enginelogger_hook.py` & `geolibs-0.0.8/geolibs/enginelogger_hook.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.7/geolibs/loading.py` & `geolibs-0.0.8/geolibs/loading.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.7/geolibs/misc.py` & `geolibs-0.0.8/geolibs/misc.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.7/pyproject.toml` & `geolibs-0.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geolibs"
-version = "v0.0.7"
+version = "v0.0.8"
 description = "A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development."
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "geolibs"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `geolibs-0.0.7/PKG-INFO` & `geolibs-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolibs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 Home-page: https://github.com/granularai/geolibs
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

