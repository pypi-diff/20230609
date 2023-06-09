# Comparing `tmp/FoKL-1.1.0.tar.gz` & `tmp/FoKL-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoKL-1.1.0.tar", last modified: Fri Jun  9 17:32:00 2023, max compression
+gzip compressed data, was "FoKL-1.1.1.tar", last modified: Fri Jun  9 18:13:34 2023, max compression
```

## Comparing `FoKL-1.1.0.tar` & `FoKL-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.664702 FoKL-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 17:31:50.000000 FoKL-1.1.0/.github/workflows/python-publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/Examples/Lorenz/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:31:50.000000 FoKL-1.1.0/Examples/Lorenz/ReadMe.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/Examples/Sinusoid/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 17:31:50.000000 FoKL-1.1.0/Examples/Sinusoid/DATA_nois.csv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 17:31:50.000000 FoKL-1.1.0/Examples/Sinusoid/ReadMe.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 17:31:50.000000 FoKL-1.1.0/Examples/Sinusoid/X.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 17:31:50.000000 FoKL-1.1.0/Examples/Sinusoid/Y.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 17:31:50.000000 FoKL-1.1.0/Examples/Sinusoid/python_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 17:31:50.000000 FoKL-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 17:32:00.664702 FoKL-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 17:31:50.000000 FoKL-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 17:31:50.000000 FoKL-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 17:32:00.664702 FoKL-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.660701 FoKL-1.1.0/src/FoKL/
--rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/FoKLRoutines.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/GP_Integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/coverage3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 17:31:50.000000 FoKL-1.1.0/src/FoKL/splineConvert500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.664702 FoKL-1.1.0/src/FoKL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 17:32:00.000000 FoKL-1.1.0/src/FoKL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 17:32:00.000000 FoKL-1.1.0/src/FoKL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:32:00.000000 FoKL-1.1.0/src/FoKL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 17:32:00.000000 FoKL-1.1.0/src/FoKL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 17:32:00.000000 FoKL-1.1.0/src/FoKL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.572816 FoKL-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.564816 FoKL-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 18:13:24.000000 FoKL-1.1.1/.github/workflows/python-publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/Examples/Lorenz/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Lorenz/ReadMe.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/Examples/Sinusoid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/DATA_nois.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/ReadMe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/X.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/Y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/python_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 18:13:24.000000 FoKL-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:13:34.572816 FoKL-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:13:24.000000 FoKL-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 18:13:24.000000 FoKL-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 18:13:34.572816 FoKL-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.572816 FoKL-1.1.1/src/FoKL/
+-rw-r--r--   0 runner    (1001) docker     (123)    34151 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/FoKLRoutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/GP_Integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/coverage3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/splineConvert500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.572816 FoKL-1.1.1/src/FoKL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/top_level.txt
```

### Comparing `FoKL-1.1.0/Examples/Sinusoid/DATA_nois.csv` & `FoKL-1.1.1/Examples/Sinusoid/DATA_nois.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/Examples/Sinusoid/X.csv` & `FoKL-1.1.1/Examples/Sinusoid/X.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/Examples/Sinusoid/Y.csv` & `FoKL-1.1.1/Examples/Sinusoid/Y.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/Examples/Sinusoid/python_test.py` & `FoKL-1.1.1/Examples/Sinusoid/python_test.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/LICENSE` & `FoKL-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/PKG-INFO` & `FoKL-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoKL
-Version: 1.1.0
+Version: 1.1.1
 Summary: Karhunen Loève decomposed Gaussian processes with forward variable selection
 Home-page: https://github.com/derek-slack/FokLPackage
 Author-email: ESMS Group <derek.slack.001@gmail.com>
 Project-URL: Bug Tracker, https://github.com/derek-slack/FokLPackage/issues
 Project-URL: Changelog, https://github.com/derek-slack/FokLPackage/releases
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `FoKL-1.1.0/pyproject.toml` & `FoKL-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/setup.cfg` & `FoKL-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/src/FoKL/FoKLRoutines.py` & `FoKL-1.1.1/src/FoKL/FoKLRoutines.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import math
 import numpy as np
 from numpy import linalg as LA
 from scipy.linalg import eigh
 import matplotlib.pyplot as plt
 
 class FoKL:
-    def splineconvert500(A):
+    def splineconvert500(self,A):
         """
         Same as splineconvert, but for a larger basis of 500
         """
 
         coef = np.loadtxt(A)
 
         phi = []
@@ -20,15 +20,15 @@
             c = coef[i * 499:(i + 1) * 499, 2]
             d = coef[i * 499:(i + 1) * 499, 3]
 
             phi.append([a, b, c, d])
 
         return phi
 
-    def coverage3(betas, normputs, data, phis, mtx, draws, plots):
+    def coverage3(self,betas, normputs, data, phis, mtx, draws, plots):
         """
             Inputs:
                 Interprets outputs of emulator
 
                 betas - betas emulator output
 
                 normputs - normalized inputs
@@ -111,15 +111,15 @@
             plt.plot(data, 'ro')
 
             plt.show()
 
         rmse = np.sqrt(np.mean(meen - data) ** 2)
         return meen, bounds, rmse
 
-    def gibbs(inputs, data, phis, Xin, discmtx, a, b, atau, btau,
+    def gibbs(self, inputs, data, phis, Xin, discmtx, a, b, atau, btau,
               draws):
         """
         'sigsqd0' is the initial guess for the obs error variance
 
         'inputs' is the set of normalized inputs -- both parameters and model
         inputs -- with columns corresponding to inputs and rows the different
         experimental designs
@@ -276,15 +276,15 @@
         lik = -(n / 2) * np.log(siglik) - (n - 1) / 2
         ev = (mmtx + 1) * np.log(n) - 2 * np.max(lik)
 
         X = X[:, 0:mmtx + 1]
 
         return betas, sigs, taus, betahat, X, ev
 
-    def emulator(inputs, data, phis, relats_in, a, b, atau, btau, tolerance, draws, gimmie, way3, threshav, threshstda, threshstdb, aic):
+    def emulator(self, inputs, data, phis, relats_in, a, b, atau, btau, tolerance, draws, gimmie, way3, threshav, threshstda, threshstdb, aic):
         """
         this version uses 3 way interactions use routines.emulator_Xin for two way interactions
 
         this version uses the 'Xin' mode of the gibbs sampler
 
         builds a single-output bss-anova emulator for a stationary dataset in an
         automated fashion
@@ -556,15 +556,15 @@
             betas = beters
             mtx = damtx
 
         return betas, mtx, evs
 
 
 
-    def GP_Integrate(betas, matrix, b, norms, phis, start, stop, y0, h, used_inputs):
+    def GP_Integrate(self, betas, matrix, b, norms, phis, start, stop, y0, h, used_inputs):
         """""
           betas is a list of arrays in which each entry to the list contains a specific row of the betas matrix,
           or the mean of the the betas matrix for each model being integrated
 
           matrix is a list of arrays containing the interaction matrix of each model
 
           b is an array of of the values of all the other inputs to the model(s) (including
```

### Comparing `FoKL-1.1.0/src/FoKL/GP_Integrate.py` & `FoKL-1.1.1/src/FoKL/GP_Integrate.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/src/FoKL/coverage3.py` & `FoKL-1.1.1/src/FoKL/coverage3.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/src/FoKL/emulator.py` & `FoKL-1.1.1/src/FoKL/emulator.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/src/FoKL/gibbs.py` & `FoKL-1.1.1/src/FoKL/gibbs.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/src/FoKL/splineConvert500.py` & `FoKL-1.1.1/src/FoKL/splineConvert500.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.0/src/FoKL.egg-info/PKG-INFO` & `FoKL-1.1.1/src/FoKL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoKL
-Version: 1.1.0
+Version: 1.1.1
 Summary: Karhunen Loève decomposed Gaussian processes with forward variable selection
 Home-page: https://github.com/derek-slack/FokLPackage
 Author-email: ESMS Group <derek.slack.001@gmail.com>
 Project-URL: Bug Tracker, https://github.com/derek-slack/FokLPackage/issues
 Project-URL: Changelog, https://github.com/derek-slack/FokLPackage/releases
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `FoKL-1.1.0/src/FoKL.egg-info/SOURCES.txt` & `FoKL-1.1.1/src/FoKL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

