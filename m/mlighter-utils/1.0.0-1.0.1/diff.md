# Comparing `tmp/mlighter-utils-1.0.0.tar.gz` & `tmp/mlighter-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlighter-utils-1.0.0.tar", last modified: Fri Jun  9 12:47:56 2023, max compression
+gzip compressed data, was "mlighter-utils-1.0.1.tar", last modified: Fri Jun  9 15:13:20 2023, max compression
```

## Comparing `mlighter-utils-1.0.0.tar` & `mlighter-utils-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.363988 mlighter-utils-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.359988 mlighter-utils-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.359988 mlighter-utils-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-09 12:47:56.363988 mlighter-utils-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-09 12:47:56.363988 mlighter-utils-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.359988 mlighter-utils-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.359988 mlighter-utils-1.0.0/src/fuzzing_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/fuzzing_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/fuzzing_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/fuzzing_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/fuzzing_utils/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.359988 mlighter-utils-1.0.0/src/fuzzing_utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/fuzzing_utils/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/src/fuzzing_utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.363988 mlighter-utils-1.0.0/src/mlighter_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-09 12:47:56.000000 mlighter-utils-1.0.0/src/mlighter_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-09 12:47:56.000000 mlighter-utils-1.0.0/src/mlighter_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:47:56.000000 mlighter-utils-1.0.0/src/mlighter_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 12:47:56.000000 mlighter-utils-1.0.0/src/mlighter_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 12:47:56.000000 mlighter-utils-1.0.0/src/mlighter_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:56.363988 mlighter-utils-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 12:47:48.000000 mlighter-utils-1.0.0/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.980915 mlighter-utils-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.980915 mlighter-utils-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.980915 mlighter-utils-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/src/mlighter_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/mlighter_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/mlighter_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/mlighter_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/mlighter_utils/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/src/mlighter_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/mlighter_utils/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/src/mlighter_utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/src/mlighter_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 15:13:20.000000 mlighter-utils-1.0.1/src/mlighter_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 15:13:20.000000 mlighter-utils-1.0.1/src/mlighter_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:13:20.000000 mlighter-utils-1.0.1/src/mlighter_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 15:13:20.000000 mlighter-utils-1.0.1/src/mlighter_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 15:13:20.000000 mlighter-utils-1.0.1/src/mlighter_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:20.984916 mlighter-utils-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-09 15:13:12.000000 mlighter-utils-1.0.1/tests/test_training.py
```

### Comparing `mlighter-utils-1.0.0/.gitignore` & `mlighter-utils-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/LICENSE` & `mlighter-utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/PKG-INFO` & `mlighter-utils-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: mlighter-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# FuzzingUtils
+# MLighterUtils
 A set of utility functions for testing templates within [MLighter](https://github.com/hdg7/mlighter)
 
+
+## Credit
 The data used comes from [here](https://github.com/jbrownlee/Datasets/)
```

### Comparing `mlighter-utils-1.0.0/setup.cfg` & `mlighter-utils-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/src/fuzzing_utils/conversion.py` & `mlighter-utils-1.0.1/src/mlighter_utils/conversion.py`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/src/fuzzing_utils/core.py` & `mlighter-utils-1.0.1/src/mlighter_utils/core.py`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/src/fuzzing_utils/data/iris.csv` & `mlighter-utils-1.0.1/src/mlighter_utils/data/iris.csv`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/src/fuzzing_utils/training.py` & `mlighter-utils-1.0.1/src/mlighter_utils/training.py`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.0.0/src/mlighter_utils.egg-info/PKG-INFO` & `mlighter-utils-1.0.1/src/mlighter_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: mlighter-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# FuzzingUtils
+# MLighterUtils
 A set of utility functions for testing templates within [MLighter](https://github.com/hdg7/mlighter)
 
+
+## Credit
 The data used comes from [here](https://github.com/jbrownlee/Datasets/)
```

### Comparing `mlighter-utils-1.0.0/tests/test_conversion.py` & `mlighter-utils-1.0.1/tests/test_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.fuzzing_utils.conversion import to_float, to_fraction, to_positive, to_positive_or_none, to_greater_than, \
+from src.mlighter_utils.conversion import to_float, to_fraction, to_positive, to_positive_or_none, to_greater_than, \
     to_greater_than_or_none, to_positive_integer_or_fraction, to_reserved_or_else, NotReserved, select_from
 
 
 class TestConversion:
     def test_select_from(self):
         assert select_from(0, [1, 2, 3]) == 1
         assert select_from(1, [1, 2, 3]) == 2
```

### Comparing `mlighter-utils-1.0.0/tests/test_training.py` & `mlighter-utils-1.0.1/tests/test_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.fuzzing_utils.training import get_default_dataset, extract_xy_train
+from src.mlighter_utils.training import get_default_dataset, extract_xy_train
 
 
 class TestTraining:
     def test_get_default_dataset(self):
         df = get_default_dataset()
         assert df is not None
         assert df.iloc[137].tolist() == [6.4, 3.1, 5.5, 1.8, 'Iris-virginica']
```

