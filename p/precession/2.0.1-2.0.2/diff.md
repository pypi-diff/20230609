# Comparing `tmp/precession-2.0.1.tar.gz` & `tmp/precession-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precession-2.0.1.tar", last modified: Sun Apr 23 18:52:59 2023, max compression
+gzip compressed data, was "precession-2.0.2.tar", last modified: Fri Jun  9 11:12:17 2023, max compression
```

## Comparing `precession-2.0.1.tar` & `precession-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-23 18:52:59.606385 precession-2.0.1/
--rw-r--r--   0 dgerosa    (501) staff       (20)     1071 2022-02-03 16:32:40.000000 precession-2.0.1/LICENSE
--rw-r--r--   0 dgerosa    (501) staff       (20)       24 2023-04-08 16:44:47.000000 precession-2.0.1/MANIFEST.in
--rw-r--r--   0 dgerosa    (501) staff       (20)      464 2023-04-23 18:52:59.605887 precession-2.0.1/PKG-INFO
--rw-r--r--   0 dgerosa    (501) staff       (20)     2755 2023-04-10 07:58:58.000000 precession-2.0.1/README.md
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-23 18:52:59.600202 precession-2.0.1/precession/
--rw-r--r--   0 dgerosa    (501) staff       (20)       54 2023-04-08 16:09:00.000000 precession-2.0.1/precession/__init__.py
--rw-r--r--   0 dgerosa    (501) staff       (20)      458 2023-04-23 18:52:19.000000 precession-2.0.1/precession/__version__.py
--rw-r--r--   0 dgerosa    (501) staff       (20)   226012 2023-04-23 18:52:21.000000 precession-2.0.1/precession/precession.py
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-23 18:52:59.604443 precession-2.0.1/precession.egg-info/
--rw-r--r--   0 dgerosa    (501) staff       (20)      464 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/PKG-INFO
--rw-r--r--   0 dgerosa    (501) staff       (20)      331 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/SOURCES.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/dependency_links.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-08 16:11:27.000000 precession-2.0.1/precession.egg-info/not-zip-safe
--rw-r--r--   0 dgerosa    (501) staff       (20)       19 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/requires.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       11 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/top_level.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       18 2023-04-10 07:39:31.000000 precession-2.0.1/requirements.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       38 2023-04-23 18:52:59.606560 precession-2.0.1/setup.cfg
--rw-r--r--   0 dgerosa    (501) staff       (20)      984 2023-04-10 13:12:57.000000 precession-2.0.1/setup.py
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-06-09 11:12:17.452373 precession-2.0.2/
+-rw-r--r--   0 dgerosa    (501) staff       (20)     1071 2022-02-03 16:32:40.000000 precession-2.0.2/LICENSE
+-rw-r--r--   0 dgerosa    (501) staff       (20)       24 2023-06-08 16:25:19.000000 precession-2.0.2/MANIFEST.in
+-rw-r--r--   0 dgerosa    (501) staff       (20)      464 2023-06-09 11:12:17.451963 precession-2.0.2/PKG-INFO
+-rw-r--r--   0 dgerosa    (501) staff       (20)     2755 2023-06-09 10:21:50.000000 precession-2.0.2/README.md
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-06-09 11:12:17.448420 precession-2.0.2/precession/
+-rw-r--r--   0 dgerosa    (501) staff       (20)       54 2023-06-08 16:25:19.000000 precession-2.0.2/precession/__init__.py
+-rw-r--r--   0 dgerosa    (501) staff       (20)      458 2023-06-09 11:10:40.000000 precession-2.0.2/precession/__version__.py
+-rw-r--r--   0 dgerosa    (501) staff       (20)   226108 2023-06-09 11:10:59.000000 precession-2.0.2/precession/precession.py
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-06-09 11:12:17.451430 precession-2.0.2/precession.egg-info/
+-rw-r--r--   0 dgerosa    (501) staff       (20)      464 2023-06-09 11:12:17.000000 precession-2.0.2/precession.egg-info/PKG-INFO
+-rw-r--r--   0 dgerosa    (501) staff       (20)      331 2023-06-09 11:12:17.000000 precession-2.0.2/precession.egg-info/SOURCES.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-06-09 11:12:17.000000 precession-2.0.2/precession.egg-info/dependency_links.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-08 16:11:27.000000 precession-2.0.2/precession.egg-info/not-zip-safe
+-rw-r--r--   0 dgerosa    (501) staff       (20)       19 2023-06-09 11:12:17.000000 precession-2.0.2/precession.egg-info/requires.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       11 2023-06-09 11:12:17.000000 precession-2.0.2/precession.egg-info/top_level.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       18 2023-06-08 16:25:19.000000 precession-2.0.2/requirements.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       38 2023-06-09 11:12:17.452523 precession-2.0.2/setup.cfg
+-rw-r--r--   0 dgerosa    (501) staff       (20)      984 2023-06-08 16:25:19.000000 precession-2.0.2/setup.py
```

### Comparing `precession-2.0.1/LICENSE` & `precession-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `precession-2.0.1/README.md` & `precession-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `precession-2.0.1/precession/precession.py` & `precession-2.0.2/precession/precession.py`

 * *Files 0% similar despite different names*

```diff
@@ -1361,15 +1361,15 @@
         theta2 = np.atleast_1d(theta2).astype(float)
         deltaphi = np.atleast_1d(deltaphi).astype(float)
         q = np.atleast_1d(q).astype(float)
 
         S1 = eval_S1(q, chi1)
         S2 = eval_S2(q, chi2)
         L = eval_L(r, q)
-        S = eval_S(theta1, theta2, deltaphi, q, chi1, chi2)
+        S = eval_S(theta1=theta1, theta2=theta2, deltaphi=deltaphi, q=q, chi1=chi1, chi2=chi2)
         J = (L**2+S**2+2*L*(S1*np.cos(theta1)+S2*np.cos(theta2)))**0.5
 
     elif theta1 is None and theta2 is None and deltaphi is None and kappa is not None and r is not None and q is not None and chi1 is None and chi2 is None:
 
         kappa = np.atleast_1d(kappa).astype(float)
 
         L = eval_L(r, q)
@@ -1454,16 +1454,16 @@
     Returns
     -------
     S: float
         Magnitude of the total spin.
     
     Examples
     --------
-    ``S = precession.eval_S(theta1,theta2,deltaphi,q,chi1,chi2)``
-    ``S = precession.eval_S(deltachi,kappa,r,chieff,q)``
+    ``S = precession.eval_S(theta1=theta1,theta2=theta2,deltaphi=deltaphi,q=q,chi1=chi1,chi2=chi2)``
+    ``S = precession.eval_S(deltachi=deltachi,kappa=kappa,r=r,chieff=chieff,q=q)``
     """
 
     if theta1 is not None and theta2 is not None and deltaphi is not None and deltachi is None and kappa is None and r is None and chieff is None and q is not None and chi1 is not None and chi2 is not None:
 
         theta1 = np.atleast_1d(theta1).astype(float)
         theta2 = np.atleast_1d(theta2).astype(float)
         deltaphi = np.atleast_1d(deltaphi).astype(float)
```

### Comparing `precession-2.0.1/setup.py` & `precession-2.0.2/setup.py`

 * *Files identical despite different names*

