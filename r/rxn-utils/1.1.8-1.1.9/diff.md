# Comparing `tmp/rxn-utils-1.1.8.tar.gz` & `tmp/rxn-utils-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-utils-1.1.8.tar", last modified: Fri Feb 10 11:57:23 2023, max compression
+gzip compressed data, was "rxn-utils-1.1.9.tar", last modified: Fri Feb 10 13:01:39 2023, max compression
```

## Comparing `rxn-utils-1.1.8.tar` & `rxn-utils-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.997848 rxn-utils-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-10 11:57:22.997848 rxn-utils-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-10 11:57:22.997848 rxn-utils-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.993848 rxn-utils-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.993848 rxn-utils-1.1.8/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.993848 rxn-utils-1.1.8/src/rxn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.993848 rxn-utils-1.1.8/src/rxn/utilities/databases/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/databases/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.993848 rxn-utils-1.1.8/src/rxn/utilities/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/scripts/stable_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/src/rxn/utilities/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.997848 rxn-utils-1.1.8/src/rxn_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-10 11:57:22.000000 rxn-utils-1.1.8/src/rxn_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:57:22.997848 rxn-utils-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_databases_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-10 11:57:14.000000 rxn-utils-1.1.8/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.685262 rxn-utils-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.685262 rxn-utils-1.1.9/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.685262 rxn-utils-1.1.9/src/rxn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/src/rxn/utilities/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/databases/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/src/rxn/utilities/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/scripts/stable_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/src/rxn_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_databases_pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_types.py
```

### Comparing `rxn-utils-1.1.8/LICENSE` & `rxn-utils-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/PKG-INFO` & `rxn-utils-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-utils
-Version: 1.1.8
+Version: 1.1.9
 Summary: General utilities (not related to chemistry)
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `rxn-utils-1.1.8/README.md` & `rxn-utils-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/setup.cfg` & `rxn-utils-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/attrs.py` & `rxn-utils-1.1.9/src/rxn/utilities/attrs.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/basic.py` & `rxn-utils-1.1.9/src/rxn/utilities/basic.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/caching.py` & `rxn-utils-1.1.9/src/rxn/utilities/caching.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/containers.py` & `rxn-utils-1.1.9/src/rxn/utilities/containers.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/databases/pymongo.py` & `rxn-utils-1.1.9/src/rxn/utilities/databases/pymongo.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/files.py` & `rxn-utils-1.1.9/src/rxn/utilities/files.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/logging.py` & `rxn-utils-1.1.9/src/rxn/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/regex.py` & `rxn-utils-1.1.9/src/rxn/utilities/regex.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/scripts/stable_shuffle.py` & `rxn-utils-1.1.9/src/rxn/utilities/scripts/stable_shuffle.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/strings.py` & `rxn-utils-1.1.9/src/rxn/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn/utilities/types.py` & `rxn-utils-1.1.9/src/rxn/utilities/types.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/src/rxn_utils.egg-info/PKG-INFO` & `rxn-utils-1.1.9/src/rxn_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-utils
-Version: 1.1.8
+Version: 1.1.9
 Summary: General utilities (not related to chemistry)
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `rxn-utils-1.1.8/src/rxn_utils.egg-info/SOURCES.txt` & `rxn-utils-1.1.9/src/rxn_utils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/rxn/utilities/__init__.py
 src/rxn/utilities/attrs.py
 src/rxn/utilities/basic.py
 src/rxn/utilities/caching.py
 src/rxn/utilities/containers.py
 src/rxn/utilities/files.py
 src/rxn/utilities/logging.py
+src/rxn/utilities/misc.py
 src/rxn/utilities/py.typed
 src/rxn/utilities/regex.py
 src/rxn/utilities/strings.py
 src/rxn/utilities/types.py
 src/rxn/utilities/databases/__init__.py
 src/rxn/utilities/databases/pymongo.py
 src/rxn/utilities/scripts/__init__.py
@@ -27,10 +28,11 @@
 src/rxn_utils.egg-info/top_level.txt
 tests/test_attrs.py
 tests/test_basic.py
 tests/test_caching.py
 tests/test_containers.py
 tests/test_databases_pymongo.py
 tests/test_files.py
+tests/test_misc.py
 tests/test_regex.py
 tests/test_strings.py
 tests/test_types.py
```

### Comparing `rxn-utils-1.1.8/tests/test_attrs.py` & `rxn-utils-1.1.9/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_basic.py` & `rxn-utils-1.1.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_caching.py` & `rxn-utils-1.1.9/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_containers.py` & `rxn-utils-1.1.9/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_databases_pymongo.py` & `rxn-utils-1.1.9/tests/test_databases_pymongo.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_files.py` & `rxn-utils-1.1.9/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_regex.py` & `rxn-utils-1.1.9/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_strings.py` & `rxn-utils-1.1.9/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.8/tests/test_types.py` & `rxn-utils-1.1.9/tests/test_types.py`

 * *Files identical despite different names*

