# Comparing `tmp/hnet-1.2.0.tar.gz` & `tmp/hnet-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnet-1.2.0.tar", last modified: Sun Apr 16 12:35:57 2023, max compression
+gzip compressed data, was "dist\hnet-1.2.1.tar", last modified: Fri Jun  9 15:56:23 2023, max compression
```

## Comparing `hnet-1.2.0.tar` & `hnet-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.740342 hnet-1.2.0/
--rw-rw-rw-   0        0        0    11557 2020-11-19 13:38:07.000000 hnet-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      135 2020-11-19 13:38:07.000000 hnet-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9555 2023-04-16 12:35:57.739543 hnet-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9038 2022-09-17 20:51:55.000000 hnet-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.631164 hnet-1.2.0/hnet/
--rw-rw-rw-   0        0        0     1993 2023-04-16 12:24:59.000000 hnet-1.2.0/hnet/__init__.py
--rw-rw-rw-   0        0        0     3510 2020-11-19 13:38:07.000000 hnet-1.2.0/hnet/adjmat_vec.py
--rw-rw-rw-   0        0        0    12158 2023-04-16 12:24:30.000000 hnet-1.2.0/hnet/examples.py
-drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.736766 hnet-1.2.0/hnet/gui/
--rw-rw-rw-   0        0        0        0 2020-11-19 13:38:07.000000 hnet-1.2.0/hnet/gui/__init__.py
--rw-rw-rw-   0        0        0    31911 2020-11-19 13:38:07.000000 hnet-1.2.0/hnet/gui/hnet_gui.py
--rw-rw-rw-   0        0        0    61970 2023-04-16 12:23:14.000000 hnet-1.2.0/hnet/hnet.py
--rw-rw-rw-   0        0        0    26476 2022-03-18 08:21:26.000000 hnet-1.2.0/hnet/hnstats.py
--rw-rw-rw-   0        0        0    17829 2021-05-23 17:59:59.000000 hnet-1.2.0/hnet/network.py
--rw-rw-rw-   0        0        0     1413 2021-05-19 09:47:36.000000 hnet-1.2.0/hnet/savefig.py
-drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.721678 hnet-1.2.0/hnet.egg-info/
--rw-rw-rw-   0        0        0     9555 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 12:35:57.740342 hnet-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1500 2023-04-16 11:37:26.000000 hnet-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.409699 hnet-1.2.1/
+-rw-rw-rw-   0        0        0    11557 2020-11-19 13:38:07.000000 hnet-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      135 2020-11-19 13:38:07.000000 hnet-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9596 2023-06-09 15:56:23.409699 hnet-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9038 2022-09-17 20:51:55.000000 hnet-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.392743 hnet-1.2.1/hnet/
+-rw-rw-rw-   0        0        0     1967 2023-06-09 15:55:03.000000 hnet-1.2.1/hnet/__init__.py
+-rw-rw-rw-   0        0        0     3510 2020-11-19 13:38:07.000000 hnet-1.2.1/hnet/adjmat_vec.py
+-rw-rw-rw-   0        0        0    12158 2023-04-16 12:24:30.000000 hnet-1.2.1/hnet/examples.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.408701 hnet-1.2.1/hnet/gui/
+-rw-rw-rw-   0        0        0        0 2020-11-19 13:38:07.000000 hnet-1.2.1/hnet/gui/__init__.py
+-rw-rw-rw-   0        0        0    31911 2020-11-19 13:38:07.000000 hnet-1.2.1/hnet/gui/hnet_gui.py
+-rw-rw-rw-   0        0        0    61970 2023-04-16 12:23:14.000000 hnet-1.2.1/hnet/hnet.py
+-rw-rw-rw-   0        0        0    26820 2023-06-09 15:54:02.000000 hnet-1.2.1/hnet/hnstats.py
+-rw-rw-rw-   0        0        0    17829 2021-05-23 17:59:59.000000 hnet-1.2.1/hnet/network.py
+-rw-rw-rw-   0        0        0     1413 2021-05-19 09:47:36.000000 hnet-1.2.1/hnet/savefig.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.407704 hnet-1.2.1/hnet.egg-info/
+-rw-rw-rw-   0        0        0     9596 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:56:23.410705 hnet-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1500 2023-04-16 11:37:26.000000 hnet-1.2.1/setup.py
```

### Comparing `hnet-1.2.0/LICENSE` & `hnet-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/PKG-INFO` & `hnet-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: hnet
-Version: 1.2.0
+Version: 1.2.1
 Summary: Graphical Hypergeometric Networks
 Home-page: https://erdogant.github.io/hnet
