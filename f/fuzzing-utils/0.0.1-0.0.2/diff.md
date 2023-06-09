# Comparing `tmp/fuzzing-utils-0.0.1.tar.gz` & `tmp/fuzzing-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzing-utils-0.0.1.tar", last modified: Thu Jun  8 18:57:21 2023, max compression
+gzip compressed data, was "fuzzing-utils-0.0.2.tar", last modified: Fri Jun  9 11:20:32 2023, max compression
```

## Comparing `fuzzing-utils-0.0.1.tar` & `fuzzing-utils-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.574206 fuzzing-utils-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.570206 fuzzing-utils-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.570206 fuzzing-utils-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-08 18:57:21.574206 fuzzing-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-08 18:57:21.574206 fuzzing-utils-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.570206 fuzzing-utils-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.570206 fuzzing-utils-0.0.1/src/fuzzing_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/fuzzing_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/fuzzing_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/fuzzing_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/fuzzing_utils/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.574206 fuzzing-utils-0.0.1/src/fuzzing_utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/fuzzing_utils/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/src/fuzzing_utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.570206 fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-08 18:57:21.000000 fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-08 18:57:21.000000 fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:57:21.000000 fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 18:57:21.000000 fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 18:57:21.000000 fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:21.574206 fuzzing-utils-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 18:57:13.000000 fuzzing-utils-0.0.1/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.798745 fuzzing-utils-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.798745 fuzzing-utils-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.798745 fuzzing-utils-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/src/fuzzing_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/src/fuzzing_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/test_training.py
```

### Comparing `fuzzing-utils-0.0.1/.gitignore` & `fuzzing-utils-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/LICENSE` & `fuzzing-utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/PKG-INFO` & `fuzzing-utils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzing-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzing-utils-0.0.1/setup.cfg` & `fuzzing-utils-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/src/fuzzing_utils/conversion.py` & `fuzzing-utils-0.0.2/src/fuzzing_utils/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import struct
 import math
 from typing import Callable, Dict
 
 import numpy as np
 
 
+def select_from(value: int | np.int64, options: list[any]) -> any:
+    """Selects a value from a list of options"""
+    return options[value % len(options)]
+
+
 def to_float(value: int | np.int64) -> float:
     """Converts an int or np.int64 to a float value, if nan or inf, returns 0.0"""
     packed = struct.pack('>q', value)
     unpacked = struct.unpack('>d', packed)[0]
 
     if math.isnan(unpacked) or math.isinf(unpacked):
         return 0.0
```

### Comparing `fuzzing-utils-0.0.1/src/fuzzing_utils/core.py` & `fuzzing-utils-0.0.2/src/fuzzing_utils/core.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/src/fuzzing_utils/data/iris.csv` & `fuzzing-utils-0.0.2/src/fuzzing_utils/data/iris.csv`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/src/fuzzing_utils/training.py` & `fuzzing-utils-0.0.2/src/fuzzing_utils/training.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/PKG-INFO` & `fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzing-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzing-utils-0.0.1/src/fuzzing_utils.egg-info/SOURCES.txt` & `fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.1/tests/test_conversion.py` & `fuzzing-utils-0.0.2/tests/test_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from src.fuzzing_utils.conversion import to_float, to_fraction, to_positive, to_positive_or_none, to_greater_than, \
-    to_greater_than_or_none, to_positive_integer_or_fraction, to_reserved_or_else, NotReserved
+    to_greater_than_or_none, to_positive_integer_or_fraction, to_reserved_or_else, NotReserved, select_from
 
 
 class TestConversion:
+    def test_select_from(self):
+        assert select_from(0, [1, 2, 3]) == 1
+        assert select_from(1, [1, 2, 3]) == 2
+        assert select_from(2, [1, 2, 3]) == 3
+        assert select_from(3, [1, 2, 3]) == 1
+
     def test_to_float(self):
         assert to_float(0) == 0.0
         assert to_float(9932) == 4.907e-320
         assert to_float(-1) == 0.0
         assert to_float(-665 * 10 ** 15) == -1.3505803869538944e+264
         assert to_float(4696837150979653632) == 1000000.5
```

### Comparing `fuzzing-utils-0.0.1/tests/test_training.py` & `fuzzing-utils-0.0.2/tests/test_training.py`

 * *Files identical despite different names*

