# Comparing `tmp/fuzzing-utils-0.0.2.tar.gz` & `tmp/fuzzing-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzing-utils-0.0.2.tar", last modified: Fri Jun  9 11:20:32 2023, max compression
+gzip compressed data, was "fuzzing-utils-0.0.3.tar", last modified: Fri Jun  9 11:28:52 2023, max compression
```

## Comparing `fuzzing-utils-0.0.2.tar` & `fuzzing-utils-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.798745 fuzzing-utils-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.798745 fuzzing-utils-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.798745 fuzzing-utils-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/src/fuzzing_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/src/fuzzing_utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/src/fuzzing_utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 11:20:32.000000 fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:32.802745 fuzzing-utils-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 11:20:24.000000 fuzzing-utils-0.0.2/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/fuzzing_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/fuzzing_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/src/fuzzing_utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.298416 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 11:28:52.000000 fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:52.302416 fuzzing-utils-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 11:28:44.000000 fuzzing-utils-0.0.3/tests/test_training.py
```

### Comparing `fuzzing-utils-0.0.2/.gitignore` & `fuzzing-utils-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/LICENSE` & `fuzzing-utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/PKG-INFO` & `fuzzing-utils-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzing-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzing-utils-0.0.2/setup.cfg` & `fuzzing-utils-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/src/fuzzing_utils/conversion.py` & `fuzzing-utils-0.0.3/src/fuzzing_utils/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     """
     Using modf as it may scale better than the above.
     Currently untested.
     """
     return math.modf(to_float(value))[0]
 
 
-def to_positive(value: int | np.int64) -> int:
-    """Converts an int or np.int64 to a positive int"""
+def to_positive(value: int | np.int64 | float) -> int:
+    """Converts an int, np.int64, or float to a positive int or float"""
     return abs(value)
 
 
-def to_positive_or_none(value: int | np.int64) -> int | None:
-    """Positive int or None"""
+def to_positive_or_none(value: int | np.int64 | float) -> int | None:
+    """Converts an int, np.int64, or float to a positive int or float"""
     if value <= 0:
         return None
     else:
         return value
 
 
 def to_greater_than(value: int | np.int64, min_value: int) -> int:
```

### Comparing `fuzzing-utils-0.0.2/src/fuzzing_utils/core.py` & `fuzzing-utils-0.0.3/src/fuzzing_utils/core.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/src/fuzzing_utils/data/iris.csv` & `fuzzing-utils-0.0.3/src/fuzzing_utils/data/iris.csv`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/src/fuzzing_utils/training.py` & `fuzzing-utils-0.0.3/src/fuzzing_utils/training.py`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/PKG-INFO` & `fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzing-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzing-utils-0.0.2/src/fuzzing_utils.egg-info/SOURCES.txt` & `fuzzing-utils-0.0.3/src/fuzzing_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzing-utils-0.0.2/tests/test_conversion.py` & `fuzzing-utils-0.0.3/tests/test_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,24 @@
         assert to_fraction(4696837150979653632) == 0.5
 
     def test_to_positive(self):
         assert to_positive(0) == 0
         assert to_positive(9932) == 9932
         assert to_positive(-1) == 1
         assert to_positive(-665 * 10 ** 15) == 665 * 10 ** 15
+        assert to_positive(0.5) == 0.5
+        assert to_positive(-0.5) == 0.5
 
     def test_to_positive_or_none(self):
         assert to_positive_or_none(0) is None
         assert to_positive_or_none(9932) == 9932
         assert to_positive_or_none(-1) is None
         assert to_positive_or_none(-665 * 10 ** 15) is None
+        assert to_positive_or_none(0.5) == 0.5
+        assert to_positive_or_none(-0.5) is None
 
     def test_to_greater_than(self):
         assert to_greater_than(0, 0) == 0
         assert to_greater_than(0, 9932) == 9932
         assert to_greater_than(100, -1) == 99
         assert to_greater_than(3, -665 * 10 ** 15) == (-665 * 10 ** 15) + 3
         assert to_greater_than(435, -40) == 395
```

### Comparing `fuzzing-utils-0.0.2/tests/test_training.py` & `fuzzing-utils-0.0.3/tests/test_training.py`

 * *Files identical despite different names*

