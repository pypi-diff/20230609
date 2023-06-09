# Comparing `tmp/cyeva-0.1.0b8.tar.gz` & `tmp/cyeva-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyeva-0.1.0b8.tar", last modified: Wed May 24 06:43:44 2023, max compression
+gzip compressed data, was "cyeva-0.1.0b9.tar", last modified: Thu May 25 03:23:29 2023, max compression
```

## Comparing `cyeva-0.1.0b8.tar` & `cyeva-0.1.0b9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/directions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/directions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/directions/wind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/levels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/levels/precip/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/levels/precip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/levels/wind/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/levels/wind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/core/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/binarize.py
--rw-r--r--   0 runner    (1001) docker     (123)    24657 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/precip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/wind.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/cyeva/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_binarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_precip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_wind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.549342 cyeva-0.1.0b9/cyeva/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.549342 cyeva-0.1.0b9/cyeva/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.549342 cyeva-0.1.0b9/cyeva/config/directions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/config/directions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/config/directions/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/cyeva/config/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/config/levels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/cyeva/config/levels/precip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/config/levels/precip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/cyeva/config/levels/wind/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/config/levels/wind/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/cyeva/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/binarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24657 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/precip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/core/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/cyeva/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/cyeva/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.549342 cyeva-0.1.0b9/cyeva.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-25 03:23:29.000000 cyeva-0.1.0b9/cyeva.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 03:23:29.000000 cyeva-0.1.0b9/cyeva.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:23:29.000000 cyeva-0.1.0b9/cyeva.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 03:23:29.000000 cyeva-0.1.0b9/cyeva.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 03:23:29.000000 cyeva-0.1.0b9/cyeva.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:23:29.553342 cyeva-0.1.0b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_binarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_precip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-25 03:23:17.000000 cyeva-0.1.0b9/tests/test_wind.py
```

### Comparing `cyeva-0.1.0b8/LICENSE` & `cyeva-0.1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/PKG-INFO` & `cyeva-0.1.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyeva
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: A package to evaluate weather forecast correction
 Home-page: https://github.com/caiyunapp/cyeva
 Author: caiyunapp
 Author-email: oss@caiyunapp.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `cyeva-0.1.0b8/README.md` & `cyeva-0.1.0b9/README.md`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/config/directions/wind.py` & `cyeva-0.1.0b9/cyeva/config/directions/wind.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/config/levels/precip/__init__.py` & `cyeva-0.1.0b9/cyeva/config/levels/precip/__init__.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/config/levels/wind/__init__.py` & `cyeva-0.1.0b9/cyeva/config/levels/wind/__init__.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/core/base.py` & `cyeva-0.1.0b9/cyeva/core/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     calc_mae,
     calc_mbe,
     calc_rss,
     calc_chi_square,
     calc_linregress,
     calc_bias_score,
     calc_binary_accuracy_ratio,
+    calc_threshold_accuracy_ratio,
+    calc_threshold_hit_ratio,
+    calc_threshold_miss_ratio,
+    calc_threshold_false_alarm_ratio,
+    calc_threshold_bias_score,
+    calc_threshold_ts,
+    calc_threshold_mae,
 )
 
 
 class Comparison:
     """A base class of comparison between obervation & forecast"""
 
     def __init__(
@@ -215,7 +222,154 @@
         """
         if observation is None:
             observation = self.observation
         if forecast is None:
             forecast = self.forecast
 
         return calc_diff_accuracy_ratio(observation, forecast, limit=limit)
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_accuracy_ratio(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_accuracy_ratio(
+            observation, forecast, threshold=threshold, compare=compare
+        )
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_hit_ratio(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_hit_ratio(
+            observation, forecast, threshold=threshold, compare=compare
+        )
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_miss_ratio(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_miss_ratio(
+            observation, forecast, threshold=threshold, compare=compare
+        )
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_false_alarm_ratio(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_false_alarm_ratio(
+            observation, forecast, threshold=threshold, compare=compare
+        )
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_bias_score(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_bias_score(
+            observation, forecast, threshold=threshold, compare=compare
+        )
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_ts(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_ts(
+            observation, forecast, threshold=threshold, compare=compare
+        )
+
+    @result_round_digit(4)
+    @source_round_digit()
+    def calc_threshold_mae(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        threshold: Number = 1,
+        compare: str = ">=",
+        *args,
+        **kwargs
+    ) -> float:
+
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_threshold_mae(
+            observation, forecast, threshold=threshold, compare=compare
+        )
```

### Comparing `cyeva-0.1.0b8/cyeva/core/binarize.py` & `cyeva-0.1.0b9/cyeva/core/binarize.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/core/precip.py` & `cyeva-0.1.0b9/cyeva/core/precip.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/core/statistic.py` & `cyeva-0.1.0b9/cyeva/core/statistic.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/core/temp.py` & `cyeva-0.1.0b9/cyeva/core/temp.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/core/wind.py` & `cyeva-0.1.0b9/cyeva/core/wind.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva/utils/decorators.py` & `cyeva-0.1.0b9/cyeva/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/cyeva.egg-info/PKG-INFO` & `cyeva-0.1.0b9/cyeva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyeva
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: A package to evaluate weather forecast correction
 Home-page: https://github.com/caiyunapp/cyeva
 Author: caiyunapp
 Author-email: oss@caiyunapp.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `cyeva-0.1.0b8/cyeva.egg-info/SOURCES.txt` & `cyeva-0.1.0b9/cyeva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/setup.py` & `cyeva-0.1.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/tests/test_binarize.py` & `cyeva-0.1.0b9/tests/test_binarize.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/tests/test_errors.py` & `cyeva-0.1.0b9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/tests/test_precip.py` & `cyeva-0.1.0b9/tests/test_precip.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/tests/test_statistic.py` & `cyeva-0.1.0b9/tests/test_statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,13 @@
             "result": -1,
         },
         {"obs": [1, 1, 1, 1, 1], "fct": [2, 2, 2, 2, 2], "result": 0},
     ]
     for case in THRESHOLD_TS_CASE:
         obs = case["obs"]
         fct = case["fct"]
-        threshold = case["threshold"]
         result = case["result"]
         _, _, _result, _ = calc_linregress(obs, fct)
         if not np.isnan(result):
             assert _result == result
         else:
             assert np.isnan(_result)
```

### Comparing `cyeva-0.1.0b8/tests/test_temp.py` & `cyeva-0.1.0b9/tests/test_temp.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b8/tests/test_wind.py` & `cyeva-0.1.0b9/tests/test_wind.py`

 * *Files identical despite different names*

