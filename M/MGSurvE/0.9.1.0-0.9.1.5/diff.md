# Comparing `tmp/MGSurvE-0.9.1.0.tar.gz` & `tmp/MGSurvE-0.9.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-0.9.1.0.tar", last modified: Wed May 10 22:32:58 2023, max compression
+gzip compressed data, was "MGSurvE-0.9.1.5.tar", last modified: Fri Jun  9 00:18:16 2023, max compression
```

## Comparing `MGSurvE-0.9.1.0.tar` & `MGSurvE-0.9.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-10 22:32:58.796788 MGSurvE-0.9.1.0/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-04-07 16:28:31.000000 MGSurvE-0.9.1.0/LICENSE
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-10 22:32:58.796788 MGSurvE-0.9.1.0/MGSurvE/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      275 2022-04-21 22:03:09.000000 MGSurvE-0.9.1.0/MGSurvE/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       23 2023-05-10 22:32:58.000000 MGSurvE-0.9.1.0/MGSurvE/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6881 2022-04-13 19:47:11.000000 MGSurvE-0.9.1.0/MGSurvE/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      604 2022-02-18 19:18:22.000000 MGSurvE-0.9.1.0/MGSurvE/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1665 2022-04-07 16:28:31.000000 MGSurvE-0.9.1.0/MGSurvE/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6409 2023-04-14 19:41:05.000000 MGSurvE-0.9.1.0/MGSurvE/kernels.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    21376 2023-05-10 22:06:43.000000 MGSurvE-0.9.1.0/MGSurvE/landscape.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4924 2022-03-21 16:18:35.000000 MGSurvE-0.9.1.0/MGSurvE/matrices.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1358 2022-02-18 19:21:24.000000 MGSurvE-0.9.1.0/MGSurvE/network.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    45037 2023-02-23 20:20:29.000000 MGSurvE-0.9.1.0/MGSurvE/optimization.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9200 2022-05-13 21:20:28.000000 MGSurvE-0.9.1.0/MGSurvE/optimizationPSO.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    18219 2023-05-10 22:01:47.000000 MGSurvE-0.9.1.0/MGSurvE/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6849 2023-03-02 20:49:07.000000 MGSurvE-0.9.1.0/MGSurvE/pointProcess.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-10 22:32:58.796788 MGSurvE-0.9.1.0/MGSurvE.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-05-10 22:32:58.000000 MGSurvE-0.9.1.0/MGSurvE.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      451 2023-05-10 22:32:58.000000 MGSurvE-0.9.1.0/MGSurvE.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-05-10 22:32:58.000000 MGSurvE-0.9.1.0/MGSurvE.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      214 2023-05-10 22:32:58.000000 MGSurvE-0.9.1.0/MGSurvE.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        8 2023-05-10 22:32:58.000000 MGSurvE-0.9.1.0/MGSurvE.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-05-10 22:32:58.796788 MGSurvE-0.9.1.0/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4162 2023-04-04 16:41:41.000000 MGSurvE-0.9.1.0/README.md
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-05-10 22:32:58.796788 MGSurvE-0.9.1.0/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1414 2023-03-29 20:42:31.000000 MGSurvE-0.9.1.0/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-09 00:18:16.372396 MGSurvE-0.9.1.5/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-09 00:18:16.370935 MGSurvE-0.9.1.5/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       23 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-0.9.1.5/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18219 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-09 00:18:16.371961 MGSurvE-0.9.1.5/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4596 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      221 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4596 2023-06-09 00:18:16.372220 MGSurvE-0.9.1.5/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4162 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-09 00:18:16.372469 MGSurvE-0.9.1.5/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/setup.py
```

### Comparing `MGSurvE-0.9.1.0/LICENSE` & `MGSurvE-0.9.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/auxiliary.py` & `MGSurvE-0.9.1.5/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/colors.py` & `MGSurvE-0.9.1.5/MGSurvE/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import matplotlib.colors as mcolors
 from matplotlib.colors import LinearSegmentedColormap
 
 def colorPaletteFromHexList(clist):
     """Generates a matplotlib-compliant cmap from a list of hex colors.
 
-    Args:
+    Args: 
         clist (list): List of hex codes (eg. '#f72585') to blend in the map.
 
     Returns:
         cmap: Matplotlib's colormap object.
     """
     c = mcolors.ColorConverter().to_rgb
     clrs = [c(i) for i in clist]
```

### Comparing `MGSurvE-0.9.1.0/MGSurvE/constants.py` & `MGSurvE-0.9.1.5/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/kernels.py` & `MGSurvE-0.9.1.5/MGSurvE/kernels.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,37 @@
 
     np.fill_diagonal(migrMat, zeroInflation)
     tauN = normalize(migrMat, axis=1, norm='l1')
     
     return tauN
 
 
+def exponentialKernel(distMat, decay=cst.AEDES_EXP_PARAMS[0]):
+    '''Calculates the migration matrix using a decaying exponential function.
+
+    Args:
+        distMat (numpy array): Distances matrix.
+        decay (float): Exponential decay rate
+
+    Returns:
+        numpy array: Migration matrix.
+    '''
+    coordsNum = len(distMat)
+    migrMat = np.empty((coordsNum, coordsNum))
+    for (i, row) in enumerate(distMat):
+        for (j, dst) in enumerate(row):
+            migrMat[i][j] = math.exp(-decay*dst)
+        for j in range(len(row)):
+            if np.isnan(migrMat[i][j]):
+                # print("NaN Warning (check points locations, distances might be too large.")
+                migrMat[i][j] = 0
+    tauN = normalize(migrMat, axis=1, norm='l1')
+    return tauN
+
+
 ###############################################################################
 # Exponential Decay
 ###############################################################################
 def exponentialDecay(dist, A=1, b=1):
     '''Calculates the probability of moving between points as a decaying exponential.
 
     Args:
```

### Comparing `MGSurvE-0.9.1.0/MGSurvE/landscape.py` & `MGSurvE-0.9.1.5/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/matrices.py` & `MGSurvE-0.9.1.5/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/network.py` & `MGSurvE-0.9.1.5/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/optimization.py` & `MGSurvE-0.9.1.5/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/optimizationPSO.py` & `MGSurvE-0.9.1.5/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/plots.py` & `MGSurvE-0.9.1.5/MGSurvE/plots.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE/pointProcess.py` & `MGSurvE-0.9.1.5/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-0.9.1.5/MGSurvE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.9.1.0
+Version: 0.9.1.5
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-0.9.1.0/PKG-INFO` & `MGSurvE-0.9.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.9.1.0
+Version: 0.9.1.5
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-0.9.1.0/README.md` & `MGSurvE-0.9.1.5/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.0/setup.py` & `MGSurvE-0.9.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     author='Hector M. Sanchez C.',
     author_email='sanchez.hmsc@berkeley.edu',
     description="MGSurvE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        'deap', 'numpy', 'scikit-learn', 'scipy', 'matplotlib==3.5.2', 'sympy',
+        'deap', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'sympy',
         'ipython', 'jupyter', 'pandas', 'compress-pickle', 'dill', 
         'vincenty', 'haversine', 'networkx', 'pointpats', 'libpysal',
-        'geopandas'
+        'geopandas', 'sympy'
     ],
     extras_require={
         'dev': [
             'pytest', 'ipykernel'
             'twine', 'wheel', 
-            'sphinx', 'sphinx_rtd_theme'
+            'sphinx', 'sphinx_rtd_theme', 'chardet'
         ],
     },
     license='GPLv3',
     classifiers=[
         'Programming Language :: Python :: 3.9',
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ]
- )
+ )
```

