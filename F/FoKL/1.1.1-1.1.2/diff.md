# Comparing `tmp/FoKL-1.1.1.tar.gz` & `tmp/FoKL-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoKL-1.1.1.tar", last modified: Fri Jun  9 18:13:34 2023, max compression
+gzip compressed data, was "FoKL-1.1.2.tar", last modified: Fri Jun  9 18:20:36 2023, max compression
```

## Comparing `FoKL-1.1.1.tar` & `FoKL-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.572816 FoKL-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.564816 FoKL-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 18:13:24.000000 FoKL-1.1.1/.github/workflows/python-publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/Examples/Lorenz/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Lorenz/ReadMe.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/Examples/Sinusoid/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/DATA_nois.csv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/ReadMe.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/X.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/Y.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 18:13:24.000000 FoKL-1.1.1/Examples/Sinusoid/python_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 18:13:24.000000 FoKL-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:13:34.572816 FoKL-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:13:24.000000 FoKL-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 18:13:24.000000 FoKL-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 18:13:34.572816 FoKL-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.568816 FoKL-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.572816 FoKL-1.1.1/src/FoKL/
--rw-r--r--   0 runner    (1001) docker     (123)    34151 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/FoKLRoutines.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/GP_Integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/coverage3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 18:13:24.000000 FoKL-1.1.1/src/FoKL/splineConvert500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:34.572816 FoKL-1.1.1/src/FoKL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 18:13:34.000000 FoKL-1.1.1/src/FoKL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.174608 FoKL-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 18:20:27.000000 FoKL-1.1.2/.github/workflows/python-publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/Examples/Lorenz/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Lorenz/ReadMe.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/Examples/Sinusoid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/DATA_nois.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/ReadMe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/X.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/Y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 18:20:27.000000 FoKL-1.1.2/Examples/Sinusoid/python_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 18:20:27.000000 FoKL-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:20:36.174608 FoKL-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:20:27.000000 FoKL-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 18:20:27.000000 FoKL-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 18:20:36.174608 FoKL-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.170608 FoKL-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.174608 FoKL-1.1.2/src/FoKL/
+-rw-r--r--   0 runner    (1001) docker     (123)    34141 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/FoKLRoutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/GP_Integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/coverage3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 18:20:27.000000 FoKL-1.1.2/src/FoKL/splineConvert500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:36.174608 FoKL-1.1.2/src/FoKL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 18:20:36.000000 FoKL-1.1.2/src/FoKL.egg-info/top_level.txt
```

### Comparing `FoKL-1.1.1/Examples/Sinusoid/DATA_nois.csv` & `FoKL-1.1.2/Examples/Sinusoid/DATA_nois.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/Examples/Sinusoid/X.csv` & `FoKL-1.1.2/Examples/Sinusoid/X.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/Examples/Sinusoid/Y.csv` & `FoKL-1.1.2/Examples/Sinusoid/Y.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/Examples/Sinusoid/python_test.py` & `FoKL-1.1.2/Examples/Sinusoid/python_test.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/LICENSE` & `FoKL-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/PKG-INFO` & `FoKL-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoKL
-Version: 1.1.1
+Version: 1.1.2
 Summary: Karhunen Loève decomposed Gaussian processes with forward variable selection
 Home-page: https://github.com/derek-slack/FokLPackage
 Author-email: ESMS Group <derek.slack.001@gmail.com>
 Project-URL: Bug Tracker, https://github.com/derek-slack/FokLPackage/issues
 Project-URL: Changelog, https://github.com/derek-slack/FokLPackage/releases
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `FoKL-1.1.1/pyproject.toml` & `FoKL-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/setup.cfg` & `FoKL-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/src/FoKL/FoKLRoutines.py` & `FoKL-1.1.2/src/FoKL/FoKLRoutines.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
                     vn = 1
                 if np.size(damtx) == 0:
                     damtx = vecs
                 else:
                     damtx = np.append(damtx, vecs, axis=0)
                 [dam,null] = np.shape(damtx)
 
-                [beters, null, null, null, xers, ev] = FokL.gibbs(inputs, data, phis, X, damtx, a, b, atau, btau, draws)
+                [beters, null, null, null, xers, ev] = FoKL.gibbs(inputs, data, phis, X, damtx, a, b, atau, btau, draws)
 
                 if aic:
                     ev = ev + (2 - np.log(n)) * (dam + 1)
 
                 betavs = np.abs(np.mean(beters[int(np.ceil((draws / 2)+1)):draws, (dam - vm + 1):dam+1], axis=0))
                 betavs2 = np.divide(np.std(np.array(beters[int(np.ceil(draws/2)+1):draws, dam-vm+1:dam+1]), axis=0), np.abs(np.mean(beters[int(np.ceil(draws / 2)):draws, dam-vm+1:dam+2], axis=0))) # betavs2 error in std deviation formatting
                 betavs3 = np.array(range(dam-vm+2, dam+2))
@@ -481,15 +481,15 @@
                         damtx_test = damtx
                         count = 1
                         for k in range(0, np.size(killtest)):
                             damtx_test = np.delete(damtx_test, (int(np.array(killtest[k]))-count), 0)
                             count = count + 1
                         damtest, null = np.shape(damtx_test)
 
-                        [betertest, null, null, null, Xtest, evtest] = FokL.gibbs(inputs, data, phis, X, damtx_test, a, b, atau, btau, draws)
+                        [betertest, null, null, null, Xtest, evtest] = FoKL.gibbs(inputs, data, phis, X, damtx_test, a, b, atau, btau, draws)
                         if aic:
                             evtest = evtest + (2 - np.log(n))*(damtest+1)
                         if evtest < evmin:
                             killset = killtest
                             evmin = evtest
                             xers = Xtest
                             beters = betertest
@@ -607,17 +607,17 @@
           Y is an array of the models that have been integrated, at the time steps
           contained in T.
           """
         def prediction(inputs):
             f = []
             for kk in range(len(inputs)):
                 if len(f) == 0:
-                    f = [FokL.bss_eval(inputs[kk], betas[kk], phis, matrix[kk]) + betas[kk][len(betas[kk]) - 1]]
+                    f = [bss_eval(inputs[kk], betas[kk], phis, matrix[kk]) + betas[kk][len(betas[kk]) - 1]]
                 else:
-                    f = np.append(f, FokL.bss_eval(inputs[kk], betas[kk], phis, matrix[kk]) + betas[kk][len(betas[kk]) - 1])
+                    f = np.append(f, bss_eval(inputs[kk], betas[kk], phis, matrix[kk]) + betas[kk][len(betas[kk]) - 1])
             return f
 
         def reorder(used, inputs):
             order = used[used != 0]
             reinputs = np.array((inputs.shape))
             for i in range(len(inputs)):
                 reinputs[order[i] - 1] = inputs[i]
```

### Comparing `FoKL-1.1.1/src/FoKL/GP_Integrate.py` & `FoKL-1.1.2/src/FoKL/GP_Integrate.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/src/FoKL/coverage3.py` & `FoKL-1.1.2/src/FoKL/coverage3.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/src/FoKL/emulator.py` & `FoKL-1.1.2/src/FoKL/emulator.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/src/FoKL/gibbs.py` & `FoKL-1.1.2/src/FoKL/gibbs.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/src/FoKL/splineConvert500.py` & `FoKL-1.1.2/src/FoKL/splineConvert500.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.1.1/src/FoKL.egg-info/PKG-INFO` & `FoKL-1.1.2/src/FoKL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoKL
-Version: 1.1.1
+Version: 1.1.2
 Summary: Karhunen Loève decomposed Gaussian processes with forward variable selection
 Home-page: https://github.com/derek-slack/FokLPackage
 Author-email: ESMS Group <derek.slack.001@gmail.com>
 Project-URL: Bug Tracker, https://github.com/derek-slack/FokLPackage/issues
 Project-URL: Changelog, https://github.com/derek-slack/FokLPackage/releases
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `FoKL-1.1.1/src/FoKL.egg-info/SOURCES.txt` & `FoKL-1.1.2/src/FoKL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