-Download-URL: https://github.com/erdogant/hnet/archive/1.2.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/hnet/archive/1.2.1.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -197,7 +199,9 @@
 * [Sphinx](https://erdogant.github.io/hnet)
 * [Github](https://github.com/erdogant/hnet)
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
+
+
```

### Comparing `hnet-1.2.0/README.md` & `hnet-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet/__init__.py` & `hnet-1.2.1/hnet/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 from hnet.adjmat_vec import (
     vec2adjmat,
     adjmat2vec,
     )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 # module level doc-string
 __doc__ = """
 HNET - Graphical Hypergeometric networks.
 =====================================================================
 
-Description
------------
 Creation of networks from datasets with mixed datatypes and with unknown function.
 Input datasets can range from generic dataframes to nested data structures with lists, missing values and enumerations.
 HNet (graphical Hypergeometric Networks) is a method where associations across variables are tested for significance by statistical inference.
 The aim is to determine a network with significant associations that can shed light on the complex relationships across variables.
 
 Examples
 --------
```

### Comparing `hnet-1.2.0/hnet/adjmat_vec.py` & `hnet-1.2.1/hnet/adjmat_vec.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet/examples.py` & `hnet-1.2.1/hnet/examples.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet/gui/hnet_gui.py` & `hnet-1.2.1/hnet/gui/hnet_gui.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet/hnet.py` & `hnet-1.2.1/hnet/hnet.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet/hnstats.py` & `hnet-1.2.1/hnet/hnstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,14 +547,15 @@
 
 
 # %% Preprocessing
 def _preprocessing(df, dtypes='pandas', y_min=10, perc_min_num=0.8, excl_background=None, white_list=None, black_list=None, verbose=3):
     if verbose>=4: print('[hnet] >preprocessing: Column names are set to str. and spaces are trimmed.')
     df.columns = df.columns.astype(str)
     df.columns = df.columns.str.strip()
+    df.columns = make_elements_unique(df.columns.values)
     df.reset_index(drop=True, inplace=True)
 
     # Convert bool columns to integer values
     df, dtypes, excl_background = _bool_processesing(df, dtypes, excl_background=excl_background, verbose=verbose)
     # Filter on white_list and black_list
     df, dtypes = _white_black_list(df, dtypes, white_list, black_list)
     # Remove columns without dtype
@@ -589,14 +590,24 @@
     else:
         savepath = os.path.join(savepath, '')
     os.makedirs(savepath, exist_ok=True)
 
     return(savepath)
 
 
+# %%
+def make_elements_unique(X):
+    uix, counts = np.unique(X, return_counts=True)
+    idx = np.where(counts>1)[0]
+    for i in idx:
+        Iloc = uix[i]==X
+        lst = X[Iloc]
+        X[Iloc] = [f"{element}_{index+1}" for index, element in enumerate(lst)]
+    return X
+
 # %% Filter adjacency matrix
 def _filter_adjmat(simmatLogP, labx, threshold=None, min_edges=None, white_list=None, black_list=None, verbose=3):
     # if (white_list is not None) and (len(white_list)<=1): raise ValueError('[hnet] >ERROR: white_list should contain at least 2 input variables.')
 
     # Filter on threshold
     if threshold is not None:
         if verbose>=3: print('[hnet] >Filtering associations on threshold > %d' %(threshold))
```

### Comparing `hnet-1.2.0/hnet/network.py` & `hnet-1.2.1/hnet/network.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet/savefig.py` & `hnet-1.2.1/hnet/savefig.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.0/hnet.egg-info/PKG-INFO` & `hnet-1.2.1/hnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: hnet
-Version: 1.2.0
+Version: 1.2.1
 Summary: Graphical Hypergeometric Networks
 Home-page: https://erdogant.github.io/hnet
-Download-URL: https://github.com/erdogant/hnet/archive/1.2.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/hnet/archive/1.2.1.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -197,7 +199,9 @@
 * [Sphinx](https://erdogant.github.io/hnet)
 * [Github](https://github.com/erdogant/hnet)
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
+
+
```

### Comparing `hnet-1.2.0/setup.py` & `hnet-1.2.1/setup.py`

 * *Files identical despite different names*

