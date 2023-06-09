# Comparing `tmp/AutoCarver-4.3.1.tar.gz` & `tmp/AutoCarver-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.3.1.tar", last modified: Mon May 22 07:50:03 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.3.2.tar", last modified: Fri Jun  9 13:59:03 2023, max compression
```

## Comparing `AutoCarver-4.3.1.tar` & `AutoCarver-4.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/
-drwxrwxrwx   0        0        0        0 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/AutoCarver/
--rw-rw-rw-   0        0        0    23989 2023-05-22 07:48:34.000000 AutoCarver-4.3.1/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0     8599 2023-05-22 07:18:35.000000 AutoCarver-4.3.1/AutoCarver/Converters.py
--rw-rw-rw-   0        0        0    52539 2023-05-22 07:18:23.000000 AutoCarver-4.3.1/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    28038 2023-05-22 07:18:44.000000 AutoCarver-4.3.1/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.3.1/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7119 2023-05-22 07:49:56.000000 AutoCarver-4.3.1/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-22 07:50:01.000000 AutoCarver-4.3.1/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 07:49:56.000000 AutoCarver-4.3.1/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 07:49:56.000000 AutoCarver-4.3.1/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.3.1/LICENSE
--rw-rw-rw-   0        0        0     7119 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-22 07:48:47.000000 AutoCarver-4.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/
+drwxrwxrwx   0        0        0        0 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/AutoCarver/
+-rw-rw-rw-   0        0        0    24083 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0     9449 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/Converters.py
+-rw-rw-rw-   0        0        0    52826 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    28159 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.3.2/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     7119 2023-06-09 13:58:57.000000 AutoCarver-4.3.2/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-09 13:59:01.000000 AutoCarver-4.3.2/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:58:57.000000 AutoCarver-4.3.2/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 13:58:57.000000 AutoCarver-4.3.2/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.3.2/LICENSE
+-rw-rw-rw-   0        0        0     7119 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-06-09 13:56:46.000000 AutoCarver-4.3.2/setup.py
```

### Comparing `AutoCarver-4.3.1/AutoCarver/AutoCarver.py` & `AutoCarver-4.3.2/AutoCarver/AutoCarver.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=True, str_nan=self.str_nan)
 
         # update of the values_orders grouped modalities in values_orders
         if best_groups:
             xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
 
         # testing adding NaNs to built groups
-        if (self.str_nan in xtab.index) & self.dropna:
+        if (self.str_nan in xtab.index) & self.dropna & (self.str_nan not in self.values_orders.get(feature)):
 
             # measuring association with target for each combination and testing for stability on TEST
             best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=False, str_nan=self.str_nan)
 
             # adding NaN to the order
             self.insert_nan(feature, xtab)
 
@@ -452,15 +452,15 @@
     if not raw:
         combinations = [groupedlist_combination(combination, values) for combination in combinations]
 
     return combinations
 
 def get_all_nan_combinations(order: GroupedList, str_nan: str, max_n_mod: int) -> List[GroupedList]:
     """ all possible combinations of modalities with numpy.nan"""
-
+    
     # computing all non-NaN combinations
     # case 0: several modalities -> several combinations
     if len(order) > 1:
         combinations = get_all_combinations(order, max_n_mod-1, raw=True)
     # case 1: unique or no modality -> two combinations
     else:
         combinations = []
@@ -480,15 +480,16 @@
 
             # adding other groups unchanged
             pre = [o for o in combi[:n]]
             nex = [o for o in combi[n+1:]]
             new_combinations += [pre + new_combination + nex]
             
     # adding NaN to order
-    order = order.append(str_nan)
+    if str_nan not in order:
+        order = order.append(str_nan)
     
     # converting back to GroupedList
     new_combinations = [groupedlist_combination(combination, order) for combination in new_combinations] 
 
     return new_combinations
```

### Comparing `AutoCarver-4.3.1/AutoCarver/Converters.py` & `AutoCarver-4.3.2/AutoCarver/Converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numpy import select, nan, tanh
 from pandas import isna, notna, DataFrame, Series, to_datetime
 from sklearn.base import BaseEstimator, TransformerMixin
