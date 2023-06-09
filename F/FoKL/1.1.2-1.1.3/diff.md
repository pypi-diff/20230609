# Comparing `tmp/FoKL-1.1.2.tar.gz` & `tmp/FoKL-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoKL-1.1.2.tar", last modified: Fri Jun  9 18:20:36 2023, max compression
+gzip compressed data, was "FoKL-1.1.3.tar", last modified: Fri Jun  9 18:30:00 2023, max compression
```

## Comparing `FoKL-1.1.2.tar` & `FoKL-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.174608 FoKL-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 18:20:27.000000 FoKL-1.1.2/.github/workflows/python-publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/Examples/Lorenz/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Lorenz/ReadMe.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/Examples/Sinusoid/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/DATA_nois.csv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/ReadMe.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/X.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/Y.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/python_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 18:20:27.000000 FoKL-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:20:36.174608 FoKL-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:20:27.000000 FoKL-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 18:20:27.000000 FoKL-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 18:20:36.174608 FoKL-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.174608 FoKL-1.1.2/src/FoKL/
--rw-r--r--   0 runner    (1001) docker     (123)    34141 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/FoKLRoutines.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/GP_Integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/coverage3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/splineConvert500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.174608 FoKL-1.1.2/src/FoKL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.909246 FoKL-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.905246 FoKL-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.909246 FoKL-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 18:29:51.000000 FoKL-1.1.3/.github/workflows/python-publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.905246 FoKL-1.1.3/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.909246 FoKL-1.1.3/Examples/Lorenz/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:29:51.000000 FoKL-1.1.3/Examples/Lorenz/ReadMe.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.909246 FoKL-1.1.3/Examples/Sinusoid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 18:29:51.000000 FoKL-1.1.3/Examples/Sinusoid/DATA_nois.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 18:29:51.000000 FoKL-1.1.3/Examples/Sinusoid/ReadMe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:29:51.000000 FoKL-1.1.3/Examples/Sinusoid/X.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:29:51.000000 FoKL-1.1.3/Examples/Sinusoid/Y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 18:29:51.000000 FoKL-1.1.3/Examples/Sinusoid/python_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 18:29:51.000000 FoKL-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:30:00.909246 FoKL-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:29:51.000000 FoKL-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 18:29:51.000000 FoKL-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 18:30:00.909246 FoKL-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.905246 FoKL-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.909246 FoKL-1.1.3/src/FoKL/
+-rw-r--r--   0 runner    (1001) docker     (123)    34137 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/FoKLRoutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/GP_Integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/coverage3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 18:29:51.000000 FoKL-1.1.3/src/FoKL/splineConvert500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:30:00.909246 FoKL-1.1.3/src/FoKL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:30:00.000000 FoKL-1.1.3/src/FoKL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:30:00.000000 FoKL-1.1.3/src/FoKL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:30:00.000000 FoKL-1.1.3/src/FoKL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:30:00.000000 FoKL-1.1.3/src/FoKL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 18:30:00.000000 FoKL-1.1.3/src/FoKL.egg-info/top_level.txt
```

### Comparing `FoKL-1.1.2/Examples/Sinusoid/DATA_nois.csv` & `FoKL-1.1.3/Examples/Sinusoid/DATA_nois.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/Examples/Sinusoid/X.csv` & `FoKL-1.1.3/Examples/Sinusoid/X.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/Examples/Sinusoid/Y.csv` & `FoKL-1.1.3/Examples/Sinusoid/Y.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/Examples/Sinusoid/python_test.py` & `FoKL-1.1.3/Examples/Sinusoid/python_test.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/LICENSE` & `FoKL-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/PKG-INFO` & `FoKL-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoKL
-Version: 1.1.2
+Version: 1.1.3
 Summary: Karhunen Loève decomposed Gaussian processes with forward variable selection
 Home-page: https://github.com/derek-slack/FokLPackage
 Author-email: ESMS Group <derek.slack.001@gmail.com>
 Project-URL: Bug Tracker, https://github.com/derek-slack/FokLPackage/issues
 Project-URL: Changelog, https://github.com/derek-slack/FokLPackage/releases
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `FoKL-1.1.2/pyproject.toml` & `FoKL-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/setup.cfg` & `FoKL-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/src/FoKL/FoKLRoutines.py` & `FoKL-1.1.3/src/FoKL/FoKLRoutines.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,98 @@
             plt.plot(data, 'ro')
 
             plt.show()
 
         rmse = np.sqrt(np.mean(meen - data) ** 2)
         return meen, bounds, rmse
 
-    def gibbs(self, inputs, data, phis, Xin, discmtx, a, b, atau, btau,
+    def emulator(self, inputs, data, phis, relats_in, a, b, atau, btau, tolerance, draws, gimmie, way3, threshav, threshstda, threshstdb, aic):
+        """
+        this version uses 3 way interactions use routines.emulator_Xin for two way interactions
+
+        this version uses the 'Xin' mode of the gibbs sampler
+
+        builds a single-output bss-anova emulator for a stationary dataset in an
+        automated fashion
+
+        function inputs:
+        'sigsqd0' is the initial guess for the obs error variance
+
+        'inputs' is the set of inputs normalized on [0,1]: matrix or numpy array
+        with columns corresponding to inputs and rows the different experimental designs
+
+        'data' are the output dataset used to build the function: column vector,
+        with entries corresponding to rows of 'inputs'
+
+        'relats' is a boolean matrix indicating which terms should be excluded
+        from the model building; for instance if a certain main effect should be
+        excluded relats will include a row with a 1 in the column for that input
+        and zeros elsewhere; if a certain two way interaction should be excluded
+        there should be a row with ones in those columns and zeros elsewhere
+        to exclude no terms 'relats = np.array([[0]])'. An example of excluding
+        the first input main effect and its interaction with the third input for
+        a case with three total inputs is:'relats = np.array([[1,0,0],[1,0,1]])'
+
+        'phis' are a data structure with the spline coefficients for the basis
+        functions, built with 'spline_coefficient.txt' and 'splineconvert' or
+        'spline_coefficient_500.txt' and 'splineconvert500' (the former provides
+        25 basis functions: enough for most things -- while the latter provides
+        500: definitely enough for anything)
+
+        'a' and 'b' are the shape and scale parameters of the ig distribution for
+        the observation error variance of the data. the observation error model is
+        white noise choose the mode of the ig distribution to match the noise in
+        the output dataset and the mean to broaden it some
+
+        'atau' and 'btau' are the parameters of the ig distribution for the 'tau
+        squared' parameter: the variance of the beta priors is iid normal mean
+        zero with variance equal to sigma squared times tau squared. tau squared
+        must be scaled in the prior such that the product of tau squared and sigma
+        squared scales with the output dataset
+
+        'tolerance' controls how hard the function builder tries to find a better
+        model once adding terms starts to show diminishing returns. a good
+        default is 3 -- large datasets could benefit from higher values
+
+        'draws' is the total number of draws from the posterior for each tested
+        model
+
+        'draws' is the total number of draws from the posterior for each tested
+
+        'gimmie' is a boolean causing the routine to return the most complex
+        model tried instead of the model with the optimum bic
+
+        'aic' is a boolean specifying the use of the aikaike information
+        criterion
+
+        function outputs:
+
+        'betas' are a draw from the posterior distribution of coefficients: matrix,
+        with rows corresponding to draws and columns corresponding to terms in the
+        GP
+
+        'mtx' is the basis function interaction matrix from the best model:
+        matrix, with rows corresponding to terms in the GP (and thus to the
+        columns of 'betas' and columns corresponding to inputs). A given entry in
+        the matrix gives the order of the basis function appearing in a given term
+        in the GP.
+        All basis functions indicated on a given row are multiplied together.
+        a zero indicates no basis function from a given input is present in a
+        given term.
+
+        'ev' is a vector of BIC values from all of the models evaluated
+        """
+
+        def perms(x):
+            """Python equivalent of MATLAB perms."""
+            # from https://stackoverflow.com/questions/38130008/python-equivalent-for-matlabs-perms
+            a = np.vstack(list(itertools.permutations(x)))[::-1]
+
+            return a
+        def gibbs(self, inputs, data, phis, Xin, discmtx, a, b, atau, btau,
               draws):
         """
         'sigsqd0' is the initial guess for the obs error variance
 
         'inputs' is the set of normalized inputs -- both parameters and model
         inputs -- with columns corresponding to inputs and rows the different
         experimental designs
@@ -275,99 +358,15 @@
 
         lik = -(n / 2) * np.log(siglik) - (n - 1) / 2
         ev = (mmtx + 1) * np.log(n) - 2 * np.max(lik)
 
         X = X[:, 0:mmtx + 1]
 
         return betas, sigs, taus, betahat, X, ev
-
-    def emulator(self, inputs, data, phis, relats_in, a, b, atau, btau, tolerance, draws, gimmie, way3, threshav, threshstda, threshstdb, aic):
-        """
-        this version uses 3 way interactions use routines.emulator_Xin for two way interactions
-
-        this version uses the 'Xin' mode of the gibbs sampler
-
-        builds a single-output bss-anova emulator for a stationary dataset in an
-        automated fashion
-
-        function inputs:
-        'sigsqd0' is the initial guess for the obs error variance
-
-        'inputs' is the set of inputs normalized on [0,1]: matrix or numpy array
-        with columns corresponding to inputs and rows the different experimental designs
-
-        'data' are the output dataset used to build the function: column vector,
-        with entries corresponding to rows of 'inputs'
-
-        'relats' is a boolean matrix indicating which terms should be excluded
-        from the model building; for instance if a certain main effect should be
-        excluded relats will include a row with a 1 in the column for that input
-        and zeros elsewhere; if a certain two way interaction should be excluded
-        there should be a row with ones in those columns and zeros elsewhere
-        to exclude no terms 'relats = np.array([[0]])'. An example of excluding
-        the first input main effect and its interaction with the third input for
-        a case with three total inputs is:'relats = np.array([[1,0,0],[1,0,1]])'
-
-        'phis' are a data structure with the spline coefficients for the basis
-        functions, built with 'spline_coefficient.txt' and 'splineconvert' or
-        'spline_coefficient_500.txt' and 'splineconvert500' (the former provides
-        25 basis functions: enough for most things -- while the latter provides
-        500: definitely enough for anything)
-
-        'a' and 'b' are the shape and scale parameters of the ig distribution for
-        the observation error variance of the data. the observation error model is
-        white noise choose the mode of the ig distribution to match the noise in
-        the output dataset and the mean to broaden it some
-
-        'atau' and 'btau' are the parameters of the ig distribution for the 'tau
-        squared' parameter: the variance of the beta priors is iid normal mean
-        zero with variance equal to sigma squared times tau squared. tau squared
-        must be scaled in the prior such that the product of tau squared and sigma
-        squared scales with the output dataset
-
-        'tolerance' controls how hard the function builder tries to find a better
-        model once adding terms starts to show diminishing returns. a good
-        default is 3 -- large datasets could benefit from higher values
-
-        'draws' is the total number of draws from the posterior for each tested
-        model
-
-        'draws' is the total number of draws from the posterior for each tested
-
-        'gimmie' is a boolean causing the routine to return the most complex
-        model tried instead of the model with the optimum bic
-
-        'aic' is a boolean specifying the use of the aikaike information
-        criterion
-
-        function outputs:
-
-        'betas' are a draw from the posterior distribution of coefficients: matrix,
-        with rows corresponding to draws and columns corresponding to terms in the
-        GP
-
-        'mtx' is the basis function interaction matrix from the best model:
-        matrix, with rows corresponding to terms in the GP (and thus to the
-        columns of 'betas' and columns corresponding to inputs). A given entry in
-        the matrix gives the order of the basis function appearing in a given term
-        in the GP.
-        All basis functions indicated on a given row are multiplied together.
-        a zero indicates no basis function from a given input is present in a
-        given term.
-
-        'ev' is a vector of BIC values from all of the models evaluated
-        """
-
-        def perms(x):
-            """Python equivalent of MATLAB perms."""
-            # from https://stackoverflow.com/questions/38130008/python-equivalent-for-matlabs-perms
-            a = np.vstack(list(itertools.permutations(x)))[::-1]
-
-            return a
-
+    
         # 'n' is the number of datapoints whereas 'm' is the number of inputs
         n, m = np.shape(inputs)
         mrel = n
         damtx = np.array([])
         evs = np.array([])
 
         # Conversion of Lines 79-100 of emulator_Xin.m
@@ -450,15 +449,15 @@
                     vn = 1
                 if np.size(damtx) == 0:
                     damtx = vecs
                 else:
                     damtx = np.append(damtx, vecs, axis=0)
                 [dam,null] = np.shape(damtx)
 
-                [beters, null, null, null, xers, ev] = FoKL.gibbs(inputs, data, phis, X, damtx, a, b, atau, btau, draws)
+                [beters, null, null, null, xers, ev] = gibbs(inputs, data, phis, X, damtx, a, b, atau, btau, draws)
 
                 if aic:
                     ev = ev + (2 - np.log(n)) * (dam + 1)
 
                 betavs = np.abs(np.mean(beters[int(np.ceil((draws / 2)+1)):draws, (dam - vm + 1):dam+1], axis=0))
                 betavs2 = np.divide(np.std(np.array(beters[int(np.ceil(draws/2)+1):draws, dam-vm+1:dam+1]), axis=0), np.abs(np.mean(beters[int(np.ceil(draws / 2)):draws, dam-vm+1:dam+2], axis=0))) # betavs2 error in std deviation formatting
                 betavs3 = np.array(range(dam-vm+2, dam+2))
@@ -481,15 +480,15 @@
                         damtx_test = damtx
                         count = 1
                         for k in range(0, np.size(killtest)):
                             damtx_test = np.delete(damtx_test, (int(np.array(killtest[k]))-count), 0)
                             count = count + 1
                         damtest, null = np.shape(damtx_test)
 
-                        [betertest, null, null, null, Xtest, evtest] = FoKL.gibbs(inputs, data, phis, X, damtx_test, a, b, atau, btau, draws)
+                        [betertest, null, null, null, Xtest, evtest] = gibbs(inputs, data, phis, X, damtx_test, a, b, atau, btau, draws)
                         if aic:
                             evtest = evtest + (2 - np.log(n))*(damtest+1)
                         if evtest < evmin:
                             killset = killtest
                             evmin = evtest
                             xers = Xtest
                             beters = betertest
```

### Comparing `FoKL-1.1.2/src/FoKL/GP_Integrate.py` & `FoKL-1.1.3/src/FoKL/GP_Integrate.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/src/FoKL/coverage3.py` & `FoKL-1.1.3/src/FoKL/coverage3.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/src/FoKL/emulator.py` & `FoKL-1.1.3/src/FoKL/emulator.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/src/FoKL/gibbs.py` & `FoKL-1.1.3/src/FoKL/gibbs.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/src/FoKL/splineConvert500.py` & `FoKL-1.1.3/src/FoKL/splineConvert500.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.2/src/FoKL.egg-info/PKG-INFO` & `FoKL-1.1.3/src/FoKL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoKL
-Version: 1.1.2
+Version: 1.1.3
 Summary: Karhunen Loève decomposed Gaussian processes with forward variable selection
 Home-page: https://github.com/derek-slack/FokLPackage
 Author-email: ESMS Group <derek.slack.001@gmail.com>
 Project-URL: Bug Tracker, https://github.com/derek-slack/FokLPackage/issues
 Project-URL: Changelog, https://github.com/derek-slack/FokLPackage/releases
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `FoKL-1.1.2/src/FoKL.egg-info/SOURCES.txt` & `FoKL-1.1.3/src/FoKL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

