# Comparing `tmp/fairxplainer-0.3.0.tar.gz` & `tmp/fairxplainer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fairxplainer-0.3.0.tar", last modified: Tue Mar 28 12:55:28 2023, max compression
+gzip compressed data, was "fairxplainer-0.4.0.tar", last modified: Fri Jun  9 05:11:06 2023, max compression
```

## Comparing `fairxplainer-0.3.0.tar` & `fairxplainer-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1120 2023-03-10 10:41:14.000000 fairxplainer-0.3.0/LICENSE
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1148 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/PKG-INFO
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)      452 2023-03-15 12:53:19.000000 fairxplainer-0.3.0/README.md
-drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer/
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        0 2023-02-17 06:32:14.000000 fairxplainer-0.3.0/fairxplainer/__init__.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     8288 2023-03-10 12:33:40.000000 fairxplainer-0.3.0/fairxplainer/backfitting.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    32039 2023-03-28 10:15:34.000000 fairxplainer-0.3.0/fairxplainer/fair_explainer.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    33071 2023-03-28 10:13:55.000000 fairxplainer-0.3.0/fairxplainer/hdmr.py
-drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer/salib_util/
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-10 12:14:41.000000 fairxplainer-0.3.0/fairxplainer/salib_util/__init__.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     2021 2023-03-10 09:04:23.000000 fairxplainer-0.3.0/fairxplainer/salib_util/results.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    13353 2023-03-10 09:05:58.000000 fairxplainer-0.3.0/fairxplainer/utils.py
-drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer/wrapper/
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-10 12:14:23.000000 fairxplainer-0.3.0/fairxplainer/wrapper/__init__.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     3125 2023-03-10 12:33:40.000000 fairxplainer-0.3.0/fairxplainer/wrapper/decision_tree_wrap.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     4926 2023-03-10 12:33:40.000000 fairxplainer-0.3.0/fairxplainer/wrapper/linear_classifier_wrap.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     3140 2023-03-10 12:33:40.000000 fairxplainer-0.3.0/fairxplainer/wrapper/mlp_wrap.py
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    10635 2023-02-17 06:32:14.000000 fairxplainer-0.3.0/fairxplainer/wrapper/shap_fairness_explanation.py
-drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer.egg-info/
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1148 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer.egg-info/PKG-INFO
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)      584 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer.egg-info/SOURCES.txt
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        1 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer.egg-info/dependency_links.txt
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)       13 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/fairxplainer.egg-info/top_level.txt
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)       79 2023-03-28 12:55:28.000000 fairxplainer-0.3.0/setup.cfg
--rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1326 2023-03-28 12:55:21.000000 fairxplainer-0.3.0/setup.py
+drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 05:11:06.892658 fairxplainer-0.4.0/
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1120 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/LICENSE
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1148 2023-06-09 05:11:06.892754 fairxplainer-0.4.0/PKG-INFO
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)      452 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/README.md
+drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 05:11:06.890843 fairxplainer-0.4.0/fairxplainer/
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/__init__.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     8288 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/backfitting.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    32145 2023-06-09 04:03:50.000000 fairxplainer-0.4.0/fairxplainer/fair_explainer.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    33093 2023-06-09 04:20:41.000000 fairxplainer-0.4.0/fairxplainer/hdmr.py
+drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 05:11:06.891718 fairxplainer-0.4.0/fairxplainer/salib_util/
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/salib_util/__init__.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     2021 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/salib_util/results.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    13377 2023-06-09 04:05:44.000000 fairxplainer-0.4.0/fairxplainer/utils.py
+drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 05:11:06.892491 fairxplainer-0.4.0/fairxplainer/wrapper/
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/wrapper/__init__.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     3125 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/wrapper/decision_tree_wrap.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     4926 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/wrapper/linear_classifier_wrap.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     3140 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/wrapper/mlp_wrap.py
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)    10635 2023-06-09 03:16:41.000000 fairxplainer-0.4.0/fairxplainer/wrapper/shap_fairness_explanation.py
+drwxr-xr-x   0 bishwamittraghosh   (501) staff       (20)        0 2023-06-09 05:11:06.891425 fairxplainer-0.4.0/fairxplainer.egg-info/
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1148 2023-06-09 05:11:06.000000 fairxplainer-0.4.0/fairxplainer.egg-info/PKG-INFO
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)      584 2023-06-09 05:11:06.000000 fairxplainer-0.4.0/fairxplainer.egg-info/SOURCES.txt
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)        1 2023-06-09 05:11:06.000000 fairxplainer-0.4.0/fairxplainer.egg-info/dependency_links.txt
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)       13 2023-06-09 05:11:06.000000 fairxplainer-0.4.0/fairxplainer.egg-info/top_level.txt
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)       79 2023-06-09 05:11:06.893098 fairxplainer-0.4.0/setup.cfg
+-rw-r--r--   0 bishwamittraghosh   (501) staff       (20)     1326 2023-06-09 05:10:36.000000 fairxplainer-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fairxplainer-0.3.0/LICENSE` & `fairxplainer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/PKG-INFO` & `fairxplainer-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairxplainer
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package for explaining bias in machine learning models
 Home-page: https://github.com/ReAILe/bias-explainer
 Author: Bishwamittra Ghosh
 Author-email: bishwamittra.ghosh@gmail.com
 License: MIT
 Keywords: Fair Machine Learning,Bias,Explainability,Global Sensitivity Analysis,Variance Decomposition,Influence Functions
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fairxplainer-0.3.0/fairxplainer/backfitting.py` & `fairxplainer-0.4.0/fairxplainer/backfitting.py`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/fairxplainer/fair_explainer.py` & `fairxplainer-0.4.0/fairxplainer/fair_explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,16 +294,17 @@
                 if (approach == "hdmr"):
                     # self._auxiliary_info['decomposed_Y'][self.sensitive_groups[idx]] = Y_estimated_decomposed
                     self._auxiliary_info['decomposed_Y'][self.sensitive_groups[idx]] = None
                     self._auxiliary_info['rmse'][self.sensitive_groups[idx]] = rmse
                     self._auxiliary_info['Y'][self.sensitive_groups[idx]] = Y
                     self._auxiliary_info['X'][self.sensitive_groups[idx]] = samples
 
-            self.result = self.result.append(
-                result_current, ignore_index=False)
+            # self.result = self.result.append(
+            #     result_current, ignore_index=False)
+            self.result = pd.concat([self.result, result_current], ignore_index=True)
 
         # if (verbose):
         #     print()
         #     print(self.result)
 
     def get_weights(self):
 
@@ -547,22 +548,22 @@
         else:
             if (compute_sp):
                 return False, None, None, None, None, None
 
             return False, None, None, None, None, None
 
     
-    def statistical_parity_dataset(self, verbose=False):
-        self._all_positive_prediction_probabilities_on_dataset = np.array(
-            list(self.group_specific_positive_prediction_probabilities_on_dataset.values()))
-        if (verbose):
-            print("Exact statistical parity:", self._all_positive_prediction_probabilities_on_dataset.max(
-            ) - self._all_positive_prediction_probabilities_on_dataset.min())
-            print("="*50)
-        return self._all_positive_prediction_probabilities_on_dataset.max() - self._all_positive_prediction_probabilities_on_dataset.min()
+    # def statistical_parity_dataset(self, verbose=False):
+    #     self._all_positive_prediction_probabilities_on_dataset = np.array(
+    #         list(self.group_specific_positive_prediction_probabilities_on_dataset.values()))
+    #     if (verbose):
+    #         print("Exact statistical parity:", self._all_positive_prediction_probabilities_on_dataset.max(
+    #         ) - self._all_positive_prediction_probabilities_on_dataset.min())
+    #         print("="*50)
+    #     return self._all_positive_prediction_probabilities_on_dataset.max() - self._all_positive_prediction_probabilities_on_dataset.min()
 
     
     def statistical_parity_sample(self, verbose=False):
         self._all_positive_prediction_probabilities = np.array(
             list(self.group_specific_positive_prediction_probabilities.values()))
         if (verbose):
             print("Empirical statistical parity:", self._all_positive_prediction_probabilities.max(
```