-from typing import List, Tuple, Any
+from typing import List, Tuple, Any, Dict
 
 
 class StringConverter(BaseEstimator, TransformerMixin):
     """ Converts specified columns a DataFrame into str
     
      - Keeps NaN inplace
      - Converts floats of int to int
@@ -221,41 +221,66 @@
         List of qualitative features to be crossed should be passed through AutoCarver early on.
     """
 
     def __init__(self, features: List[str], copy: bool=True) -> None:
         
         self.features = features[:]
         self.copy = copy
-        self.new_features = list()
+        self.new_features: List[str] = list()
+        self.values: Dict[str, List[Any]] = dict()
 
     def fit(self, X: DataFrame, y: Series=None) -> None:
         
         # iterating over each feature
-        for i, feature in enumerate(self.features):
+        for i, feature1 in enumerate(self.features):
+            
+            # unique values of feature1
+            unq1 = X[feature1].astype(str).unique()
+            
+            for feature2 in self.features[i+1:]:
             
-            # adding features names to the list of built features
-            self.new_features += [f'{f}_x_{feature}' for f in self.features[i+1:]]
+                # adding features names to the list of built features
+                self.new_features += [f'{feature2}_x_{feature1}']
+            
+                # unique values of feature2
+                unq2 = X[feature2].astype(str).unique()
+                
+                self.values.update({
+                    f'{feature2}_x_{feature1}': [u2 + '_x_' + u1 for u2 in unq2 for u1 in unq1]
+                })
 
         return self
 
     
 
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
         
         # coppying dataframe
         Xc = X
         if self.copy:
             Xc = X.copy()
             
         # converting features to strings
-        Xc[self.features] = Xc[self.features].astype(str)
+        Xc_features = Xc[self.features].astype(str)
         
         # iterating over each group
         for i, feature in enumerate(self.features):
             
+            # features to cross with
+            Xc_tocross = Xc_features[self.features[i+1:]]
+            
+            # feature to be crossed
+            Xc_crosser = Xc_features[feature]
+
+            # crossing features
+            Xc_crossed = Xc_tocross.apply(lambda u: u + '_x_' + Xc_crosser)\
+                                   .rename({f: f"{f}_x_{feature}" for f in self.features[i+1:]}, axis=1)
+            
             # applying normalization to the feature
-            Xc = Xc.join(
-                Xc[self.features[i+1:]].apply(lambda u: u + '_x_' + Xc[feature])\
-                                       .rename({f: f"{f}_x_{feature}" for f in self.features[i+1:]}, axis=1)
-            )
+            Xc = Xc.join(Xc_crossed)
+        
+        del Xc_features
+        del Xc_crossed
+        del Xc_tocross
+        del Xc_crosser
         
         return Xc
```

### Comparing `AutoCarver-4.3.1/AutoCarver/Discretizers.py` & `AutoCarver-4.3.2/AutoCarver/Discretizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             super().__init__(iterable)
 
             # création des groupes
             self.contained = {v: [v] for v in iterable}
 
     def group_list(self, to_discard: List[Any], to_keep: Any) -> None:
         """ Groups elements to_discard into values to_keep"""
-
+        
         for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
             self.group(discarded, kept)
 
     def group(self, discarded: Any, kept: Any) -> None:
         """ Groups the discarded value with the kept value"""
 
         # checking that those values are distinct
@@ -616,15 +616,15 @@
         self.verbose = verbose
 
         # parameters to handle missing/unknown values
         self.remove_unknown = remove_unknown
         self.str_nan = str_nan
         
         # initiating features' values orders to all possible values
-        self.known_values = list(set([value for group in self.chained_orders for value in group.values()]))
+        self.known_values = list(set([v for o in self.chained_orders for v in o.values()]))
         self.values_orders = {f: GroupedList(self.known_values[:] + [self.str_nan]) for f in self.features}
 
     def fit(self, X: DataFrame, y: Series=None) -> None:
         
         # filling nans
         Xc = X[self.features].fillna(self.str_nan)
         
@@ -641,39 +641,49 @@
 
             # checking for unknown values (values to present in an order of self.chained_orders)
             missing = [value for value in values if notna(value) and (value not in self.known_values)]
 
             # converting unknown values to NaN
             if self.remove_unknown & (len(missing) > 0):
 
