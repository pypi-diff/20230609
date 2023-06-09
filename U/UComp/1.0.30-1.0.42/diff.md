# Comparing `tmp/UComp-1.0.30.tar.gz` & `tmp/UComp-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.30.tar", last modified: Wed Jun  7 17:20:54 2023, max compression
+gzip compressed data, was "UComp-1.0.42.tar", last modified: Fri Jun  9 15:22:48 2023, max compression
```

## Comparing `UComp-1.0.30.tar` & `UComp-1.0.42.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:20:54.537787 UComp-1.0.30/
--rw-rw-rw-   0        0        0      233 2023-06-06 16:58:27.000000 UComp-1.0.30/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-07 17:20:54.553433 UComp-1.0.30/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.30/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 17:20:54.537787 UComp-1.0.30/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.30/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.30/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.30/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.30/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    22455 2023-06-07 16:57:13.000000 UComp-1.0.30/UComp/UCmodule.py
--rw-rw-rw-   0        0        0       57 2023-06-07 16:15:43.000000 UComp-1.0.30/UComp/__init__.py
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.30/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    27981 2023-06-07 16:58:42.000000 UComp-1.0.30/UComp/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:20:54.537787 UComp-1.0.30/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 17:20:54.000000 UComp-1.0.30/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 17:20:54.553433 UComp-1.0.30/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-07 17:20:45.000000 UComp-1.0.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:22:48.809122 UComp-1.0.42/
+-rw-rw-rw-   0        0        0      356 2023-06-09 15:08:24.000000 UComp-1.0.42/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-06-09 15:22:48.809122 UComp-1.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.42/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:22:48.793506 UComp-1.0.42/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.42/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.42/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    10831 2023-06-09 15:21:08.000000 UComp-1.0.42/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11596 2023-06-09 12:22:16.000000 UComp-1.0.42/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.42/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.42/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24258 2023-06-09 15:20:10.000000 UComp-1.0.42/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      121 2023-06-09 12:24:40.000000 UComp-1.0.42/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.42/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.42/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.42/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.42/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29985 2023-06-09 15:19:29.000000 UComp-1.0.42/UComp/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:22:48.809122 UComp-1.0.42/UComp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-06-09 15:22:48.000000 UComp-1.0.42/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-09 15:22:48.000000 UComp-1.0.42/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:22:48.000000 UComp-1.0.42/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-09 15:22:48.000000 UComp-1.0.42/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 15:22:48.000000 UComp-1.0.42/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:22:48.809122 UComp-1.0.42/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-09 15:21:22.000000 UComp-1.0.42/setup.py
```

### Comparing `UComp-1.0.30/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.42/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.30/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.42/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.30/UComp/libopenblas.dll` & `UComp-1.0.42/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.30/UComp/tools.py` & `UComp-1.0.42/UComp/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,50 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import multiprocessing as mp
-# from UComp.UCmodule import *
-from UComp import UCmodule as uc
+if False:
+    import UCmodule as uc
+else:
+    from UComp import UCmodule as uc
 import seaborn as sns
 import scipy.stats as stats
 
 
+ipi = pd.read_pickle("ipi.bin")
+gdp = pd.read_pickle("gdp.bin")
+airpas = pd.read_pickle("airpas.bin")
+
+
+def ts(y, start='1990', freq='A'):
+    """
+    Converts a numpy vector or matrix into a pandas time series
+    """
+    if isinstance(y, list):
+        y = np.array(y)
+    elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
+        return y
+    if len(y.shape) > 1 and y.shape[0] < y.shape[1]:
+        y = y.T
+    time = pd.date_range(start=start, periods=y.shape[0], freq=freq)
+    y = np.array(y, dtype=float)
+    if len(y.shape) > 1:
+        return pd.DataFrame(y, time)
+    else:
+        return pd.Series(y, time)
+
 
 def obj2array(y):
     if isinstance(y, uc.UCmodel):
         x = y.v.values
     elif isinstance(y, uc.ETSmodel):
         x = y.comp[:, 0].values
     elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         x = y.values
