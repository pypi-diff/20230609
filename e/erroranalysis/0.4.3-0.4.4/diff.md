# Comparing `tmp/erroranalysis-0.4.3.tar.gz` & `tmp/erroranalysis-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/erroranalysis-0.4.3.tar", last modified: Wed Apr 26 01:12:10 2023, max compression
+gzip compressed data, was "dist/erroranalysis-0.4.4.tar", last modified: Fri Jun  9 16:58:36 2023, max compression
```

## Comparing `erroranalysis-0.4.3.tar` & `erroranalysis-0.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/cohort_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_report/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/matrix_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/process_categoricals.py
--rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/surrogate_error_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32082 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/analyzer/error_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/ebm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/gbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/report/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/report/error_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_cohort_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_error_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)    32660 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_matrix_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_pyspark_surrogate_error_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_root_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_surrogate_error_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/cohort_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/_internal/error_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/error_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/_internal/error_report/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/error_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/matrix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/process_categoricals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41676 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/surrogate_error_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/_internal/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32091 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/analyzer/error_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/error_correlation_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/error_correlation_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/error_correlation_methods/ebm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/error_correlation_methods/gbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/report/error_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/erroranalysis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/erroranalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:58:36.000000 erroranalysis-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_cohort_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_error_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32680 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_matrix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_pyspark_surrogate_error_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_root_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-06-09 16:57:42.000000 erroranalysis-0.4.4/tests/test_surrogate_error_tree.py
```

### Comparing `erroranalysis-0.4.3/LICENSE` & `erroranalysis-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/PKG-INFO` & `erroranalysis-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroranalysis
-Version: 0.4.3
+Version: 0.4.4
 Summary: Core error analysis APIs
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `erroranalysis-0.4.3/README.md` & `erroranalysis-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/cohort_filter.py` & `erroranalysis-0.4.4/erroranalysis/_internal/cohort_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/constants.py` & `erroranalysis-0.4.4/erroranalysis/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/matrix_filter.py` & `erroranalysis-0.4.4/erroranalysis/_internal/matrix_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/metrics.py` & `erroranalysis-0.4.4/erroranalysis/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/process_categoricals.py` & `erroranalysis-0.4.4/erroranalysis/_internal/process_categoricals.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/surrogate_error_tree.py` & `erroranalysis-0.4.4/erroranalysis/_internal/surrogate_error_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,29 +298,29 @@
         pred_y = filtered_df[PRED_Y]
         dropped_cols.append(PRED_Y)
     input_data = filtered_df.drop(columns=dropped_cols)
     is_pandas = isinstance(analyzer.dataset, pd.DataFrame)
     if is_pandas:
         true_y = true_y.to_numpy()
     else:
-        input_data = input_data.to_numpy()
+        input_data = input_data.to_numpy(copy=True)
     if is_model_analyzer:
         pred_y = analyzer.model.predict(input_data)
     if analyzer.model_task == ModelTask.CLASSIFICATION:
         diff = pred_y != true_y
     else:
         diff = pred_y - true_y
     if not isinstance(diff, np.ndarray):
         diff = np.array(diff)
     if not isinstance(pred_y, np.ndarray):
         pred_y = np.array(pred_y)
     if not isinstance(true_y, np.ndarray):
         true_y = np.array(true_y)
     if is_pandas:
-        input_data = input_data.to_numpy()
+        input_data = input_data.to_numpy(copy=True)
 
     if analyzer.categorical_features:
         # Inplace replacement of columns
         if len(input_data) != len(analyzer.string_indexed_data):
             _, _, _, string_indexed_data = \
                 process_categoricals(
                     all_feature_names=analyzer._feature_names,
```

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/utils.py` & `erroranalysis-0.4.4/erroranalysis/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/_internal/version_checker.py` & `erroranalysis-0.4.4/erroranalysis/_internal/version_checker.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/analyzer/error_analyzer.py` & `erroranalysis-0.4.4/erroranalysis/analyzer/error_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
         :return: The computed importances or correlation between the
             features and error.
         :rtype: list[float]
         """
         input_data = self.dataset
         diff = self.get_diff()
         if isinstance(self.dataset, pd.DataFrame):
-            input_data = input_data.to_numpy()
+            input_data = input_data.to_numpy(copy=True)
         if self.categorical_features:
             # Inplace replacement of columns
             indexes = self.categorical_indexes
             string_ind_data = self.string_indexed_data
             for idx, c_i in enumerate(indexes):
                 input_data[:, c_i] = string_ind_data[:, idx]
         # for very large number of rows mutual information
```

### Comparing `erroranalysis-0.4.3/erroranalysis/error_correlation_methods/ebm.py` & `erroranalysis-0.4.4/erroranalysis/error_correlation_methods/ebm.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/error_correlation_methods/gbm.py` & `erroranalysis-0.4.4/erroranalysis/error_correlation_methods/gbm.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis/report/error_report.py` & `erroranalysis-0.4.4/erroranalysis/report/error_report.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/erroranalysis.egg-info/PKG-INFO` & `erroranalysis-0.4.4/erroranalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroranalysis
-Version: 0.4.3
+Version: 0.4.4
 Summary: Core error analysis APIs
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `erroranalysis-0.4.3/erroranalysis.egg-info/SOURCES.txt` & `erroranalysis-0.4.4/erroranalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/setup.py` & `erroranalysis-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/tests/test_cohort_filter.py` & `erroranalysis-0.4.4/tests/test_cohort_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from erroranalysis._internal.cohort_filter import filter_from_cohort
-from erroranalysis._internal.constants import (PRED_Y, ROW_INDEX, TRUE_Y,
-                                               ModelTask)
+from erroranalysis._internal.constants import (ARG, COLUMN, METHOD, PRED_Y,
+                                               ROW_INDEX, TRUE_Y, ModelTask)
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
 from rai_test_utils.datasets.tabular import (create_diabetes_data,
                                              create_iris_data,
                                              create_simple_titanic_data)
 from rai_test_utils.models.sklearn import (
     create_sklearn_random_forest_regressor, create_sklearn_svm_classifier,
     create_titanic_pipeline)
+from raiutils.cohort import CohortFilterMethods
 
 TOL = 1e-10
 SEPAL_WIDTH = 'sepal width'
 EMBARKED = 'embarked'
 CLASSIFICATION_OUTCOME = 'Classification outcome'
 REGRESSION_ERROR = 'Regression error'
 
 
 class TestCohortFilter(object):
 
     def test_cohort_filter_equal(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
-        filters = [{'arg': [2.8],
-                    'column': SEPAL_WIDTH,
-                    'method': 'equal'}]
+        filters = [{ARG: [2.8],
+                    COLUMN: SEPAL_WIDTH,
+                    METHOD: CohortFilterMethods.METHOD_EQUAL}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[X_test[SEPAL_WIDTH] == 2.8]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
                            model,
@@ -49,17 +50,17 @@
     @pytest.mark.parametrize('use_str_labels', [True, False])
     def test_cohort_filter_target(self, use_str_labels, target_type):
         if target_type == 'Predicted Y':
             pytest.skip("Skipping this test due to a bug condition "
                         "in Predicted Y cohort filtering")
         X_train, X_test, y_train, y_test, feature_names, classes = \
             create_iris_pandas(use_str_labels)
-        filters = [{'arg': [2],
-                    'column': target_type,
-                    'method': 'includes'}]
+        filters = [{ARG: [2],
+                    COLUMN: target_type,
+                    METHOD: CohortFilterMethods.METHOD_INCLUDES}]
         validation_data = create_validation_data(X_test, y_test)
         if use_str_labels:
             validation_filter = y_test == classes[2]
         else:
             classes = np.unique(y_test).tolist()
             validation_filter = y_test == 2
         validation_data = validation_data.loc[validation_filter]
@@ -75,17 +76,17 @@
                            model_task,
                            filters=filters,
                            classes=classes)
 
     def test_cohort_filter_less(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
-        filters = [{'arg': [2.8],
-                    'column': SEPAL_WIDTH,
-                    'method': 'less'}]
+        filters = [{ARG: [2.8],
+                    COLUMN: SEPAL_WIDTH,
+                    METHOD: CohortFilterMethods.METHOD_LESS}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[X_test[SEPAL_WIDTH] < 2.8]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
                            model,
@@ -96,17 +97,17 @@
                            model_task,
                            filters=filters)
 
     def test_cohort_filter_less_and_equal(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
 
-        filters = [{'arg': [2.8],
-                    'column': SEPAL_WIDTH,
-                    'method': 'less and equal'}]
+        filters = [{ARG: [2.8],
+                    COLUMN: SEPAL_WIDTH,
+                    METHOD: CohortFilterMethods.METHOD_LESS_AND_EQUAL}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[X_test[SEPAL_WIDTH] <= 2.8]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
                            model,
@@ -116,17 +117,17 @@
                            categorical_features,
                            model_task,
                            filters=filters)
 
     def test_cohort_filter_greater(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
-        filters = [{'arg': [2.8],
-                    'column': SEPAL_WIDTH,
-                    'method': 'greater'}]
+        filters = [{ARG: [2.8],
+                    COLUMN: SEPAL_WIDTH,
+                    METHOD: CohortFilterMethods.METHOD_GREATER}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[X_test[SEPAL_WIDTH] > 2.8]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
                            model,
@@ -136,17 +137,17 @@
                            categorical_features,
                            model_task,
                            filters=filters)
 
     def test_cohort_filter_greater_and_equal(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
-        filters = [{'arg': [2.8],
-                    'column': SEPAL_WIDTH,
-                    'method': 'greater and equal'}]
+        filters = [{ARG: [2.8],
+                    COLUMN: SEPAL_WIDTH,
+                    METHOD: CohortFilterMethods.METHOD_GREATER_AND_EQUAL}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[X_test[SEPAL_WIDTH] >= 2.8]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
                            model,
@@ -156,17 +157,17 @@
                            categorical_features,
                            model_task,
                            filters=filters)
 
     def test_cohort_filter_in_the_range_of(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
-        filters = [{'arg': [2.8, 3.4],
-                    'column': SEPAL_WIDTH,
-                    'method': 'in the range of'}]
+        filters = [{ARG: [2.8, 3.4],
+                    COLUMN: SEPAL_WIDTH,
+                    METHOD: CohortFilterMethods.METHOD_RANGE}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[
             (X_test[SEPAL_WIDTH] <= 3.4) & (X_test[SEPAL_WIDTH] >= 2.8)]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
@@ -186,17 +187,17 @@
             create_iris_pandas()
         model = create_sklearn_svm_classifier(X_train, y_train)
         model_task = ModelTask.CLASSIFICATION
         categorical_features = []
 
         # the index 1, corresponds to incorrect prediction
         # the index 0 correspond to correct prediction
-        filters = [{'arg': arg,
-                    'column': CLASSIFICATION_OUTCOME,
-                    'method': 'includes'}]
+        filters = [{ARG: arg,
+                    COLUMN: CLASSIFICATION_OUTCOME,
+                    METHOD: CohortFilterMethods.METHOD_INCLUDES}]
         pred_y = model.predict(X_test)
         validation_data = create_validation_data(X_test, y_test, pred_y)
         if correct_prediction:
             validation_filter = validation_data[PRED_Y] == validation_data[
                 TRUE_Y]
         else:
             validation_filter = validation_data[PRED_Y] != validation_data[
@@ -217,17 +218,17 @@
     def test_cohort_filter_includes(self):
         X_train, X_test, y_train, y_test, numeric, categorical = \
             create_simple_titanic_data()
         feature_names = categorical + numeric
         clf = create_titanic_pipeline(X_train, y_train)
         categorical_features = categorical
         # the indexes 0, 2 correspond to S, C
-        filters = [{'arg': [0, 2],
-                    'column': EMBARKED,
-                    'method': 'includes'}]
+        filters = [{ARG: [0, 2],
+                    COLUMN: EMBARKED,
+                    METHOD: CohortFilterMethods.METHOD_INCLUDES}]
         validation_data = create_validation_data(X_test, y_test)
         filter_embarked = X_test[EMBARKED].isin(['S', 'C'])
         validation_data = validation_data.loc[filter_embarked]
         model_task = ModelTask.CLASSIFICATION
         run_error_analyzer(validation_data,
                            clf,
                            X_test,
@@ -240,17 +241,17 @@
     def test_cohort_filter_excludes(self):
         X_train, X_test, y_train, y_test, numeric, categorical = \
             create_simple_titanic_data()
         feature_names = categorical + numeric
         clf = create_titanic_pipeline(X_train, y_train)
         categorical_features = categorical
         # the indexes other than 0, 2 correspond to Q
-        filters = [{'arg': [0, 2],
-                    'column': EMBARKED,
-                    'method': 'excludes'}]
+        filters = [{ARG: [0, 2],
+                    COLUMN: EMBARKED,
+                    METHOD: CohortFilterMethods.METHOD_EXCLUDES}]
         validation_data = create_validation_data(X_test, y_test)
         filter_embarked = X_test[EMBARKED].isin(['Q'])
         validation_data = validation_data.loc[filter_embarked]
         model_task = ModelTask.CLASSIFICATION
         run_error_analyzer(validation_data,
                            clf,
                            X_test,
@@ -265,17 +266,17 @@
         X_train, X_test, y_train, y_test, numeric, categorical = \
             create_simple_titanic_data()
         feature_names = categorical + numeric
         clf = create_titanic_pipeline(X_train, y_train)
         categorical_features = categorical
         # the indexes 1, 2 correspond to false positives and false negatives
         # the indexes 0, 3 correspond to true positives and true negatives
-        filters = [{'arg': arg,
-                    'column': CLASSIFICATION_OUTCOME,
-                    'method': 'includes'}]
+        filters = [{ARG: arg,
+                    COLUMN: CLASSIFICATION_OUTCOME,
+                    METHOD: CohortFilterMethods.METHOD_INCLUDES}]
         pred_y = clf.predict(X_test)
         validation_data = create_validation_data(X_test, y_test, pred_y)
         if not outcome:
             validation_filter = validation_data[PRED_Y] != validation_data[
                 TRUE_Y]
         else:
             validation_filter = validation_data[PRED_Y] == validation_data[
@@ -292,17 +293,17 @@
                            model_task,
                            filters=filters)
 
     def test_cohort_filter_index(self):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_iris_pandas()
         # filter on index, which can be done from the RAI dashboard
-        filters = [{'arg': [40],
-                    'column': ROW_INDEX,
-                    'method': 'less and equal'}]
+        filters = [{ARG: [40],
+                    COLUMN: ROW_INDEX,
+                    METHOD: CohortFilterMethods.METHOD_LESS_AND_EQUAL}]
         validation_data = create_validation_data(X_test, y_test)
         validation_data = validation_data.loc[validation_data[ROW_INDEX] <= 40]
         model_task = ModelTask.CLASSIFICATION
         model = create_sklearn_svm_classifier(X_train, y_train)
         categorical_features = []
         run_error_analyzer(validation_data,
                            model,
@@ -317,17 +318,17 @@
         X_train, X_test, y_train, y_test, feature_names = \
             create_diabetes_data()
         X_train = pd.DataFrame(X_train, columns=feature_names)
         X_test = pd.DataFrame(X_test, columns=feature_names)
 
         # filter on regression error, which can be done from the
         # RAI dashboard
-        filters = [{'arg': [40],
-                    'column': REGRESSION_ERROR,
-                    'method': 'less and equal'}]
+        filters = [{ARG: [40],
+                    COLUMN: REGRESSION_ERROR,
+                    METHOD: CohortFilterMethods.METHOD_LESS_AND_EQUAL}]
 
         model = create_sklearn_random_forest_regressor(X_train, y_train)
         pred_y = model.predict(X_test)
 
         validation_data = create_validation_data(X_test, y_test, pred_y)
         validation_filter = abs(validation_data[PRED_Y] - validation_data[
             TRUE_Y]) <= 40.0
```

### Comparing `erroranalysis-0.4.3/tests/test_error_report.py` & `erroranalysis-0.4.4/tests/test_error_report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
-import uuid
-
 import numpy as np
 import pandas as pd
 import pytest
 
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
 from erroranalysis._internal.error_report import ErrorReport
 from rai_test_utils.datasets.tabular import (create_cancer_data,
                                              create_housing_data,
-                                             create_iris_data)
+                                             create_iris_data,
+                                             create_simple_titanic_data)
 from rai_test_utils.models.model_utils import (create_models_classification,
                                                create_models_regression)
+from rai_test_utils.models.sklearn import \
+    create_complex_classification_pipeline
+from rai_test_utils.utilities import is_valid_uuid
 
 
 class TestErrorReport(object):
 
     @pytest.mark.parametrize('alter_feature_names', [True, False])
     def test_error_report_iris(self, alter_feature_names):
         X_train, X_test, y_train, y_test, feature_names, _ = \
@@ -75,21 +77,29 @@
 
         for model in models:
             categorical_features = []
             run_error_analyzer(model, X_test, y_test, feature_names,
                                categorical_features,
                                filter_features=filter_features)
 
-
-def is_valid_uuid(id):
-    try:
-        uuid.UUID(str(id))
-        return True
-    except ValueError:
-        return False
+    def test_error_report_titanic(self):
+        X_train, X_test, y_train, y_test, numeric, categorical = \
+            create_simple_titanic_data()
+
+        # Drop all numeric features
+        X_train = X_train.drop(['pclass', 'age', 'fare'], axis=1)
+        X_test = X_test.drop(['pclass', 'age', 'fare'], axis=1)
+
+        clf = create_complex_classification_pipeline(
+            X_train, y_train, [], ['embarked', 'sex'])
+
+        # Pass the remaining categorical features
+        run_error_analyzer(clf, X_test, y_test, ['embarked', 'sex'],
+                           ['embarked', 'sex'],
+                           filter_features=[])
 
 
 def run_error_analyzer(model, X_test, y_test, feature_names,
                        categorical_features, expect_user_warnings=False,
                        filter_features=None):
     if expect_user_warnings and pd.__version__[0] == '0':
         with pytest.warns(UserWarning,
```

### Comparing `erroranalysis-0.4.3/tests/test_importances.py` & `erroranalysis-0.4.4/tests/test_importances.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,19 @@
                                        categorical_features)
         model_analyzer.compute_importances(error_correlation_method)
         t1 = time.time()
         execution_time = t1 - t0
         print(execution_time)
         # assert we don't take too long and downsample the dataset
         # note execution time is in seconds
-        assert execution_time < 20
+        # note GBM_SHAP is slower than the other methods
+        if error_correlation_method == GBM_SHAP:
+            assert execution_time < 35
+        else:
+            assert execution_time < 25
 
     @pytest.mark.parametrize('num_rows', [1, 2, 3, 4])
     @pytest.mark.parametrize('error_correlation_method',
                              [MUTUAL_INFO, EBM, GBM_SHAP])
     def test_small_data_importances(self, num_rows, error_correlation_method):
         # validate we can run on very few rows
         X_train, y_train, X_test, y_test, _ = \
```

### Comparing `erroranalysis-0.4.3/tests/test_matrix_filter.py` & `erroranalysis-0.4.4/tests/test_matrix_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from erroranalysis._internal.cohort_filter import filter_from_cohort
-from erroranalysis._internal.constants import (ROW_INDEX, TRUE_Y, MatrixParams,
-                                               Metrics, ModelTask, f1_metrics,
+from erroranalysis._internal.constants import (ARG, COLUMN, METHOD, ROW_INDEX,
+                                               TRUE_Y, MatrixParams, Metrics,
+                                               ModelTask, f1_metrics,
                                                metric_to_display_name,
                                                precision_metrics,
                                                recall_metrics)
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
 from erroranalysis._internal.matrix_filter import (CATEGORY1, CATEGORY2, COUNT,
                                                    FALSE_COUNT, FN, FP,
                                                    INTERVAL_MAX, INTERVAL_MIN,
@@ -46,34 +47,34 @@
                                      y_test, feature_names, model_task)
 
     def test_matrix_filter_iris_filters(self):
         # Validate the shift cohort functionality where base
         # cohort was chosen in tree view
         X_train, X_test, y_train, y_test, feature_names, _ = create_iris_data()
 
-        filters = [{'arg': [2.85],
-                    'column': feature_names[1],
-                    'method': 'less and equal'}]
+        filters = [{ARG: [2.85],
+                    COLUMN: feature_names[1],
+                    METHOD: 'less and equal'}]
 
         model_task = ModelTask.CLASSIFICATION
         run_error_analyzer_on_models(X_train, y_train, X_test,
                                      y_test, feature_names,
                                      model_task, filters=filters)
 
     def test_matrix_filter_iris_filters_pandas(self):
         # Validate the shift cohort functionality where base
         # cohort was chosen in tree view
         X_train, X_test, y_train, y_test, feature_names, _ = create_iris_data()
 
         X_train = pd.DataFrame(X_train, columns=feature_names)
         X_test = pd.DataFrame(X_test, columns=feature_names)
 
-        filters = [{'arg': [2.85],
-                    'column': feature_names[1],
-                    'method': 'less and equal'}]
+        filters = [{ARG: [2.85],
+                    COLUMN: feature_names[1],
+                    METHOD: 'less and equal'}]
 
         model_task = ModelTask.CLASSIFICATION
         run_error_analyzer_on_models(X_train, y_train, X_test,
                                      y_test, feature_names,
                                      model_task, filters=filters)
 
     def test_matrix_filter_iris_quantile_binning(self):
@@ -218,32 +219,32 @@
         # Validate the shift cohort functionality where base
         # cohort was chosen in matrix view
         (X_train, X_test, y_train, y_test,
             feature_names, _) = create_cancer_data()
 
         composite_filters = [{'compositeFilters':
                              [{'compositeFilters':
-                              [{'arg': [11.364, 13.182],
-                                'column': 'mean radius',
-                                'method': 'in the range of'}],
+                              [{ARG: [11.364, 13.182],
+                                COLUMN: 'mean radius',
+                                METHOD: 'in the range of'}],
                                'operation': 'and'},
                               {'compositeFilters':
-                               [{'arg': [13.182, 15],
-                                 'column': 'mean radius',
-                                 'method': 'in the range of'}],
+                               [{ARG: [13.182, 15],
+                                 COLUMN: 'mean radius',
+                                 METHOD: 'in the range of'}],
                                'operation': 'and'},
                               {'compositeFilters':
-                               [{'arg': [15, 16.817],
-                                 'column': 'mean radius',
-                                 'method': 'in the range of'}],
+                               [{ARG: [15, 16.817],
+                                 COLUMN: 'mean radius',
+                                 METHOD: 'in the range of'}],
                                'operation': 'and'},
                               {'compositeFilters':
-                               [{'arg': [16.817, 18.635],
-                                 'column': 'mean radius',
-                                 'method': 'in the range of'}],
+                               [{ARG: [16.817, 18.635],
+                                 COLUMN: 'mean radius',
+                                 METHOD: 'in the range of'}],
                                'operation': 'and'}],
                              'operation': 'or'}]
 
         model_task = ModelTask.CLASSIFICATION
         run_error_analyzer_on_models(X_train, y_train, X_test,
                                      y_test, feature_names, model_task,
                                      composite_filters=composite_filters)
@@ -289,20 +290,20 @@
                                          y_test, feature_names, model_task,
                                          matrix_features=[feature_names[3]],
                                          metric=metric)
 
     def test_matrix_filter_housing_filters(self):
         X_train, X_test, y_train, y_test, feature_names = create_housing_data()
 
-        filters = [{'arg': [600],
-                    'column': 'Population',
-                    'method': 'less and equal'},
-                   {'arg': [6],
-                    'column': 'AveRooms',
-                    'method': 'greater'}]
+        filters = [{ARG: [600],
+                    COLUMN: 'Population',
+                    METHOD: 'less and equal'},
+                   {ARG: [6],
+                    COLUMN: 'AveRooms',
+                    METHOD: 'greater'}]
 
         model_task = ModelTask.REGRESSION
         run_error_analyzer_on_models(X_train, y_train, X_test,
                                      y_test, feature_names,
                                      model_task, filters=filters)
 
     def test_matrix_filter_housing_quantile_binning(self):
```

### Comparing `erroranalysis-0.4.3/tests/test_metrics.py` & `erroranalysis-0.4.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/tests/test_pyspark_surrogate_error_tree.py` & `erroranalysis-0.4.4/tests/test_pyspark_surrogate_error_tree.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/tests/test_root_stats.py` & `erroranalysis-0.4.4/tests/test_root_stats.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.3/tests/test_surrogate_error_tree.py` & `erroranalysis-0.4.4/tests/test_surrogate_error_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
 
     @pytest.mark.parametrize('analyzer_type', [AnalyzerType.MODEL,
                                                AnalyzerType.PREDICTIONS])
     def test_surrogate_error_tree_categorical_filtered(self, analyzer_type):
         X_train, X_test, y_train, y_test, categorical_features = \
             create_adult_census_data()
         model = create_kneighbors_classifier(X_train, y_train)
-        filters = [{'arg': [40],
-                    'column': 'Age',
-                    'method': 'less and equal'}]
+        filters = [{ARG: [40],
+                    COLUMN: 'Age',
+                    METHOD: 'less and equal'}]
         run_error_analyzer(model, X_test, y_test, list(X_train.columns),
                            analyzer_type, categorical_features,
                            filters=filters)
 
     def test_large_data_surrogate_error_tree(self):
         # validate tree trains quickly for large data
         X_train, y_train, X_test, y_test, _ = \
```