### Comparing `fairxplainer-0.3.0/fairxplainer/hdmr.py` & `fairxplainer-0.4.0/fairxplainer/hdmr.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,22 +635,22 @@
 
     # Initialize each variable
     S, S_a, S_b = [np.zeros((n,)) for _ in range(3)]
 
     # Analysis of covariance
     for j in range(n):
         # Covariance matrix of jth term of Y_em and actual Y
-        C = np.cov(np.stack((Y_em[:, j], Y.reshape(R,)), axis=0))
+        C = np.cov(np.stack((Y_em[:, j], Y.reshape(R,)), axis=0), bias=True)
 
         # Total sensitivity of jth term         ( = Eq. 19 of Li et al )
         # S[j] = C[0, 1] / V_Y
         S[j] = C[0, 1]
 
         # Covariance matrix of jth term with emulator Y without jth term
-        C = np.cov(np.stack((Y_em[:, j], Y0 - Y_em[:, j]), axis=0))
+        C = np.cov(np.stack((Y_em[:, j], Y0 - Y_em[:, j]), axis=0), bias=True)
 
         # Structural contribution of jth term   ( = Eq. 20 of Li et al )
         # S_a[j] = C[0, 0] / V_Y
         S_a[j] = C[0, 0]
 
         # Correlative contribution of jth term  ( = Eq. 21 of Li et al )
         # S_b[j] = C[0, 1] / V_Y