-    elif isinstance(y, np.array):
+    elif isinstance(y, np.ndarray):
         x = y
     return x
 
 
 def pacfFun(ACF):
     nCoef = len(ACF)
     fi = np.zeros(nCoef)
@@ -57,14 +81,27 @@
     ind = np.where(~np.isnan(x))[0]
     ind1 = ind.min()
     ind2 = ind.max()
     return x[ind1 : ind2+1]
 
 
 def sumStats(y, decimals=5):
+    """
+    SumStats
+    Summary statistics of a matrix of variables
+
+    Inputs:
+    - y: a vector or matrix of time series
+    - decimals: number of decimals for the table
+
+    Returns:
+    Table of values
+
+    Author: Diego J. Pedregal
+    """
     x = obj2array(y)
     x = x[~np.isnan(x)]
     q25 = np.quantile(x, 0.25)
     q75 = np.quantile(x, 0.75)
     maxx = np.max(x)
     minx = np.min(x)
     meanx = np.mean(x)
@@ -106,14 +143,23 @@
                  "Variance: ",
                  "Skewness: ",
                  "Kurtosis: "]
     return out
 
 
 def gaussTest(y, axes=None):
+    """
+    gausTests
+    Tests of gaussianity of a time series
+
+    Inputs:
+    - y: a numpy vector or a Pandas time series object
+
+    Author: Diego J. Pedregal
+    """
     x = obj2array(y)
     x = x[~np.isnan(x)]
     n = len(x)
     nbins = int(np.sqrt(n))
     stdx = np.std(x)
     varx = stdx ** 2
     # Opening figure
@@ -146,14 +192,28 @@
     stat, pvalue = stats.shapiro(x)
     print('Shapiro Gaussianity test:')
     print('=========================')
     print(f"Stat: {stat:.4f}   P-value: {pvalue:.4f}")
 
 
 def ident(y, nCoef=None, nPar=0, axes=None):
+    """
+    ident
+    Autocorrelation functions of a time series
+
+    Inputs:
+    - y: a numpy vector or a pandas time series
+    - nCoef: number of autocorrelation coefficients to estimate
+    - nPar: number of parameters in a model if y is a residual
+
+    Returns:
+    A vector with all the dimensions
+
+    Author: Diego J. Pedregal
+    """
     if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         s = y.resample('Y').count()[1]
     else:
         s = 1
     x = obj2array(y)
     if nCoef is None:
         nCoef = max(min(37, int(np.floor(len(x) / 4))), s)
@@ -217,14 +277,23 @@
     if axes == None:
         fig, axes = plt.subplots(nrows=2, ncols=1, figsize=(8, 6))
     plotBar(ACF, axes[0], s, n)
     plotBar(PACF, axes[1], s, n, "PACF")
 
 
 def cusum(x, axes=None):
+    """
+    cusum
+    Cusum and cusum squared tests
+
+    Inputs:
+    - y: a numpy vector or a Pandas time series
+
+    Author: Diego J. Pedregal
+    """
     x = obj2array(x)
     n = len(x)
     mz = np.nanmean(x)
     stdz = np.nanstd(x)
     NMiss = ~np.isnan(x)
     Miss = np.isnan(x)
     standz = np.full((n, 1), np.nan)
@@ -259,14 +328,24 @@
     ax1.plot(t / n, color="red", linestyle="solid")
     ax1.plot(cusumsq, color="black", linestyle="solid")
     ax1.set_ylabel("CUSUMsq")
     plt.show(block=False)
 
 
 def varTest(x, parts=1/3):
+    """
+    varTest
+    Homoscedasticity tests
+
+    Inputs:
+    - y: a numpy vector or a Pandas time series
+    - parts: fraction of the sample to estimate variances
+
+    Author: Diego J. Pedregal
+    """
     x = obj2array(x)
     x = x[~np.isnan(x)]
     n = len(x)
     n1 = int(np.floor(n * parts))
     varStat = np.nanvar(x[:n1]) / np.nanvar(x[-n1:])
     if varStat > 1:
         varStat = 1 / varStat
