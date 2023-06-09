# Comparing `tmp/arfs-1.1.0.tar.gz` & `tmp/arfs-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.1.0.tar", last modified: Sun May 21 19:19:53 2023, max compression
+gzip compressed data, was "arfs-1.1.1.tar", last modified: Fri Jun  9 19:58:50 2023, max compression
```

## Comparing `arfs-1.1.0.tar` & `arfs-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:53.045740 arfs-1.1.0/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-05-21 19:19:53.046741 arfs-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.0/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-05-21 19:19:53.053742 arfs-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.602690 arfs-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.764751 arfs-1.1.0/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-05-21 19:17:41.000000 arfs-1.1.0/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.0/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.604700 arfs-1.1.0/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.894743 arfs-1.1.0/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.0/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.0/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:53.008742 arfs-1.1.0/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    90381 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15449 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.1.0/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21796 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.0/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    28685 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.0/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.0/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:52.829741 arfs-1.1.0/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.0/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-21 19:19:52.000000 arfs-1.1.0/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 19:19:53.036742 arfs-1.1.0/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.0/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.0/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.913235 arfs-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0    11069 2023-06-09 19:58:50.914041 arfs-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.1/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1389 2023-06-09 19:58:50.922056 arfs-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.422546 arfs-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.603543 arfs-1.1.1/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-06-09 19:55:54.000000 arfs-1.1.1/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.1/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.426560 arfs-1.1.1/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.739579 arfs-1.1.1/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.1/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.1/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.869895 arfs-1.1.1/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    90379 2023-06-09 19:54:49.000000 arfs-1.1.1/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15449 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.1.1/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21796 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.1/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    30283 2023-05-31 17:10:21.000000 arfs-1.1.1/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.1/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.1/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.667545 arfs-1.1.1/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.1/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      365 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 19:58:50.000000 arfs-1.1.1/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 19:58:50.901949 arfs-1.1.1/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.1/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.1/tests/test_featselect.py
```

### Comparing `arfs-1.1.0/LICENSE.md` & `arfs-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/PKG-INFO` & `arfs-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.0
+Version: 1.1.1
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.1.0/README.md` & `arfs-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/setup.cfg` & `arfs-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/association.py` & `arfs-1.1.1/src/arfs/association.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/benchmark.py` & `arfs-1.1.1/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-1.1.1/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/dataset/data/housing.zip` & `arfs-1.1.1/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/feature_selection/__init__.py` & `arfs-1.1.1/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/feature_selection/allrelevant.py` & `arfs-1.1.1/src/arfs/feature_selection/allrelevant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1500,15 +1500,16 @@
         """
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a dataframe")
 
         if sample_weight is not None:
-            sample_weight = _check_sample_weight(sample_weight, X)
+            sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
+            
 
         # crit, keep_vars, df_vimp, mean_shadow
         _, self.selected_features_, self.sha_cutoff_df, self.mean_shadow = _boostaroota(
             X,
             y,
             # metric=self.metric,
             estimator=self.estimator,
@@ -1942,16 +1943,15 @@
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a pandas DataFrame")
 
         self.feature_names_in_ = X.columns.to_numpy()
         y = pd.Series(y) if not isinstance(y, pd.Series) else y
 
         if sample_weight is not None:
-            sample_weight = pd.Series(sample_weight)
-            sample_weight = _check_sample_weight(sample_weight, X)
+            sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
 
         # internal encoding (ordinal encoding)
         X, obj_feat, cat_idx = get_pandas_cat_codes(X)
 
         self.selected_features_, self.cv_df, self.sha_cutoff = _reduce_vars_lgb_cv(
             X,
             y,
@@ -2295,15 +2295,15 @@
         The target validation data.
     weight_val : array-like of shape (n_val_samples,)
         The sample weights for validation data.
     category_cols : array-like or None, optional (default=None)
         The indices of categorical columns. If None, no categorical columns will be considered.
     early_stopping_rounds : int, optional (default=20)
         Activates early stopping. Validation metric needs to improve at least once in every early_stopping_rounds
-        round(s) to continue training.
+        round(s) to continue training._train_lgb_model
     **params : dict
         Other parameters passed to the LightGBM model.
 
     Returns
     -------
     tuple of (Booster, numpy.ndarray, int)
         The trained LightGBM model, its SHAP values for X_train, and the best iteration reached during training.
```

### Comparing `arfs-1.1.0/src/arfs/feature_selection/base.py` & `arfs-1.1.1/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/feature_selection/mrmr.py` & `arfs-1.1.1/src/arfs/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/feature_selection/summary.py` & `arfs-1.1.1/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/feature_selection/unsupervised.py` & `arfs-1.1.1/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/feature_selection/variable_importance.py` & `arfs-1.1.1/src/arfs/feature_selection/variable_importance.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/gbm.py` & `arfs-1.1.1/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/parallel.py` & `arfs-1.1.1/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/preprocessing.py` & `arfs-1.1.1/src/arfs/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # Settings and libraries
 from __future__ import print_function
 from tqdm.auto import tqdm
 
 # pandas
 import pandas as pd
+from pandas.api.types import IntervalDtype
 
 # numpy
 import numpy as np
 
 # sklearn
 from sklearn.preprocessing import OrdinalEncoder
 from sklearn.base import BaseEstimator, TransformerMixin
@@ -382,41 +383,49 @@
         # Map is faster than replace
     if return_cat:
         df.loc[:, non_num_cols] = df.loc[:, non_num_cols].astype("category")
     return df, cat_var_df, inv_mapper, mapper
 
 
 class TreeDiscretizer(BaseEstimator, TransformerMixin):
-    """Bin continuous data into intervals and return a pandas DF. It supports regression and binary classification.
-    Discretization (otherwise known as quantization or binning) provides a way to partition continuous features into discrete values.
-    Certain datasets with continuous features may benefit from discretization, because discretization can transform the dataset
-    of continuous attributes to one with only nominal attributes.
-    One-hot encoded discretized features can make a model more expressive, while maintaining interpretability.
-    For instance, pre-processing with a discretizer can introduce nonlinearity to linear models.
-    For more advanced possibilities, in particular smooth ones, see Generating polynomial features further below.
-
-    TreeDiscretizer uses univariate regularized trees (one per column to bin), find the optimal partition and returns
-    pandas numerical interval for numerical continuous columns and pd.Categorical for categorical columns.
-    Similar levels are therefore grouped together. This reduces the dimensionality and regularizes the model.
-    This is a substitution to proper regularization scheme such as
+    """The purpose of the function is to discretize continuous and/or categorical data, returning a pandas DataFrame. 
+    It is designed to support regression and binary classification tasks. Discretization, also known as quantization or binning, 
+    allows for the partitioning of continuous features into discrete values. In certain datasets with continuous attributes, 
+    discretization can be beneficial as it transforms the dataset into one with only nominal attributes. 
+    Additionally, for categorical predictors, grouping levels can help reduce overfitting and create meaningful clusters.
+
+    By encoding discretized features, a model can become more expressive while maintaining interpretability. 
+    For example, preprocessing with a discretizer can introduce nonlinearity to linear models. 
+    For more advanced possibilities, particularly smooth ones, you can refer to the section on generating polynomial features.
+    The TreeDiscretizer function utilizes univariate regularized trees, with one tree per column to be binned. 
+    It finds the optimal partition and returns numerical intervals for numerical continuous columns and pd.Categorical for categorical columns. 
+    This approach groups similar levels together, reducing dimensionality and regularizing the model.
+    
+    TreeDiscretizer handles missing values for both numerical and categorical predictors, 
+    eliminating the need for encoding categorical predictors separately.
+
+    Notes
+    -----
+     This is a substitution to proper regularization scheme such as
      - GroupLasso (categorical predictors, which are usually encoded as multiple dummy variables: one for each category.
                    It makes sense in many analyses to consider these dummy variables (representing one categorical predictor)
                    together rather than separately)
      - FusedLasso (One drawback of the Lasso is it ignores ordering of the features, FusedLasso takes into account the ordering)
 
-    TreeDiscretizer handles missing values, both for numerical and categorical predictors. No need for encoding the categorical predictors.
-
-
     Parameters
     ----------
     bin_features : List of string, str or None
         the list of names of the variable that has to be binned, or "all", "numerical" or "categorical"
         for splitting and grouping all, only numerical or only categorical columns.
     n_bins : int
         the number of bins that has to be created while binning the variables in "bin_features" list
+    n_bins_max : int, optional
+        the maximum number of levels that a categorical column can have in order to avoid being binned
+    num_bins_as_category: bool, default=False
+        save the numeric bins as pandas category or as pandas interval
     boost_params : dic
         the boosting parameters dictionary
     raw : bool
         returns raw levels (non human-interpretable) or levels matching the orginal ones
     task : str
         either regression or classification (binary)
 
@@ -451,23 +460,27 @@
     >>> disc.fit(X=df[predictors], y=df['Frequency'], sample_weight=df['Exposure'])
     """
 
     def __init__(
         self,
         bin_features="all",
         n_bins=10,
+        n_bins_max=None,
+        num_bins_as_category=False,
         boost_params=None,
         raw=False,
         task="regression",
     ):
         if (boost_params is not None) & (not isinstance(boost_params, dict)):
             raise TypeError("boost_kwargs should be a dictionary")
 
         self.bin_features = bin_features
         self.n_bins = n_bins
