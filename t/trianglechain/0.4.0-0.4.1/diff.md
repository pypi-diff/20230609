# Comparing `tmp/trianglechain-0.4.0.tar.gz` & `tmp/trianglechain-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.4.0.tar", last modified: Mon Jun  5 12:30:46 2023, max compression
+gzip compressed data, was "trianglechain-0.4.1.tar", last modified: Fri Jun  9 15:12:25 2023, max compression
```

## Comparing `trianglechain-0.4.0.tar` & `trianglechain-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.771258 trianglechain-0.4.0/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.4.0/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-06-05 12:29:15.000000 trianglechain-0.4.0/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.4.0/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.4.0/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-05 12:30:46.771324 trianglechain-0.4.0/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.4.0/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.4.0/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-06-05 12:30:46.771685 trianglechain-0.4.0/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.765245 trianglechain-0.4.0/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.769211 trianglechain-0.4.0/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/LineChain.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28003 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-06-05 12:29:22.000000 trianglechain-0.4.0/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16850 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/params.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19680 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.770357 trianglechain-0.4.0/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.4.0/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.771136 trianglechain-0.4.0/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_linechain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_params.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.094668 trianglechain-0.4.1/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.4.1/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1670 2023-06-09 15:11:54.000000 trianglechain-0.4.1/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.4.1/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.4.1/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-09 15:12:25.094738 trianglechain-0.4.1/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.4.1/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.4.1/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-06-09 15:12:25.095086 trianglechain-0.4.1/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.088569 trianglechain-0.4.1/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.092606 trianglechain-0.4.1/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28003 2023-06-05 12:25:46.000000 trianglechain-0.4.1/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-06-09 15:11:46.000000 trianglechain-0.4.1/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-05 12:25:46.000000 trianglechain-0.4.1/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16854 2023-06-09 15:08:20.000000 trianglechain-0.4.1/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19680 2023-06-05 12:25:46.000000 trianglechain-0.4.1/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.093653 trianglechain-0.4.1/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.4.1/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.094538 trianglechain-0.4.1/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_trianglechain.py
```

### Comparing `trianglechain-0.4.0/CONTRIBUTING.rst` & `trianglechain-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/HISTORY.rst` & `trianglechain-0.4.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+0.4.1 (2023-06-09)
+++++++++++++++++++
+
+* FIX: RGB(A) colors in plt.contour
+
 0.4.0 (2023-06-05)
 ++++++++++++++++++
 
 * FEATURE: n_sigma_for_one_sided_tail free parameter to manually set the threshold when to use a 2-sided or 1-sided interval
 * FIX: correct normalization when using samples with prob
 * FIX: avoid upper limits with +- 0.0 and lower limits with -- 0.0
```

### Comparing `trianglechain-0.4.0/LICENSE` & `trianglechain-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/PKG-INFO` & `trianglechain-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.0
+Version: 0.4.1
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.4.0/README.md` & `trianglechain-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/pyproject.toml` & `trianglechain-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/setup.cfg` & `trianglechain-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/BaseChain.py` & `trianglechain-0.4.1/src/trianglechain/BaseChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/LineChain.py` & `trianglechain-0.4.1/src/trianglechain/LineChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/TriangleChain.py` & `trianglechain-0.4.1/src/trianglechain/TriangleChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/bestfit.py` & `trianglechain-0.4.1/src/trianglechain/bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/density_estimation.py` & `trianglechain-0.4.1/src/trianglechain/density_estimation.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/limits.py` & `trianglechain-0.4.1/src/trianglechain/limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/make_subplots.py` & `trianglechain-0.4.1/src/trianglechain/make_subplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,27 +428,27 @@
                 else:
                     delete_later = False
                 axc.contour(
                     x_grid,
                     y_grid,
                     de,
                     levels=[lvl, np.inf],
-                    colors=color,
+                    colors=[color],
                     alpha=alpha,
                     **line_kwargs,
                 )
                 if delete_later:
                     del line_kwargs["zorder"]
             else:
                 axc.contour(
                     x_grid,
                     y_grid,
                     de,
                     levels=[lvl, np.inf],
-                    colors=color,
+                    colors=[color],
                     alpha=alpha,
                     **line_kwargs,
                 )
     # dummy plot to get legend
     plt.plot(data[columns[i]][0], data[columns[j]][0], label=label, color=color)
```

### Comparing `trianglechain-0.4.0/src/trianglechain/params.py` & `trianglechain-0.4.1/src/trianglechain/params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/utils_pj_hpd.py` & `trianglechain-0.4.1/src/trianglechain/utils_pj_hpd.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain/utils_plots.py` & `trianglechain-0.4.1/src/trianglechain/utils_plots.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.4.1/src/trianglechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.0
+Version: 0.4.1
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.4.0/src/trianglechain.egg-info/SOURCES.txt` & `trianglechain-0.4.1/src/trianglechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/tests/test_bestfit.py` & `trianglechain-0.4.1/tests/test_bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/tests/test_limits.py` & `trianglechain-0.4.1/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/tests/test_linechain.py` & `trianglechain-0.4.1/tests/test_linechain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/tests/test_params.py` & `trianglechain-0.4.1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.0/tests/test_trianglechain.py` & `trianglechain-0.4.1/tests/test_trianglechain.py`

 * *Files identical despite different names*

