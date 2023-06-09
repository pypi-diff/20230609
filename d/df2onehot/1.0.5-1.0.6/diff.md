# Comparing `tmp/df2onehot-1.0.5.tar.gz` & `tmp/df2onehot-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df2onehot-1.0.5.tar", last modified: Sat May 27 17:35:28 2023, max compression
+gzip compressed data, was "dist\df2onehot-1.0.6.tar", last modified: Fri Jun  9 15:44:47 2023, max compression
```

## Comparing `df2onehot-1.0.5.tar` & `df2onehot-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 17:35:28.977246 df2onehot-1.0.5/
--rw-rw-rw-   0        0        0     1122 2021-02-09 21:19:52.000000 df2onehot-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-17 21:33:01.000000 df2onehot-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3188 2023-05-27 17:35:28.977246 df2onehot-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2022-03-13 15:33:54.000000 df2onehot-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 17:35:28.967306 df2onehot-1.0.5/df2onehot/
--rw-rw-rw-   0        0        0      600 2023-05-27 17:35:16.000000 df2onehot-1.0.5/df2onehot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 17:35:28.975283 df2onehot-1.0.5/df2onehot/data/
--rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.5/df2onehot/data/__init__.py
--rw-rw-rw-   0        0        0    20842 2023-05-27 17:32:59.000000 df2onehot-1.0.5/df2onehot/df2onehot.py
--rw-rw-rw-   0        0        0     1053 2023-05-27 17:28:37.000000 df2onehot-1.0.5/df2onehot/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-27 17:35:28.976249 df2onehot-1.0.5/df2onehot/tests/
--rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.5/df2onehot/tests/__init__.py
--rw-rw-rw-   0        0        0     3813 2022-03-13 13:41:37.000000 df2onehot-1.0.5/df2onehot/tests/test_df2onehot.py
--rw-rw-rw-   0        0        0    10215 2021-02-09 21:19:52.000000 df2onehot-1.0.5/df2onehot/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 17:35:28.974254 df2onehot-1.0.5/df2onehot.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-05-27 17:35:28.000000 df2onehot-1.0.5/df2onehot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-05-27 17:35:28.000000 df2onehot-1.0.5/df2onehot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 17:35:28.000000 df2onehot-1.0.5/df2onehot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-27 17:35:28.000000 df2onehot-1.0.5/df2onehot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 17:35:28.000000 df2onehot-1.0.5/df2onehot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 17:35:28.977246 df2onehot-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1424 2023-05-27 16:56:41.000000 df2onehot-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:44:47.613761 df2onehot-1.0.6/
+-rw-rw-rw-   0        0        0     1122 2021-02-09 21:19:52.000000 df2onehot-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-17 21:33:01.000000 df2onehot-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3229 2023-06-09 15:44:47.612760 df2onehot-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2022-03-13 15:33:54.000000 df2onehot-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:44:47.598832 df2onehot-1.0.6/df2onehot/
+-rw-rw-rw-   0        0        0      600 2023-06-09 15:44:22.000000 df2onehot-1.0.6/df2onehot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:44:47.609804 df2onehot-1.0.6/df2onehot/data/
+-rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.6/df2onehot/data/__init__.py
+-rw-rw-rw-   0        0        0    21335 2023-06-09 15:39:27.000000 df2onehot-1.0.6/df2onehot/df2onehot.py
+-rw-rw-rw-   0        0        0     1053 2023-05-27 17:28:37.000000 df2onehot-1.0.6/df2onehot/examples.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:44:47.611765 df2onehot-1.0.6/df2onehot/tests/
+-rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.6/df2onehot/tests/__init__.py
+-rw-rw-rw-   0        0        0     3813 2022-03-13 13:41:37.000000 df2onehot-1.0.6/df2onehot/tests/test_df2onehot.py
+-rw-rw-rw-   0        0        0    10215 2021-02-09 21:19:52.000000 df2onehot-1.0.6/df2onehot/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:44:47.606811 df2onehot-1.0.6/df2onehot.egg-info/
+-rw-rw-rw-   0        0        0     3229 2023-06-09 15:44:47.000000 df2onehot-1.0.6/df2onehot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-09 15:44:47.000000 df2onehot-1.0.6/df2onehot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:44:47.000000 df2onehot-1.0.6/df2onehot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-09 15:44:47.000000 df2onehot-1.0.6/df2onehot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 15:44:47.000000 df2onehot-1.0.6/df2onehot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:44:47.613761 df2onehot-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2023-05-27 16:56:41.000000 df2onehot-1.0.6/setup.py
```

### Comparing `df2onehot-1.0.5/LICENSE` & `df2onehot-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.5/PKG-INFO` & `df2onehot-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: df2onehot
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.
 Home-page: https://erdogant.github.io/df2onehot
-Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.5.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.6.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -83,7 +85,9 @@
 
 <hr>
 
 #### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
+
+
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: df2onehot Version: 1.0.5 Summary: Python package
+Metadata-Version: 2.1 Name: df2onehot Version: 1.0.6 Summary: Python package
 df2onehot is to convert a pandas dataframe into a stuctured dataframe. Home-
-page: https://erdogant.github.io/df2onehot Download-URL: https://github.com/
-erdogant/df2onehot/archive/1.0.5.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # df2onehot [![Python](https://img.shields.io/pypi/
-pyversions/df2onehot)](https://img.shields.io/pypi/pyversions/df2onehot) [!
-[PyPI Version](https://img.shields.io/pypi/v/df2onehot)](https://pypi.org/
-project/df2onehot/) [![License](https://img.shields.io/badge/license-MIT-
-green.svg)](https://github.com/erdogant/df2onehot/blob/master/LICENSE) [!
-[Downloads](https://pepy.tech/badge/df2onehot/month)](https://pepy.tech/
-project/df2onehot/month) [![Downloads](https://pepy.tech/badge/df2onehot)]
-(https://pepy.tech/project/df2onehot) [![DOI](https://zenodo.org/badge/
-245003302.svg)](https://zenodo.org/badge/latestdoi/245003302) [![Sphinx](https:
-//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-df2onehot/)   ``df2onehot`` is a Python package to convert unstructured
-DataFrames into structured dataframes, such as one-hot dense arrays. # **â­ï¸
-Star this repo if you like it â­ï¸** # #### Install df2onehot from PyPI
-```bash pip install df2onehot ``` #### Import df2onehot package ```python from
-df2onehot import df2onehot ``` # ### [Documentation pages](https://
-erdogant.github.io/df2onehot/) On the [documentation pages](https://
-erdogant.github.io/df2onehot/) you can find detailed information about the
-working of the ``df2onehot`` with many examples.
+page: https://erdogant.github.io/df2onehot Author: Erdogan Taskesen Author-
+email: erdogant@gmail.com License: UNKNOWN Download-URL: https://github.com/
+erdogant/df2onehot/archive/1.0.6.tar.gz Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # df2onehot [!
+[Python](https://img.shields.io/pypi/pyversions/df2onehot)](https://
+img.shields.io/pypi/pyversions/df2onehot) [![PyPI Version](https://
+img.shields.io/pypi/v/df2onehot)](https://pypi.org/project/df2onehot/) [!
+[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
+github.com/erdogant/df2onehot/blob/master/LICENSE) [![Downloads](https://
+pepy.tech/badge/df2onehot/month)](https://pepy.tech/project/df2onehot/month) [!
+[Downloads](https://pepy.tech/badge/df2onehot)](https://pepy.tech/project/
+df2onehot) [![DOI](https://zenodo.org/badge/245003302.svg)](https://zenodo.org/
+badge/latestdoi/245003302) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-
+Green)](https://erdogant.github.io/df2onehot/)   ``df2onehot`` is a Python
+package to convert unstructured DataFrames into structured dataframes, such as
+one-hot dense arrays. # **â­ï¸ Star this repo if you like it â­ï¸** # ####
+Install df2onehot from PyPI ```bash pip install df2onehot ``` #### Import
+df2onehot package ```python from df2onehot import df2onehot ``` # ###
+[Documentation pages](https://erdogant.github.io/df2onehot/) On the
+[documentation pages](https://erdogant.github.io/df2onehot/) you can find
+detailed information about the working of the ``df2onehot`` with many examples.
 ===============================================================================
 ### Examples ```python results = df2onehot(df) ``` ```python # Force features
 (int or float) to be numeric if unique non-zero values are above percentage.
 out = df2onehot(df, perc_min_num=0.8) ``` ```python # Remove categorical
 features for which less then 2 values exists. out = df2onehot(df, y_min=2) ```
 ```python # Combine two rules above. out = df2onehot(df, y_min=2,
 perc_min_num=0.8) ``` # * [Example: Process Mixed dataset](https://
```

### Comparing `df2onehot-1.0.5/README.md` & `df2onehot-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.5/df2onehot/__init__.py` & `df2onehot-1.0.6/df2onehot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  	set_dtypes,
  	is_DataFrame,
     set_y,
 )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 # module level doc-string
 __doc__ = """
 df2onehot is an Python package to convert a pandas dataframe into a stuctured dataframe.
 =============================================================================================
 
 Example
```

### Comparing `df2onehot-1.0.5/df2onehot/df2onehot.py` & `df2onehot-1.0.6/df2onehot/df2onehot.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,18 @@
     args['perc_min_num'] = perc_min_num
     args['deep_extract'] = deep_extract
     args['excl_background'] = excl_background
     labx = []
     labels = None
     disable = (True if (verbose==0 or verbose>3) else False)
 
+    if len(np.unique(df.columns))!=len(df.columns):
+        if verbose>2: print('[df2onehot] >WARNING> The column labels must be unique.')
+        df.columns = make_elements_unique(df.columns.values)
+
     # Reset index
     df = df.copy()
     df.reset_index(drop=True, inplace=True)
     # Determine Dtypes
     df, dtypes = set_dtypes(df, args['dtypes'], deep_extract=args['deep_extract'], perc_min_num=args['perc_min_num'], verbose=args['verbose'])
     # If any column is a list, also expand the list!
     if args['deep_extract']:
@@ -475,7 +479,18 @@
         df['feat_2'].iloc[0] = ['4', '45']
         df['feat_2'].iloc[15] = 1
         df['feat_2'].iloc[20] = 10
     else:
         df = dz.get(data=data, url=url, sep=sep, overwrite=overwrite)
 
     return df
+
+
+# %%
+def make_elements_unique(X):
+    uix, counts = np.unique(X, return_counts=True)
+    idx = np.where(counts>1)[0]
+    for i in idx:
+        Iloc = uix[i]==X
+        lst = X[Iloc]
+        X[Iloc] = [f"{element}_{index+1}" for index, element in enumerate(lst)]
+    return X
```

### Comparing `df2onehot-1.0.5/df2onehot/examples.py` & `df2onehot-1.0.6/df2onehot/examples.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.5/df2onehot/tests/test_df2onehot.py` & `df2onehot-1.0.6/df2onehot/tests/test_df2onehot.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.5/df2onehot/utils.py` & `df2onehot-1.0.6/df2onehot/utils.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.5/df2onehot.egg-info/PKG-INFO` & `df2onehot-1.0.6/df2onehot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: df2onehot
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.
 Home-page: https://erdogant.github.io/df2onehot
-Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.5.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.6.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -83,7 +85,9 @@
 
 <hr>
 
 #### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
+
+
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: df2onehot Version: 1.0.5 Summary: Python package
+Metadata-Version: 2.1 Name: df2onehot Version: 1.0.6 Summary: Python package
 df2onehot is to convert a pandas dataframe into a stuctured dataframe. Home-
-page: https://erdogant.github.io/df2onehot Download-URL: https://github.com/
-erdogant/df2onehot/archive/1.0.5.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # df2onehot [![Python](https://img.shields.io/pypi/
-pyversions/df2onehot)](https://img.shields.io/pypi/pyversions/df2onehot) [!
-[PyPI Version](https://img.shields.io/pypi/v/df2onehot)](https://pypi.org/
-project/df2onehot/) [![License](https://img.shields.io/badge/license-MIT-
-green.svg)](https://github.com/erdogant/df2onehot/blob/master/LICENSE) [!
-[Downloads](https://pepy.tech/badge/df2onehot/month)](https://pepy.tech/
-project/df2onehot/month) [![Downloads](https://pepy.tech/badge/df2onehot)]
-(https://pepy.tech/project/df2onehot) [![DOI](https://zenodo.org/badge/
-245003302.svg)](https://zenodo.org/badge/latestdoi/245003302) [![Sphinx](https:
-//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-df2onehot/)   ``df2onehot`` is a Python package to convert unstructured
-DataFrames into structured dataframes, such as one-hot dense arrays. # **â­ï¸
-Star this repo if you like it â­ï¸** # #### Install df2onehot from PyPI
-```bash pip install df2onehot ``` #### Import df2onehot package ```python from
-df2onehot import df2onehot ``` # ### [Documentation pages](https://
-erdogant.github.io/df2onehot/) On the [documentation pages](https://
-erdogant.github.io/df2onehot/) you can find detailed information about the
-working of the ``df2onehot`` with many examples.
+page: https://erdogant.github.io/df2onehot Author: Erdogan Taskesen Author-
+email: erdogant@gmail.com License: UNKNOWN Download-URL: https://github.com/
+erdogant/df2onehot/archive/1.0.6.tar.gz Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # df2onehot [!
+[Python](https://img.shields.io/pypi/pyversions/df2onehot)](https://
+img.shields.io/pypi/pyversions/df2onehot) [![PyPI Version](https://
+img.shields.io/pypi/v/df2onehot)](https://pypi.org/project/df2onehot/) [!
+[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
+github.com/erdogant/df2onehot/blob/master/LICENSE) [![Downloads](https://
+pepy.tech/badge/df2onehot/month)](https://pepy.tech/project/df2onehot/month) [!
+[Downloads](https://pepy.tech/badge/df2onehot)](https://pepy.tech/project/
+df2onehot) [![DOI](https://zenodo.org/badge/245003302.svg)](https://zenodo.org/
+badge/latestdoi/245003302) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-
+Green)](https://erdogant.github.io/df2onehot/)   ``df2onehot`` is a Python
+package to convert unstructured DataFrames into structured dataframes, such as
+one-hot dense arrays. # **â­ï¸ Star this repo if you like it â­ï¸** # ####
+Install df2onehot from PyPI ```bash pip install df2onehot ``` #### Import
+df2onehot package ```python from df2onehot import df2onehot ``` # ###
+[Documentation pages](https://erdogant.github.io/df2onehot/) On the
+[documentation pages](https://erdogant.github.io/df2onehot/) you can find
+detailed information about the working of the ``df2onehot`` with many examples.
 ===============================================================================
 ### Examples ```python results = df2onehot(df) ``` ```python # Force features
 (int or float) to be numeric if unique non-zero values are above percentage.
 out = df2onehot(df, perc_min_num=0.8) ``` ```python # Remove categorical
 features for which less then 2 values exists. out = df2onehot(df, y_min=2) ```
 ```python # Combine two rules above. out = df2onehot(df, y_min=2,
 perc_min_num=0.8) ``` # * [Example: Process Mixed dataset](https://
```

### Comparing `df2onehot-1.0.5/setup.py` & `df2onehot-1.0.6/setup.py`

 * *Files identical despite different names*