-            	# alerting user
+                # alerting user
                 print(f"Order for {feature} was not provided for values: {missing}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)")
 
                 # adding missing valyes to the order
                 order = self.values_orders.get(feature)
                 order.update({self.str_nan: missing + order.get(self.str_nan)})
 
             # alerting user
             else:
                 assert not len(missing) > 0, f"Order for {feature} needs to be provided for values: {missing}, otherwise set remove_unknown=True"
 
             # iterating over each specified orders
             for order in self.chained_orders:
                 
-                # identifying modalities which rarest values
-                to_keep = values[frequencies >= self.min_freq]
+                # values that are frequent enough
+                to_keep = list(values[frequencies >= self.min_freq])
+
+                # all values from the order 
+                values_order = [o for v in order for o in order.get(v)]
+
+                # values from the order to group (not frequent enough or absent)
+                to_discard = [value for value in values_order if value not in to_keep]
 
-                # grouping rare modalities
-                to_discard = [[value for value in order.get(group) if (not value in to_keep)] for group in order]  # identifying rare values
-                to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identifying observation to input
-                Xc[feature] = select(to_input, to_input, default=Xc[feature])  # regroupement des naf peu fréquents
+                # values to group into discarded values
+                value_to_group = [order.get_group(value) for value in to_discard]
+
+                # values of the series to input
+                df_to_input = [Xc[feature] == discarded for discarded in to_discard]  # identifying observation to input
+
+                # inputing non frequent values
+                Xc[feature] = select(df_to_input, value_to_group, default=Xc[feature])
                 
                 # historizing in the feature's order
-                for discarded, kept in zip(to_discard, order):
-                    self.values_orders.get(feature).group_list(discarded, kept)  # historisation dans l'order
+                for discarded, kept in zip(to_discard, value_to_group):
+                    self.values_orders.get(feature).group(discarded, kept)
                     
                 # updating frequencies of each modality for the next ordering
                 frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
                 values, frequencies = frequencies.index, frequencies.values
         
         super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=str)
         super().fit(X, y)
@@ -960,24 +970,25 @@
 
         # filling up NaNs
         Xc[self.features] = Xc[self.features].fillna(self.str_nan)
 
         # grouping values inside groups of modalities
         for n, feature in enumerate(self.features):
 
-        	# verbose if requested
+            # verbose if requested
             if self.verbose: 
                 print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             # grouping modalities
             Xc[feature] = select([~Xc[feature].isin(self.to_keep[feature])], [self.default_value], default=Xc[feature])
 
         return Xc
 
 
+
 def find_quantiles(df_feature: Series, q: int, len_df: int=None, quantiles: List[float]=None) -> List[float]:
     """ Découpage en quantile de la feature.
     
     Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
     Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
     Une fois il n'y a plus de valeurs qui soient sur-représentées,
     on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
```

### Comparing `AutoCarver-4.3.1/AutoCarver/FeatureSelector.py` & `AutoCarver-4.3.2/AutoCarver/FeatureSelector.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,18 @@
         ols_df = DataFrame({'feature': x[~nans], 'target': y[~nans]})
         
         # fitting regression of feature by target
         regression = ols('feature~C(target)', ols_df).fit()
         
         # updating association
         if regression.rsquared:
-            association.update({'R_measure': sqrt(regression.rsquared)})
+            if regression.rsquared >= 0:
+                association.update({'R_measure': sqrt(regression.rsquared)})
+            else:
+                association.update({'R_measure': nan})
         
     return active, association
 
 
 def zscore_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Computes outliers based on the z-score
```

### Comparing `AutoCarver-4.3.1/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.3.2/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.3.1
+Version: 4.3.2
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.3.1/LICENSE` & `AutoCarver-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.1/PKG-INFO` & `AutoCarver-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.3.1
+Version: 4.3.2
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.3.1/README.md` & `AutoCarver-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.1/setup.py` & `AutoCarver-4.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='AutoCarver',
-    version='4.3.1',
+    version='4.3.2',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
     project_urls = {
```

