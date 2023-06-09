# Comparing `tmp/prepper-1.1.4.tar.gz` & `tmp/prepper-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepper-1.1.4.tar", last modified: Mon Apr  3 14:11:20 2023, max compression
+gzip compressed data, was "prepper-1.1.5.tar", last modified: Fri Jun  9 20:50:37 2023, max compression
```

## Comparing `prepper-1.1.4.tar` & `prepper-1.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:11:20.337146 prepper-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:11:20.333146 prepper-1.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:11:20.333146 prepper-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-03 14:10:57.000000 prepper-1.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-03 14:10:57.000000 prepper-1.1.4/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-03 14:10:57.000000 prepper-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-03 14:10:57.000000 prepper-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-03 14:10:57.000000 prepper-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-03 14:11:20.337146 prepper-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-03 14:10:57.000000 prepper-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:11:20.333146 prepper-1.1.4/prepper/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 14:11:20.000000 prepper-1.1.4/prepper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/exportable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26726 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/io_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:11:20.337146 prepper-1.1.4/prepper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/tests/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-03 14:10:57.000000 prepper-1.1.4/prepper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:11:20.337146 prepper-1.1.4/prepper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-03 14:11:20.000000 prepper-1.1.4/prepper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-03 14:11:20.000000 prepper-1.1.4/prepper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:11:20.000000 prepper-1.1.4/prepper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-03 14:11:20.000000 prepper-1.1.4/prepper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 14:11:20.000000 prepper-1.1.4/prepper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-03 14:10:57.000000 prepper-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:11:20.337146 prepper-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-09 20:50:27.000000 prepper-1.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 20:50:27.000000 prepper-1.1.5/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-09 20:50:27.000000 prepper-1.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-09 20:50:27.000000 prepper-1.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-09 20:50:27.000000 prepper-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:50:37.749493 prepper-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 20:50:27.000000 prepper-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/prepper/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/exportable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26985 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/io_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/prepper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/prepper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-09 20:50:27.000000 prepper-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:50:37.749493 prepper-1.1.5/setup.cfg
```

### Comparing `prepper-1.1.4/.github/workflows/python-publish.yml` & `prepper-1.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/.github/workflows/python-test.yml` & `prepper-1.1.5/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/.gitignore` & `prepper-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/.pre-commit-config.yaml` & `prepper-1.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/LICENSE` & `prepper-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/prepper/caching.py` & `prepper-1.1.5/prepper/caching.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/prepper/enums.py` & `prepper-1.1.5/prepper/enums.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/prepper/exportable.py` & `prepper-1.1.5/prepper/exportable.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import uuid
 import warnings
 from abc import ABCMeta
 from inspect import Parameter, signature
 from typing import Any, Dict, List, Tuple
 
 import h5py
+import joblib
 import loguru
 import numpy as np
 
 from prepper import H5StoreException
 from prepper.caching import break_key, make_cache_name
 from prepper.enums import H5StoreTypes
 from prepper.utils import check_equality
@@ -140,14 +141,21 @@
                 for kwkey, kwvalue in value.items():
                     instance._constructor_args[kwkey] = kwvalue
                 continue
             instance._constructor_args[key] = value
 
         return instance
 
+    def __hash__(self):
+        keys = list(self._constructor_args.keys())
+        values = list(self._constructor_args.values())
+
+        digest = joblib.hash(keys + values, hash_name="sha1")
+        return int.from_bytes(bytes(digest, encoding="utf-8"), "big")
+
     def __getnewargs_ex__(self):
         return (), self._constructor_args
 
     def __eq__(self, other) -> bool:
         if not isinstance(self, type(other)):
             return False
 
@@ -178,15 +186,15 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._initialized_from_file = False
 
     @property
     def initialized_from_file(self):
-        return self._initialized_from_file
+        return getattr(self, "_initialized_from_file", False)
 
     @classmethod
     def from_hdf5(cls, path, group="/"):
         if not os.path.exists(path):
             raise FileNotFoundError(f"Could not find file {path}")
 
         with h5py.File(path, mode="r", track_order=True) as hdf5_file:
```

### Comparing `prepper-1.1.4/prepper/io_handlers.py` & `prepper-1.1.5/prepper/io_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,22 @@
                     break
     if class_already_written:
         # This class has already been written to the file, so we just need to write a reference to it
         with h5py.File(file, mode="a", track_order=True) as hdf5_file:
             hdf5_file[group] = h5py.SoftLink(clone_group)
         return existing_groups
 
-    for validator, writer in writers.values():
-        if validator(value):
+    for name, (validator, writer) in writers.items():
+        try:
+            is_valid = validator(value)
+        except Exception as e:
+            msg = f"Failed to check condition {name} for value {value} of type {type(value)}!"
+            loguru.logger.error(msg, exc_info=True)
+            is_valid = False
+        if is_valid:
             attrs, existing_groups = writer(
                 file, group, value, existing_groups
             )
 
             with h5py.File(file, mode="a", track_order=True) as hdf5_file:
                 try:
                     entry = hdf5_file[group]
```

### Comparing `prepper-1.1.4/prepper/tests/test_IO.py` & `prepper-1.1.5/prepper/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/prepper/tests/test_decorators.py` & `prepper-1.1.5/prepper/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/prepper/utils.py` & `prepper-1.1.5/prepper/utils.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/prepper.egg-info/SOURCES.txt` & `prepper-1.1.5/prepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prepper-1.1.4/pyproject.toml` & `prepper-1.1.5/pyproject.toml`

 * *Files identical despite different names*