```

### Comparing `fairxplainer-0.3.0/fairxplainer/salib_util/results.py` & `fairxplainer-0.4.0/fairxplainer/salib_util/results.py`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/fairxplainer/utils.py` & `fairxplainer-0.4.0/fairxplainer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     return pearsonr(synthetic_truth, fif)
 
 
 
 """
     Code source: https://github.com/meelgroup/justicia
 """
-from feature_engine import discretisers as dsc
+from feature_engine.discretisation import EqualWidthDiscretiser as dsc
 def get_discretized_df(data, columns_to_discretize=None, verbose=False):
     """ 
     returns train_test_splitted and discretized df
     """
 
     if(columns_to_discretize is None):
         columns_to_discretize = data.columns.to_list()
```

### Comparing `fairxplainer-0.3.0/fairxplainer/wrapper/decision_tree_wrap.py` & `fairxplainer-0.4.0/fairxplainer/wrapper/decision_tree_wrap.py`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/fairxplainer/wrapper/linear_classifier_wrap.py` & `fairxplainer-0.4.0/fairxplainer/wrapper/linear_classifier_wrap.py`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/fairxplainer/wrapper/mlp_wrap.py` & `fairxplainer-0.4.0/fairxplainer/wrapper/mlp_wrap.py`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/fairxplainer/wrapper/shap_fairness_explanation.py` & `fairxplainer-0.4.0/fairxplainer/wrapper/shap_fairness_explanation.py`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/fairxplainer.egg-info/PKG-INFO` & `fairxplainer-0.4.0/fairxplainer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairxplainer
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package for explaining bias in machine learning models
 Home-page: https://github.com/ReAILe/bias-explainer
 Author: Bishwamittra Ghosh
 Author-email: bishwamittra.ghosh@gmail.com
 License: MIT
 Keywords: Fair Machine Learning,Bias,Explainability,Global Sensitivity Analysis,Variance Decomposition,Influence Functions
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fairxplainer-0.3.0/fairxplainer.egg-info/SOURCES.txt` & `fairxplainer-0.4.0/fairxplainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fairxplainer-0.3.0/setup.py` & `fairxplainer-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # with open('requirements.txt') as f:
 #     required = f.read().splitlines()
 
 
 setup(
   name = 'fairxplainer',
   packages = ['fairxplainer', 'fairxplainer.salib_util', 'fairxplainer.wrapper'],
-  version = 'v0.3.0',
+  version = 'v0.4.0',
   license='MIT',
   description = 'A Python package for explaining bias in machine learning models',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Bishwamittra Ghosh',
   author_email = 'bishwamittra.ghosh@gmail.com',
   url = 'https://github.com/ReAILe/bias-explainer',
```

