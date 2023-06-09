# Comparing `tmp/fuzzing-utils-0.0.3.tar.gz` & `tmp/fuzzing-utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzing-utils-0.0.3.tar", last modified: Fri Jun  9 11:28:52 2023, max compression
+gzip compressed data, was "fuzzing-utils-0.1.0.tar", last modified: Fri Jun  9 12:13:32 2023, max compression
```

## Comparing `fuzzing-utils-0.0.3.tar` & `fuzzing-utils-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/fuzzing_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/fuzzing_utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.787357 fuzzing-utils-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.779358 fuzzing-utils-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.783357 fuzzing-utils-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 12:13:32.787357 fuzzing-utils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 12:13:32.787357 fuzzing-utils-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.783357 fuzzing-utils-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.783357 fuzzing-utils-0.1.0/src/fuzzing_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/fuzzing_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/fuzzing_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/fuzzing_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/fuzzing_utils/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.787357 fuzzing-utils-0.1.0/src/fuzzing_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/fuzzing_utils/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/src/fuzzing_utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.787357 fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 12:13:32.000000 fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 12:13:32.000000 fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:13:32.000000 fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 12:13:32.000000 fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 12:13:32.000000 fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:32.787357 fuzzing-utils-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 12:13:23.000000 fuzzing-utils-0.1.0/tests/test_training.py
```

### Comparing `fuzzing-utils-0.0.3/.gitignore` & `fuzzing-utils-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/LICENSE` & `fuzzing-utils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/PKG-INFO` & `fuzzing-utils-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzing-utils
-Version: 0.0.3
+Version: 0.1.0
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzing-utils-0.0.3/setup.cfg` & `fuzzing-utils-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/src/fuzzing_utils/conversion.py` & `fuzzing-utils-0.1.0/src/fuzzing_utils/conversion.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/src/fuzzing_utils/core.py` & `fuzzing-utils-0.1.0/src/fuzzing_utils/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 
 
 def exit_fuzz() -> None:
     """Exits the program using os._exit(0)"""
     os._exit(0)
 
 
-def save_input(byte_arr: np.ndarray, file_name: str) -> None:
-    """Saves a binary array to a file, with the extension .npy then exits"""
+def save_input(byte_arr: np.ndarray | List, file_name: str) -> None:
+    """Saves a binary array (or list which will be converted using an np.int64 encoding) to a file,
+    with the extension .npy, then exits"""
+    if isinstance(byte_arr, list):
+        byte_arr = np.array(byte_arr, dtype=np.int64)
     byte_arr.tofile(file_name + '.npy')
     exit()
 
 
 def load_input(file_name: str) -> np.ndarray:
     """Loads a binary array from a file, using the data type np.int64"""
     return np.fromfile(file_name, dtype=np.int64)
```

### Comparing `fuzzing-utils-0.0.3/src/fuzzing_utils/data/iris.csv` & `fuzzing-utils-0.1.0/src/fuzzing_utils/data/iris.csv`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/src/fuzzing_utils/training.py` & `fuzzing-utils-0.1.0/src/fuzzing_utils/training.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/PKG-INFO` & `fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzing-utils
-Version: 0.0.3
+Version: 0.1.0
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/SOURCES.txt` & `fuzzing-utils-0.1.0/src/fuzzing_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/tests/test_conversion.py` & `fuzzing-utils-0.1.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.3/tests/test_training.py` & `fuzzing-utils-0.1.0/tests/test_training.py`

 * *Files identical despite different names*