+        self.n_bins_max = n_bins_max
+        self.num_bins_as_category = num_bins_as_category
         self.boost_params = {}
         self.raw = raw
         self.task = task
         if boost_params is not None:
             self.boost_params = boost_params
 
         # force some params
@@ -499,14 +512,15 @@
 
         Returns
         -------
         X :
             pd.DataFrame with the binned and grouped columns
         """
         X = X.copy()
+        
         if self.bin_features is None:
             self.bin_features = list(X.select_dtypes("number").columns)
             self.cat_features = []
         elif isinstance(self.bin_features, list):
             self.cat_features = list(
                 set(self.bin_features)
                 - set(list(X[self.bin_features].select_dtypes("number").columns))
@@ -519,14 +533,18 @@
         elif isinstance(self.bin_features, str) and (self.bin_features == "numerical"):
             self.bin_features = list(X.select_dtypes("number").columns)
         elif isinstance(self.bin_features, str) and (
             self.bin_features == "categorical"
         ):
             self.bin_features = list(X.select_dtypes(["category", "object"]).columns)
             self.cat_features = self.bin_features
+            
+        self.n_unique_table_ = X[self.bin_features].nunique()
+        # transform only the columns with more than n_bins_max
+        self.bin_features = self.n_unique_table_[self.n_unique_table_ > self.n_bins_max].index.to_list() if self.n_bins_max else self.bin_features
 
         for col in self.bin_features:
             is_categorical = (self.cat_features is not None) and (
                 col in self.cat_features
             )
             if is_categorical:
                 encoder = OrdinalEncoder(
@@ -537,15 +555,21 @@
                     X[col]
                     .astype("category")
                     .cat.add_categories("missing_added")
                     .fillna("missing_added")
                 )
                 # encode
                 self.ordinal_encoder_dic[col] = encoder.fit(X[[col]])
-                X[col] = encoder.transform(X[[col]]).ravel()
+                dum = encoder.transform(X[[col]])
+                if isinstance(dum, pd.DataFrame):
+                    X[col] = dum.values.ravel()
+                else:
+                    X[col] = dum.ravel()
+                
+                
             else:
                 encoder = None
 
             gbm_param = self.boost_params.copy()
             tree = GradientBoosting(
                 cat_feat=None, params=gbm_param, show_learning_curve=False
             )
@@ -557,15 +581,20 @@
             # create the bins series
             # predict, group by original values
             # create monotonicly increasing bin for pd.cut
             X[f"{col}_g"] = tree.predict(X[[col]])
 
             if is_categorical:
                 # retrieve original values
-                X[col] = encoder.inverse_transform(X[[col]]).ravel()
+                dum = encoder.inverse_transform(X[[col]])
+                if isinstance(dum, pd.DataFrame):
+                    X[col] = dum.values.ravel()
+                else:
+                    X[col] = dum.ravel()
+                
                 self.cat_bin_dict[col] = (
                     X[[f"{col}_g", col]]
                     .groupby(f"{col}_g")
                     .apply(lambda x: " / ".join(map(str, x[col].unique())))
                     .to_dict()
                 )
             else:
@@ -594,28 +623,30 @@
                 ]
 
             del tree
 
         return self
 
     def transform(self, X):
-        """Apply the discretizer on `X`.
+        """Apply the discretizer on `X`. Only the columns with more than n_bins_max unique values will be transformed.
+        
         Parameters
         ----------
         X :
             Input data shape (n_samples, n_features), where `n_samples` is the number of samples and
             `n_features` is the number of features.
 
 
         Returns
         -------
         X :
             pd.DataFrame with the binned and grouped columns
         """
         X = X.copy()
