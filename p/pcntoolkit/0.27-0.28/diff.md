# Comparing `tmp/pcntoolkit-0.27.tar.gz` & `tmp/pcntoolkit-0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcntoolkit-0.27.tar", last modified: Mon Mar  6 12:50:07 2023, max compression
+gzip compressed data, was "pcntoolkit-0.28.tar", last modified: Fri Jun  9 09:46:53 2023, max compression
```

## Comparing `pcntoolkit-0.27.tar` & `pcntoolkit-0.28.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.608670 pcntoolkit-0.27/
--rwxr-xr-x   0 andmar   (10406) preclineu   (670)    35140 2019-12-04 10:18:22.000000 pcntoolkit-0.27/LICENSE
--rw-r--r--   0 andmar   (10406) preclineu   (670)      288 2023-03-06 12:50:07.607669 pcntoolkit-0.27/PKG-INFO
--rw-r--r--   0 andmar   (10406) preclineu   (670)     2603 2022-04-01 12:52:51.000000 pcntoolkit-0.27/README.md
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.516675 pcntoolkit-0.27/pcntoolkit/
--rw-r--r--   0 andmar   (10406) preclineu   (670)      108 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/__init__.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)      129 2021-01-05 13:47:08.000000 pcntoolkit-0.27/pcntoolkit/configs.py
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.540675 pcntoolkit-0.27/pcntoolkit/dataio/
--rw-r--r--   0 andmar   (10406) preclineu   (670)       21 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/dataio/__init__.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    11707 2022-10-21 12:03:27.000000 pcntoolkit-0.27/pcntoolkit/dataio/fileio.py
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.569670 pcntoolkit-0.27/pcntoolkit/model/
--rw-r--r--   0 andmar   (10406) preclineu   (670)     3049 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/model/NP.py
--rwxr-xr-x   0 andmar   (10406) preclineu   (670)     3131 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/model/NPR.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    10439 2022-05-12 07:32:14.000000 pcntoolkit-0.27/pcntoolkit/model/SHASH.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)      120 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/model/__init__.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    11634 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/model/architecture.py
--rwxr-xr-x   0 andmar   (10406) preclineu   (670)    22084 2022-02-25 09:00:58.000000 pcntoolkit-0.27/pcntoolkit/model/bayesreg.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    15342 2022-02-25 09:00:58.000000 pcntoolkit-0.27/pcntoolkit/model/gp.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    42923 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/model/hbr.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     7985 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/model/rfa.py
--rwxr-xr-x   0 andmar   (10406) preclineu   (670)    56183 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/normative.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    13624 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/normative_NP.py
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.594669 pcntoolkit-0.27/pcntoolkit/normative_model/
--rw-r--r--   0 andmar   (10406) preclineu   (670)      140 2020-07-07 07:41:12.000000 pcntoolkit-0.27/pcntoolkit/normative_model/__init__.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     1511 2021-04-20 13:14:45.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_base.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     9143 2022-11-11 12:27:44.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_blr.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     2052 2022-02-25 09:00:58.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_gpr.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    16507 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_hbr.py
--rwxr-xr-x   0 andmar   (10406) preclineu   (670)     8436 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_np.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     1970 2022-02-25 09:00:58.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_rfa.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     1005 2022-02-25 09:00:58.000000 pcntoolkit-0.27/pcntoolkit/normative_model/norm_utils.py
--rwxr-xr-x   0 andmar   (10406) preclineu   (670)    53512 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/normative_parallel.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     8879 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/trendsurf.py
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.603671 pcntoolkit-0.27/pcntoolkit/util/
--rw-r--r--   0 andmar   (10406) preclineu   (670)       19 2021-12-08 08:21:30.000000 pcntoolkit-0.27/pcntoolkit/util/__init__.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)     7946 2022-08-05 09:40:02.000000 pcntoolkit-0.27/pcntoolkit/util/hbr_utils.py
--rw-r--r--   0 andmar   (10406) preclineu   (670)    53277 2023-03-06 12:49:38.000000 pcntoolkit-0.27/pcntoolkit/util/utils.py
-drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-03-06 12:50:07.535672 pcntoolkit-0.27/pcntoolkit.egg-info/
--rw-r--r--   0 andmar   (10406) preclineu   (670)      288 2023-03-06 12:50:07.000000 pcntoolkit-0.27/pcntoolkit.egg-info/PKG-INFO
--rw-r--r--   0 andmar   (10406) preclineu   (670)     1070 2023-03-06 12:50:07.000000 pcntoolkit-0.27/pcntoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 andmar   (10406) preclineu   (670)        1 2023-03-06 12:50:07.000000 pcntoolkit-0.27/pcntoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 andmar   (10406) preclineu   (670)        1 2021-01-05 14:05:25.000000 pcntoolkit-0.27/pcntoolkit.egg-info/not-zip-safe
--rw-r--r--   0 andmar   (10406) preclineu   (670)      180 2023-03-06 12:50:07.000000 pcntoolkit-0.27/pcntoolkit.egg-info/requires.txt
--rw-r--r--   0 andmar   (10406) preclineu   (670)       11 2023-03-06 12:50:07.000000 pcntoolkit-0.27/pcntoolkit.egg-info/top_level.txt
--rw-r--r--   0 andmar   (10406) preclineu   (670)       38 2023-03-06 12:50:07.609670 pcntoolkit-0.27/setup.cfg
--rw-r--r--   0 andmar   (10406) preclineu   (670)      798 2023-03-06 12:49:38.000000 pcntoolkit-0.27/setup.py
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.424765 pcntoolkit-0.28/
+-rwxr-xr-x   0 andmar   (10406) preclineu   (670)    35140 2019-12-04 10:18:22.000000 pcntoolkit-0.28/LICENSE
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      260 2023-06-09 09:46:53.422766 pcntoolkit-0.28/PKG-INFO
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     2603 2022-04-01 12:52:51.000000 pcntoolkit-0.28/README.md
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.148780 pcntoolkit-0.28/pcntoolkit/
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      108 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/__init__.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      129 2021-01-05 13:47:08.000000 pcntoolkit-0.28/pcntoolkit/configs.py
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.191778 pcntoolkit-0.28/pcntoolkit/dataio/
+-rw-r--r--   0 andmar   (10406) preclineu   (670)       21 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/dataio/__init__.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    11707 2022-10-21 12:03:27.000000 pcntoolkit-0.28/pcntoolkit/dataio/fileio.py
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.269776 pcntoolkit-0.28/pcntoolkit/model/
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     3049 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/model/NP.py
+-rwxr-xr-x   0 andmar   (10406) preclineu   (670)     3131 2023-03-06 12:49:38.000000 pcntoolkit-0.28/pcntoolkit/model/NPR.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    10361 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/model/SHASH.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      120 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/model/__init__.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    11634 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/model/architecture.py
+-rwxr-xr-x   0 andmar   (10406) preclineu   (670)    22084 2022-02-25 09:00:58.000000 pcntoolkit-0.28/pcntoolkit/model/bayesreg.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    15342 2022-02-25 09:00:58.000000 pcntoolkit-0.28/pcntoolkit/model/gp.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    49102 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/model/hbr.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     7985 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/model/rfa.py
+-rwxr-xr-x   0 andmar   (10406) preclineu   (670)    56716 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/normative.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    13624 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/normative_NP.py
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.382770 pcntoolkit-0.28/pcntoolkit/normative_model/
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      140 2020-07-07 07:41:12.000000 pcntoolkit-0.28/pcntoolkit/normative_model/__init__.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     1511 2021-04-20 13:14:45.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_base.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     9143 2022-11-11 12:27:44.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_blr.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     2052 2022-02-25 09:00:58.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_gpr.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    25174 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_hbr.py
+-rwxr-xr-x   0 andmar   (10406) preclineu   (670)     8436 2023-03-06 12:49:38.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_np.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     1970 2022-02-25 09:00:58.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_rfa.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     1005 2022-02-25 09:00:58.000000 pcntoolkit-0.28/pcntoolkit/normative_model/norm_utils.py
+-rwxr-xr-x   0 andmar   (10406) preclineu   (670)    53512 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/normative_parallel.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     8983 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/trendsurf.py
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.415770 pcntoolkit-0.28/pcntoolkit/util/
+-rw-r--r--   0 andmar   (10406) preclineu   (670)       19 2021-12-08 08:21:30.000000 pcntoolkit-0.28/pcntoolkit/util/__init__.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     7945 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/util/hbr_utils.py
+-rw-r--r--   0 andmar   (10406) preclineu   (670)    53282 2023-06-09 09:45:48.000000 pcntoolkit-0.28/pcntoolkit/util/utils.py
+drwxr-xr-x   0 andmar   (10406) preclineu   (670)        0 2023-06-09 09:46:53.179778 pcntoolkit-0.28/pcntoolkit.egg-info/
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      260 2023-06-09 09:46:52.000000 pcntoolkit-0.28/pcntoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 andmar   (10406) preclineu   (670)     1070 2023-06-09 09:46:52.000000 pcntoolkit-0.28/pcntoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 andmar   (10406) preclineu   (670)        1 2023-06-09 09:46:52.000000 pcntoolkit-0.28/pcntoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 andmar   (10406) preclineu   (670)        1 2021-01-05 14:05:25.000000 pcntoolkit-0.28/pcntoolkit.egg-info/not-zip-safe
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      145 2023-06-09 09:46:52.000000 pcntoolkit-0.28/pcntoolkit.egg-info/requires.txt
+-rw-r--r--   0 andmar   (10406) preclineu   (670)       11 2023-06-09 09:46:52.000000 pcntoolkit-0.28/pcntoolkit.egg-info/top_level.txt
+-rw-r--r--   0 andmar   (10406) preclineu   (670)       38 2023-06-09 09:46:53.426765 pcntoolkit-0.28/setup.cfg
+-rw-r--r--   0 andmar   (10406) preclineu   (670)      718 2023-06-09 09:45:48.000000 pcntoolkit-0.28/setup.py
```

### Comparing `pcntoolkit-0.27/LICENSE` & `pcntoolkit-0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/README.md` & `pcntoolkit-0.28/README.md`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/dataio/fileio.py` & `pcntoolkit-0.28/pcntoolkit/dataio/fileio.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/model/NP.py` & `pcntoolkit-0.28/pcntoolkit/model/NP.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/model/NPR.py` & `pcntoolkit-0.28/pcntoolkit/model/NPR.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/model/architecture.py` & `pcntoolkit-0.28/pcntoolkit/model/architecture.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/model/bayesreg.py` & `pcntoolkit-0.28/pcntoolkit/model/bayesreg.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/model/gp.py` & `pcntoolkit-0.28/pcntoolkit/model/gp.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/model/hbr.py` & `pcntoolkit-0.28/pcntoolkit/model/hbr.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,220 +5,328 @@
 
 @author: seykia
 @author: augub
 """
 
 from __future__ import print_function
 from __future__ import division
+from collections import OrderedDict
+
 from ast import Param
 from tkinter.font import names
 
 import numpy as np
-import pymc3 as pm
-import theano
+import pymc as pm
+import pytensor
+import arviz as az
+import xarray
+
 from itertools import product
 from functools import reduce
 
-import theano
-from pymc3 import Metropolis, NUTS, Slice, HamiltonianMC
+from pymc import Metropolis, NUTS, Slice, HamiltonianMC
 from scipy import stats
 import bspline
 from bspline import splinelab
 
-from model.SHASH import SHASHo2, SHASHb, SHASHo
 from util.utils import create_poly_basis
 from util.utils import expand_all
 from pcntoolkit.util.utils import cartesian_product
+from pcntoolkit.model.SHASH import *
 
-from theano import printing, function
 
 def bspline_fit(X, order, nknots):
     feature_num = X.shape[1]
     bsp_basis = []
 
     for i in range(feature_num):
-        minx = np.min(X[:,i])
-        maxx = np.max(X[:,i])
-        delta = maxx-minx
+        minx = np.min(X[:, i])
+        maxx = np.max(X[:, i])
+        delta = maxx - minx
         # Expand range by 20% (10% on both sides)
-        splinemin = minx-0.1*delta
-        splinemax = maxx+0.1*delta
+        splinemin = minx - 0.1 * delta
+        splinemax = maxx + 0.1 * delta
         knots = np.linspace(splinemin, splinemax, nknots)
         k = splinelab.augknt(knots, order)
         bsp_basis.append(bspline.Bspline(k, order))
 
     return bsp_basis
 
+
 def bspline_transform(X, bsp_basis):
     if type(bsp_basis) != list:
         temp = []
         temp.append(bsp_basis)
         bsp_basis = temp
 
     feature_num = len(bsp_basis)
     X_transformed = []
     for f in range(feature_num):
         X_transformed.append(np.array([bsp_basis[f](i) for i in X[:, f]]))
     X_transformed = np.concatenate(X_transformed, axis=1)
 
     return X_transformed
 
+
 def create_poly_basis(X, order):
-    """ compute a polynomial basis expansion of the specified order"""
+    """compute a polynomial basis expansion of the specified order"""
 
     if len(X.shape) == 1:
         X = X[:, np.newaxis]
     D = X.shape[1]
     Phi = np.zeros((X.shape[0], D * order))
     colid = np.arange(0, D)
     for d in range(1, order + 1):
-        Phi[:, colid] = X ** d
+        Phi[:, colid] = X**d
         colid += D
-
     return Phi
 
 
-def from_posterior(param, samples, distribution=None, half=False, freedom=1):
-    if len(samples.shape) > 1:
-        shape = samples.shape[1:]
-    else:
-        shape = None
-
-    if (distribution is None):
+def from_posterior(param, samples, shape,  distribution=None, half=False, freedom=1):
+    if distribution is None:
         smin, smax = np.min(samples), np.max(samples)
         width = smax - smin
         x = np.linspace(smin, smax, 1000)
         y = stats.gaussian_kde(np.ravel(samples))(x)
         if half:
             x = np.concatenate([x, [x[-1] + 0.1 * width]])
             y = np.concatenate([y, [0]])
         else:
             x = np.concatenate([[x[0] - 0.1 * width], x, [x[-1] + 0.1 * width]])
             y = np.concatenate([[0], y, [0]])
         if shape is None:
             return pm.distributions.Interpolated(param, x, y)
         else:
             return pm.distributions.Interpolated(param, x, y, shape=shape)
-    elif (distribution == 'normal'):
+    elif distribution == "normal":
         temp = stats.norm.fit(samples)
         if shape is None:
             return pm.Normal(param, mu=temp[0], sigma=freedom * temp[1])
         else:
             return pm.Normal(param, mu=temp[0], sigma=freedom * temp[1], shape=shape)
-    elif (distribution == 'hnormal'):
+    elif distribution == "hnormal":
         temp = stats.halfnorm.fit(samples)
         if shape is None:
             return pm.HalfNormal(param, sigma=freedom * temp[1])
         else:
             return pm.HalfNormal(param, sigma=freedom * temp[1], shape=shape)
-    elif (distribution == 'hcauchy'):
+    elif distribution == "hcauchy":
         temp = stats.halfcauchy.fit(samples)
         if shape is None:
             return pm.HalfCauchy(param, freedom * temp[1])
         else:
             return pm.HalfCauchy(param, freedom * temp[1], shape=shape)
-    elif (distribution == 'uniform'):
+    elif distribution == "uniform":
         upper_bound = np.percentile(samples, 95)
         lower_bound = np.percentile(samples, 5)
         r = np.abs(upper_bound - lower_bound)
         if shape is None:
-            return pm.Uniform(param, lower=lower_bound - freedom * r,
-                              upper=upper_bound + freedom * r)
+            return pm.Uniform(
+                param, lower=lower_bound - freedom * r, upper=upper_bound + freedom * r
+            )
         else:
-            return pm.Uniform(param, lower=lower_bound - freedom * r,
-                              upper=upper_bound + freedom * r, shape=shape)
-    elif (distribution == 'huniform'):
+            return pm.Uniform(
+                param,
+                lower=lower_bound - freedom * r,
+                upper=upper_bound + freedom * r,
+                shape=shape,
+            )
+    elif distribution == "huniform":
         upper_bound = np.percentile(samples, 95)
         lower_bound = np.percentile(samples, 5)
         r = np.abs(upper_bound - lower_bound)
         if shape is None:
             return pm.Uniform(param, lower=0, upper=upper_bound + freedom * r)
         else:
-            return pm.Uniform(param, lower=0, upper=upper_bound + freedom * r, shape=shape)
+            return pm.Uniform(
+                param, lower=0, upper=upper_bound + freedom * r, shape=shape
+            )
 
-    elif (distribution == 'gamma'):
+    elif distribution == "gamma":
         alpha_fit, loc_fit, invbeta_fit = stats.gamma.fit(samples)
         if shape is None:
-            return pm.Gamma(param, alpha=freedom * alpha_fit, beta=freedom / invbeta_fit)
+            return pm.Gamma(
+                param, alpha=freedom * alpha_fit, beta=freedom / invbeta_fit
+            )
         else:
-            return pm.Gamma(param, alpha=freedom * alpha_fit, beta=freedom / invbeta_fit, shape=shape)
+            return pm.Gamma(
+                param,
+                alpha=freedom * alpha_fit,
+                beta=freedom / invbeta_fit,
+                shape=shape,
+            )
 
-    elif (distribution == 'igamma'):
+    elif distribution == "igamma":
         alpha_fit, loc_fit, beta_fit = stats.gamma.fit(samples)
         if shape is None:
-            return pm.InverseGamma(param, alpha=freedom * alpha_fit, beta=freedom * beta_fit)
+            return pm.InverseGamma(
+                param, alpha=freedom * alpha_fit, beta=freedom * beta_fit
+            )
         else:
-            return pm.InverseGamma(param, alpha=freedom * alpha_fit, beta=freedom * beta_fit, shape=shape)
+            return pm.InverseGamma(
+                param, alpha=freedom * alpha_fit, beta=freedom * beta_fit, shape=shape
+            )
 
 
-def hbr(X, y, batch_effects, batch_effects_size, configs, trace=None):
+def hbr(X, y, batch_effects, configs, idata=None):
     """
     :param X: [N×P] array of clinical covariates
     :param y: [N×1] array of neuroimaging measures
     :param batch_effects: [N×M] array of batch effects
     :param batch_effects_size: [b1, b2,...,bM] List of counts of unique values of batch effects
     :param configs:
-    :param trace:
-    :param return_shared_variables: If true, returns references to the shared variables. The values of the shared variables can be set manually, allowing running the same model on different data without re-compiling it. 
+    :param idata:
+    :param return_shared_variables: If true, returns references to the shared variables. The values of the shared variables can be set manually, allowing running the same model on different data without re-compiling it.
     :return:
     """
-    X = theano.shared(X)
-    X = theano.tensor.cast(X,'floatX')
-    y = theano.shared(y)
-    y = theano.tensor.cast(y,'floatX')
 
+    # Make a param builder that will make the correct calls
+    pb = ParamBuilder(X, y, batch_effects, idata, configs)
 
-    with pm.Model() as model:
-
-        # Make a param builder that will make the correct calls
-        pb = ParamBuilder(model, X, y, batch_effects, trace, configs)
+    def get_sample_dims(var):
+        if configs[f'random_{var}']:
+            return 'datapoints'
+        elif configs[f'random_slope_{var}']:
+            return 'datapoints'
+        elif configs[f'random_intercept_{var}']:
+            return 'datapoints'
+        elif configs[f'linear_{var}']:
+            return 'datapoints'
+        return None
+
+    with pm.Model(coords=pb.coords) as model:
+        model.add_coord("datapoints", np.arange(X.shape[0]), mutable=True)
+        X = pm.MutableData("X", X, dims=("datapoints", "basis_functions"))
+        pb.X = X
+        y = pm.MutableData("y", np.squeeze(y), dims="datapoints")
+        pb.model = model
+        pb.batch_effect_indices = tuple(
+            [
+                pm.Data(
+                    pb.batch_effect_dim_names[i],
+                    pb.batch_effect_indices[i],
+                    mutable=True,
+                    dims="datapoints",
+                )
+                for i in range(len(pb.batch_effect_indices))
+            ]
+        )
 
-        if configs['likelihood'] == 'Normal':
-            mu = pb.make_param("mu", mu_slope_mu_params = (0.,10.), 
-                               sigma_slope_mu_params = (5.,), 
-                               mu_intercept_mu_params=(0.,10.), 
-                               sigma_intercept_mu_params = (5.,)).get_samples(pb)
-            sigma = pb.make_param("sigma", mu_sigma_params = (10., 5.),
-                                  sigma_sigma_params = (5.,)).get_samples(pb)
-            sigma_plus = pm.math.log(1+pm.math.exp(sigma))
-            y_like = pm.Normal('y_like',mu=mu, sigma=sigma_plus, observed=y)
+        if configs["likelihood"] == "Normal":
+            
+            mu = pm.Deterministic(
+                "mu_samples",
+                pb.make_param(
+                    "mu",
+                    mu_slope_mu_params=(0.0, 3.0),
+                    sigma_slope_mu_params=(3.0,),
+                    mu_intercept_mu_params=(0.0, 3.0),
+                    sigma_intercept_mu_params=(3.0,),
+                ).get_samples(pb),
+                dims=get_sample_dims('mu'),
+            )
+            sigma = pm.Deterministic(
+                "sigma_samples",
+                pb.make_param(
+                    "sigma", mu_sigma_params=(0.0, 2.0), sigma_sigma_params=(2.0,)
+                ).get_samples(pb),
+                dims=get_sample_dims('sigma'),
+            )
+            sigma_plus = pm.Deterministic(
+                "sigma_plus_samples", pm.math.log(1 + pm.math.exp(sigma/3))*3, dims=get_sample_dims('sigma')
+            )
+            y_like = pm.Normal(
+                "y_like", mu, sigma=sigma_plus, observed=y, dims="datapoints"
+            )
 
-        elif configs['likelihood'] in ['SHASHb','SHASHo','SHASHo2']:
+        elif configs["likelihood"] in ["SHASHb", "SHASHo", "SHASHo2"]:
             """
             Comment 1
-            The current parameterizations are tuned towards standardized in- and output data. 
+            The current parameterizations are tuned towards standardized in- and output data.
             It is possible to adjust the priors through the XXX_dist and XXX_params kwargs, like here we do with epsilon_params.
-            Supported distributions are listed in the Prior class. 
-
+            Supported distributions are listed in the Prior class.
             Comment 2
-            Any mapping that is applied here after sampling should also be applied in util.hbr_utils.forward in order for the functions there to properly work. 
+            Any mapping that is applied here after sampling should also be applied in util.hbr_utils.forward in order for the functions there to properly work.
             For example, the softplus applied to sigma here is also applied in util.hbr_utils.forward
             """
-            SHASH_map = {'SHASHb':SHASHb,'SHASHo':SHASHo,'SHASHo2':SHASHo2}
-
-            mu =            pb.make_param("mu",         slope_mu_params = (0.,3.), mu_intercept_mu_params=(0.,1.), sigma_intercept_mu_params = (1.,)).get_samples(pb)
-            sigma =         pb.make_param("sigma",      sigma_params = (1.,2.),    slope_sigma_params=(0.,1.),     intercept_sigma_params = (1., 1.)).get_samples(pb)
-            sigma_plus =    pm.math.log(1+pm.math.exp(sigma))
-            epsilon =       pb.make_param("epsilon",    epsilon_params = (0.,1.),  slope_epsilon_params=(0.,1.), intercept_epsilon_params=(0.,1)).get_samples(pb)
-            delta =         pb.make_param("delta",      delta_params=(1.5,2.),     slope_delta_params=(0.,1),   intercept_delta_params=(2., 1)).get_samples(pb)
-            delta_plus =    pm.math.log(1+pm.math.exp(delta)) + 0.3
-            y_like = SHASH_map[configs['likelihood']]('y_like', mu=mu, sigma=sigma_plus, epsilon=epsilon, delta=delta_plus, observed = y)
-
-    return model
+            SHASH_map = {"SHASHb": SHASHb, "SHASHo": SHASHo, "SHASHo2": SHASHo2}
 
+            mu = pm.Deterministic(
+                "mu_samples",
+                pb.make_param(
+                    "mu",
+                    slope_mu_params=(0.0, 2.0),
+                    mu_slope_mu_params=(0.0, 2.0),
+                    sigma_slope_mu_params=(2.0,),
+                    mu_intercept_mu_params=(0.0, 2.0),
+                    sigma_intercept_mu_params=(2.0,),
+                ).get_samples(pb),
+                dims=get_sample_dims('mu'),
+            )
+            sigma = pm.Deterministic(
+                "sigma_samples",
+                pb.make_param(
+                    "sigma",
+                    sigma_params=(1.0, 1.0),
+                    sigma_dist="normal",
+                    slope_sigma_params=(0.0, 1.0),
+                    intercept_sigma_params=(1.0, 1.0),
+                ).get_samples(pb),
+                dims=get_sample_dims('sigma'),
+            )
+            sigma_plus = pm.Deterministic(
+                "sigma_plus_samples", np.log(1 + np.exp(sigma)), dims=get_sample_dims('sigma')
+            )
+            epsilon = pm.Deterministic(
+                "epsilon_samples",
+                pb.make_param(
+                    "epsilon",
+                    epsilon_params=(0.0, 1.0),
+                    slope_epsilon_params=(0.0, 0.2),
+                    intercept_epsilon_params=(0.0, 0.2),
+                ).get_samples(pb),
+                dims=get_sample_dims('epsilon'),
+            )
+            delta = pm.Deterministic(
+                "delta_samples",
+                pb.make_param(
+                    "delta",
+                    delta_params=(1.0, 1.0),
+                    delta_dist="normal",
+                    slope_delta_params=(0.0, 0.2),
+                    intercept_delta_params=(1.0, 0.3),
+                ).get_samples(pb),
+                dims=get_sample_dims('delta'),
+            )
+            delta_plus = pm.Deterministic(
+                "delta_plus_samples",
+                np.log(1 + np.exp(delta * 10)) / 10 + 0.3,
+                dims=get_sample_dims('delta'),
+            )
+            y_like = SHASH_map[configs["likelihood"]](
+                "y_like",
+                mu=mu,
+                sigma=sigma_plus,
+                epsilon=epsilon,
+                delta=delta_plus,
+                observed=y,
+                dims="datapoints",
+            )
+        return model
 
+  
 
 class HBR:
 
     """Hierarchical Bayesian Regression for normative modeling
 
     Basic usage::
 
         model = HBR(configs)
-        trace = model.estimate(X, y, batch_effects)
+        idata = model.estimate(X, y, batch_effects)
         ys,s2 = model.predict(X, batch_effects)
 
     where the variables are
 
     :param configs: a dictionary of model configurations.
     :param X: N-by-P input matrix of P features for N subjects
     :param y: N-by-1 vector of outputs.
@@ -226,703 +334,917 @@
 
     :returns: * ys - predictive mean
               * s2 - predictive variance
 
     Written by S.M. Kia
     """
 
-    def get_step_methods(self, m):
-        """
-        This can be used to assign default step functions. However, the nuts initialization keyword doesnt work together with this... so better not use it. 
-
-        STEP_METHODS = (
-            NUTS,
-            HamiltonianMC,
-            Metropolis,
-            BinaryMetropolis,
-            BinaryGibbsMetropolis,
-            Slice,
-            CategoricalGibbsMetropolis,
-        )
-        :param m: a PyMC3 model
-        :return:
-        """
-        samplermap = {'NUTS': NUTS, 'MH': Metropolis, 'Slice': Slice, 'HMC': HamiltonianMC}
-        fallbacks = [Metropolis]         # We are using MH as a fallback method here
-        if self.configs['sampler'] == 'NUTS':
-            step_kwargs = {'nuts': {'target_accept': self.configs['target_accept']}}
-        else:
-            step_kwargs = None
-        return pm.sampling.assign_step_methods(m, methods=[samplermap[self.configs['sampler']]] + fallbacks,
-                                               step_kwargs=step_kwargs)
-
     def __init__(self, configs):
         self.bsp = None
-        self.model_type = configs['type']
+        self.model_type = configs["type"]
         self.configs = configs
 
     def get_modeler(self):
-        return {'nn': nn_hbr}.get(self.model_type, hbr)
-        
+        return hbr
+
     def transform_X(self, X):
-        if self.model_type == 'polynomial':
-            Phi = create_poly_basis(X, self.configs['order'])
-        elif self.model_type == 'bspline':
+        if self.model_type == "polynomial":
+            Phi = create_poly_basis(X, self.configs["order"])
+        elif self.model_type == "bspline":
             if self.bsp is None:
-                self.bsp = bspline_fit(X, self.configs['order'], self.configs['nknots'])
+                self.bsp = bspline_fit(X, self.configs["order"], self.configs["nknots"])
             bspline = bspline_transform(X, self.bsp)
-            Phi = np.concatenate((X, bspline), axis = 1)
+            Phi = np.concatenate((X, bspline), axis=1)
         else:
             Phi = X
         return Phi
 
-
-    def find_map(self, X, y, batch_effects,method='L-BFGS-B'):
-        """ Function to estimate the model """
+    def find_map(self, X, y, batch_effects, method="L-BFGS-B"):
+        """Function to estimate the model"""
         X, y, batch_effects = expand_all(X, y, batch_effects)
-
-        self.batch_effects_num = batch_effects.shape[1]
-        self.batch_effects_size = []
-        for i in range(self.batch_effects_num):
-            self.batch_effects_size.append(len(np.unique(batch_effects[:, i])))
-
         X = self.transform_X(X)
         modeler = self.get_modeler()
-        with modeler(X, y, batch_effects, self.batch_effects_size, self.configs) as m:
+        with modeler(X, y, batch_effects, self.configs) as m:
             self.MAP = pm.find_MAP(method=method)
         return self.MAP
 
-    def estimate(self, X, y, batch_effects):
-
-        """ Function to estimate the model """
+    def estimate(self, X, y, batch_effects, **kwargs):
+        """Function to estimate the model"""
         X, y, batch_effects = expand_all(X, y, batch_effects)
-
-        self.batch_effects_num = batch_effects.shape[1]
-        self.batch_effects_size = []
-        for i in range(self.batch_effects_num):
-            self.batch_effects_size.append(len(np.unique(batch_effects[:, i])))
-
         X = self.transform_X(X)
         modeler = self.get_modeler()
-        with modeler(X, y, batch_effects, self.batch_effects_size, self.configs) as m:
-            self.trace = pm.sample(draws=self.configs['n_samples'],
-                                   tune=self.configs['n_tuning'],
-                                   chains=self.configs['n_chains'],
-                                   init=self.configs['init'], n_init=500000,
-                                   cores=self.configs['cores'])
-        return self.trace
-
-    def predict(self, X, batch_effects, pred='single'):
-        """ Function to make predictions from the model """
+        if hasattr(self, 'idata'):
+            del self.idata
+        with modeler(X, y, batch_effects, self.configs) as m:
+            self.idata = pm.sample(
+                draws=self.configs["n_samples"],
+                tune=self.configs["n_tuning"],
+                chains=self.configs["n_chains"],
+                init=self.configs["init"],
+                n_init=500000,
+                cores=self.configs["cores"],
+            )
+        self.vars_to_sample = ['y_like']
+        if self.configs['remove_datapoints_from_posterior']:
+            chain = self.idata.posterior.coords['chain'].data
+            draw = self.idata.posterior.coords['draw'].data
+            for j in self.idata.posterior.variables.mapping.keys():
+                if j.endswith('_samples'):
+                    dummy_array = xarray.DataArray(data = np.zeros((len(chain), len(draw), 1)), coords = {'chain':chain, 'draw':draw,'empty':np.array([0])}, name=j)
+                    self.idata.posterior[j] = dummy_array
+                    self.vars_to_sample.append(j)
+        return self.idata
+
+    def predict(
+        self, X, batch_effects, batch_effects_maps, pred="single", var_names=None, **kwargs
+    ):
+        """Function to make predictions from the model
+        Args:
+            X: Covariates
+            batch_effects: batch effects corresponding to X
+            all_batch_effects: combinations of all batch effects that were present the training data
+        """
         X, batch_effects = expand_all(X, batch_effects)
 
-        samples = self.configs['n_samples']
+        samples = self.configs["n_samples"]
         y = np.zeros([X.shape[0], 1])
+        X = self.transform_X(X)
+        modeler = self.get_modeler()
 
-        if pred == 'single':
-            X = self.transform_X(X)
-            modeler = self.get_modeler()
-            with modeler(X, y, batch_effects, self.batch_effects_size, self.configs):
-                ppc = pm.sample_posterior_predictive(self.trace, samples=samples, progressbar=True)
-            pred_mean = ppc['y_like'].mean(axis=0)
-            pred_var = ppc['y_like'].var(axis=0)
+        # Make an array with occurences of all the values in be_train, but with the same size as be_test
+        truncated_batch_effects_train = np.stack(
+            [
+                np.resize(np.array(list(batch_effects_maps[i].keys())), X.shape[0])
+                for i in range(batch_effects.shape[1])
+            ],
+            axis=1,
+        )
+
+        # See if a list of var_names is provided, set to self.vars_to_sample otherwise
+        if (var_names is None) or (var_names == ['y_like']):
+            var_names = self.vars_to_sample
+
+        n_samples = X.shape[0]
+        with modeler(X, y, truncated_batch_effects_train, self.configs) as model:
+            # For each batch effect dim
+            for i in range(batch_effects.shape[1]):
+                # Make a map that maps batch effect values to their index
+                valmap = batch_effects_maps[i]
+                # Compute those indices for the test data
+                indices = list(map(lambda x: valmap[x], batch_effects[:, i]))
+                # Those indices need to be used by the model
+                pm.set_data({f"batch_effect_{i}": indices})
+
+            self.idata = pm.sample_posterior_predictive(
+                trace=self.idata,
+                extend_inferencedata=True,
+                progressbar=True,
+                var_names=var_names,
+            )
+        pred_mean = self.idata.posterior_predictive["y_like"].to_numpy().mean(axis=(0, 1))
+        pred_var = self.idata.posterior_predictive["y_like"].to_numpy().var(axis=(0, 1))
 
         return pred_mean, pred_var
 
     def estimate_on_new_site(self, X, y, batch_effects):
-        """ Function to adapt the model """
+        """Function to adapt the model"""
         X, y, batch_effects = expand_all(X, y, batch_effects)
-
-        self.batch_effects_num = batch_effects.shape[1]
-        self.batch_effects_size = []
-        for i in range(self.batch_effects_num):
-            self.batch_effects_size.append(len(np.unique(batch_effects[:, i])))
-
         X = self.transform_X(X)
         modeler = self.get_modeler()
-        with modeler(X, y, batch_effects, self.batch_effects_size,
-                     self.configs, trace=self.trace) as m:
-            self.trace = pm.sample(self.configs['n_samples'],
-                                   tune=self.configs['n_tuning'],
-                                   chains=self.configs['n_chains'],
-                                   target_accept=self.configs['target_accept'],
-                                   init=self.configs['init'], n_init=50000,
-                                   cores=self.configs['cores'])
-        return self.trace
+        with modeler(X, y, batch_effects, self.configs, idata=self.idata) as m:
+            self.idata = pm.sample(
+                self.configs["n_samples"],
+                tune=self.configs["n_tuning"],
+                chains=self.configs["n_chains"],
+                target_accept=self.configs["target_accept"],
+                init=self.configs["init"],
+                n_init=50000,
+                cores=self.configs["cores"],
+            )
+        return self.idata
 
     def predict_on_new_site(self, X, batch_effects):
-        """ Function to make predictions from the model """
+        """Function to make predictions from the model"""
         X, batch_effects = expand_all(X, batch_effects)
-
-        samples = self.configs['n_samples']
+        samples = self.configs["n_samples"]
         y = np.zeros([X.shape[0], 1])
-
         X = self.transform_X(X)
         modeler = self.get_modeler()
-        with modeler(X, y, batch_effects, self.batch_effects_size, self.configs, trace=self.trace):
-            ppc = pm.sample_posterior_predictive(self.trace, samples=samples, progressbar=True)
-        pred_mean = ppc['y_like'].mean(axis=0)
-        pred_var = ppc['y_like'].var(axis=0)
+        with modeler(X, y, batch_effects, self.configs, idata=self.idata):
+            self.idata = pm.sample_posterior_predictive(
+                self.idata, extend_inferencedata=True, progressbar=True
+            )
+        pred_mean = self.idata.posterior_predictive["y_like"].mean(axis=(0, 1))
+        pred_var = self.idata.posterior_predictive["y_like"].var(axis=(0, 1))
 
         return pred_mean, pred_var
 
     def generate(self, X, batch_effects, samples):
-        """ Function to generate samples from posterior predictive distribution """
+        """Function to generate samples from posterior predictive distribution"""
         X, batch_effects = expand_all(X, batch_effects)
 
         y = np.zeros([X.shape[0], 1])
 
         X = self.transform_X(X)
         modeler = self.get_modeler()
-        with modeler(X, y, batch_effects, self.batch_effects_size, self.configs):
-            ppc = pm.sample_posterior_predictive(self.trace, samples=samples, progressbar=True)
-
-        generated_samples = np.reshape(ppc['y_like'].squeeze().T, [X.shape[0] * samples, 1])
+        with modeler(X, y, batch_effects, self.configs):
+            ppc = pm.sample_posterior_predictive(self.idata, progressbar=True)
+        generated_samples = np.reshape(
+            ppc.posterior_predictive["y_like"].squeeze().T, [X.shape[0] * samples, 1]
+        )
         X = np.repeat(X, samples)
         if len(X.shape) == 1:
             X = np.expand_dims(X, axis=1)
         batch_effects = np.repeat(batch_effects, samples, axis=0)
         if len(batch_effects.shape) == 1:
             batch_effects = np.expand_dims(batch_effects, axis=1)
-
         return X, batch_effects, generated_samples
 
-    def sample_prior_predictive(self, X, batch_effects, samples, trace=None):
-        """ Function to sample from prior predictive distribution """
-
-        if len(X.shape) == 1:
-            X = np.expand_dims(X, axis=1)
-        if len(batch_effects.shape) == 1:
-            batch_effects = np.expand_dims(batch_effects, axis=1)
-
-        self.batch_effects_num = batch_effects.shape[1]
-        self.batch_effects_size = []
-        for i in range(self.batch_effects_num):
-            self.batch_effects_size.append(len(np.unique(batch_effects[:, i])))
-
-        y = np.zeros([X.shape[0], 1])
+    def sample_prior_predictive(self, X, batch_effects, samples, y = None, idata=None):
+        """Function to sample from prior predictive distribution"""
+        if y is None:
+            y = np.zeros([X.shape[0], 1])
+        X, y, batch_effects = expand_all(X, y, batch_effects)
 
-        if self.model_type == 'linear':
-            with hbr(X, y, batch_effects, self.batch_effects_size, self.configs,
-                     trace):
-                ppc = pm.sample_prior_predictive(samples=samples)
-        return ppc
+        X = self.transform_X(X)
+        modeler = self.get_modeler()
+        with modeler(X, y, batch_effects, self.configs, idata):
+            self.idata = pm.sample_prior_predictive(samples=samples)
+        return self.idata
 
     def get_model(self, X, y, batch_effects):
         X, y, batch_effects = expand_all(X, y, batch_effects)
-
-        self.batch_effects_num = batch_effects.shape[1]
-        self.batch_effects_size = []
-        for i in range(self.batch_effects_num):
-            self.batch_effects_size.append(len(np.unique(batch_effects[:, i])))
         modeler = self.get_modeler()
         X = self.transform_X(X)
-        return modeler(X, y, batch_effects, self.batch_effects_size, self.configs, self.trace)
-
-    def create_dummy_inputs(self, covariate_ranges = [[0.1,0.9,0.01]]):
+        idata = self.idata if hasattr(self, "idata") else None
+        return modeler(X, y, batch_effects, self.configs, idata=idata)
 
+    def create_dummy_inputs(self, covariate_ranges=[[0.1, 0.9, 0.01]]):
         arrays = []
         for i in range(len(covariate_ranges)):
-            arrays.append(np.arange(covariate_ranges[i][0],covariate_ranges[i][1], covariate_ranges[i][2]))
+            arrays.append(
+                np.arange(
+                    covariate_ranges[i][0],
+                    covariate_ranges[i][1],
+                    covariate_ranges[i][2],
+                )
+            )
         X = cartesian_product(arrays)
         X_dummy = np.concatenate([X for i in range(np.prod(self.batch_effects_size))])
-
         arrays = []
         for i in range(self.batch_effects_num):
             arrays.append(np.arange(0, self.batch_effects_size[i]))
         batch_effects = cartesian_product(arrays)
         batch_effects_dummy = np.repeat(batch_effects, X.shape[0], axis=0)
+        return X_dummy, batch_effects_dummy
 
-        return X_dummy, batch_effects_dummy 
+    def Rhats(self, var_names, thin = 1, resolution = 100):
+        """Get Rhat of posterior samples as function of sampling iteration"""
+        idata = self.idata
+        testvars = az.extract(idata, group='posterior', var_names=var_names, combined=False)
+        rhat_dict={}
+        for var_name in var_names:
+            var = np.stack(testvars[var_name].to_numpy())[:,::thin]     
+            var = var.reshape((var.shape[0], var.shape[1], -1))
+            vardim = var.shape[2]
+            interval_skip=var.shape[1]//resolution
+            rhats_var = np.zeros((resolution, vardim))
+            for v in range(vardim):
+                for j in range(resolution):
+                    rhats_var[j,v] = az.rhat(var[:,:j*interval_skip,v])
+            rhat_dict[var_name] = rhats_var
+        return rhat_dict
 
 class Prior:
     """
-    A wrapper class for a PyMC3 distribution. 
-    - creates a fitted distribution from the trace, if one is present
+    A wrapper class for a PyMC distribution.
+    - creates a fitted distribution from the idata, if one is present
     - overloads the __getitem__ function with something that switches between indexing or not, based on the shape
     """
-    def __init__(self, name, dist, params, pb, shape=(1,)) -> None:
+
+    def __init__(self, name, dist, params, pb, has_random_effect=False) -> None:
         self.dist = None
         self.name = name
-        self.shape = shape
-        self.has_random_effect = True if len(shape)>1 else False
-        self.distmap = {'normal': pm.Normal,
-                   'hnormal': pm.HalfNormal,
-                   'gamma': pm.Gamma,
-                   'uniform': pm.Uniform,
-                   'igamma': pm.InverseGamma,
-                   'hcauchy': pm.HalfCauchy}
+        self.has_random_effect = has_random_effect
+        self.distmap = {
+            "normal": pm.Normal,
+            "hnormal": pm.HalfNormal,
+            "gamma": pm.Gamma,
+            "uniform": pm.Uniform,
+            "igamma": pm.InverseGamma,
+            "hcauchy": pm.HalfCauchy,
+            "hstudt": pm.HalfStudentT,
+            "studt": pm.StudentT,
+        }
         self.make_dist(dist, params, pb)
- 
+
     def make_dist(self, dist, params, pb):
-        """This creates a pymc3 distribution. If there is a trace, the distribution is fitted to the trace. If there isn't a trace, the prior is parameterized by the values in (params)"""
+        """This creates a pymc distribution. If there is a idata, the distribution is fitted to the idata. If there isn't a idata, the prior is parameterized by the values in (params)"""
         with pb.model as m:
-            if (pb.trace is not None) and (not self.has_random_effect):
-                int_dist = from_posterior(param=self.name,
-                                            samples=pb.trace[self.name],
-                                            distribution=dist,
-                                            freedom=pb.configs['freedom'])
-                self.dist = int_dist.reshape(self.shape)
+            if pb.idata is not None:
+                # Get samples
+                samples = az.extract(pb.idata, var_names=self.name)
+                # Define mapping to new shape
+                def get_new_dim_size(tup):
+                    oldsize, name = tup
+                    if name.startswith('batch_effect_'):
+                        ind = pb.batch_effect_dim_names.index(name)
+                        return len(np.unique(pb.batch_effect_indices[ind].container.data))
+                    return oldsize
+                
+                new_shape = list(map(get_new_dim_size, zip(samples.shape,samples.dims)))
+                if len(new_shape) == 1:
+                    new_shape = None
+                else:
+                    new_shape = new_shape[:-1]
+                self.dist = from_posterior(
+                    param=self.name,
+                    samples=samples.to_numpy(),
+                    shape = new_shape,
+                    distribution=dist,
+                    freedom=pb.configs["freedom"],
+                )
+
             else:
-                shape_prod = np.product(np.array(self.shape))
-                print(self.name)
-                print(f"dist={dist}")
-                print(f"params={params}")
-                int_dist = self.distmap[dist](self.name, *params, shape=shape_prod)
-                self.dist = int_dist.reshape(self.shape)
+                dims = []
+                if self.has_random_effect:
+                    dims = dims + pb.batch_effect_dim_names
+                if self.name.startswith("slope") or self.name.startswith("offset_slope"):
+                    dims = dims + ["basis_functions"]
+                if dims == []:
+                    self.dist = self.distmap[dist](self.name, *params)
+                else:
+                    self.dist = self.distmap[dist](self.name, *params, dims=dims)
 
     def __getitem__(self, idx):
         """The idx here is the index of the batch-effect. If the prior does not model batch effects, this should return the same value for each index"""
         assert self.dist is not None, "Distribution not initialized"
         if self.has_random_effect:
             return self.dist[idx]
         else:
             return self.dist
 
 
 class ParamBuilder:
     """
-    A class that simplifies the construction of parameterizations. 
-    It has a lot of attributes necessary for creating the model, including the data, but it is never saved with the model. 
+    A class that simplifies the construction of parameterizations.
+    It has a lot of attributes necessary for creating the model, including the data, but it is never saved with the model.
     It also contains a lot of decision logic for creating the parameterizations.
     """
 
-    def __init__(self, model, X, y, batch_effects, trace, configs):
+    def __init__(self, X, y, batch_effects, idata, configs):
         """
 
         :param model: model to attach all the distributions to
         :param X: Covariates
         :param y: IDPs
-        :param batch_effects: I guess this speaks for itself
-        :param trace:  idem
+        :param batch_effects: array of batch effects
+        :param idata:  idem
         :param configs: idem
         """
-        self.model = model
+        self.model = None  # Needs to be set later, because coords need to be passed at construction of Model
         self.X = X
+        self.n_basis_functions = X.shape[1]
         self.y = y
-        self.batch_effects = batch_effects
-        self.trace = trace
+        self.batch_effects = batch_effects.astype(np.int16)
+        self.idata: az.InferenceData = idata
         self.configs = configs
 
-        self.feature_num = X.shape[1].eval().item()
-        self.y_shape = y.shape.eval()
-        self.n_ys = y.shape[0].eval().item()
+        self.y_shape = y.shape
+        self.n_ys = y.shape[0]
         self.batch_effects_num = batch_effects.shape[1]
 
-        self.batch_effects_size = []
-        self.all_idx = []
-        for i in range(self.batch_effects_num):
-            # Count the unique values for each batch effect
-            self.batch_effects_size.append(len(np.unique(self.batch_effects[:, i])))
-            # Store the unique values for each batch effect
-            self.all_idx.append(np.int16(np.unique(self.batch_effects[:, i])))
-        # Make a cartesian product of all the unique values of each batch effect
-        self.be_idx = list(product(*self.all_idx))
-
-        # Make tuples of batch effects ID's and indices of datapoints with that specific combination of batch effects
-        self.be_idx_tups = []
-        for be in self.be_idx:
-            a = []
-            for i, b in enumerate(be):
-                a.append(self.batch_effects[:, i] == b)
-            idx = reduce(np.logical_and, a).nonzero()
-            if idx[0].shape[0] != 0:
-                self.be_idx_tups.append((be, idx))
+        self.batch_effect_dim_names = []
+        self.batch_effect_indices = []
+        self.coords = OrderedDict()
+        self.coords["basis_functions"] = np.arange(self.n_basis_functions)
 
-    def make_param(self, name, dim = (1,), **kwargs):
-        if self.configs.get(f'linear_{name}', False):
-            # First make a slope and intercept, and use those to make a linear parameterization 
-            slope_parameterization = self.make_param(f'slope_{name}', dim=[self.feature_num], **kwargs)
-            intercept_parameterization = self.make_param(f'intercept_{name}', **kwargs)
-            return LinearParameterization(name=name, dim=dim, 
-                                    slope_parameterization=slope_parameterization, 
-                                    intercept_parameterization=intercept_parameterization,
-                                    pb=self, 
-                                    **kwargs)
-        
-        elif self.configs.get(f'random_{name}', False):
-            if self.configs.get(f'centered_{name}', True):
-                return CentralRandomFixedParameterization(name=name, pb=self, dim=dim, **kwargs)
+        for i in range(self.batch_effects_num):
+            batch_effect_dim_name = f"batch_effect_{i}"
+            self.batch_effect_dim_names.append(batch_effect_dim_name)
+            this_be_values, this_be_indices = np.unique(
+                self.batch_effects[:, i], return_inverse=True
+            )
+            self.coords[batch_effect_dim_name] = this_be_values
+            self.batch_effect_indices.append(this_be_indices)
+
+    def make_param(self, name, **kwargs):
+        if self.configs.get(f"linear_{name}", False):
+            # First make a slope and intercept, and use those to make a linear parameterization
+            slope_parameterization = self.make_param(f"slope_{name}", **kwargs)
+            intercept_parameterization = self.make_param(f"intercept_{name}", **kwargs)
+            return LinearParameterization(
+                name=name,
+                slope_parameterization=slope_parameterization,
+                intercept_parameterization=intercept_parameterization,
+                **kwargs,
+            )
+
+        elif self.configs.get(f"random_{name}", False):
+            if self.configs.get(f"centered_{name}", True):
+                return CentralRandomFixedParameterization(name=name, pb=self, **kwargs)
             else:
-                return NonCentralRandomFixedParameterization(name=name, pb=self, dim=dim, **kwargs)
+                return NonCentralRandomFixedParameterization(
+                    name=name, pb=self, **kwargs
+                )
         else:
-            return FixedParameterization(name=name, dim=dim, pb=self,**kwargs)
+            return FixedParameterization(name=name, pb=self, **kwargs)
 
 
 class Parameterization:
     """
     This is the top-level parameterization class from which all the other parameterizations inherit.
     """
-    def __init__(self, name, dim):
+
+    def __init__(self, name):
         self.name = name
-        self.dim = dim
-        print(name, type(self))
+        # print(name, type(self))
 
     def get_samples(self, pb):
-
-        with pb.model:
-            samples = theano.tensor.zeros([pb.n_ys, *self.dim])
-            for be, idx in pb.be_idx_tups:
-                samples = theano.tensor.set_subtensor(samples[idx], self.dist[be])
-        return samples
+        pass
 
 
 class FixedParameterization(Parameterization):
     """
     A parameterization that takes a single value for all input. It does not depend on anything except its hyperparameters
     """
-    def __init__(self, name, dim, pb:ParamBuilder, **kwargs):
-        super().__init__(name, dim)
-        dist = kwargs.get(f'{name}_dist','normal')
-        params = kwargs.get(f'{name}_params',(0.,1.))
-        self.dist = Prior(name, dist, params, pb, shape = dim)
+
+    def __init__(self, name, pb: ParamBuilder, **kwargs):
+        super().__init__(name)
+        dist = kwargs.get(f"{name}_dist", "normal")
+        params = kwargs.get(f"{name}_params", (0.0, 1.0))
+        self.dist = Prior(name, dist, params, pb)
+
+    def get_samples(self, pb):
+        with pb.model:
+            return self.dist[0]
 
 
 class CentralRandomFixedParameterization(Parameterization):
     """
     A parameterization that is fixed for each batch effect. This is sampled in a central fashion;
-    the values are sampled from normal distribution with a group mean and group variance 
+    the values are sampled from normal distribution with a group mean and group variance
     """
-    def __init__(self, name, dim, pb:ParamBuilder, **kwargs):
-        super().__init__(name, dim)
+
+    def __init__(self, name, pb: ParamBuilder, **kwargs):
+        super().__init__(name)
 
         # Normal distribution is default for mean
-        mu_dist = kwargs.get(f'mu_{name}_dist','normal')
-        mu_params = kwargs.get(f'mu_{name}_params',(0.,1.))
-        mu_prior = Prior(f'mu_{name}', mu_dist, mu_params, pb, shape = dim)
-
-        # HalfCauchy is default for sigma
-        sigma_dist = kwargs.get(f'sigma_{name}_dist','hcauchy')
-        sigma_params = kwargs.get(f'sigma_{name}_params',(1.,))
-        sigma_prior = Prior(f'sigma_{name}',sigma_dist, sigma_params, pb, shape = [*pb.batch_effects_size, *dim])
+        mu_dist = kwargs.get(f"mu_{name}_dist", "normal")
+        mu_params = kwargs.get(f"mu_{name}_params", (0.0, 1.0))
+        mu_prior = Prior(f"mu_{name}", mu_dist, mu_params, pb)
+
+        # HalfNormal is default for sigma
+        sigma_dist = kwargs.get(f"sigma_{name}_dist", "hnormal")
+        sigma_params = kwargs.get(f"sigma_{name}_params", (1.0,))
+        sigma_prior = Prior(f"sigma_{name}", sigma_dist, sigma_params, pb)
+
+        dims = (
+            [*pb.batch_effect_dim_names, "basis_functions"]
+            if self.name.startswith("slope")
+            else pb.batch_effect_dim_names
+        )
+        self.dist = pm.Normal(
+            name=name,
+            mu=mu_prior.dist,
+            sigma=sigma_prior.dist,
+            dims=dims,
+        )
+
+    def get_samples(self, pb: ParamBuilder):
+        with pb.model:
+            samples = self.dist[pb.batch_effect_indices]
+            return samples
 
-        self.dist = pm.Normal(name=name, mu=mu_prior.dist, sigma=sigma_prior.dist, shape = [*pb.batch_effects_size, *dim])
-    
 
 class NonCentralRandomFixedParameterization(Parameterization):
     """
     A parameterization that is fixed for each batch effect. This is sampled in a non-central fashion;
-    the values are a sum of a group mean and noise values scaled with a group scaling factor 
+    the values are a sum of a group mean and noise values scaled with a group scaling factor
     """
-    def __init__(self, name,dim,  pb:ParamBuilder, **kwargs):
-        super().__init__(name, dim)
+
+    def __init__(self, name, pb: ParamBuilder, **kwargs):
+        super().__init__(name)
 
         # Normal distribution is default for mean
-        mu_dist = kwargs.get(f'mu_{name}_dist','normal')
-        mu_params = kwargs.get(f'mu_{name}_params',(0.,1.))
-        mu_prior = Prior(f'mu_{name}', mu_dist, mu_params, pb, shape = dim)
-
-        # HalfCauchy is default for sigma
-        sigma_dist = kwargs.get(f'sigma_{name}_dist','hcauchy')
-        sigma_params = kwargs.get(f'sigma_{name}_params',(1.,))
-        sigma_prior = Prior(f'sigma_{name}',sigma_dist, sigma_params, pb, shape = dim)
+        mu_dist = kwargs.get(f"mu_{name}_dist", "normal")
+        mu_params = kwargs.get(f"mu_{name}_params", (0.0, 1.0))
+        mu_prior = Prior(f"mu_{name}", mu_dist, mu_params, pb)
+
+        # HalfNormal is default for sigma
+        sigma_dist = kwargs.get(f"sigma_{name}_dist", "hnormal")
+        sigma_params = kwargs.get(f"sigma_{name}_params", (1.0,))
+        sigma_prior = Prior(f"sigma_{name}", sigma_dist, sigma_params, pb)
 
         # Normal is default for offset
-        offset_dist = kwargs.get(f'offset_{name}_dist','normal')
-        offset_params = kwargs.get(f'offset_{name}_params',(0.,1.))
-        offset_prior = Prior(f'offset_{name}',offset_dist, offset_params, pb, shape = [*pb.batch_effects_size, *dim])
+        offset_dist = kwargs.get(f"offset_{name}_dist", "normal")
+        offset_params = kwargs.get(f"offset_{name}_params", (0.0, 1.0))
+        offset_prior = Prior(
+            f"offset_{name}", offset_dist, offset_params, pb, has_random_effect=True
+        )
+        dims = (
+            [*pb.batch_effect_dim_names, "basis_functions"]
+            if self.name.startswith("slope")
+            else pb.batch_effect_dim_names
+        )
+        self.dist = pm.Deterministic(
+            name=name,
+            var=mu_prior.dist + sigma_prior.dist * offset_prior.dist,
+            dims=dims,
+        )
 
-        self.dist = pm.Deterministic(name=name, var=mu_prior.dist+sigma_prior.dist*offset_prior.dist)
+    def get_samples(self, pb: ParamBuilder):
+        with pb.model:
+            samples = self.dist[pb.batch_effect_indices]
+            return samples
 
 
 class LinearParameterization(Parameterization):
     """
-    A parameterization that can model a linear dependence on X. 
+    A parameterization that can model a linear dependence on X.
     """
-    def __init__(self, name, dim, slope_parameterization, intercept_parameterization, pb, **kwargs):
-        super().__init__( name, dim)
+
+    def __init__(
+        self, name, slope_parameterization, intercept_parameterization, **kwargs
+    ):
+        super().__init__(name)
         self.slope_parameterization = slope_parameterization
         self.intercept_parameterization = intercept_parameterization
 
-    def get_samples(self, pb:ParamBuilder):
+    def get_samples(self, pb):
         with pb.model:
-            samples = theano.tensor.zeros([pb.n_ys, *self.dim])
-            for be, idx in pb.be_idx_tups:
-                dot = theano.tensor.dot(pb.X[idx,:], self.slope_parameterization.dist[be]).T
-                intercept = self.intercept_parameterization.dist[be]
-                samples = theano.tensor.set_subtensor(samples[idx,:],dot+intercept)
-        return samples
+            intc = self.intercept_parameterization.get_samples(pb)
+            slope_samples = self.slope_parameterization.get_samples(pb)
+            if pb.configs[f"random_slope_{self.name}"]:
+                slope = pb.X * slope_samples
+                slope = slope.sum(axis=-1)
+            else:
+                slope = pb.X @ self.slope_parameterization.get_samples(pb)
+
+            samples = pm.math.flatten(intc) + pm.math.flatten(slope)
+            return samples
 
 
 def get_design_matrix(X, nm, basis="linear"):
     if basis == "bspline":
         Phi = bspline_transform(X, nm.hbr.bsp)
     elif basis == "polynomial":
         Phi = create_poly_basis(X, 3)
     else:
         Phi = X
     return Phi
 
 
-
-def nn_hbr(X, y, batch_effects, batch_effects_size, configs, trace=None):
-    n_hidden = configs['nn_hidden_neuron_num']
-    n_layers = configs['nn_hidden_layers_num']
+def nn_hbr(X, y, batch_effects, batch_effects_size, configs, idata=None):
+    n_hidden = configs["nn_hidden_neuron_num"]
+    n_layers = configs["nn_hidden_layers_num"]
     feature_num = X.shape[1]
     batch_effects_num = batch_effects.shape[1]
     all_idx = []
     for i in range(batch_effects_num):
         all_idx.append(np.int16(np.unique(batch_effects[:, i])))
     be_idx = list(product(*all_idx))
 
     # Initialize random weights between each layer for the mu:
-    init_1 = pm.floatX(np.random.randn(feature_num, n_hidden) * np.sqrt(1 / feature_num))
+    init_1 = pm.floatX(
+        np.random.randn(feature_num, n_hidden) * np.sqrt(1 / feature_num)
+    )
     init_out = pm.floatX(np.random.randn(n_hidden) * np.sqrt(1 / n_hidden))
 
     std_init_1 = pm.floatX(np.random.rand(feature_num, n_hidden))
     std_init_out = pm.floatX(np.random.rand(n_hidden))
 
     # And initialize random weights between each layer for sigma_noise:
-    init_1_noise = pm.floatX(np.random.randn(feature_num, n_hidden) * np.sqrt(1 / feature_num))
+    init_1_noise = pm.floatX(
+        np.random.randn(feature_num, n_hidden) * np.sqrt(1 / feature_num)
+    )
     init_out_noise = pm.floatX(np.random.randn(n_hidden) * np.sqrt(1 / n_hidden))
 
     std_init_1_noise = pm.floatX(np.random.rand(feature_num, n_hidden))
     std_init_out_noise = pm.floatX(np.random.rand(n_hidden))
 
     # If there are two hidden layers, then initialize weights for the second layer:
     if n_layers == 2:
         init_2 = pm.floatX(np.random.randn(n_hidden, n_hidden) * np.sqrt(1 / n_hidden))
         std_init_2 = pm.floatX(np.random.rand(n_hidden, n_hidden))
-        init_2_noise = pm.floatX(np.random.randn(n_hidden, n_hidden) * np.sqrt(1 / n_hidden))
+        init_2_noise = pm.floatX(
+            np.random.randn(n_hidden, n_hidden) * np.sqrt(1 / n_hidden)
+        )
         std_init_2_noise = pm.floatX(np.random.rand(n_hidden, n_hidden))
 
     with pm.Model() as model:
+        X = pm.Data("X", X)
+        y = pm.Data("y", y)
 
-        X = pm.Data('X', X)
-        y = pm.Data('y', y)
-
-        if trace is not None:  # Used when estimating/predicting on a new site
-            weights_in_1_grp = from_posterior('w_in_1_grp', trace['w_in_1_grp'],
-                                              distribution='normal', freedom=configs['freedom'])
-
-            weights_in_1_grp_sd = from_posterior('w_in_1_grp_sd', trace['w_in_1_grp_sd'],
-                                                 distribution='hcauchy', freedom=configs['freedom'])
+        if idata is not None:  # Used when estimating/predicting on a new site
+            weights_in_1_grp = from_posterior(
+                "w_in_1_grp",
+                idata["w_in_1_grp"],
+                distribution="normal",
+                freedom=configs["freedom"],
+            )
+
+            weights_in_1_grp_sd = from_posterior(
+                "w_in_1_grp_sd",
+                idata["w_in_1_grp_sd"],
+                distribution="hcauchy",
+                freedom=configs["freedom"],
+            )
 
             if n_layers == 2:
-                weights_1_2_grp = from_posterior('w_1_2_grp', trace['w_1_2_grp'],
-                                                 distribution='normal', freedom=configs['freedom'])
-
-                weights_1_2_grp_sd = from_posterior('w_1_2_grp_sd', trace['w_1_2_grp_sd'],
-                                                    distribution='hcauchy', freedom=configs['freedom'])
-
-            weights_2_out_grp = from_posterior('w_2_out_grp', trace['w_2_out_grp'],
-                                               distribution='normal', freedom=configs['freedom'])
-
-            weights_2_out_grp_sd = from_posterior('w_2_out_grp_sd', trace['w_2_out_grp_sd'],
-                                                  distribution='hcauchy', freedom=configs['freedom'])
-
-            mu_prior_intercept = from_posterior('mu_prior_intercept', trace['mu_prior_intercept'],
-                                                distribution='normal', freedom=configs['freedom'])
-            sigma_prior_intercept = from_posterior('sigma_prior_intercept', trace['sigma_prior_intercept'],
-                                                   distribution='hcauchy', freedom=configs['freedom'])
+                weights_1_2_grp = from_posterior(
+                    "w_1_2_grp",
+                    idata["w_1_2_grp"],
+                    distribution="normal",
+                    freedom=configs["freedom"],
+                )
+
+                weights_1_2_grp_sd = from_posterior(
+                    "w_1_2_grp_sd",
+                    idata["w_1_2_grp_sd"],
+                    distribution="hcauchy",
+                    freedom=configs["freedom"],
+                )
+
+            weights_2_out_grp = from_posterior(
+                "w_2_out_grp",
+                idata["w_2_out_grp"],
+                distribution="normal",
+                freedom=configs["freedom"],
+            )
+
+            weights_2_out_grp_sd = from_posterior(
+                "w_2_out_grp_sd",
+                idata["w_2_out_grp_sd"],
+                distribution="hcauchy",
+                freedom=configs["freedom"],
+            )
+
+            mu_prior_intercept = from_posterior(
+                "mu_prior_intercept",
+                idata["mu_prior_intercept"],
+                distribution="normal",
+                freedom=configs["freedom"],
+            )
+            sigma_prior_intercept = from_posterior(
+                "sigma_prior_intercept",
+                idata["sigma_prior_intercept"],
+                distribution="hcauchy",
+                freedom=configs["freedom"],
+            )
 
         else:
             # Group the mean distribution for input to the hidden layer:
-            weights_in_1_grp = pm.Normal('w_in_1_grp', 0, sd=1,
-                                         shape=(feature_num, n_hidden), testval=init_1)
+            weights_in_1_grp = pm.Normal(
+                "w_in_1_grp", 0, sd=1, shape=(feature_num, n_hidden), testval=init_1
+            )
 
             # Group standard deviation:
-            weights_in_1_grp_sd = pm.HalfCauchy('w_in_1_grp_sd', 1.,
-                                                shape=(feature_num, n_hidden), testval=std_init_1)
+            weights_in_1_grp_sd = pm.HalfCauchy(
+                "w_in_1_grp_sd", 1.0, shape=(feature_num, n_hidden), testval=std_init_1
+            )
 
             if n_layers == 2:
                 # Group the mean distribution for hidden layer 1 to hidden layer 2:
-                weights_1_2_grp = pm.Normal('w_1_2_grp', 0, sd=1,
-                                            shape=(n_hidden, n_hidden), testval=init_2)
+                weights_1_2_grp = pm.Normal(
+                    "w_1_2_grp", 0, sd=1, shape=(n_hidden, n_hidden), testval=init_2
+                )
 
                 # Group standard deviation:
-                weights_1_2_grp_sd = pm.HalfCauchy('w_1_2_grp_sd', 1.,
-                                                   shape=(n_hidden, n_hidden), testval=std_init_2)
+                weights_1_2_grp_sd = pm.HalfCauchy(
+                    "w_1_2_grp_sd", 1.0, shape=(n_hidden, n_hidden), testval=std_init_2
+                )
 
             # Group the mean distribution for hidden to output:
-            weights_2_out_grp = pm.Normal('w_2_out_grp', 0, sd=1,
-                                          shape=(n_hidden,), testval=init_out)
+            weights_2_out_grp = pm.Normal(
+                "w_2_out_grp", 0, sd=1, shape=(n_hidden,), testval=init_out
+            )
 
             # Group standard deviation:
-            weights_2_out_grp_sd = pm.HalfCauchy('w_2_out_grp_sd', 1.,
-                                                 shape=(n_hidden,), testval=std_init_out)
+            weights_2_out_grp_sd = pm.HalfCauchy(
+                "w_2_out_grp_sd", 1.0, shape=(n_hidden,), testval=std_init_out
+            )
 
             # mu_prior_intercept = pm.Uniform('mu_prior_intercept', lower=-100, upper=100)
-            mu_prior_intercept = pm.Normal('mu_prior_intercept', mu=0., sigma=1e3)
-            sigma_prior_intercept = pm.HalfCauchy('sigma_prior_intercept', 5)
+            mu_prior_intercept = pm.Normal("mu_prior_intercept", mu=0.0, sigma=1e3)
+            sigma_prior_intercept = pm.HalfCauchy("sigma_prior_intercept", 5)
 
         # Now create separate weights for each group, by doing
         # weights * group_sd + group_mean, we make sure the new weights are
         # coming from the (group_mean, group_sd) distribution.
-        weights_in_1_raw = pm.Normal('w_in_1', 0, sd=1,
-                                     shape=(batch_effects_size + [feature_num, n_hidden]))
+        weights_in_1_raw = pm.Normal(
+            "w_in_1", 0, sd=1, shape=(batch_effects_size + [feature_num, n_hidden])
+        )
         weights_in_1 = weights_in_1_raw * weights_in_1_grp_sd + weights_in_1_grp
 
         if n_layers == 2:
-            weights_1_2_raw = pm.Normal('w_1_2', 0, sd=1,
-                                        shape=(batch_effects_size + [n_hidden, n_hidden]))
+            weights_1_2_raw = pm.Normal(
+                "w_1_2", 0, sd=1, shape=(batch_effects_size + [n_hidden, n_hidden])
+            )
             weights_1_2 = weights_1_2_raw * weights_1_2_grp_sd + weights_1_2_grp
 
-        weights_2_out_raw = pm.Normal('w_2_out', 0, sd=1,
-                                      shape=(batch_effects_size + [n_hidden]))
+        weights_2_out_raw = pm.Normal(
+            "w_2_out", 0, sd=1, shape=(batch_effects_size + [n_hidden])
+        )
         weights_2_out = weights_2_out_raw * weights_2_out_grp_sd + weights_2_out_grp
 
-        intercepts_offset = pm.Normal('intercepts_offset', mu=0, sd=1,
-                                      shape=(batch_effects_size))
+        intercepts_offset = pm.Normal(
+            "intercepts_offset", mu=0, sd=1, shape=(batch_effects_size)
+        )
 
-        intercepts = pm.Deterministic('intercepts', intercepts_offset +
-                                      mu_prior_intercept * sigma_prior_intercept)
+        intercepts = pm.Deterministic(
+            "intercepts", intercepts_offset + mu_prior_intercept * sigma_prior_intercept
+        )
 
         # Build the neural network and estimate y_hat:
-        y_hat = theano.tensor.zeros(y.shape)
+        y_hat = pytensor.tensor.zeros(y.shape)
         for be in be_idx:
             # Find the indices corresponding to 'group be':
             a = []
             for i, b in enumerate(be):
                 a.append(batch_effects[:, i] == b)
             idx = reduce(np.logical_and, a).nonzero()
             if idx[0].shape[0] != 0:
-                act_1 = pm.math.tanh(theano.tensor.dot(X[idx, :], weights_in_1[be]))
+                act_1 = pm.math.tanh(pytensor.tensor.dot(X[idx, :], weights_in_1[be]))
                 if n_layers == 2:
-                    act_2 = pm.math.tanh(theano.tensor.dot(act_1, weights_1_2[be]))
-                    y_hat = theano.tensor.set_subtensor(y_hat[idx, 0],
-                                                        intercepts[be] + theano.tensor.dot(act_2, weights_2_out[be]))
+                    act_2 = pm.math.tanh(pytensor.tensor.dot(act_1, weights_1_2[be]))
+                    y_hat = pytensor.tensor.set_subtensor(
+                        y_hat[idx, 0],
+                        intercepts[be] + pytensor.tensor.dot(act_2, weights_2_out[be]),
+                    )
                 else:
-                    y_hat = theano.tensor.set_subtensor(y_hat[idx, 0],
-                                                        intercepts[be] + theano.tensor.dot(act_1, weights_2_out[be]))
+                    y_hat = pytensor.tensor.set_subtensor(
+                        y_hat[idx, 0],
+                        intercepts[be] + pytensor.tensor.dot(act_1, weights_2_out[be]),
+                    )
 
         # If we want to estimate varying noise terms across groups:
-        if configs['random_noise']:
-            if configs['hetero_noise']:
-                if trace is not None:  # # Used when estimating/predicting on a new site
-                    weights_in_1_grp_noise = from_posterior('w_in_1_grp_noise',
-                                                            trace['w_in_1_grp_noise'],
-                                                            distribution='normal', freedom=configs['freedom'])
-
-                    weights_in_1_grp_sd_noise = from_posterior('w_in_1_grp_sd_noise',
-                                                               trace['w_in_1_grp_sd_noise'],
-                                                               distribution='hcauchy', freedom=configs['freedom'])
+        if configs["random_noise"]:
+            if configs["hetero_noise"]:
+                if idata is not None:  # # Used when estimating/predicting on a new site
+                    weights_in_1_grp_noise = from_posterior(
+                        "w_in_1_grp_noise",
+                        idata["w_in_1_grp_noise"],
+                        distribution="normal",
+                        freedom=configs["freedom"],
+                    )
+
+                    weights_in_1_grp_sd_noise = from_posterior(
+                        "w_in_1_grp_sd_noise",
+                        idata["w_in_1_grp_sd_noise"],
+                        distribution="hcauchy",
+                        freedom=configs["freedom"],
+                    )
 
                     if n_layers == 2:
-                        weights_1_2_grp_noise = from_posterior('w_1_2_grp_noise',
-                                                               trace['w_1_2_grp_noise'],
-                                                               distribution='normal', freedom=configs['freedom'])
-
-                        weights_1_2_grp_sd_noise = from_posterior('w_1_2_grp_sd_noise',
-                                                                  trace['w_1_2_grp_sd_noise'],
-                                                                  distribution='hcauchy', freedom=configs['freedom'])
-
-                    weights_2_out_grp_noise = from_posterior('w_2_out_grp_noise',
-                                                             trace['w_2_out_grp_noise'],
-                                                             distribution='normal', freedom=configs['freedom'])
-
-                    weights_2_out_grp_sd_noise = from_posterior('w_2_out_grp_sd_noise',
-                                                                trace['w_2_out_grp_sd_noise'],
-                                                                distribution='hcauchy', freedom=configs['freedom'])
+                        weights_1_2_grp_noise = from_posterior(
+                            "w_1_2_grp_noise",
+                            idata["w_1_2_grp_noise"],
+                            distribution="normal",
+                            freedom=configs["freedom"],
+                        )
+
+                        weights_1_2_grp_sd_noise = from_posterior(
+                            "w_1_2_grp_sd_noise",
+                            idata["w_1_2_grp_sd_noise"],
+                            distribution="hcauchy",
+                            freedom=configs["freedom"],
+                        )
+
+                    weights_2_out_grp_noise = from_posterior(
+                        "w_2_out_grp_noise",
+                        idata["w_2_out_grp_noise"],
+                        distribution="normal",
+                        freedom=configs["freedom"],
+                    )
+
+                    weights_2_out_grp_sd_noise = from_posterior(
+                        "w_2_out_grp_sd_noise",
+                        idata["w_2_out_grp_sd_noise"],
+                        distribution="hcauchy",
+                        freedom=configs["freedom"],
+                    )
 
                 else:
                     # The input layer to the first hidden layer:
-                    weights_in_1_grp_noise = pm.Normal('w_in_1_grp_noise', 0, sd=1,
-                                                       shape=(feature_num, n_hidden),
-                                                       testval=init_1_noise)
-                    weights_in_1_grp_sd_noise = pm.HalfCauchy('w_in_1_grp_sd_noise', 1,
-                                                              shape=(feature_num, n_hidden),
-                                                              testval=std_init_1_noise)
+                    weights_in_1_grp_noise = pm.Normal(
+                        "w_in_1_grp_noise",
+                        0,
+                        sd=1,
+                        shape=(feature_num, n_hidden),
+                        testval=init_1_noise,
+                    )
+                    weights_in_1_grp_sd_noise = pm.HalfCauchy(
+                        "w_in_1_grp_sd_noise",
+                        1,
+                        shape=(feature_num, n_hidden),
+                        testval=std_init_1_noise,
+                    )
 
                     # The first hidden layer to second hidden layer:
                     if n_layers == 2:
-                        weights_1_2_grp_noise = pm.Normal('w_1_2_grp_noise', 0, sd=1,
-                                                          shape=(n_hidden, n_hidden),
-                                                          testval=init_2_noise)
-                        weights_1_2_grp_sd_noise = pm.HalfCauchy('w_1_2_grp_sd_noise', 1,
-                                                                 shape=(n_hidden, n_hidden),
-                                                                 testval=std_init_2_noise)
+                        weights_1_2_grp_noise = pm.Normal(
+                            "w_1_2_grp_noise",
+                            0,
+                            sd=1,
+                            shape=(n_hidden, n_hidden),
+                            testval=init_2_noise,
+                        )
+                        weights_1_2_grp_sd_noise = pm.HalfCauchy(
+                            "w_1_2_grp_sd_noise",
+                            1,
+                            shape=(n_hidden, n_hidden),
+                            testval=std_init_2_noise,
+                        )
 
                     # The second hidden layer to output layer:
-                    weights_2_out_grp_noise = pm.Normal('w_2_out_grp_noise', 0, sd=1,
-                                                        shape=(n_hidden,),
-                                                        testval=init_out_noise)
-                    weights_2_out_grp_sd_noise = pm.HalfCauchy('w_2_out_grp_sd_noise', 1,
-                                                               shape=(n_hidden,),
-                                                               testval=std_init_out_noise)
+                    weights_2_out_grp_noise = pm.Normal(
+                        "w_2_out_grp_noise",
+                        0,
+                        sd=1,
+                        shape=(n_hidden,),
+                        testval=init_out_noise,
+                    )
+                    weights_2_out_grp_sd_noise = pm.HalfCauchy(
+                        "w_2_out_grp_sd_noise",
+                        1,
+                        shape=(n_hidden,),
+                        testval=std_init_out_noise,
+                    )
 
                     # mu_prior_intercept_noise = pm.HalfNormal('mu_prior_intercept_noise', sigma=1e3)
                     # sigma_prior_intercept_noise = pm.HalfCauchy('sigma_prior_intercept_noise', 5)
 
                 # Now create separate weights for each group:
-                weights_in_1_raw_noise = pm.Normal('w_in_1_noise', 0, sd=1,
-                                                   shape=(batch_effects_size + [feature_num, n_hidden]))
-                weights_in_1_noise = weights_in_1_raw_noise * weights_in_1_grp_sd_noise + weights_in_1_grp_noise
+                weights_in_1_raw_noise = pm.Normal(
+                    "w_in_1_noise",
+                    0,
+                    sd=1,
+                    shape=(batch_effects_size + [feature_num, n_hidden]),
+                )
+                weights_in_1_noise = (
+                    weights_in_1_raw_noise * weights_in_1_grp_sd_noise
+                    + weights_in_1_grp_noise
+                )
 
                 if n_layers == 2:
-                    weights_1_2_raw_noise = pm.Normal('w_1_2_noise', 0, sd=1,
-                                                      shape=(batch_effects_size + [n_hidden, n_hidden]))
-                    weights_1_2_noise = weights_1_2_raw_noise * weights_1_2_grp_sd_noise + weights_1_2_grp_noise
-
-                weights_2_out_raw_noise = pm.Normal('w_2_out_noise', 0, sd=1,
-                                                    shape=(batch_effects_size + [n_hidden]))
-                weights_2_out_noise = weights_2_out_raw_noise * weights_2_out_grp_sd_noise + weights_2_out_grp_noise
+                    weights_1_2_raw_noise = pm.Normal(
+                        "w_1_2_noise",
+                        0,
+                        sd=1,
+                        shape=(batch_effects_size + [n_hidden, n_hidden]),
+                    )
+                    weights_1_2_noise = (
+                        weights_1_2_raw_noise * weights_1_2_grp_sd_noise
+                        + weights_1_2_grp_noise
+                    )
+
+                weights_2_out_raw_noise = pm.Normal(
+                    "w_2_out_noise", 0, sd=1, shape=(batch_effects_size + [n_hidden])
+                )
+                weights_2_out_noise = (
+                    weights_2_out_raw_noise * weights_2_out_grp_sd_noise
+                    + weights_2_out_grp_noise
+                )
 
                 # intercepts_offset_noise = pm.Normal('intercepts_offset_noise', mu=0, sd=1,
                 #                          shape=(batch_effects_size))
 
                 # intercepts_noise = pm.Deterministic('intercepts_noise', mu_prior_intercept_noise +
                 #                      intercepts_offset_noise * sigma_prior_intercept_noise)
 
                 # Build the neural network and estimate the sigma_y:
-                sigma_y = theano.tensor.zeros(y.shape)
+                sigma_y = pytensor.tensor.zeros(y.shape)
                 for be in be_idx:
                     a = []
                     for i, b in enumerate(be):
                         a.append(batch_effects[:, i] == b)
                     idx = reduce(np.logical_and, a).nonzero()
                     if idx[0].shape[0] != 0:
-                        act_1_noise = pm.math.sigmoid(theano.tensor.dot(X[idx, :], weights_in_1_noise[be]))
+                        act_1_noise = pm.math.sigmoid(
+                            pytensor.tensor.dot(X[idx, :], weights_in_1_noise[be])
+                        )
                         if n_layers == 2:
-                            act_2_noise = pm.math.sigmoid(theano.tensor.dot(act_1_noise, weights_1_2_noise[be]))
-                            temp = pm.math.log1pexp(theano.tensor.dot(act_2_noise, weights_2_out_noise[be])) + 1e-5
+                            act_2_noise = pm.math.sigmoid(
+                                pytensor.tensor.dot(act_1_noise, weights_1_2_noise[be])
+                            )
+                            temp = (
+                                pm.math.log1pexp(
+                                    pytensor.tensor.dot(
+                                        act_2_noise, weights_2_out_noise[be]
+                                    )
+                                )
+                                + 1e-5
+                            )
                         else:
-                            temp = pm.math.log1pexp(theano.tensor.dot(act_1_noise, weights_2_out_noise[be])) + 1e-5
-                        sigma_y = theano.tensor.set_subtensor(sigma_y[idx, 0], temp)
+                            temp = (
+                                pm.math.log1pexp(
+                                    pytensor.tensor.dot(
+                                        act_1_noise, weights_2_out_noise[be]
+                                    )
+                                )
+                                + 1e-5
+                            )
+                        sigma_y = pytensor.tensor.set_subtensor(sigma_y[idx, 0], temp)
 
             else:  # homoscedastic noise:
-                if trace is not None:  # Used for transferring the priors
-                    upper_bound = np.percentile(trace['sigma_noise'], 95)
-                    sigma_noise = pm.Uniform('sigma_noise', lower=0, upper=2 * upper_bound, shape=(batch_effects_size))
+                if idata is not None:  # Used for transferring the priors
+                    upper_bound = np.percentile(idata["sigma_noise"], 95)
+                    sigma_noise = pm.Uniform(
+                        "sigma_noise",
+                        lower=0,
+                        upper=2 * upper_bound,
+                        shape=(batch_effects_size),
+                    )
                 else:
-                    sigma_noise = pm.Uniform('sigma_noise', lower=0, upper=100, shape=(batch_effects_size))
+                    sigma_noise = pm.Uniform(
+                        "sigma_noise", lower=0, upper=100, shape=(batch_effects_size)
+                    )
 
-                sigma_y = theano.tensor.zeros(y.shape)
+                sigma_y = pytensor.tensor.zeros(y.shape)
                 for be in be_idx:
                     a = []
                     for i, b in enumerate(be):
                         a.append(batch_effects[:, i] == b)
                     idx = reduce(np.logical_and, a).nonzero()
                     if idx[0].shape[0] != 0:
-                        sigma_y = theano.tensor.set_subtensor(sigma_y[idx, 0], sigma_noise[be])
+                        sigma_y = pytensor.tensor.set_subtensor(
+                            sigma_y[idx, 0], sigma_noise[be]
+                        )
 
         else:  # do not allow for random noise terms across groups:
-            if trace is not None:  # Used for transferring the priors
-                upper_bound = np.percentile(trace['sigma_noise'], 95)
-                sigma_noise = pm.Uniform('sigma_noise', lower=0, upper=2 * upper_bound)
+            if idata is not None:  # Used for transferring the priors
+                upper_bound = np.percentile(idata["sigma_noise"], 95)
+                sigma_noise = pm.Uniform("sigma_noise", lower=0, upper=2 * upper_bound)
             else:
-                sigma_noise = pm.Uniform('sigma_noise', lower=0, upper=100)
-            sigma_y = theano.tensor.zeros(y.shape)
+                sigma_noise = pm.Uniform("sigma_noise", lower=0, upper=100)
+            sigma_y = pytensor.tensor.zeros(y.shape)
             for be in be_idx:
                 a = []
                 for i, b in enumerate(be):
                     a.append(batch_effects[:, i] == b)
                 idx = reduce(np.logical_and, a).nonzero()
                 if idx[0].shape[0] != 0:
-                    sigma_y = theano.tensor.set_subtensor(sigma_y[idx, 0], sigma_noise)
-
-        if configs['skewed_likelihood']:
-            skewness = pm.Uniform('skewness', lower=-10, upper=10, shape=(batch_effects_size))
-            alpha = theano.tensor.zeros(y.shape)
+                    sigma_y = pytensor.tensor.set_subtensor(
+                        sigma_y[idx, 0], sigma_noise
+                    )
+
+        if configs["skewed_likelihood"]:
+            skewness = pm.Uniform(
+                "skewness", lower=-10, upper=10, shape=(batch_effects_size)
+            )
+            alpha = pytensor.tensor.zeros(y.shape)
             for be in be_idx:
                 a = []
                 for i, b in enumerate(be):
                     a.append(batch_effects[:, i] == b)
                 idx = reduce(np.logical_and, a).nonzero()
                 if idx[0].shape[0] != 0:
-                    alpha = theano.tensor.set_subtensor(alpha[idx, 0], skewness[be])
+                    alpha = pytensor.tensor.set_subtensor(alpha[idx, 0], skewness[be])
         else:
             alpha = 0  # symmetrical normal distribution
 
-        y_like = pm.SkewNormal('y_like', mu=y_hat, sigma=sigma_y, alpha=alpha, observed=y)
+        y_like = pm.SkewNormal(
+            "y_like", mu=y_hat, sigma=sigma_y, alpha=alpha, observed=y
+        )
 
     return model
```