@@ -285,16 +364,15 @@
     1D convolution: filtering or polynomial multiplication
 
     *args: list of vectors to convolute
 
     Returns:
     Convolution of all input vectors
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     n = len(args)
     if n > 2:
         return conv(args[0], conv(*args[1:]))
     else:
         # Convolution of two vectors
        return np.convolve(args[0], args[1])
@@ -307,16 +385,15 @@
     MA: MA numerator polynomial
     AR: AR denominator polynomial
     y: a vector, ts or tsibble object
 
     Returns:
     Filtered time series
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     # Filtering a time series with linear filter
     if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         xs = y.values
         y.t = y.index
         timeSeries = True
     else:
@@ -349,16 +426,15 @@
     y: a vector, ts or tsibble object
     difs: vector with differencing orders
     seas: vector of seasonal periods
 
     Returns:
     Differenced time series
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     # Mixture of differences operating on x
     n = len(difs)
     pol = np.array([1])
     for i in range(n):
         poli = np.concatenate(([1], np.zeros(seas[i] - 1), [-1]))
         if difs[i] > 0:
@@ -374,16 +450,15 @@
     Roots of polynomial
 
     x: coefficients of polynomial in descending order
 
     Returns:
     Roots of polynomial
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     # Roots of a polynomial
     if isinstance(x, list):
         x = np.array(x)
     if len(x) > 1:
         return np.roots(x)
     else:
@@ -393,16 +468,15 @@
 def zplane(MApoly=[1], ARpoly=[1]):
     """
     Real-imaginary plane to show roots of digital filters (ARMA)
 
     MApoly: coefficients of numerator polynomial in descending order
     ARpoly: coefficients of denominator polynomial in descending order
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     if isinstance(MApoly, list):
         MApoly = np.array(MApoly)
     if isinstance(ARpoly, list):
         ARpoly = np.array(ARpoly)
     # zplane plot
     arRoots = np.roots(ARpoly)
@@ -461,16 +535,15 @@
     MApoly: coefficients of numerator polynomial in descending order
     ARpoly: coefficients of denominator polynomial in descending order
     n: number of coefficients
 
     Returns:
     Time series representation of the ARMA model
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     # Converts ARMA to pure AR
     return armaFilter(MApoly, ARpoly, [1] + [0] * (n - 1))
 
 
 def acft(MApoly=[1], ARpoly=[1], ncoef=38, s=1):
     """
@@ -478,16 +551,16 @@
     Inputs:
         MApoly: coefficients of numerator polynomial in descending order
         ARpoly: coefficients of denominator polynomial in descending order
         ncoef: number of coefficients
         s: seasonal period, number of observations per year
     Returns:
         Theoretical autocorrelation functions
-    Author:
-        Diego J. Pedregal
+
+    Author: Diego J. Pedregal
     """
     # Theoretical ACF and PACF from ARMA model
     correct = True
     if len(ARpoly) > 1 and any(np.abs(np.roots(ARpoly)) >= 1):
         print('Non-stationary model')
         correct = False
     if len(MApoly) > 1 and any(np.abs(np.roots(MApoly)) >= 1):
@@ -540,16 +613,16 @@
         h: forecasting horizon
         step: observations ahead to move the forecasting origin
         output: output TRUE/FALSE
         window: fixed window width in number of observations (None for non-fixed)
         parallel: run forecasts in parallel
     Returns:
         A vector with all the dimensions
-    Author:
-        Diego J. Pedregal
+
+    Author: Diego J. Pedregal
     """
     # Rolling for nSeries
     # out = [h, nOrigs, nModels, nSeries]
     if y.ndim == 1:
         y = y.reshape(-1, 1)
     nSeries = y.shape[1]
     n = y.shape[0]