+
         for col in self.bin_features:
             if self.raw:
                 # predict each univariate tree
                 X[col] = self.tree_dic[col].predict(X[[col]])
             else:
                 if (self.cat_features is not None) and (col in self.cat_features):
                     # apply the systematic imputation (missing might be grouped
@@ -634,16 +665,19 @@
                     # retrieve the association the tree learnt for missing values
                     X[col].fillna(self.tree_imputer[col], inplace=True)
                     # apply the binning
                     X[col] = pd.cut(
                         X[col],
                         bins=self.bin_upper_bound_dic[col],
                         include_lowest=True,
-                        precision=1,
+                        precision=2,
                     )
+                    
+                    if not self.num_bins_as_category:
+                        X[col] = X[col].astype(IntervalDtype())
         return X
 
 
 def highlight_discarded(s):
     """highlight X in red and V in green.
 
     Parameters
```

### Comparing `arfs-1.1.0/src/arfs/sampling.py` & `arfs-1.1.1/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs/utils.py` & `arfs-1.1.1/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/src/arfs.egg-info/PKG-INFO` & `arfs-1.1.1/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.0
+Version: 1.1.1
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.1.0/src/arfs.egg-info/SOURCES.txt` & `arfs-1.1.1/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/tests/test_allrelevant.py` & `arfs-1.1.1/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.0/tests/test_featselect.py` & `arfs-1.1.1/tests/test_featselect.py`

 * *Files identical despite different names*