### Comparing `pcntoolkit-0.27/pcntoolkit/model/rfa.py` & `pcntoolkit-0.28/pcntoolkit/model/rfa.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative.py` & `pcntoolkit-0.28/pcntoolkit/normative.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             n = Xz_tr.shape[0]
             k = len(getattr(nm, alg).hyp)
             BIC = k * np.log(n) + 2 * nlZ
             results['BIC'] = BIC    
     
     return results
 
-def save_results(respfile, Yhat, S2, maskvol, Z=None, outputsuffix=None, 
+def save_results(respfile, Yhat, S2, maskvol, Z=None, Y=None, outputsuffix=None, 
                  results=None, save_path=''):
     
     print("Writing outputs ...")
     if respfile is None:
         exfile = None
         file_ext = '.pkl'
     else:
@@ -240,15 +240,17 @@
     fileio.save(Yhat, os.path.join(save_path, 'yhat' + ext), example=exfile, 
                                    mask=maskvol)
     fileio.save(S2, os.path.join(save_path, 'ys2' + ext), example=exfile, 
                 mask=maskvol)
     if Z is not None:
         fileio.save(Z, os.path.join(save_path, 'Z' + ext), example=exfile, 
                     mask=maskvol)
-
+    if Y is not None:
+        fileio.save(Y, os.path.join(save_path, 'Y' + ext), example=exfile, 
+                    mask=maskvol)
     if results is not None:        
         for metric in list(results.keys()):
             if (metric == 'NLL' or metric == 'BIC') and file_ext == '.nii.gz':
                 fileio.save(results[metric], os.path.join(save_path, metric + str(outputsuffix) + '.pkl'), 
                         example=exfile, mask=maskvol)
             else:
                 fileio.save(results[metric], os.path.join(save_path, metric + ext), 
@@ -666,33 +668,36 @@
      When using parallel prediction, do not pass the model path. It will be 
      automatically decided.
     :param outputsuffix: Text string to add to the output filenames
     :param batch_size: batch size (for use with normative_parallel)
     :param job_id: batch id
     :param fold: which cross-validation fold to use (default = 0)
     :param fold: list of model IDs to predict (if not specified all are computed)
+    :param return_y: return the (transformed) response variable (default = False)
 
     All outputs are written to disk in the same format as the input. These are:
 
     :outputs: * Yhat - predictive mean
               * S2 - predictive variance
               * Z - Z scores
+              * Y - response variable (if return_y is True)
     '''
     
     
     model_path = kwargs.pop('model_path', 'Models')
     job_id = kwargs.pop('job_id', None)
     batch_size = kwargs.pop('batch_size', None)
     outputsuffix = kwargs.pop('outputsuffix', 'predict')
     outputsuffix = "_" + outputsuffix.replace("_", "")
     inputsuffix = kwargs.pop('inputsuffix', 'estimate')
     inputsuffix = "_" + inputsuffix.replace("_", "")
     alg = kwargs.pop('alg')
     fold = kwargs.pop('fold',0)
     models = kwargs.pop('models', None)
+    return_y = kwargs.pop('return_y', False)
     
     if alg == 'gpr':
         raise(ValueError, "gpr is not supported with predict()")
         
     if respfile is not None and not os.path.exists(respfile):
         print("Response file does not exist. Only returning predictions")
         respfile = None
@@ -812,18 +817,23 @@
             
             results = evaluate(Y, Yhat, S2=S2, mY=mY, sY=sY)
         else:    
             results = evaluate(Y, Yhat, S2=S2, 
                            metrics = ['Rho', 'RMSE', 'SMSE', 'EXPV'])
         
         print("Evaluations Writing outputs ...")
-        save_results(respfile, Yhat, S2, maskvol, Z=Z, 
-                     outputsuffix=outputsuffix, results=results)
         
-        return (Yhat, S2, Z)
+        if return_y:
+            save_results(respfile, Yhat, S2, maskvol, Z=Z, Y=Y,
+                     outputsuffix=outputsuffix, results=results)
+            return (Yhat, S2, Z, Y)
+        else:
+            save_results(respfile, Yhat, S2, maskvol, Z=Z, 
+                     outputsuffix=outputsuffix, results=results)
+            return (Yhat, S2, Z)
 
     
 def transfer(covfile, respfile, testcov=None, testresp=None, maskfile=None, 
              **kwargs):
     '''
     Transfer learning on the basis of a pre-estimated normative model by using 
     the posterior distribution over the parameters as an informed prior for 
@@ -1433,8 +1443,8 @@
     all_args = ', '.join(pos_args + kw_args)
 
     # Executing the target function
     exec(func + '(' + all_args + ')')
 
 # For running from the command line:
 if __name__ == "__main__":
-    main(sys.argv[1:])
+    main(sys.argv[1:])
```

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_NP.py` & `pcntoolkit-0.28/pcntoolkit/normative_NP.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_base.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_base.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_blr.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_blr.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_gpr.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_gpr.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_hbr.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_hbr.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,20 +5,26 @@
 
 @author: seykia
 @author: augub
 """
 
 from __future__ import print_function
 from __future__ import division
+from sys import exit
 
+from itertools import product
 
 import os
 import warnings
 import sys
+
+import xarray
+import arviz as az
 import numpy as np
+from scipy import special as spp
 from ast import literal_eval as make_tuple
 
 try:
     from pcntoolkit.dataio import fileio
     from pcntoolkit.normative_model.norm_base import NormBase
     from pcntoolkit.model.hbr import HBR
 except ImportError:
@@ -30,298 +36,589 @@
     del path
     import dataio.fileio as fileio
     from model.hbr import HBR
     from norm_base import NormBase
 
 
 class NormHBR(NormBase):
-        
-    """ HBR multi-batch normative modelling class. By default, this function 
-    estimates a linear model with random intercept, random slope, and random 
+
+    """HBR multi-batch normative modelling class. By default, this function
+    estimates a linear model with random intercept, random slope, and random
     homoscedastic noise.
-    
+
     :param X: [N×P] array of clinical covariates
     :param y: [N×1] array of neuroimaging measures
     :param trbefile: the address to the batch effects file for the training set.
         the batch effect array should be a [N×M] array where M is the number of
         the type of batch effects. For example when the site and gender is modeled
-        as batch effects M=2. Each column in the batch effect array contains the 
+        as batch effects M=2. Each column in the batch effect array contains the
         batch ID (starting from 0) for each sample. If not specified (default=None)
-        then all samples assumed to be from the same batch (i.e., the batch effect 
+        then all samples assumed to be from the same batch (i.e., the batch effect
                                                             is not modelled).
     :param tsbefile: Similar to trbefile for the test set.
     :param model_type: Specifies the type of the model from 'linear', 'plynomial',
         and 'bspline' (defauls is 'linear').
     :param likelihood: specifies the type of likelihood among 'Normal' 'SHASHb','SHASHo',
         and 'SHASHo2' (defauls is normal).
     :param linear_mu: Boolean (default='True') to decide whether the mean (mu) is
         parametrized on a linear function (thus changes with covariates) or it is fixed.
     :param linear_sigma: Boolean (default='False') to decide whether the variance (sigma) is
         parametrized on a linear function (heteroscedastic noise) or it is fixed for
         each batch (homoscedastic noise).
     :param linear_epsilon: Boolean (default='False') to decide the parametrization
-        of epsilon for the SHASH likelihood that controls its skewness. 
-        If True, epsilon is  parametrized on a linear function 
+        of epsilon for the SHASH likelihood that controls its skewness.
+        If True, epsilon is  parametrized on a linear function
         (thus changes with covariates) otherwise it is fixed for each batch.
     :param linear_delta: Boolean (default='False') to decide the parametrization
-        of delta for the SHASH likelihood that controls its kurtosis. 
-        If True, delta is  parametrized on a linear function 
+        of delta for the SHASH likelihood that controls its kurtosis.
+        If True, delta is  parametrized on a linear function
         (thus changes with covariates) otherwise it is fixed for each batch.
-    :param random_intercept_{parameter}: if parameters mu (default='True'), 
+    :param random_intercept_{parameter}: if parameters mu (default='True'),
         sigma (default='False'), epsilon (default='False'), and delta (default='False')
-        are parametrized on a linear function, then this boolean decides 
+        are parametrized on a linear function, then this boolean decides
         whether the intercept can vary across batches.
-    :param random_slope_{parameter}: if parameters mu (default='True'), 
+    :param random_slope_{parameter}: if parameters mu (default='True'),
         sigma (default='False'), epsilon (default='False'), and delta (default='False')
-        are parametrized on a linear function, then this boolean decides 
+        are parametrized on a linear function, then this boolean decides
         whether the slope can vary across batches.
-    :param centered_intercept_{parameter}: if parameters mu (default='False'), 
+    :param centered_intercept_{parameter}: if parameters mu (default='False'),
         sigma (default='False'), epsilon (default='False'), and delta (default='False')
-        are parametrized on a linear function, then this boolean decides 
+        are parametrized on a linear function, then this boolean decides
         whether the parameters of intercept are estimated in a centered or
         non-centered manner (default). While centered estimation runs faster
         it may cause some problems for the sampler (the funnel of hell).
-    :param centered_slope_{parameter}: if parameters mu (default='False'), 
+    :param centered_slope_{parameter}: if parameters mu (default='False'),
         sigma (default='False'), epsilon (default='False'), and delta (default='False')
-        are parametrized on a linear function, then this boolean decides 
+        are parametrized on a linear function, then this boolean decides
         whether the parameters of slope are estimated in a centered or
         non-centered manner (default). While centered estimation runs faster
         it may cause some problems for the sampler (the funnel of hell).
     :param sampler: specifies the type of PyMC sampler (Defauls is 'NUTS').
-    :param n_samples: The number of samples to draw (Default is '1000'). Please 
-        note that this parameter must be specified in a string fromat ('1000' and 
-                                                                       not 1000).  
-    :param n_tuning: String that specifies the number of iterations to adjust 
+    :param n_samples: The number of samples to draw (Default is '1000'). Please
+        note that this parameter must be specified in a string fromat ('1000' and
+                                                                       not 1000).
+    :param n_tuning: String that specifies the number of iterations to adjust
         the samplers's step sizes, scalings or similar (defauls is '500').
-    :param n_chains: String that specifies the number of chains to sample. Defauls 
-        is '1' for faster estimation, but note that sampling independent chains 
+    :param n_chains: String that specifies the number of chains to sample. Defauls
+        is '1' for faster estimation, but note that sampling independent chains
         is important for some convergence checks.
     :param cores: String that specifies the number of chains to run in parallel.
         (defauls is '1').
     :param Initialization method to use for auto-assigned NUTS samplers. The
-        defauls is 'jitter+adapt_diag' that starts with a identity mass matrix 
+        defauls is 'jitter+adapt_diag' that starts with a identity mass matrix
         and then adapt a diagonal based on the variance of the tuning samples
         while adding a uniform jitter in [-1, 1] to the starting point in each chain.
-    :param target_accept: String that of a float in [0, 1] that regulates the 
+    :param target_accept: String that of a float in [0, 1] that regulates the
         step size such that we approximate this acceptance rate. The defauls is '0.8'
         but higher values like 0.9 or 0.95 often work better for problematic posteriors.
     :param order: String that defines the order of bspline or polynomial model.
         The defauls is '3'.
     :param nknots: String that defines the numbers of knots for the bspline model.
-        The defauls is '5'. Higher values increase the model complexity with negative 
+        The defauls is '5'. Higher values increase the model complexity with negative
         effect on the spped of estimations.
     :param nn_hidden_layers_num: String the specifies the number of hidden layers
         in neural network model. It can be either '1' or '2'. The default is set to '2'.
-    :param nn_hidden_neuron_num: String that specifies the number of neurons in 
+    :param nn_hidden_neuron_num: String that specifies the number of neurons in
         the hidden layers. The defauls is set to  '2'.
-        
+
     Written by S.de Boer and S.M. Kia
-    
+
     """
 
     def __init__(self, **kwargs):
-
         self.configs = dict()
         # inputs
-        self.configs['trbefile'] = kwargs.pop('trbefile', None)
-        self.configs['tsbefile'] = kwargs.pop('tsbefile', None)
+        self.configs["trbefile"] = kwargs.get("trbefile", None)
+        self.configs["tsbefile"] = kwargs.get("tsbefile", None)
         # Model settings
-        self.configs['type'] = kwargs.pop('model_type', 'linear')
-        self.configs['random_noise'] = kwargs.pop('random_noise', 'True') == 'True'
-        self.configs['likelihood'] = kwargs.pop('likelihood', 'Normal')
+        self.configs["type"] = kwargs.get("model_type", "linear")
+        self.configs["random_noise"] = kwargs.get("random_noise", "True") == "True"
+        self.configs["likelihood"] = kwargs.get("likelihood", "Normal")
         # sampler settings
-        self.configs['n_samples'] = int(kwargs.pop('n_samples', '1000'))
-        self.configs['n_tuning'] = int(kwargs.pop('n_tuning', '500'))
-        self.configs['n_chains'] = int(kwargs.pop('n_chains', '1'))
-        self.configs['sampler'] = kwargs.pop('sampler', 'NUTS')
-        self.configs['target_accept'] = float(kwargs.pop('target_accept', '0.8'))
-        self.configs['init'] = kwargs.pop('init', 'jitter+adapt_diag')
-        self.configs['cores'] = int(kwargs.pop('cores', '1'))
+        self.configs["n_samples"] = int(kwargs.get("n_samples", "1000"))
+        self.configs["n_tuning"] = int(kwargs.get("n_tuning", "500"))
+        self.configs["n_chains"] = int(kwargs.get("n_chains", "1"))
+        self.configs["sampler"] = kwargs.get("sampler", "NUTS")
+        self.configs["target_accept"] = float(kwargs.get("target_accept", "0.8"))
+        self.configs["init"] = kwargs.get("init", "jitter+adapt_diag")
+        self.configs["cores"] = int(kwargs.get("cores", "1"))
+        self.configs["remove_datapoints_from_posterior"] = kwargs.get("remove_datapoints_from_posterior","True") == "True"
         # model transfer setting
-        self.configs['freedom'] = int(kwargs.pop('freedom', '1'))
-        self.configs['transferred'] = False
+        self.configs["freedom"] = int(kwargs.get("freedom", "1"))
+        self.configs["transferred"] = False
         # deprecated settings
-        self.configs['skewed_likelihood'] = kwargs.pop('skewed_likelihood', 'False') == 'True'
+        self.configs["skewed_likelihood"] = (
+            kwargs.get("skewed_likelihood", "False") == "True"
+        )
         # misc
-        self.configs['pred_type'] = kwargs.pop('pred_type', 'single')
+        self.configs["pred_type"] = kwargs.get("pred_type", "single")
 
-        if self.configs['type'] == 'bspline':
-            self.configs['order'] = int(kwargs.pop('order', '3'))
-            self.configs['nknots'] = int(kwargs.pop('nknots', '5'))
-        elif self.configs['type'] == 'polynomial':
-            self.configs['order'] = int(kwargs.pop('order', '3'))
-        elif self.configs['type'] == 'nn':
-            self.configs['nn_hidden_neuron_num'] = int(kwargs.pop('nn_hidden_neuron_num', '2'))
-            self.configs['nn_hidden_layers_num'] = int(kwargs.pop('nn_hidden_layers_num', '2'))
-            if self.configs['nn_hidden_layers_num'] > 2:
-                raise ValueError("Using " + str(self.configs['nn_hidden_layers_num']) \
-                                 + " layers was not implemented. The number of " \
-                                 + " layers has to be less than 3.")
-        elif self.configs['type'] == 'linear':
+        if self.configs["type"] == "bspline":
+            self.configs["order"] = int(kwargs.get("order", "3"))
+            self.configs["nknots"] = int(kwargs.get("nknots", "5"))
+        elif self.configs["type"] == "polynomial":
+            self.configs["order"] = int(kwargs.get("order", "3"))
+        elif self.configs["type"] == "nn":
+            self.configs["nn_hidden_neuron_num"] = int(
+                kwargs.get("nn_hidden_neuron_num", "2")
+            )
+            self.configs["nn_hidden_layers_num"] = int(
+                kwargs.get("nn_hidden_layers_num", "2")
+            )
+            if self.configs["nn_hidden_layers_num"] > 2:
+                raise ValueError(
+                    "Using "
+                    + str(self.configs["nn_hidden_layers_num"])
+                    + " layers was not implemented. The number of "
+                    + " layers has to be less than 3."
+                )
+        elif self.configs["type"] == "linear":
             pass
         else:
-            raise ValueError("Unknown model type, please specify from 'linear', \
-                             'polynomial', 'bspline', or 'nn'.")
-
-        if self.configs['type'] in ['bspline', 'polynomial', 'linear']:
-
-            for p in ['mu', 'sigma', 'epsilon', 'delta']:
-                self.configs[f'linear_{p}'] = kwargs.pop(f'linear_{p}', 'False') == 'True'
+            raise ValueError(
+                "Unknown model type, please specify from 'linear', \
+                             'polynomial', 'bspline', or 'nn'."
+            )
+
+        if self.configs["type"] in ["bspline", "polynomial", "linear"]:
+            for p in ["mu", "sigma", "epsilon", "delta"]:
+                self.configs[f"linear_{p}"] = (
+                    kwargs.get(f"linear_{p}", "False") == "True"
+                )
 
                 ######## Deprecations (remove in later version)
-                if f'{p}_linear' in kwargs.keys():
-                    print(f'The keyword \'{p}_linear\' is deprecated. It is now automatically replaced with \'linear_{p}\'')
-                    self.configs[f'linear_{p}'] = kwargs.pop(f'{p}_linear', 'False') == 'True'
-                ##### End Deprecations 
-
-                for c in ['centered','random']:
-                    self.configs[f'{c}_{p}'] = kwargs.pop(f'{c}_{p}', 'False') == 'True'
-                    for sp in ['slope','intercept']:
-                        self.configs[f'{c}_{sp}_{p}'] = kwargs.pop(f'{c}_{sp}_{p}', 'False') == 'True'
+                if f"{p}_linear" in kwargs.keys():
+                    print(
+                        f"The keyword '{p}_linear' is deprecated. It is now automatically replaced with 'linear_{p}'"
+                    )
+                    self.configs[f"linear_{p}"] = (
+                        kwargs.get(f"{p}_linear", "False") == "True"
+                    )
+                ##### End Deprecations
+
+                for c in ["centered", "random"]:
+                    self.configs[f"{c}_{p}"] = kwargs.get(f"{c}_{p}", "False") == "True"
+                    for sp in ["slope", "intercept"]:
+                        self.configs[f"{c}_{sp}_{p}"] = (
+                            kwargs.get(f"{c}_{sp}_{p}", "False") == "True"
+                        )
 
             ######## Deprecations (remove in later version)
-            if self.configs['linear_sigma']:
-                if 'random_noise' in kwargs.keys():
-                    print("The keyword \'random_noise\' is deprecated. It is now automatically replaced with \'random_intercept_sigma\', because sigma is linear")
-                    self.configs['random_intercept_sigma'] = kwargs.pop('random_noise','True') == 'True'
-            elif 'random_noise' in kwargs.keys():
-                print("The keyword \'random_noise\' is deprecated. It is now automatically replaced with \'random_sigma\', because sigma is fixed")
-                self.configs['random_sigma'] = kwargs.pop('random_noise','True') == 'True'
-            if 'random_slope' in kwargs.keys():
-                print("The keyword \'random_slope\' is deprecated. It is now automatically replaced with \'random_intercept_mu\'")
-                self.configs['random_slope_mu'] = kwargs.pop('random_slope','True') == 'True'
-            ##### End Deprecations 
-
+            if self.configs["linear_sigma"]:
+                if "random_noise" in kwargs.keys():
+                    print(
+                        "The keyword 'random_noise' is deprecated. It is now automatically replaced with 'random_intercept_sigma', because sigma is linear"
+                    )
+                    self.configs["random_intercept_sigma"] = (
+                        kwargs.get("random_noise", "True") == "True"
+                    )
+            elif "random_noise" in kwargs.keys():
+                print(
+                    "The keyword 'random_noise' is deprecated. It is now automatically replaced with 'random_sigma', because sigma is fixed"
+                )
+                self.configs["random_sigma"] = (
+                    kwargs.get("random_noise", "True") == "True"
+                )
+            if "random_slope" in kwargs.keys():
+                print(
+                    "The keyword 'random_slope' is deprecated. It is now automatically replaced with 'random_intercept_mu'"
+                )
+                self.configs["random_slope_mu"] = (
+                    kwargs.get("random_slope", "True") == "True"
+                )
+            ##### End Deprecations
 
         ## Default parameters
-        self.configs['linear_mu'] = kwargs.pop('linear_mu','True') == 'True'
-        self.configs['random_mu'] = kwargs.pop('random_mu','True') == 'True'
-        self.configs['random_intercept_mu'] = kwargs.pop('random_intercept_mu','True') == 'True'
-        self.configs['random_slope_mu'] = kwargs.pop('random_slope_mu','True') == 'True'
-        self.configs['random_sigma'] = kwargs.pop('random_sigma','True') == 'True'
-        self.configs['centered_sigma'] = kwargs.pop('centered_sigma','True') == 'True'
+        self.configs["linear_mu"] = kwargs.get("linear_mu", "True") == "True"
+        self.configs["random_mu"] = kwargs.get("random_mu", "True") == "True"
+        self.configs["random_intercept_mu"] = (
+            kwargs.get("random_intercept_mu", "True") == "True"
+        )
+        self.configs["random_slope_mu"] = (
+            kwargs.get("random_slope_mu", "True") == "True"
+        )
+        self.configs["random_sigma"] = kwargs.get("random_sigma", "True") == "True"
+        self.configs["centered_sigma"] = kwargs.get("centered_sigma", "True") == "True"
         ## End default parameters
 
         self.hbr = HBR(self.configs)
 
     @property
     def n_params(self):
         return 1
 
     @property
     def neg_log_lik(self):
         return -1
 
     def estimate(self, X, y, **kwargs):
-
-        trbefile = kwargs.pop('trbefile', None)
+        trbefile = kwargs.get("trbefile", None)
         if trbefile is not None:
             batch_effects_train = fileio.load(trbefile)
         else:
-            print('Could not find batch-effects file! Initilizing all as zeros ...')
+            print("Could not find batch-effects file! Initilizing all as zeros ...")
             batch_effects_train = np.zeros([X.shape[0], 1])
 
+        self.batch_effects_maps = [
+            {v: i for i, v in enumerate(np.unique(batch_effects_train[:, j]))}
+            for j in range(batch_effects_train.shape[1])
+        ]
+
         self.hbr.estimate(X, y, batch_effects_train)
 
         return self
 
     def predict(self, Xs, X=None, Y=None, **kwargs):
-
-        tsbefile = kwargs.pop('tsbefile', None)
+        tsbefile = kwargs.get("tsbefile", None)
         if tsbefile is not None:
             batch_effects_test = fileio.load(tsbefile)
         else:
-            print('Could not find batch-effects file! Initilizing all as zeros ...')
+            print("Could not find batch-effects file! Initilizing all as zeros ...")
             batch_effects_test = np.zeros([Xs.shape[0], 1])
 
-        pred_type = self.configs['pred_type']
+        pred_type = self.configs["pred_type"]
 
-        if self.configs['transferred'] == False:
-            yhat, s2 = self.hbr.predict(Xs, batch_effects_test, pred=pred_type)
+        if self.configs["transferred"] == False:
+            yhat, s2 = self.hbr.predict(
+                X=Xs,
+                batch_effects=batch_effects_test,
+                batch_effects_maps=self.batch_effects_maps,
+                pred=pred_type,
+                **kwargs,
+            )
         else:
-            raise ValueError("This is a transferred model. Please use predict_on_new_sites function.")
+            raise ValueError(
+                "This is a transferred model. Please use predict_on_new_sites function."
+            )
 
         return yhat.squeeze(), s2.squeeze()
 
+    
+
     def estimate_on_new_sites(self, X, y, batch_effects):
         self.hbr.estimate_on_new_site(X, y, batch_effects)
-        self.configs['transferred'] = True
+        self.configs["transferred"] = True
         return self
 
     def predict_on_new_sites(self, X, batch_effects):
-
         yhat, s2 = self.hbr.predict_on_new_site(X, batch_effects)
         return yhat, s2
 
-    def extend(self, X, y, batch_effects, X_dummy_ranges=[[0.1, 0.9, 0.01]],
-               merge_batch_dim=0, samples=10, informative_prior=False):
-
+    def extend(
+        self,
+        X,
+        y,
+        batch_effects,
+        X_dummy_ranges=[[0.1, 0.9, 0.01]],
+        merge_batch_dim=0,
+        samples=10,
+        informative_prior=False,
+    ):
         X_dummy, batch_effects_dummy = self.hbr.create_dummy_inputs(X_dummy_ranges)
 
-        X_dummy, batch_effects_dummy, Y_dummy = self.hbr.generate(X_dummy,
-                                                                  batch_effects_dummy, samples)
-
-        batch_effects[:, merge_batch_dim] = batch_effects[:, merge_batch_dim] + \
-                                            np.max(batch_effects_dummy[:, merge_batch_dim]) + 1
+        X_dummy, batch_effects_dummy, Y_dummy = self.hbr.generate(
+            X_dummy, batch_effects_dummy, samples
+        )
+
+        batch_effects[:, merge_batch_dim] = (
+            batch_effects[:, merge_batch_dim]
+            + np.max(batch_effects_dummy[:, merge_batch_dim])
+            + 1
+        )
 
         if informative_prior:
-            self.hbr.adapt(np.concatenate((X_dummy, X)),
-                           np.concatenate((Y_dummy, y)),
-                           np.concatenate((batch_effects_dummy, batch_effects)))
+            self.hbr.adapt(
+                np.concatenate((X_dummy, X)),
+                np.concatenate((Y_dummy, y)),
+                np.concatenate((batch_effects_dummy, batch_effects)),
+            )
         else:
-            self.hbr.estimate(np.concatenate((X_dummy, X)),
-                              np.concatenate((Y_dummy, y)),
-                              np.concatenate((batch_effects_dummy, batch_effects)))
+            self.hbr.estimate(
+                np.concatenate((X_dummy, X)),
+                np.concatenate((Y_dummy, y)),
+                np.concatenate((batch_effects_dummy, batch_effects)),
+            )
 
         return self
 
-    def tune(self, X, y, batch_effects, X_dummy_ranges=[[0.1, 0.9, 0.01]],
-             merge_batch_dim=0, samples=10, informative_prior=False):
-
+    def tune(
+        self,
+        X,
+        y,
+        batch_effects,
+        X_dummy_ranges=[[0.1, 0.9, 0.01]],
+        merge_batch_dim=0,
+        samples=10,
+        informative_prior=False,
+    ):
         tune_ids = list(np.unique(batch_effects[:, merge_batch_dim]))
 
         X_dummy, batch_effects_dummy = self.hbr.create_dummy_inputs(X_dummy_ranges)
 
         for idx in tune_ids:
             X_dummy = X_dummy[batch_effects_dummy[:, merge_batch_dim] != idx, :]
-            batch_effects_dummy = batch_effects_dummy[batch_effects_dummy[:, merge_batch_dim] != idx, :]
-
-        X_dummy, batch_effects_dummy, Y_dummy = self.hbr.generate(X_dummy,
-                                                                  batch_effects_dummy, samples)
+            batch_effects_dummy = batch_effects_dummy[
+                batch_effects_dummy[:, merge_batch_dim] != idx, :
+            ]
+
+        X_dummy, batch_effects_dummy, Y_dummy = self.hbr.generate(
+            X_dummy, batch_effects_dummy, samples
+        )
 
         if informative_prior:
-            self.hbr.adapt(np.concatenate((X_dummy, X)),
-                           np.concatenate((Y_dummy, y)),
-                           np.concatenate((batch_effects_dummy, batch_effects)))
+            self.hbr.adapt(
+                np.concatenate((X_dummy, X)),
+                np.concatenate((Y_dummy, y)),
+                np.concatenate((batch_effects_dummy, batch_effects)),
+            )
         else:
-            self.hbr.estimate(np.concatenate((X_dummy, X)),
-                              np.concatenate((Y_dummy, y)),
-                              np.concatenate((batch_effects_dummy, batch_effects)))
+            self.hbr.estimate(
+                np.concatenate((X_dummy, X)),
+                np.concatenate((Y_dummy, y)),
+                np.concatenate((batch_effects_dummy, batch_effects)),
+            )
 
         return self
 
-    def merge(self, nm, X_dummy_ranges=[[0.1, 0.9, 0.01]], merge_batch_dim=0,
-              samples=10):
-
+    def merge(
+        self, nm, X_dummy_ranges=[[0.1, 0.9, 0.01]], merge_batch_dim=0, samples=10
+    ):
         X_dummy1, batch_effects_dummy1 = self.hbr.create_dummy_inputs(X_dummy_ranges)
         X_dummy2, batch_effects_dummy2 = nm.hbr.create_dummy_inputs(X_dummy_ranges)
 
-        X_dummy1, batch_effects_dummy1, Y_dummy1 = self.hbr.generate(X_dummy1,
-                                                                     batch_effects_dummy1, samples)
-        X_dummy2, batch_effects_dummy2, Y_dummy2 = nm.hbr.generate(X_dummy2,
-                                                                   batch_effects_dummy2, samples)
-
-        batch_effects_dummy2[:, merge_batch_dim] = batch_effects_dummy2[:, merge_batch_dim] + \
-                                                   np.max(batch_effects_dummy1[:, merge_batch_dim]) + 1
-
-        self.hbr.estimate(np.concatenate((X_dummy1, X_dummy2)),
-                          np.concatenate((Y_dummy1, Y_dummy2)),
-                          np.concatenate((batch_effects_dummy1,
-                                          batch_effects_dummy2)))
+        X_dummy1, batch_effects_dummy1, Y_dummy1 = self.hbr.generate(
+            X_dummy1, batch_effects_dummy1, samples
+        )
+        X_dummy2, batch_effects_dummy2, Y_dummy2 = nm.hbr.generate(
+            X_dummy2, batch_effects_dummy2, samples
+        )
+
+        batch_effects_dummy2[:, merge_batch_dim] = (
+            batch_effects_dummy2[:, merge_batch_dim]
+            + np.max(batch_effects_dummy1[:, merge_batch_dim])
+            + 1
+        )
+
+        self.hbr.estimate(
+            np.concatenate((X_dummy1, X_dummy2)),
+            np.concatenate((Y_dummy1, Y_dummy2)),
+            np.concatenate((batch_effects_dummy1, batch_effects_dummy2)),
+        )
 
         return self
 
     def generate(self, X, batch_effects, samples=10):
-
-        X, batch_effects, generated_samples = self.hbr.generate(X, batch_effects,
-                                                                samples)
+        X, batch_effects, generated_samples = self.hbr.generate(
+            X, batch_effects, samples
+        )
         return X, batch_effects, generated_samples
+        
+    def get_mcmc_quantiles(self, X, batch_effects=None, z_scores=None):
+
+        """
+        Computes quantiles of an estimated normative model.
+
+        Args:
+            X ([N*p]ndarray): covariates for which the quantiles are computed (must be scaled if scaler is set)
+            batch_effects (ndarray): the batch effects corresponding to X
+            z_scores (ndarray): Use this to determine which quantiles will be computed. The resulting quantiles will have the z-scores given in this list. 
+        """
+        # Set batch effects to zero if none are provided
+        if batch_effects is None:
+            batch_effects = batch_effects_test = np.zeros([X.shape[0], 1])
+            
+
+        # Set the z_scores for which the quantiles are computed
+        if z_scores is None:
+            z_scores = np.arange(-3, 4)
+        likelihood=self.configs['likelihood']
+
+        # Determine the variables to predict
+        if self.configs["likelihood"] == "Normal":
+            var_names = ["mu_samples", "sigma_plus_samples"]
+        elif self.configs["likelihood"].startswith("SHASH"):
+            var_names = [
+                "mu_samples",
+                "sigma_plus_samples",
+                "epsilon_samples",
+                "delta_plus_samples",
+            ]
+        else:
+            exit("Unknown likelihood: " + self.configs["likelihood"])
+
+        # Delete the posterior predictive if it already exists
+        if 'posterior_predictive' in self.hbr.idata.groups():
+            del self.hbr.idata.posterior_predictive
+            
+        # Do a forward to get the posterior predictive in the idata
+        self.hbr.predict(
+            X=X,
+            batch_effects=batch_effects,
+            batch_effects_maps=self.batch_effects_maps,
+            pred="single",
+            var_names=var_names+["y_like"],
+        )
+
+        # Extract the relevant samples from the idata
+        post_pred = az.extract(
+            self.hbr.idata, "posterior_predictive", var_names=var_names
+        )
+
+        # Separate the samples into a list so that they can be unpacked 
+        array_of_vars = list(map(lambda x: post_pred[x], var_names))
+
+        # Create an array to hold the quantiles
+        len_synth_data, n_mcmc_samples = post_pred["mu_samples"].shape
+        quantiles = np.zeros((z_scores.shape[0], len_synth_data, n_mcmc_samples))
+
+        # Compute the quantile iteratively for each z-score
+        for i, j in enumerate(z_scores):
+            zs = np.full((len_synth_data, n_mcmc_samples), j, dtype=float)
+            quantiles[i] = xarray.apply_ufunc(
+                quantile,
+                *array_of_vars,
+                kwargs={"zs": zs, "likelihood":  self.configs['likelihood']},
+            )
+        return quantiles.mean(axis=-1)
+    
+
+    def get_mcmc_zscores(self, X, y, batch_effects=None):
+
+        """
+        Computes zscores of data given an estimated model
+
+        Args:
+            X ([N*p]ndarray): covariates
+            y ([N*1]ndarray): response variables
+            batch_effects (ndarray): the batch effects corresponding to X
+        """
+        # Set batch effects to zero if none are provided
+        print(self.configs['likelihood'])
+        if batch_effects is None:
+            batch_effects = batch_effects_test = np.zeros([X.shape[0], 1])
+            
+        # Determine the variables to predict
+        if self.configs["likelihood"] == "Normal":
+            var_names = ["mu_samples", "sigma_plus_samples"]
+        elif self.configs["likelihood"].startswith("SHASH"):
+            var_names = [
+                "mu_samples",
+                "sigma_plus_samples",
+                "epsilon_samples",
+                "delta_plus_samples",
+            ]
+        else:
+            exit("Unknown likelihood: " + self.configs["likelihood"])
+
+        # Delete the posterior predictive if it already exists
+        if 'posterior_predictive' in self.hbr.idata.groups():
+            del self.hbr.idata.posterior_predictive
+            
+        # Do a forward to get the posterior predictive in the idata
+        self.hbr.predict(
+            X=X,
+            batch_effects=batch_effects,
+            batch_effects_maps=self.batch_effects_maps,
+            pred="single",
+            var_names=var_names+["y_like"],
+        )
+
+        # Extract the relevant samples from the idata
+        post_pred = az.extract(
+            self.hbr.idata, "posterior_predictive", var_names=var_names
+        )
+
+        # Separate the samples into a list so that they can be unpacked 
+        array_of_vars = list(map(lambda x: post_pred[x], var_names))
+
+        # Create an array to hold the quantiles
+        len_data, n_mcmc_samples = post_pred["mu_samples"].shape
+
+        # Compute the quantile iteratively for each z-score
+        z_scores =  xarray.apply_ufunc(
+            z_score,
+            *array_of_vars,
+            kwargs={"y": y, "likelihood": self.configs['likelihood']},
+        )
+        return z_scores.mean(axis=-1)
+    
+    
+
+def S_inv(x, e, d):
+    return np.sinh((np.arcsinh(x) + e) / d)
+
+def K(p, x):
+    """
+    Computes the values of spp.kv(p,x) for only the unique values of p
+    """
+
+    ps, idxs = np.unique(p, return_inverse=True)
+    return spp.kv(ps, x)[idxs].reshape(p.shape)
+
+def P(q):
+    """
+    The P function as given in Jones et al.
+    :param q:
+    :return:
+    """
+    frac = np.exp(1 / 4) / np.sqrt(8 * np.pi)
+    K1 = K((q + 1) / 2, 1 / 4)
+    K2 = K((q - 1) / 2, 1 / 4)
+    a = (K1 + K2) * frac
+    return a
+
+def m(epsilon, delta, r):
+    """
+    The r'th uncentered moment. Given by Jones et al.
+    """
+    frac1 = 1 / np.power(2, r)
+    acc = 0
+    for i in range(r + 1):
+        combs = spp.comb(r, i)
+        flip = np.power(-1, i)
+        ex = np.exp((r - 2 * i) * epsilon / delta)
+        p = P((r - 2 * i) / delta)
+        acc += combs * flip * ex * p
+    return frac1 * acc
+
+def quantile( mu, sigma, epsilon=None, delta=None, zs=0, likelihood = "Normal"):
+    """Get the zs'th quantiles given likelihood parameters"""
+    if likelihood.startswith('SHASH'):
+        if likelihood == "SHASHo":
+            quantiles = S_inv(zs,epsilon,delta)*sigma + mu
+        elif likelihood == "SHASHo2":
+            sigma_d = sigma/delta
+            quantiles = S_inv(zs,epsilon,delta)*sigma_d + mu
+        elif likelihood == "SHASHb":
+            true_mu = m(epsilon, delta, 1)
+            true_sigma = np.sqrt((m(epsilon, delta, 2) - true_mu ** 2))
+            SHASH_c = ((S_inv(zs,epsilon,delta)-true_mu)/true_sigma)
+            quantiles = SHASH_c *sigma + mu
+    elif likelihood == 'Normal':
+        quantiles = zs*sigma + mu
+    else:
+        exit("Unsupported likelihood")
+    return quantiles
+
+    
+def z_score(mu, sigma, epsilon=None, delta=None, y=None, likelihood = "Normal"):
+    """Get the z-scores of Y, given likelihood parameters"""
+    if likelihood.startswith('SHASH'):
+        if likelihood == "SHASHo":
+            SHASH = (y-mu)/sigma
+            Z = np.sinh(np.arcsinh(SHASH)*delta - epsilon)
+        elif likelihood == "SHASHo2":
+            sigma_d = sigma/delta
+            SHASH = (y-mu)/sigma_d
+            Z = np.sinh(np.arcsinh(SHASH)*delta - epsilon)
+        elif likelihood == "SHASHb":
+            true_mu = m(epsilon, delta, 1)
+            true_sigma = np.sqrt((m(epsilon, delta, 2) - true_mu ** 2))
+            SHASH_c = ((y-mu)/sigma)
+            SHASH = SHASH_c * true_sigma + true_mu
+            Z = np.sinh(np.arcsinh(SHASH) * delta - epsilon)
+    elif likelihood == 'Normal':
+        Z = (y-mu)/sigma
+    else:
+        exit("Unsupported likelihood")
+    return Z
+
```

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_np.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_np.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_rfa.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_rfa.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_model/norm_utils.py` & `pcntoolkit-0.28/pcntoolkit/normative_model/norm_utils.py`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/pcntoolkit/normative_parallel.py` & `pcntoolkit-0.28/pcntoolkit/normative_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -912,15 +912,15 @@
 
     # writes bash file into processing dir
     with open(processing_dir+job_name, 'w') as bash_file:
         bash_file.writelines(bash_environment + output_changedir + \
                              job_call + ["\n"])
 
     # changes permissoins for bash.sh file
-    os.chmod(processing_dir + job_name, 0o700)
+    os.chmod(processing_dir + job_name, 0o770)
 
 
 def qsub_nm(job_path,
             log_path,
             memory,
             duration):
     
@@ -1117,15 +1117,15 @@
 
     # writes bash file into processing dir
     with open(processing_dir+job_name, 'w') as bash_file:
         bash_file.writelines(bash_environment + output_changedir + \
                              job_call + ["\n"] + [sbatch_exit])
 
     # changes permissoins for bash.sh file
-    os.chmod(processing_dir + job_name, 0o700)
+    os.chmod(processing_dir + job_name, 0o770)
 
 def sbatch_nm(job_path,
               log_path):
     
     '''This function submits a job.sh scipt to the torque custer using the qsub
     command.
```

### Comparing `pcntoolkit-0.27/pcntoolkit/trendsurf.py` & `pcntoolkit-0.28/pcntoolkit/trendsurf.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     if args.covfile is not None:
         raise(NotImplementedError, "Covariates not implemented yet.")
 
     return filename, maskfile, basis, args.a, args.o
 
 
 def estimate(filename, maskfile, basis, ard=False, outputall=False,
-             saveoutput=True):
+             saveoutput=True, **kwargs):
     """ Estimate a trend surface model
 
     This will estimate a trend surface model, independently for each subject.
     This is currently fit using a polynomial model of a specified degree.
     The models are estimated on the basis of data stored on disk in ascii or
     neuroimaging data formats (currently nifti only). Ascii data should be in
     tab or space delimited format with the number of voxels in rows and the
@@ -162,15 +162,18 @@
               * ys2 - predictive variance
               * trendcoeff - coefficients from the trend surface model
               * negloglik - Negative log marginal likelihood
               * hyp - hyperparameters
               * explainedvar - explained variance
               * rmse - standardised mean squared error
     """
-
+    
+    # parse arguments
+    optim = kwargs.get('optimizer', 'powell')
+    
     # load data
     print("Processing data in", filename)
     Y, X, mask = load_data(filename, maskfile)
     Y = np.round(10000*Y)/10000  # truncate precision to avoid numerical probs
     if len(Y.shape) == 1:
         Y = Y[:, np.newaxis]
     N = Y.shape[1]
@@ -200,15 +203,15 @@
     rmse = np.zeros(N)
     ev = np.zeros(N)
     m = np.zeros((N, Phi.shape[1]))
     bs2 = np.zeros((N, Phi.shape[1]))
     for i in range(0, N):
         print("Estimating model ", i+1, "of", N)
         breg = BLR()
-        hyp[i, :] = breg.estimate(hyp0, Phi, Yz[:, i])
+        hyp[i, :] = breg.estimate(hyp0, Phi, Yz[:, i], optimizer=optim)
         m[i, :] = breg.m
         nlZ[i] = breg.nlZ
 
         # compute extra measures (e.g. marginal variances)?
         if outputall:
             bs2[i] = np.sqrt(np.diag(np.linalg.inv(breg.A)))
```

### Comparing `pcntoolkit-0.27/pcntoolkit/util/hbr_utils.py` & `pcntoolkit-0.28/pcntoolkit/util/hbr_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import numpy as np
 from scipy import stats
 import scipy.special as spp
 import pickle
 import matplotlib.pyplot as plt
 import pandas as pd
-import pymc3 as pm
+import pymc as pm
 from pcntoolkit.model.SHASH import *
 from pcntoolkit.model.hbr import bspline_transform
 
 """
 @author: augub
 """
 
@@ -55,15 +55,15 @@
             Z = np.sinh(np.arcsinh(SHASH)*delta - epsilon)
         elif likelihood == "SHASHb":
             true_mu = m(epsilon, delta, 1)
             true_sigma = np.sqrt((m(epsilon, delta, 2) - true_mu ** 2))
             SHASH_c = ((Y-mu)/sigma)
             SHASH = SHASH_c * true_sigma + true_mu
             Z = np.sinh(np.arcsinh(SHASH) * delta - epsilon)
-    elif likelihood == 'Normal':
+    if likelihood == 'Normal':
         Z = (Y-params['mu'])/params['sigma']
     else:
         exit("Unsupported likelihood")
     return Z
 
 
 def get_MCMC_quantiles(synthetic_X, z_scores, model, be):
@@ -109,15 +109,15 @@
             sigma_d = sigma/delta
             quantiles = S_inv(zs,epsilon,delta)*sigma_d + mu
         elif likelihood == "SHASHb":
             true_mu = m(epsilon, delta, 1)
             true_sigma = np.sqrt((m(epsilon, delta, 2) - true_mu ** 2))
             SHASH_c = ((S_inv(zs,epsilon,delta)-true_mu)/true_sigma)
             quantiles = SHASH_c *sigma + mu
-    elif likelihood == 'Normal':
+    if likelihood == 'Normal':
         quantiles = zs*params['sigma'] + params['mu']
     else:
         exit("Unsupported likelihood")
     return quantiles
 
 
 def single_parameter_forward(X, Z, model, sample, p_name):
@@ -153,16 +153,16 @@
     # TODO think if this is the correct spot for this
     mapfuncs={'sigma': lambda x: np.log(1+np.exp(x)), 'delta':lambda x :np.log(1+np.exp(x)) + 0.3}
 
     likelihood = model.configs['likelihood']
 
     if likelihood == 'Normal':
         parameter_list = ['mu','sigma']
-    elif likelihood in ['SHASHb','SHASHo','SHASHo2']:
-        parameter_list = ['mu','sigma','epsilon','delta']
+    # elif likelihood in ['SHASHb','SHASHo','SHASHo2']:
+    #     parameter_list = ['mu','sigma','epsilon','delta']
     else:
         exit("Unsupported likelihood")
 
     for i in parameter_list:
         if not (i in mapfuncs.keys()):
             mapfuncs[i] = lambda x: x
```

### Comparing `pcntoolkit-0.27/pcntoolkit/util/utils.py` & `pcntoolkit-0.28/pcntoolkit/util/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from abc import ABCMeta, abstractmethod
 import pickle
 import matplotlib.pyplot as plt
 import pandas as pd
 import bspline
 from bspline import splinelab
 from sklearn.datasets import make_regression
-import pymc3 as pm
+import pymc as pm
 from io import StringIO
 import subprocess
 import re
 from sklearn.metrics import roc_auc_score
 import scipy.special as spp
 
 
@@ -1318,24 +1318,24 @@
 def get_package_versions():
     
     import platform
     versions = dict()
     versions['Python'] = platform.python_version()
     
     try: 
-        import theano
-        versions['Theano'] = theano.__version__
+        import pytensor
+        versions['pytensor'] = pytensor.__version__
     except:
-        versions['Theano'] = ''
+        versions['pytensor'] = ''
         
     try: 
-        import pymc3
-        versions['PyMC3'] = pymc3.__version__
+        import pymc
+        versions['PyMC'] = pymc.__version__
     except:
-        versions['PyMC3'] = ''
+        versions['PyMC'] = ''
         
     try: 
         import pcntoolkit
         versions['PCNtoolkit'] = pcntoolkit.__version__
     except:
         versions['PCNtoolkit'] = ''
         
@@ -1446,15 +1446,15 @@
         if reply[:1] == 'y':
             return True
         if reply[:1] == 'n':
             return False
 
 
 
-#====== This is stuff used for the SHASH distributions, but using numpy (not pymc or theano) ===
+#====== This is stuff used for the SHASH distributions, but using numpy (not pymc or pytensor) ===
 
 def K(p, x):
     return np.array(spp.kv(p, x))
 
 def P(q):
     """
     The P function as given in Jones et al.
```

### Comparing `pcntoolkit-0.27/pcntoolkit.egg-info/SOURCES.txt` & `pcntoolkit-0.28/pcntoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcntoolkit-0.27/setup.py` & `pcntoolkit-0.28/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(name='pcntoolkit',
-      version='0.27',
+      version='0.28',
       description='Predictive Clinical Neuroscience toolkit',
       url='http://github.com/amarquand/PCNtoolkit',
       author='Andre Marquand',
       author_email='andre.marquand@donders.ru.nl',
       license='GNU GPLv3',
       packages=find_packages(),
       install_requires=[
           'argparse',
           'nibabel>=2.5.1',
           'six',
           'scikit-learn', 
           'bspline',
           'matplotlib',
-          'numpy>=1.19.5,<1.23',
+          'numpy',
           'scipy>=1.3.2',
           'pandas>=0.25.3',
           'torch>=1.1.0', 
           'sphinx-tabs',
-          'pymc3>=3.8,<=3.9.3',
-          'theano==1.0.5',
-          'arviz==0.11.0'
+          'pymc>=5.1.0',
+          'arviz==0.13.0'
       ],
-      #python_requires='<3.10',
       zip_safe=False)
```

