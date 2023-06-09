# Comparing `tmp/UComp-1.0.40.tar.gz` & `tmp/UComp-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.40.tar", last modified: Fri Jun  9 15:10:38 2023, max compression
+gzip compressed data, was "UComp-1.0.41.tar", last modified: Fri Jun  9 15:13:42 2023, max compression
```

## Comparing `UComp-1.0.40.tar` & `UComp-1.0.41.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:10:38.652170 UComp-1.0.40/
--rw-rw-rw-   0        0        0      356 2023-06-09 15:08:24.000000 UComp-1.0.40/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-09 15:10:38.653162 UComp-1.0.40/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.40/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 15:10:38.641170 UComp-1.0.40/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.40/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.40/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    10800 2023-06-09 12:22:16.000000 UComp-1.0.40/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11596 2023-06-09 12:22:16.000000 UComp-1.0.40/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.40/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.40/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    25043 2023-06-09 12:22:16.000000 UComp-1.0.40/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      121 2023-06-09 12:24:40.000000 UComp-1.0.40/UComp/__init__.py
--rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.40/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.40/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.40/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.40/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29438 2023-06-09 15:06:21.000000 UComp-1.0.40/UComp/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:10:38.651164 UComp-1.0.40/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-09 15:10:38.000000 UComp-1.0.40/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-09 15:10:38.000000 UComp-1.0.40/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:10:38.000000 UComp-1.0.40/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-09 15:10:38.000000 UComp-1.0.40/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 15:10:38.000000 UComp-1.0.40/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 15:10:38.654451 UComp-1.0.40/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-09 15:10:18.000000 UComp-1.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:13:42.783030 UComp-1.0.41/
+-rw-rw-rw-   0        0        0      356 2023-06-09 15:08:24.000000 UComp-1.0.41/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-06-09 15:13:42.798637 UComp-1.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.41/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:13:42.767390 UComp-1.0.41/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.41/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.41/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    10800 2023-06-09 12:22:16.000000 UComp-1.0.41/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11596 2023-06-09 12:22:16.000000 UComp-1.0.41/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.41/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.41/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24756 2023-06-09 14:56:32.000000 UComp-1.0.41/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      121 2023-06-09 12:24:40.000000 UComp-1.0.41/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.41/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.41/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.41/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.41/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29438 2023-06-09 15:06:21.000000 UComp-1.0.41/UComp/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:13:42.783030 UComp-1.0.41/UComp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-06-09 15:13:42.000000 UComp-1.0.41/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-09 15:13:42.000000 UComp-1.0.41/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:13:42.000000 UComp-1.0.41/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-09 15:13:42.000000 UComp-1.0.41/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 15:13:42.000000 UComp-1.0.41/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:13:42.798637 UComp-1.0.41/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-09 15:13:37.000000 UComp-1.0.41/setup.py
```

### Comparing `UComp-1.0.40/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.41/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/ETSmodule.py` & `UComp-1.0.41/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/PTSmodule.py` & `UComp-1.0.41/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.41/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/UCmodule.py` & `UComp-1.0.41/UComp/UCmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,19 +109,14 @@
     def __init__(self, y: pd.DataFrame, s: int = np.nan, u: np.array = np.array([]), model: str = "?/none/?/?",
                  h: int = 9999, lambdaBoxCox: np.array = np.array(1.0), outlier: float = 9999.0, tTest: bool = False,
                  criterion: str = "aic", periods: np.array = np.array([np.nan]), verbose: bool = False,
                  stepwise: bool = False, p0: np.array = np.array([-9999.9]), arma: bool = False,
                  TVP: np.array = np.array([0.0]),
                  trendOptions: str = "none/rw/llt/dt", seasonalOptions: str = "none/equal/different",
                  irregularOptions: str = "none/arma(0,0)", MSOE: bool = False, PTSnames: bool = False):
-        def UCsetup(y, u=None, model=None, outlier=None, stepwise=None, tTest=None, p0=None, h=None,
-                    lambda_=None, criterion=None, periods=None, verbose=None, arma=None, TVP=None,
-                    trendOptions=None, seasonalOptions=None, irregularOptions=None):
-
-
         if isinstance(y, np.ndarray) and np.isnan(s):
             raise ValueError("Either 'y' should be a Panda time series or 's' should be supplied!!")
         if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
             s = y.resample('Y').count()[1]
         if np.isnan(lambdaBoxCox):
             lambdaBoxCox = np.array([9999.9])
         if (any(np.isnan(TVP)) and u.size != 0):
```

### Comparing `UComp-1.0.40/UComp/airpas.bin` & `UComp-1.0.41/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/gdp.bin` & `UComp-1.0.41/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/ipi.bin` & `UComp-1.0.41/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/libopenblas.dll` & `UComp-1.0.41/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/UComp/tools.py` & `UComp-1.0.41/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.40/setup.py` & `UComp-1.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.40',
+    version='1.0.41',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