@@ -582,16 +655,16 @@
         output: output TRUE/FALSE
         graph: graphical output TRUE/FALSE
         window: fixed window width in number of observations (None for non-fixed)
         parallel: run forecasts in parallel
         *args, **kwargs: rest of inputs to forecFun function
     Returns:
         Next time stamp
-    Author:
-        Diego J. Pedregal
+
+    Author: Diego J. Pedregal
     """
     # Rolling for 1 series
     # out = [h, nOrigs, nModels]
     n = len(y)
     origs = range(orig, n - h + 1, step)
     nOr = len(origs)
     if window is None:
@@ -637,18 +710,16 @@
         y a vector or matrix of time series (the same used in slide call)
         orig starting forecasting origin (the same used in slide call)
         step observations ahead to move the forecasting origin (the same used in slide call)
         errorFun user function to calculate error measures
         collectFun aggregation function (mean, median, etc.)
     Returns:
         Errors table
-    Author:
-        Diego J. Pedregal
-    Examples:
-        plotSlide(py1, AirPassengers, 100, 1, errorFun)
+
+    Author: Diego J. Pedregal
     """
     # py1 = [h, nOrigs, nModels, nSeries]
     h = py1.shape[0]
     nOrigs = py1.shape[1]
     nMethods = py1.shape[2]
     nSeries = py1.shape[3]
     if pd.isna(nSeries):
@@ -688,20 +759,16 @@
     Inputs:
         py:         matrix of forecasts (h x nMethods x nForecasts)
         y:          a matrix of actual values (n x nForecasts)
         s:          seasonal period, number of observations per year
         collectFun: aggregation function (mean, median, etc.)
     Returns:
         Table of results
-    Author:
-        Diego J. Pedregal
-    Examples:
-        accuracy(py, y, 12)
-    #' @rdname Accuracy
-    :rtype: object
+
+    Author: Diego J. Pedregal
     """
     # Accuracy for 1 time series y and several forecasting methods py and h steps ahead
     # py is h x nMethods x nSeries
     # y is n x nSeries
     spy = len(py.shape)
     if (isinstance(py, pd.Series) or isinstance(py, pd.DataFrame)) and isinstance(y, pd.Series):
         tpy = py.index
@@ -763,14 +830,26 @@
                                    np.nansum(np.abs(e), axis=0) / np.nansum(np.abs(fRW), axis=0),
                                    np.sqrt(np.nansum(p * p, axis=0) / np.nansum(theil * theil, axis=0))))
         out[i, :] = collectFun(aux, axis=1)
     return pd.DataFrame(out, index=rownames, columns=colnames)
 
 
 def tsDisplay(y, nCoef=None, nPar=0):
+    """
+    tsDisplay
+    Displays a time series plot with autocorrelation functions
+
+    Inputs:
+    - y: a numpy vector or a Pandas time series object
+    - nCoef: number of autocorrelation coefficients to estimate
+    - nPar: number of parameters in a model if y is a residual
+    - s: seasonal period, number of observations per year
+
+    Author: Diego J. Pedregal
+    """
     if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         s = y.resample('Y').count()[1]
     else:
         s = 1
     # x = obj2array(y)
     # if s is None:
     #     s = frequency(x)
@@ -793,16 +872,15 @@
     y: a vector, ts or tsibble object
     parts: proportion of sample to include in ratio of variances test
     nCoef: number of autocorrelation coefficients to estimate
     nPar: number of parameters in a model if y is a residual
     s: seasonal period, number of observations per year
     avoid: number of observations to avoid at beginning of sample to eliminate initial effects
 
-    Author:
-    Diego J. Pedregal
+    Author: Diego J. Pedregal
     """
     if isinstance(x, pd.Series) or isinstance(x, pd.DataFrame):
         s = x.resample('Y').count()[1]
     else:
         s = 1
     print("Summary statistics:")
     print("===================")
```

### Comparing `UComp-1.0.30/setup.py` & `UComp-1.0.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.30',
+    version='1.0.42',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

