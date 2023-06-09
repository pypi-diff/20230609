# Comparing `tmp/sleqp-0.1.0.tar.gz` & `tmp/sleqp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleqp-0.1.0.tar", last modified: Tue Jun  7 20:45:56 2022, max compression
+gzip compressed data, was "sleqp-1.0.0.tar", last modified: Fri Jun  9 13:41:50 2023, max compression
```

## Comparing `sleqp-0.1.0.tar` & `sleqp-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2022-06-07 20:45:56.604748 sleqp-0.1.0/
--rw-r--r--   0 christoph  (1000) christoph  (1000)     7652 2021-10-01 15:49:08.000000 sleqp-0.1.0/LICENSE.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)       91 2022-06-02 18:17:56.000000 sleqp-0.1.0/MANIFEST.in
--rw-r--r--   0 christoph  (1000) christoph  (1000)      673 2022-06-07 20:45:56.604748 sleqp-0.1.0/PKG-INFO
--rw-r--r--   0 christoph  (1000) christoph  (1000)      126 2022-06-02 18:17:56.000000 sleqp-0.1.0/pyproject.toml
--rw-r--r--   0 christoph  (1000) christoph  (1000)       12 2020-12-15 16:14:17.000000 sleqp-0.1.0/requirements.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)       38 2022-06-07 20:45:56.604748 sleqp-0.1.0/setup.cfg
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2712 2022-06-02 12:20:33.000000 sleqp-0.1.0/setup.py
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2022-06-07 20:45:56.534747 sleqp-0.1.0/src/
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2022-06-07 20:45:56.591414 sleqp-0.1.0/src/extension/
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1153 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/call.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     3827 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/callback.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)       80 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/cmp.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)    24276 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/csleqp.pxd
--rw-r--r--   0 christoph  (1000) christoph  (1000)    12186 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/func.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)      635 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/gil.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1896 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/hess_struct.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1927 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/iterate.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1696 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/log.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     7767 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/lsq.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     5295 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/options.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1992 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/params.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)    10327 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/problem.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     6507 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/scale.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)  2946191 2022-05-30 10:45:07.000000 sleqp-0.1.0/src/extension/sleqp.c
--rw-r--r--   0 christoph  (1000) christoph  (1000)      625 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/sleqp.pyx
--rw-r--r--   0 christoph  (1000) christoph  (1000)    11197 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/solver.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     3868 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/sparse.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1158 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/sparse_matrix.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     6350 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/types.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)      229 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/version.pxi
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2263 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/extension/working_set.pxi
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2022-06-07 20:45:56.601414 sleqp-0.1.0/src/sleqp/
--rw-r--r--   0 christoph  (1000) christoph  (1000)       58 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/__init__.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1323 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_bounds.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     1517 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_cons.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2537 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_cons_func.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2139 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_derivative.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2113 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_func.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     3556 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_hessian.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)      948 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/_linear.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     5462 2022-06-02 18:17:56.000000 sleqp-0.1.0/src/sleqp/minimize.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)  2924485 2022-06-02 12:14:16.000000 sleqp-0.1.0/src/sleqp.c
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2022-06-07 20:45:56.604748 sleqp-0.1.0/src/sleqp.egg-info/
--rw-r--r--   0 christoph  (1000) christoph  (1000)      673 2022-06-07 20:45:55.000000 sleqp-0.1.0/src/sleqp.egg-info/PKG-INFO
--rw-r--r--   0 christoph  (1000) christoph  (1000)      986 2022-06-07 20:45:56.000000 sleqp-0.1.0/src/sleqp.egg-info/SOURCES.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)        1 2022-06-07 20:45:55.000000 sleqp-0.1.0/src/sleqp.egg-info/dependency_links.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)       12 2022-06-07 20:45:56.000000 sleqp-0.1.0/src/sleqp.egg-info/requires.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)        6 2022-06-07 20:45:56.000000 sleqp-0.1.0/src/sleqp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.553554 sleqp-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-28 08:35:37.000000 sleqp-1.0.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-09 13:28:30.000000 sleqp-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-09 13:41:50.553554 sleqp-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 13:28:30.000000 sleqp-1.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-09 13:28:30.000000 sleqp-1.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:41:50.553554 sleqp-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2023-06-09 13:39:40.000000 sleqp-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.545554 sleqp-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.549554 sleqp-1.0.0/src/extension/
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/call.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/callback.pxi
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/cmp.pxi
+-rw-rw-rw-   0 root         (0) root         (0)    26164 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/csleqp.pxd
+-rw-rw-rw-   0 root         (0) root         (0)     6111 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/dyn.pxi
+-rw-rw-rw-   0 root         (0) root         (0)    11767 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/func.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/gil.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/hess_struct.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/iterate.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/log.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/lsq.pxi
+-rw-rw-rw-   0 root         (0) root         (0)    12748 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/problem.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     6478 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/scale.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     7318 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/settings.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/sleqp.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    10919 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/solver.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/sparse.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/sparse_matrix.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     6620 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/types.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/version.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/working_set.pxi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.549554 sleqp-1.0.0/src/sleqp/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_cons.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_cons_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_hessian.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_linear.py
+-rw-rw-rw-   0 root         (0) root         (0)     6465 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/minimize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.553554 sleqp-1.0.0/src/sleqp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/top_level.txt
```

### Comparing `sleqp-0.1.0/LICENSE.txt` & `sleqp-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/PKG-INFO` & `sleqp-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleqp
-Version: 0.1.0
+Version: 1.0.0
 Summary: Active set-based NLP solver
 Author: Christoph Hansknecht
 Author-email: c.hansknecht@tu-braunschweig.de
 Classifier: Programming Language :: Cython
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: LICENSE.txt
```

### Comparing `sleqp-0.1.0/setup.py` & `sleqp-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 
 import numpy
 
 project_description = 'Active set-based NLP solver'
 long_description = 'This package provides SLEQP, an open-source solver for large-scale nonlinear continuous optimization. SLEQP is available as a callable library with interfaces to C, Python, AMPL, and MATLAB / Octave. It uses an active set method based on a combination of successive linear programming and equality constrained quadratic programming.'
 project_name = 'sleqp'
-project_version = '0.1.0'
+project_version = '1.0.0'
 license_file = 'LICENSE.txt'
 maintainer_name = 'Christoph Hansknecht'
 maintainer_email = 'c.hansknecht@tu-braunschweig.de'
 
 local_env = os.getenv('SLEQP_LOCAL_BUILD')
 local_build = (local_env is not None)
```

### Comparing `sleqp-0.1.0/src/extension/call.pxi` & `sleqp-1.0.0/src/extension/call.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/extension/callback.pxi` & `sleqp-1.0.0/src/extension/callback.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/extension/csleqp.pxd` & `sleqp-1.0.0/src/extension/csleqp.pxd`

 * *Files 9% similar despite different names*

```diff
@@ -89,14 +89,20 @@
     SLEQP_PARAMETRIC_CAUCHY_COARSE
     SLEQP_PARAMETRIC_CAUCHY_FINE
 
   ctypedef enum SLEQP_INITIAL_TR_CHOICE:
     SLEQP_INITIAL_TR_CHOICE_NARROW
     SLEQP_INITIAL_TR_CHOICE_WIDE
 
+  ctypedef enum SLEQP_AUG_JAC_METHOD:
+    SLEQP_AUG_JAC_AUTO,
+    SLEQP_AUG_JAC_STANDARD,
+    SLEQP_AUG_JAC_REDUCED,
+    SLEQP_AUG_JAC_DIRECT
+
   ctypedef enum SLEQP_LINESEARCH:
     SLEQP_LINESEARCH_EXACT
     SLEQP_LINESEARCH_APPROX
 
   ctypedef enum SLEQP_VALUE_REASON:
     SLEQP_VALUE_REASON_NONE,
     SLEQP_VALUE_REASON_INIT,
@@ -106,56 +112,58 @@
     SLEQP_VALUE_REASON_TRYING_SOC_ITERATE,
     SLEQP_VALUE_REASON_REJECTED_ITERATE
 
   ctypedef enum SLEQP_DUAL_ESTIMATION_TYPE:
     SLEQP_DUAL_ESTIMATION_TYPE_LP,
     SLEQP_DUAL_ESTIMATION_TYPE_LSQ,
 
-  ctypedef enum SLEQP_PARAM:
-    SLEQP_PARAM_ZERO_EPS,
-    SLEQP_PARAM_EPS,
-    SLEQP_PARAM_DERIV_PERTURBATION,
-    SLEQP_PARAM_DERIV_TOL,
-    SLEQP_PARAM_CAUCHY_TAU,
-    SLEQP_PARAM_CAUCHY_ETA,
-    SLEQP_PARAM_LINESEARCH_TAU,
-    SLEQP_PARAM_LINESEARCH_ETA,
-    SLEQP_PARAM_LINESEARCH_CUTOFF,
-    SLEQP_PARAM_FEAS_TOL,
-    SLEQP_PARAM_SLACK_TOL,
-    SLEQP_PARAM_STAT_TOL,
-    SLEQP_PARAM_ACCEPTED_REDUCTION,
-    SLEQP_PARAM_DEADPOINT_BOUND
-
-  ctypedef enum SLEQP_OPTION_INT:
-    SLEQP_OPTION_INT_NUM_QUASI_NEWTON_ITERATES,
-    SLEQP_OPTION_INT_MAX_NEWTON_ITERATIONS,
-    SLEQP_OPTION_INT_NUM_THREADS
-
-  ctypedef enum SLEQP_OPTION_ENUM:
-    SLEQP_OPTION_ENUM_DERIV_CHECK,
-    SLEQP_OPTION_ENUM_HESS_EVAL,
-    SLEQP_OPTION_ENUM_DUAL_ESTIMATION_TYPE,
-    SLEQP_OPTION_ENUM_FLOAT_WARNING_FLAGS,
-    SLEQP_OPTION_ENUM_FLOAT_ERROR_FLAGS,
-    SLEQP_OPTION_ENUM_BFGS_SIZING,
-    SLEQP_OPTION_ENUM_TR_SOLVER,
-    SLEQP_OPTION_ENUM_POLISHING_TYPE,
-    SLEQP_OPTION_ENUM_STEP_RULE,
-    SLEQP_OPTION_ENUM_LINESEARCH,
-    SLEQP_OPTION_ENUM_PARAMETRIC_CAUCHY,
-    SLEQP_OPTION_ENUM_INITIAL_TR_CHOICE
-
-  ctypedef enum SLEQP_OPTION_BOOL:
-    SLEQP_OPTION_BOOL_PERFORM_NEWTON_STEP,
-    SLEQP_OPTION_BOOL_GLOBAL_PENALTY_RESETS,
-    SLEQP_OPTION_BOOL_PERFORM_SOC,
-    SLEQP_OPTION_BOOL_USE_QUADRATIC_MODEL,
-    SLEQP_OPTION_BOOL_ENABLE_PREPROCESSOR,
-    SLEQP_OPTION_BOOL_LP_RESOLVES
+  ctypedef enum SLEQP_SETTINGS_REAL:
+    SLEQP_SETTINGS_REAL_ZERO_EPS,
+    SLEQP_SETTINGS_REAL_EPS,
+    SLEQP_SETTINGS_REAL_DERIV_PERTURBATION,
+    SLEQP_SETTINGS_REAL_DERIV_TOL,
+    SLEQP_SETTINGS_REAL_CAUCHY_TAU,
+    SLEQP_SETTINGS_REAL_CAUCHY_ETA,
+    SLEQP_SETTINGS_REAL_LINESEARCH_TAU,
+    SLEQP_SETTINGS_REAL_LINESEARCH_ETA,
+    SLEQP_SETTINGS_REAL_LINESEARCH_CUTOFF,
+    SLEQP_SETTINGS_REAL_FEAS_TOL,
+    SLEQP_SETTINGS_REAL_SLACK_TOL,
+    SLEQP_SETTINGS_REAL_STAT_TOL,
+    SLEQP_SETTINGS_REAL_ACCEPTED_REDUCTION,
+    SLEQP_SETTINGS_REAL_DEADPOINT_BOUND
+
+  ctypedef enum SLEQP_SETTINGS_INT:
+    SLEQP_SETTINGS_INT_NUM_QUASI_NEWTON_ITERATES,
+    SLEQP_SETTINGS_INT_MAX_NEWTON_ITERATIONS,
+    SLEQP_SETTINGS_INT_NUM_THREADS
+
+  ctypedef enum SLEQP_SETTINGS_ENUM:
+    SLEQP_SETTINGS_ENUM_DERIV_CHECK,
+    SLEQP_SETTINGS_ENUM_HESS_EVAL,
+    SLEQP_SETTINGS_ENUM_DUAL_ESTIMATION_TYPE,
+    SLEQP_SETTINGS_ENUM_FLOAT_WARNING_FLAGS,
+    SLEQP_SETTINGS_ENUM_FLOAT_ERROR_FLAGS,
+    SLEQP_SETTINGS_ENUM_BFGS_SIZING,
+    SLEQP_SETTINGS_ENUM_TR_SOLVER,
+    SLEQP_SETTINGS_ENUM_POLISHING_TYPE,
+    SLEQP_SETTINGS_ENUM_STEP_RULE,
+    SLEQP_SETTINGS_ENUM_LINESEARCH,
+    SLEQP_SETTINGS_ENUM_PARAMETRIC_CAUCHY,
+    SLEQP_SETTINGS_ENUM_INITIAL_TR_CHOICE,
+    SLEQP_SETTINGS_ENUM_AUG_JAC_METHOD
+
+  ctypedef enum SLEQP_SETTINGS_BOOL:
+    SLEQP_SETTINGS_BOOL_PERFORM_NEWTON_STEP,
+    SLEQP_SETTINGS_BOOL_GLOBAL_PENALTY_RESETS,
+    SLEQP_SETTINGS_BOOL_PERFORM_SOC,
+    SLEQP_SETTINGS_BOOL_USE_QUADRATIC_MODEL,
+    SLEQP_SETTINGS_BOOL_ENABLE_RESTORATION_PHASE,
+    SLEQP_SETTINGS_BOOL_ENABLE_PREPROCESSOR,
+    SLEQP_SETTINGS_BOOL_LP_RESOLVES
 
   ctypedef enum SLEQP_SOLVER_STATE_REAL:
     SLEQP_SOLVER_STATE_REAL_TRUST_RADIUS,
     SLEQP_SOLVER_STATE_REAL_LP_TRUST_RADIUS,
     SLEQP_SOLVER_STATE_REAL_SCALED_OBJ_VAL,
     SLEQP_SOLVER_STATE_REAL_SCALED_MERIT_VAL,
     SLEQP_SOLVER_STATE_REAL_SCALED_FEAS_RES,
@@ -192,30 +200,27 @@
     double* data
     int* indices
 
     int dim
     int nnz
     int nnz_max
 
-  ctypedef struct SleqpSparseMatrix:
+  ctypedef struct SleqpMat:
     pass
 
   ctypedef struct SleqpProblem:
     pass
 
   ctypedef struct SleqpSolver:
     pass
 
   ctypedef struct SleqpScaling:
     pass
 
-  ctypedef struct SleqpParams:
-    pass
-
-  ctypedef struct SleqpOptions:
+  ctypedef struct SleqpSettings:
     pass
 
   ctypedef struct SleqpWorkingSet:
     pass
 
   ctypedef struct SleqpIterate:
     pass
@@ -261,51 +266,51 @@
                                            int dim)
 
   SLEQP_RETCODE sleqp_vec_push(SleqpVec* vec,
                                          int idx,
                                          double value)
 
   # Sparse matrices
-  SLEQP_RETCODE sleqp_sparse_matrix_create(SleqpSparseMatrix** matrix,
+  SLEQP_RETCODE sleqp_mat_create(SleqpMat** matrix,
                                            int num_rows,
                                            int num_cols,
                                            int nnz_max)
 
-  SLEQP_RETCODE sleqp_sparse_matrix_reserve(SleqpSparseMatrix* matrix,
+  SLEQP_RETCODE sleqp_mat_reserve(SleqpMat* matrix,
                                             int nnz)
 
-  SLEQP_RETCODE sleqp_sparse_matrix_resize(SleqpSparseMatrix* matrix,
+  SLEQP_RETCODE sleqp_mat_resize(SleqpMat* matrix,
                                            int num_rows,
                                            int num_cols)
 
-  int sleqp_sparse_matrix_num_cols(SleqpSparseMatrix* matrix)
+  int sleqp_mat_num_cols(SleqpMat* matrix)
 
-  int sleqp_sparse_matrix_num_rows(SleqpSparseMatrix* matrix)
+  int sleqp_mat_num_rows(SleqpMat* matrix)
 
-  int sleqp_sparse_matrix_nnz(SleqpSparseMatrix* matrix)
+  int sleqp_mat_nnz(SleqpMat* matrix)
 
-  int sleqp_sparse_matrix_nnz_max(SleqpSparseMatrix* matrix)
+  int sleqp_mat_nnz_max(SleqpMat* matrix)
 
-  double* sleqp_sparse_matrix_data(SleqpSparseMatrix* matrix)
+  double* sleqp_mat_data(SleqpMat* matrix)
 
-  int* sleqp_sparse_matrix_cols(SleqpSparseMatrix* matrix)
+  int* sleqp_mat_cols(SleqpMat* matrix)
 
-  int* sleqp_sparse_matrix_rows(SleqpSparseMatrix* matrix)
+  int* sleqp_mat_rows(SleqpMat* matrix)
 
-  SLEQP_RETCODE sleqp_sparse_matrix_push(SleqpSparseMatrix* matrix,
+  SLEQP_RETCODE sleqp_mat_push(SleqpMat* matrix,
                                          int row,
                                          int col,
                                          double value)
 
-  SLEQP_RETCODE sleqp_sparse_matrix_push_column(SleqpSparseMatrix* matrix,
+  SLEQP_RETCODE sleqp_mat_push_col(SleqpMat* matrix,
                                                 int col)
 
-  SLEQP_RETCODE sleqp_sparse_matrix_capture(SleqpSparseMatrix* matrix)
+  SLEQP_RETCODE sleqp_mat_capture(SleqpMat* matrix)
 
-  SLEQP_RETCODE sleqp_sparse_matrix_release(SleqpSparseMatrix** matrix)
+  SLEQP_RETCODE sleqp_mat_release(SleqpMat** matrix)
 
   # Functions
   ctypedef SLEQP_RETCODE (*SLEQP_FUNC_SET)(SleqpFunc* func,
                                            SleqpVec* x,
                                            SLEQP_VALUE_REASON reason,
                                            bool* reject,
                                            void* func_data)
@@ -326,19 +331,18 @@
                                                 void* func_data)
 
   ctypedef SLEQP_RETCODE (*SLEQP_FUNC_CONS_VAL)(SleqpFunc* func,
                                                 SleqpVec* cons_val,
                                                 void* func_data)
 
   ctypedef SLEQP_RETCODE (*SLEQP_FUNC_CONS_JAC)(SleqpFunc* func,
-                                                SleqpSparseMatrix* cons_jac,
+                                                SleqpMat* cons_jac,
                                                 void* func_data)
 
   ctypedef SLEQP_RETCODE (*SLEQP_FUNC_HESS_PROD)(SleqpFunc* func,
-                                                 const double* obj_dual,
                                                  const SleqpVec* direction,
                                                  const SleqpVec* cons_duals,
                                                  SleqpVec* product,
                                                  void* func_data)
 
   ctypedef SLEQP_RETCODE (*SLEQP_FUNC_FREE)(void* func_data)
 
@@ -407,15 +411,15 @@
   SLEQP_RETCODE sleqp_iterate_set_obj_val(SleqpIterate* iterate,
                                           double value)
 
   SleqpVec* sleqp_iterate_obj_grad(SleqpIterate* iterate)
 
   SleqpVec* sleqp_iterate_cons_val(SleqpIterate* iterate)
 
-  SleqpSparseMatrix* sleqp_iterate_cons_jac(SleqpIterate* iterate)
+  SleqpMat* sleqp_iterate_cons_jac(SleqpIterate* iterate)
 
   SleqpWorkingSet* sleqp_iterate_working_set(SleqpIterate* iterate)
 
   SleqpVec* sleqp_iterate_cons_dual(SleqpIterate* iterate)
 
   SleqpVec* sleqp_iterate_vars_dual(SleqpIterate* iterate)
 
@@ -478,20 +482,61 @@
 
   SLEQP_RETCODE sleqp_lsq_func_create(SleqpFunc** fstar,
                                       SleqpLSQCallbacks* callbacks,
                                       int num_variables,
                                       int num_constraints,
                                       int num_residuals,
                                       double levenberg_marquardt,
-                                      SleqpParams* params,
+                                      SleqpSettings* settings,
                                       void* func_data)
 
   SLEQP_RETCODE sleqp_lsq_func_set_callbacks(SleqpFunc* func,
                                              SleqpLSQCallbacks* callbacks)
 
+  # Dynamic
+
+  ctypedef SLEQP_RETCODE (*SLEQP_DYN_FUNC_EVAL)(SleqpFunc* func,
+                                                double* obj_val,
+                                                SleqpVec* cons_val,
+                                                double* error,
+                                                void* func_data)
+
+  ctypedef SLEQP_RETCODE (*SLEQP_DYN_FUNC_SET_ERROR_BOUND)(SleqpFunc* func,
+                                                           double error_bound,
+                                                           void* func_data)
+
+  ctypedef SLEQP_RETCODE (*SLEQP_DYN_FUNC_SET_OBJ_WEIGHT)(SleqpFunc* func,
+                                                          double obj_weight,
+                                                          void* func_data)
+
+  ctypedef SLEQP_RETCODE (*SLEQP_DYN_FUNC_SET_CONS_WEIGHTS)(SleqpFunc* func,
+                                                            const double* cons_weights,
+                                                            void* func_data)
+
+  ctypedef struct SleqpDynFuncCallbacks:
+    SLEQP_FUNC_SET set_value,
+    SLEQP_FUNC_NONZEROS nonzeros,
+    SLEQP_DYN_FUNC_SET_ERROR_BOUND set_error_bound,
+    SLEQP_DYN_FUNC_SET_OBJ_WEIGHT set_obj_weight,
+    SLEQP_DYN_FUNC_SET_CONS_WEIGHTS set_cons_weights,
+    SLEQP_DYN_FUNC_EVAL eval,
+    SLEQP_FUNC_OBJ_GRAD obj_grad,
+    SLEQP_FUNC_CONS_JAC cons_jac,
+    SLEQP_FUNC_HESS_PROD hess_prod,
+    SLEQP_FUNC_FREE func_free
+
+  SLEQP_RETCODE sleqp_dyn_func_create(SleqpFunc** fstar,
+                                      SleqpDynFuncCallbacks* callbacks,
+                                      int num_variables,
+                                      int num_constraints,
+                                      void* func_data)
+
+  SLEQP_RETCODE sleqp_dyn_func_set_callbacks(SleqpFunc* func,
+                                             SleqpDynFuncCallbacks* callbacks)
+
   # Scaling
 
   SLEQP_RETCODE sleqp_scaling_create(SleqpScaling** scaling,
                                      int num_variables,
                                      int num_constraints)
 
   int sleqp_scaling_num_vars(SleqpScaling* scaling)
@@ -532,25 +577,23 @@
                                                            double nominal_value);
 
   SLEQP_RETCODE sleqp_obj_scaling_from_grad(SleqpScaling* scaling,
                                             SleqpVec* gradient,
                                             double eps)
 
   SLEQP_RETCODE sleqp_scaling_from_cons_jac(SleqpScaling* scaling,
-                                            SleqpSparseMatrix* cons_jac,
+                                            SleqpMat* cons_jac,
                                             double eps)
 
   SLEQP_RETCODE sleqp_scaling_release(SleqpScaling** scaling)
 
   # Solver
 
   SLEQP_RETCODE sleqp_solver_create(SleqpSolver** star,
                                     SleqpProblem* problem,
-                                    SleqpParams* params,
-                                    SleqpOptions* options,
                                     SleqpVec* x,
                                     SleqpScaling* scaling)
 
   const char* sleqp_solver_info(const SleqpSolver* solver)
 
   SLEQP_RETCODE sleqp_solver_solve(SleqpSolver* solver,
                                    int max_num_iterations,
@@ -596,30 +639,30 @@
 
   SLEQP_RETCODE sleqp_solver_release(SleqpSolver** star)
 
   # Problem
 
   SLEQP_RETCODE sleqp_problem_create_simple(SleqpProblem** star,
                                             SleqpFunc* func,
-                                            SleqpParams* params,
                                             const SleqpVec* var_lb,
                                             const SleqpVec* var_ub,
                                             const SleqpVec* cons_lb,
-                                            const SleqpVec* cons_ub)
+                                            const SleqpVec* cons_ub,
+                                            SleqpSettings* settings)
 
   SLEQP_RETCODE sleqp_problem_create(SleqpProblem** star,
                                      SleqpFunc* func,
-                                     SleqpParams* params,
                                      const SleqpVec* var_lb,
                                      const SleqpVec* var_ub,
                                      const SleqpVec* genereal_lb,
                                      const SleqpVec* genereal_ub,
-                                     const SleqpSparseMatrix* linear_coeffs,
+                                     const SleqpMat* linear_coeffs,
                                      const SleqpVec* linear_lb,
-                                     const SleqpVec* linear_ub)
+                                     const SleqpVec* linear_ub,
+                                     SleqpSettings* settings)
 
   int sleqp_problem_num_cons(SleqpProblem* problem)
 
   int sleqp_problem_num_vars(SleqpProblem* problem)
 
   SleqpVec* sleqp_problem_vars_lb(SleqpProblem* problem)
 
@@ -627,54 +670,52 @@
 
   SleqpVec* sleqp_problem_cons_lb(SleqpProblem* problem)
 
   SleqpVec* sleqp_problem_cons_ub(SleqpProblem* problem)
 
   SLEQP_RETCODE sleqp_problem_release(SleqpProblem** star)
 
-  # Parameters
-
-  SLEQP_RETCODE sleqp_params_create(SleqpParams** star)
+  # Settings
 
-  double sleqp_params_value(const SleqpParams* params,
-                            SLEQP_PARAM param)
+  SLEQP_RETCODE sleqp_settings_create(SleqpSettings** star)
 
-  SLEQP_RETCODE sleqp_params_set_value(SleqpParams* params,
-                                       SLEQP_PARAM param,
-                                       double value)
+  SLEQP_RETCODE sleqp_settings_read_file(SleqpSettings* settings,
+                                         const char* settings_filename)
 
-  SLEQP_RETCODE sleqp_params_release(SleqpParams** star)
+  int sleqp_settings_enum_value(const SleqpSettings* options,
+                                SLEQP_SETTINGS_ENUM option)
 
-  # Options
+  SLEQP_RETCODE sleqp_settings_set_enum_value(SleqpSettings* options,
+                                              SLEQP_SETTINGS_ENUM option,
+                                              int value)
 
-  SLEQP_RETCODE sleqp_options_create(SleqpOptions** star)
+  int sleqp_settings_int_value(const SleqpSettings* options,
+                               SLEQP_SETTINGS_INT option)
 
-  int sleqp_options_enum_value(const SleqpOptions* options,
-                               SLEQP_OPTION_ENUM option)
-
-  SLEQP_RETCODE sleqp_options_set_enum_value(SleqpOptions* options,
-                                             SLEQP_OPTION_ENUM option,
+  SLEQP_RETCODE sleqp_settings_set_int_value(SleqpSettings* options,
+                                             SLEQP_SETTINGS_INT option,
                                              int value)
 
-  int sleqp_options_int_value(const SleqpOptions* options,
-                              SLEQP_OPTION_INT option)
 
-  SLEQP_RETCODE sleqp_options_set_int_value(SleqpOptions* options,
-                                            SLEQP_OPTION_INT option,
-                                            int value)
+  bool sleqp_settings_bool_value(const SleqpSettings* options,
+                                 SLEQP_SETTINGS_BOOL option)
+
+  SLEQP_RETCODE sleqp_settings_set_bool_value(SleqpSettings* options,
+                                              SLEQP_SETTINGS_BOOL option,
+                                              bool value)
 
+  double sleqp_settings_real_value(const SleqpSettings* settings,
+                                   SLEQP_SETTINGS_REAL param)
 
-  bool sleqp_options_bool_value(const SleqpOptions* options,
-                                SLEQP_OPTION_BOOL option)
+  SLEQP_RETCODE sleqp_settings_set_real_value(SleqpSettings* settings,
+                                              SLEQP_SETTINGS_REAL param,
+                                              double value)
 
-  SLEQP_RETCODE sleqp_options_set_bool_value(SleqpOptions* options,
-                                             SLEQP_OPTION_BOOL option,
-                                             bool value)
 
-  SLEQP_RETCODE sleqp_options_release(SleqpOptions** star)
+  SLEQP_RETCODE sleqp_settings_release(SleqpSettings** star)
 
   # Logging
 
   void sleqp_log_set_level(SLEQP_LOG_LEVEL value)
 
   ctypedef void (*SLEQP_LOG_HANDLER)(SLEQP_LOG_LEVEL level,
                                      libc.time.time_t time,
```

### Comparing `sleqp-0.1.0/src/extension/func.pxi` & `sleqp-1.0.0/src/extension/func.pxi`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,14 @@
 
     if do_reject is True:
       reject[0] = True
       return csleqp.SLEQP_OKAY
     else:
       reject[0] = False
 
-    def try_call(f):
-      try:
-        return f()
-      except AttributeError:
-        return 0
-
   except BaseException as exception:
     store_func_exc(func_obj, exception)
     return csleqp.SLEQP_ERROR
 
   return csleqp.SLEQP_OKAY
 
 
@@ -183,15 +177,15 @@
   with gil:
     return sleqp_func_cons_val(func,
                                cons_vals,
                                func_data)
 
 
 cdef csleqp.SLEQP_RETCODE sleqp_func_cons_jac(csleqp.SleqpFunc* func,
-                                              csleqp.SleqpSparseMatrix* cons_jac,
+                                              csleqp.SleqpMat* cons_jac,
                                               void* func_data):
   cdef int num_vars
   cdef int num_cons
   try:
 
     func_obj = (<object> func_data)
 
@@ -213,73 +207,69 @@
     store_func_exc(func_obj, exception)
     return csleqp.SLEQP_ERROR
 
   return csleqp.SLEQP_OKAY
 
 
 cdef csleqp.SLEQP_RETCODE sleqp_func_cons_jac_nogil(csleqp.SleqpFunc* func,
-                                                    csleqp.SleqpSparseMatrix* cons_jac,
+                                                    csleqp.SleqpMat* cons_jac,
                                                     void* func_data) nogil:
   with gil:
     return sleqp_func_cons_jac(func,
                                cons_jac,
                                func_data)
 
 
-cdef csleqp.SLEQP_RETCODE sleqp_func_hess_product(csleqp.SleqpFunc* func,
-                                                  const double* obj_dual,
-                                                  const csleqp.SleqpVec* direction,
-                                                  const csleqp.SleqpVec* cons_dual,
-                                                  csleqp.SleqpVec* product,
-                                                  void* func_data):
+cdef csleqp.SLEQP_RETCODE sleqp_func_hess_prod(csleqp.SleqpFunc* func,
+                                               const csleqp.SleqpVec* direction,
+                                               const csleqp.SleqpVec* cons_dual,
+                                               csleqp.SleqpVec* product,
+                                               void* func_data):
 
   cdef int num_vars
 
   try:
 
     assert cons_dual
     assert direction
     assert product
 
     func_obj = (<object> func_data)
 
     num_vars = csleqp.sleqp_func_num_vars(func)
 
-    o_dual = obj_dual[0] if obj_dual else 0.
     direction_array = sleqp_sparse_vec_to_array(direction)
     cons_dual_array = sleqp_sparse_vec_to_array(cons_dual)
 
-    product_array = func_obj.hess_prod(o_dual, direction_array, cons_dual_array)
+    product_array = func_obj.hess_prod(direction_array, cons_dual_array)
 
     assert product_array is not None, "hess_prod(...) returned 'None'"
     assert product_array.ndim == 1, "Hessian product must be a vector"
     assert product_array.size == num_vars, "Hessian product has wrong size"
 
     csleqp_call(array_to_sleqp_sparse_vec(product_array, product))
 
   except BaseException as exception:
     store_func_exc(func_obj, exception)
     return csleqp.SLEQP_ERROR
 
   return csleqp.SLEQP_OKAY
 
 
-cdef csleqp.SLEQP_RETCODE sleqp_func_hess_product_nogil(csleqp.SleqpFunc* func,
-                                                        const double* obj_dual,
-                                                        const csleqp.SleqpVec* direction,
-                                                        const csleqp.SleqpVec* cons_dual,
-                                                        csleqp.SleqpVec* product,
-                                                        void* func_data) nogil:
+cdef csleqp.SLEQP_RETCODE sleqp_func_hess_prod_nogil(csleqp.SleqpFunc* func,
+                                                     const csleqp.SleqpVec* direction,
+                                                     const csleqp.SleqpVec* cons_dual,
+                                                     csleqp.SleqpVec* product,
+                                                     void* func_data) nogil:
   with gil:
-    return sleqp_func_hess_product(func,
-                                   obj_dual,
-                                   direction,
-                                   cons_dual,
-                                   product,
-                                   func_data)
+    return sleqp_func_hess_prod(func,
+                                direction,
+                                cons_dual,
+                                product,
+                                func_data)
 
 
 cdef csleqp.SLEQP_RETCODE sleqp_func_free(void* func_data):
   return csleqp.SLEQP_OKAY
 
 
 cdef object funcs = weakref.WeakSet()
@@ -289,23 +279,23 @@
   if release_gil:
     callbacks[0].set_value = &sleqp_func_set_nogil
     callbacks[0].nonzeros  = &sleqp_func_nonzeros_nogil
     callbacks[0].obj_val   = &sleqp_func_obj_val_nogil
     callbacks[0].obj_grad  = &sleqp_func_obj_grad_nogil
     callbacks[0].cons_val  = &sleqp_func_cons_val_nogil
     callbacks[0].cons_jac  = &sleqp_func_cons_jac_nogil
-    callbacks[0].hess_prod = &sleqp_func_hess_product_nogil
+    callbacks[0].hess_prod = &sleqp_func_hess_prod_nogil
   else:
     callbacks[0].set_value = &sleqp_func_set
     callbacks[0].nonzeros  = &sleqp_func_nonzeros
     callbacks[0].obj_val   = &sleqp_func_obj_val
     callbacks[0].obj_grad  = &sleqp_func_obj_grad
     callbacks[0].cons_val  = &sleqp_func_cons_val
     callbacks[0].cons_jac  = &sleqp_func_cons_jac
-    callbacks[0].hess_prod = &sleqp_func_hess_product
+    callbacks[0].hess_prod = &sleqp_func_hess_prod
 
   callbacks.func_free = &sleqp_func_free
 
 
 cdef update_func_callbacks():
   cdef _Func func
   cdef csleqp.SleqpFuncCallbacks callbacks
```

### Comparing `sleqp-0.1.0/src/extension/gil.pxi` & `sleqp-1.0.0/src/extension/gil.pxi`

 * *Files 10% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 
   if value == release_gil:
     return
 
   release_gil = value
   update_log_handler()
   update_func_callbacks()
+  update_dyn_func_callbacks()
   update_lsq_func_callbacks()
   update_solver_callbacks()
```

### Comparing `sleqp-0.1.0/src/extension/hess_struct.pxi` & `sleqp-1.0.0/src/extension/hess_struct.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/extension/iterate.pxi` & `sleqp-1.0.0/src/extension/iterate.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/extension/log.pxi` & `sleqp-1.0.0/src/extension/log.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/extension/lsq.pxi` & `sleqp-1.0.0/src/extension/lsq.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -123,17 +123,14 @@
   except BaseException as exception:
     store_func_exc(func_obj, exception)
     return csleqp.SLEQP_ERROR
 
   return csleqp.SLEQP_OKAY
 
 
-cdef object lsq_funcs = weakref.WeakSet()
-
-
 cdef csleqp.SLEQP_RETCODE sleqp_lsq_jac_adjoint_nogil(csleqp.SleqpFunc* func,
                                                       const csleqp.SleqpVec* adjoint_direction,
                                                       csleqp.SleqpVec* product,
                                                       void* func_data) nogil:
   with gil:
     return sleqp_lsq_jac_adjoint(func,
                                  adjoint_direction,
@@ -158,14 +155,16 @@
     callbacks.lsq_jac_adjoint      = &sleqp_lsq_jac_adjoint
     callbacks.cons_val             = &sleqp_func_cons_val
     callbacks.cons_jac             = &sleqp_func_cons_jac
 
   callbacks.func_free = &sleqp_func_free
 
 
+cdef object lsq_funcs = weakref.WeakSet()
+
 cdef update_lsq_func_callbacks():
   cdef _Func func
   cdef csleqp.SleqpLSQCallbacks callbacks
 
   set_lsq_func_callbacks(&callbacks)
 
   for obj in lsq_funcs:
@@ -176,26 +175,22 @@
 
 cdef csleqp.SLEQP_RETCODE create_lsq_func(csleqp.SleqpFunc** cfunc,
                                           object func,
                                           int num_variables,
                                           int num_constraints,
                                           int num_residuals,
                                           double levenberg_marquardt,
-                                          csleqp.SleqpParams* params):
+                                          csleqp.SleqpSettings* settings):
   cdef csleqp.SleqpLSQCallbacks callbacks
-  cdef csleqp.SLEQP_RETCODE retcode
 
   assert func is not None
 
   set_lsq_func_callbacks(&callbacks)
 
-  retcode = csleqp.sleqp_lsq_func_create(cfunc,
-                                         &callbacks,
-                                         num_variables,
-                                         num_constraints,
-                                         num_residuals,
-                                         levenberg_marquardt,
-                                         params,
-                                         <void*> func)
-  
-  return retcode
-    
+  return csleqp.sleqp_lsq_func_create(cfunc,
+                                      &callbacks,
+                                      num_variables,
+                                      num_constraints,
+                                      num_residuals,
+                                      levenberg_marquardt,
+                                      settings,
+                                      <void*> func)
```

### Comparing `sleqp-0.1.0/src/extension/problem.pxi` & `sleqp-1.0.0/src/extension/problem.pxi`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #cython: language_level=3
 
 
 cdef csleqp.SLEQP_RETCODE create_problem(csleqp.SleqpProblem** problem,
                                          csleqp.SleqpFunc* cfunc,
-                                         csleqp.SleqpParams* cparams,
                                          np.ndarray var_lb,
                                          np.ndarray var_ub,
                                          np.ndarray general_lb,
                                          np.ndarray general_ub,
+                                         csleqp.SleqpSettings* csettings,
                                          object linear_coeffs = None,
                                          np.ndarray linear_lb = None,
                                          np.ndarray linear_ub = None):
 
   assert var_lb is not None
   assert var_ub is not None
 
@@ -23,50 +23,50 @@
 
   cdef csleqp.SleqpVec* general_lb_vec
   cdef csleqp.SleqpVec* general_ub_vec
 
   cdef csleqp.SleqpVec* linear_lb_vec
   cdef csleqp.SleqpVec* linear_ub_vec
 
-  cdef csleqp.SleqpSparseMatrix* linear_coeffs_mat
+  cdef csleqp.SleqpMat* linear_coeffs_mat
 
   cdef int num_vars = var_lb.shape[0]
   cdef int num_cons = general_lb.shape[0]
 
   assert cfunc != NULL
 
   cdef int num_linear_constraints = 0
 
   if linear_coeffs is not None:
     num_linear_constraints = linear_coeffs.shape[0]
 
   try:
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&var_lb_vec,
-                                                        num_vars))
+                                              num_vars))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&var_ub_vec,
-                                                        num_vars))
+                                              num_vars))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&general_lb_vec,
-                                                        num_cons))
+                                              num_cons))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&general_ub_vec,
-                                                        num_cons))
+                                              num_cons))
 
-    csleqp_call(csleqp.sleqp_sparse_matrix_create(&linear_coeffs_mat,
-                                                  num_linear_constraints,
-                                                  num_vars,
-                                                  0))
+    csleqp_call(csleqp.sleqp_mat_create(&linear_coeffs_mat,
+                                        num_linear_constraints,
+                                        num_vars,
+                                        0))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&linear_lb_vec,
-                                                        num_linear_constraints))
+                                              num_linear_constraints))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&linear_ub_vec,
-                                                        num_linear_constraints))
+                                              num_linear_constraints))
 
     array_to_sleqp_sparse_vec(var_lb, var_lb_vec)
     array_to_sleqp_sparse_vec(var_ub, var_ub_vec)
     array_to_sleqp_sparse_vec(general_lb, general_lb_vec)
     array_to_sleqp_sparse_vec(general_ub, general_ub_vec)
 
     if linear_lb is not None:
@@ -77,33 +77,33 @@
 
     if linear_coeffs is not None:
       csleqp_call(matrix_to_sleqp_sparse_matrix(linear_coeffs,
                                                 linear_coeffs_mat))
 
     csleqp_call(csleqp.sleqp_problem_create(problem,
                                             cfunc,
-                                            cparams,
                                             var_lb_vec,
                                             var_ub_vec,
                                             general_lb_vec,
                                             general_ub_vec,
                                             linear_coeffs_mat,
                                             linear_lb_vec,
-                                            linear_ub_vec))
+                                            linear_ub_vec,
+                                            csettings))
 
     return csleqp.SLEQP_OKAY
 
   except BaseException as exception:
     return csleqp.SLEQP_ERROR
 
   finally:
     csleqp_call(csleqp.sleqp_vec_free(&linear_ub_vec))
     csleqp_call(csleqp.sleqp_vec_free(&linear_lb_vec))
 
-    csleqp_call(csleqp.sleqp_sparse_matrix_release(&linear_coeffs_mat))
+    csleqp_call(csleqp.sleqp_mat_release(&linear_coeffs_mat))
 
     csleqp_call(csleqp.sleqp_vec_free(&general_ub_vec))
     csleqp_call(csleqp.sleqp_vec_free(&general_lb_vec))
 
     csleqp_call(csleqp.sleqp_vec_free(&var_ub_vec))
     csleqp_call(csleqp.sleqp_vec_free(&var_lb_vec))
 
@@ -113,35 +113,41 @@
   cdef _Func funcref
 
   def __cinit__(self):
     self.cproblem = NULL
 
   @staticmethod
   cdef _Problem create(csleqp.SleqpFunc* cfunc,
-                       csleqp.SleqpParams* cparams,
-                       np.ndarray var_lb,
-                       np.ndarray var_ub,
-                       np.ndarray cons_lb,
-                       np.ndarray cons_ub,
+                       object var_lb,
+                       object var_ub,
+                       object cons_lb,
+                       object cons_ub,
+                       csleqp.SleqpSettings* csettings,
                        object linear_coeffs = None,
                        np.ndarray linear_lb = None,
                        np.ndarray linear_ub = None):
 
     cdef _Problem _problem = _Problem()
 
+    var_lb = np.atleast_1d(var_lb)
+    var_ub = np.atleast_1d(var_ub)
+
+    cons_lb = np.atleast_1d(cons_lb)
+    cons_ub = np.atleast_1d(cons_ub)
+
     cdef int num_vars = var_lb.shape[0]
     cdef int num_cons = cons_lb.shape[0]
 
     csleqp_call(create_problem(&_problem.cproblem,
                                cfunc,
-                               cparams,
                                var_lb,
                                var_ub,
                                cons_lb,
                                cons_ub,
+                               csettings,
                                linear_coeffs,
                                linear_lb,
                                linear_ub))
 
     _problem.funcref = _Func()
     _problem.funcref.set_func(cfunc)
 
@@ -175,53 +181,99 @@
   def hess_struct(self) -> HessianStruct:
     return HessianStruct(self.funcref)
 
   def __dealloc__(self):
     csleqp_call(csleqp.sleqp_problem_release(&self.cproblem))
 
 
-cdef class Problem:
+cdef class BaseProblem:
   cdef dict __dict__
 
-  cdef _Problem problem
-  cdef _Func funcref
-
+  cdef object _problem
   cdef object _func
+  cdef Settings _settings
+
+  def __init__(self, problem):
+    self._problem = problem
+
+  @property
+  def num_vars(self) -> int:
+    return self._problem.num_vars
+
+  @property
+  def num_cons(self) -> int:
+    return self._problem.num_cons
+
+  @property
+  def var_lb(self) -> np.array:
+    return self._problem.var_lb
+
+  @property
+  def var_ub(self) -> np.array:
+    return self._problem.var_ub
+
+  @property
+  def cons_lb(self) -> np.array:
+    return self._problem.cons_lb
+
+  @property
+  def cons_ub(self) -> np.array:
+    return self._problem.cons_ub
+
+  @property
+  def func(self) -> object:
+    return self._func
+
+  @property
+  def settings(self) -> object:
+    return self._settings
+
+
+cdef class Problem(BaseProblem):
+  cdef _Func funcref
 
   def __cinit__(self,
                 object func,
-                Params params,
-                np.ndarray var_lb,
-                np.ndarray var_ub,
-                np.ndarray cons_lb,
-                np.ndarray cons_ub,
+                object var_lb=[],
+                object var_ub=[],
+                object cons_lb=[],
+                object cons_ub=[],
+                Settings settings=None,
                 **properties):
 
-    cdef int num_vars = var_lb.shape[0]
-    cdef int num_cons = cons_lb.shape[0]
+    cdef int num_vars = np.atleast_1d(var_lb).shape[0]
+    cdef int num_cons = np.atleast_1d(cons_lb).shape[0]
     cdef csleqp.SleqpFunc* cfunc
+    cdef csleqp.SleqpSettings* csettings
+
+    if settings is None:
+      self._settings = Settings()
+    else:
+      self._settings = settings
+
+    csettings = <csleqp.SleqpSettings*> self._settings.settings
 
     self.funcref = _Func()
 
     csleqp_call(create_func(&cfunc,
                             func,
                             num_vars,
                             num_cons))
 
     assert cfunc != NULL
 
     self._func = func
 
     try:
       self.problem = _Problem.create(cfunc,
-                                     params.params,
                                      var_lb,
                                      var_ub,
                                      cons_lb,
                                      cons_ub,
+                                     csettings,
                                      properties.get('linear_coeffs', None),
                                      properties.get('linear_lb', None),
                                      properties.get('linear_ub', None))
 
       self.funcref.set_func(cfunc)
       funcs.add(self.funcref)
 
@@ -229,131 +281,154 @@
       csleqp_call(csleqp.sleqp_func_release(&cfunc))
 
     try:
       func.set_hessian_struct(self.hess_struct)
     except AttributeError:
       pass
 
-  @property
-  def func(self):
-      return self._func
-
-  @property
-  def num_vars(self) -> int:
-    return self.problem.num_vars
-
-  @property
-  def num_cons(self) -> int:
-    return self.problem.num_cons
-
-  @property
-  def var_lb(self) -> np.array:
-    return self.problem.var_lb
-
-  @property
-  def var_ub(self) -> np.array:
-    return self.problem.var_ub
-
-  @property
-  def cons_lb(self) -> np.array:
-    return self.problem.cons_lb
-
-  @property
-  def cons_ub(self) -> np.array:
-    return self.problem.cons_ub
+  # Actual arguments processed in __cinit__
+  def __init__(self, *args, **kwds):
+    super().__init__(self.problem)
 
   @property
   def hess_struct(self) -> HessianStruct:
     return self.problem.hess_struct
 
   def _get_problem(self):
     return self.problem
 
-cdef class LSQProblem:
-  cdef dict __dict__
 
-  cdef _Problem problem
+cdef class LSQProblem(BaseProblem):
   cdef _Func funcref
 
-  cdef object _func
-
   def __cinit__(self,
                 object func,
-                Params params,
-                np.ndarray var_lb,
-                np.ndarray var_ub,
-                np.ndarray cons_lb,
-                np.ndarray cons_ub,
                 num_residuals,
+                object var_lb=[],
+                object var_ub=[],
+                object cons_lb=[],
+                object cons_ub=[],
+                Settings settings=None,
                 **properties):
 
-    cdef int num_vars = var_lb.shape[0]
-    cdef int num_cons = cons_lb.shape[0]
+    cdef int num_vars = np.atleast_1d(var_lb).shape[0]
+    cdef int num_cons = np.atleast_1d(cons_lb).shape[0]
     cdef csleqp.SleqpFunc* cfunc
+    cdef csleqp.SleqpSettings* csettings
+
+    if settings is None:
+      self._settings = Settings()
+    else:
+      self._settings = settings
+
+    csettings = <csleqp.SleqpSettings*> self._settings.settings
 
     self.funcref = _Func()
 
     csleqp_call(create_lsq_func(&cfunc,
                                 func,
                                 num_vars,
                                 num_cons,
                                 num_residuals,
                                 properties.get('regularization', 0.),
-                                params.params))
+                                csettings))
 
     assert cfunc != NULL
 
     self._func = func
 
     try:
       self.problem = _Problem.create(cfunc,
-                                     params.params,
                                      var_lb,
                                      var_ub,
                                      cons_lb,
-                                     cons_ub)
+                                     cons_ub,
+                                     csettings,
+                                     properties.get('linear_coeffs', None),
+                                     properties.get('linear_lb', None),
+                                     properties.get('linear_ub', None))
 
       self.funcref.set_func(cfunc)
       lsq_funcs.add(self.funcref)
 
     finally:
       csleqp_call(csleqp.sleqp_func_release(&cfunc))
 
     try:
       func.set_hessian_struct(self.hess_struct)
     except AttributeError:
       pass
 
-  @property
-  def func(self):
-      return self._func
+  # Actual arguments processed in __cinit__
+  def __init__(self, *args, **kwds):
+    super().__init__(self.problem)
 
-  @property
-  def num_vars(self) -> int:
-    return self.problem.num_vars
+  def _get_problem(self):
+    return self.problem
 
-  @property
-  def num_cons(self) -> int:
-    return self.problem.num_cons
 
-  @property
-  def var_lb(self) -> np.array:
-    return self.problem.var_lb
+cdef class DynProblem(BaseProblem):
+  cdef _Func funcref
 
-  @property
-  def var_ub(self) -> np.array:
-    return self.problem.var_ub
+  def __cinit__(self,
+                object func,
+                object var_lb=[],
+                object var_ub=[],
+                object cons_lb=[],
+                object cons_ub=[],
+                Settings settings=None,
+                **properties):
 
-  @property
-  def cons_lb(self) -> np.array:
-    return self.problem.cons_lb
+    cdef int num_vars = np.atleast_1d(var_lb).shape[0]
+    cdef int num_cons = np.atleast_1d(cons_lb).shape[0]
+    cdef csleqp.SleqpFunc* cfunc
+    cdef csleqp.SleqpSettings* csettings
 
-  @property
-  def cons_ub(self) -> np.array:
-    return self.problem.cons_ub
+    if settings is None:
+      self._settings = Settings()
+    else:
+      self._settings = settings
+
+    csettings = <csleqp.SleqpSettings*> self._settings.settings
+
+    self.funcref = _Func()
+
+    csleqp_call(create_dyn_func(&cfunc,
+                                func,
+                                num_vars,
+                                num_cons))
+
+    assert cfunc != NULL
+    self._func = func
+
+    try:
+      self.problem = _Problem.create(cfunc,
+                                     var_lb,
+                                     var_ub,
+                                     cons_lb,
+                                     cons_ub,
+                                     csettings,
+                                     properties.get('linear_coeffs', None),
+                                     properties.get('linear_lb', None),
+                                     properties.get('linear_ub', None))
+
+      self.funcref.set_func(cfunc)
+      dyn_funcs.add(self.funcref)
+
+      pass
+    finally:
+      csleqp_call(csleqp.sleqp_func_release(&cfunc))
+    try:
+      func.set_hessian_struct(self.hess_struct)
+    except AttributeError:
+      pass
+
+  # Actual arguments processed in __cinit__
+  def __init__(self, *args, **kwds):
+    super().__init__(self.problem)
 
   @property
   def hess_struct(self) -> HessianStruct:
     return self.problem.hess_struct
 
   def _get_problem(self):
     return self.problem
```

### Comparing `sleqp-0.1.0/src/extension/scale.pxi` & `sleqp-1.0.0/src/extension/scale.pxi`

 * *Files 5% similar despite different names*

```diff
@@ -16,44 +16,44 @@
       return
     self._token = getattr(obj, '_token', None)
 
 cdef class Scaling:
   cdef dict __dict__
   cdef csleqp.SleqpScaling* scaling
   cdef csleqp.SleqpVec* gradient
-  cdef csleqp.SleqpSparseMatrix* cons_jac
+  cdef csleqp.SleqpMat* cons_jac
 
   def __cinit__(self,
                 int num_vars,
                 int num_cons,
                 *args,
                 **keywords):
 
     csleqp_call(csleqp.sleqp_scaling_create(&self.scaling,
                                             num_vars,
                                             num_cons))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&self.gradient,
                                                         num_vars))
 
-    csleqp_call(csleqp.sleqp_sparse_matrix_create(&self.cons_jac,
+    csleqp_call(csleqp.sleqp_mat_create(&self.cons_jac,
                                                   num_cons,
                                                   num_vars,
                                                   0))
 
   @property
   def num_vars(self):
     return csleqp.sleqp_scaling_num_vars(self.scaling)
 
   @property
   def num_cons(self):
     return csleqp.sleqp_scaling_num_cons(self.scaling)
 
   def __dealloc__(self):
-    csleqp_call(csleqp.sleqp_sparse_matrix_release(&self.cons_jac))
+    csleqp_call(csleqp.sleqp_mat_release(&self.cons_jac))
     csleqp_call(csleqp.sleqp_vec_free(&self.gradient))
     csleqp_call(csleqp.sleqp_scaling_release(&self.scaling))
 
   def __str__(self):
     val = "Scaling(num_variables={0}, num_constraints={1})\n".format(self.num_vars,
                                                                      self.num_cons)
```

### Comparing `sleqp-0.1.0/src/extension/sleqp.pyx` & `sleqp-1.0.0/src/extension/sleqp.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 # This has to be the first import
 include "types.pxi"
 
 include "gil.pxi"
 include "call.pxi"
 include "callback.pxi"
 include "cmp.pxi"
+include "dyn.pxi"
 include "sparse.pxi"
 include "sparse_matrix.pxi"
 include "func.pxi"
 include "hess_struct.pxi"
 include "iterate.pxi"
 include "log.pxi"
 include "lsq.pxi"
-include "options.pxi"
-include "params.pxi"
+include "settings.pxi"
 include "problem.pxi"
 include "scale.pxi"
 include "solver.pxi"
 include "version.pxi"
 include "working_set.pxi"
```

### Comparing `sleqp-0.1.0/src/extension/solver.pxi` & `sleqp-1.0.0/src/extension/solver.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -8,45 +8,37 @@
 
   cdef dict __dict__
 
   cdef object __weakref__
 
   cdef csleqp.SleqpSolver* solver
   cdef object problem
-  cdef Params params
-  cdef Options options
   cdef csleqp.SleqpVec* residuals
 
   cdef list callback_handles
 
   def __cinit__(self,
                 object problem,
-                Params params,
-                Options options,
                 np.ndarray primal,
                 Scaling scaling=None):
 
     cdef csleqp.SleqpVec* primal_vec
     cdef _Problem _problem = <_Problem> problem._get_problem()
 
-    self.params = params
-    self.options = options
     self.callback_handles = []
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&primal_vec,
                                                         problem.num_vars))
 
     csleqp_call(csleqp.sleqp_vec_create_empty(&self.residuals, 0))
 
     array_to_sleqp_sparse_vec(primal, primal_vec)
 
     csleqp_call(csleqp.sleqp_solver_create(&self.solver,
                                            _problem.cproblem,
-                                           params.params,
-                                           options.options,
                                            primal_vec,
                                            scaling.scaling if scaling is not None else NULL))
 
     csleqp_call(csleqp.sleqp_vec_free(&primal_vec))
 
     self.problem = problem
```

### Comparing `sleqp-0.1.0/src/extension/sparse.pxi` & `sleqp-1.0.0/src/extension/sparse.pxi`

 * *Files 14% similar despite different names*

```diff
@@ -88,51 +88,50 @@
     matrix = scipy.sparse.csc_matrix(matrix)
 
   assert scipy.sparse.isspmatrix_csc(matrix)
 
   return CSCIterator(matrix)
 
 cdef csleqp.SLEQP_RETCODE matrix_to_sleqp_sparse_matrix(object mat,
-                                                        csleqp.SleqpSparseMatrix* matrix) \
+                                                        csleqp.SleqpMat* matrix) \
                                                         except csleqp.SLEQP_ERROR:
   assert matrix
 
   if mat is None:
     return csleqp.SLEQP_OKAY
 
   assert mat.ndim == 2
 
-  num_rows = csleqp.sleqp_sparse_matrix_num_rows(matrix)
-  num_cols = csleqp.sleqp_sparse_matrix_num_cols(matrix)
+  num_rows = csleqp.sleqp_mat_num_rows(matrix)
+  num_cols = csleqp.sleqp_mat_num_cols(matrix)
 
   assert mat.shape == (num_rows, num_cols)
 
   if num_rows == 0 or num_cols == 0:
     return csleqp.SLEQP_OKAY
 
   cdef int last_col = -1
 
   matrix_iter = matrix_iterator(mat)
 
   for (row, col), data in matrix_iter:
     while last_col != col:
       last_col += 1
-      csleqp_call(csleqp.sleqp_sparse_matrix_push_column(matrix, last_col))
+      csleqp_call(csleqp.sleqp_mat_push_col(matrix, last_col))
 
-    nnz = csleqp.sleqp_sparse_matrix_nnz(matrix)
-    nnz_max = csleqp.sleqp_sparse_matrix_nnz_max(matrix)
+    nnz = csleqp.sleqp_mat_nnz(matrix)
+    nnz_max = csleqp.sleqp_mat_nnz_max(matrix)
 
     if nnz == nnz_max:
-      print("Matrix is full. reserving {0}".format(matrix_iter.length_bound()))
-      csleqp_call(csleqp.sleqp_sparse_matrix_reserve(matrix,
-                                                     matrix_iter.length_bound()))
-
-    csleqp_call(csleqp.sleqp_sparse_matrix_push(matrix,
-                                                row,
-                                                col,
-                                                data))
+      csleqp_call(csleqp.sleqp_mat_reserve(matrix,
+                                           matrix_iter.length_bound()))
 
-  while last_col < csleqp.sleqp_sparse_matrix_num_cols(matrix) - 1:
+    csleqp_call(csleqp.sleqp_mat_push(matrix,
+                                      row,
+                                      col,
+                                      data))
+
+  while last_col < csleqp.sleqp_mat_num_cols(matrix) - 1:
     last_col += 1
-    csleqp_call(csleqp.sleqp_sparse_matrix_push_column(matrix, last_col))
+    csleqp_call(csleqp.sleqp_mat_push_col(matrix, last_col))
 
   return csleqp.SLEQP_OKAY
```

### Comparing `sleqp-0.1.0/src/extension/sparse_matrix.pxi` & `sleqp-1.0.0/src/extension/sparse_matrix.pxi`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 #cython: language_level=3
 
 cimport numpy as np
 
 from scipy.sparse import csc_matrix
 
 cdef class MatrixRef:
-  cdef csleqp.SleqpSparseMatrix* matrix
+  cdef csleqp.SleqpMat* matrix
 
   cdef _release(self):
     if self.matrix:
-      csleqp_call(csleqp.sleqp_sparse_matrix_release(&self.matrix))
+      csleqp_call(csleqp.sleqp_mat_release(&self.matrix))
 
-  cdef _set_matrix(self, csleqp.SleqpSparseMatrix* matrix):
+  cdef _set_matrix(self, csleqp.SleqpMat* matrix):
     self._release()
 
-    csleqp_call(csleqp.sleqp_sparse_matrix_capture(matrix))
+    csleqp_call(csleqp.sleqp_mat_capture(matrix))
 
     self.matrix = matrix
 
   def __dealloc__(self):
     self._release()
 
-cdef object sleqp_sparse_matrix_to_scipy(csleqp.SleqpSparseMatrix* _matrix):
+cdef object sleqp_sparse_matrix_to_scipy(csleqp.SleqpMat* _matrix):
   cdef MatrixRef matrix_ref = MatrixRef()
 
   matrix_ref._set_matrix(_matrix)
 
-  num_cols = csleqp.sleqp_sparse_matrix_num_cols(_matrix)
+  num_cols = csleqp.sleqp_mat_num_cols(_matrix)
 
-  num_rows = csleqp.sleqp_sparse_matrix_num_rows(_matrix)
+  num_rows = csleqp.sleqp_mat_num_rows(_matrix)
 
-  nnz = csleqp.sleqp_sparse_matrix_nnz(_matrix)
+  nnz = csleqp.sleqp_mat_nnz(_matrix)
 
-  data = np.asarray(<double[:nnz]> csleqp.sleqp_sparse_matrix_data(_matrix))
+  data = np.asarray(<double[:nnz]> csleqp.sleqp_mat_data(_matrix))
 
-  indices = np.asarray(<int[:nnz]> csleqp.sleqp_sparse_matrix_rows(_matrix))
+  indices = np.asarray(<int[:nnz]> csleqp.sleqp_mat_rows(_matrix))
 
-  indptr = np.asarray(<int[:num_cols + 1]> csleqp.sleqp_sparse_matrix_cols(_matrix))
+  indptr = np.asarray(<int[:num_cols + 1]> csleqp.sleqp_mat_cols(_matrix))
 
   matrix = csc_matrix((data, indices, indptr), shape=(num_rows, num_cols))
 
   matrix._ref = matrix_ref
 
   return matrix
```

### Comparing `sleqp-0.1.0/src/extension/types.pxi` & `sleqp-1.0.0/src/extension/types.pxi`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,25 @@
 class InitialTRChoice(_DocEnum):
   """
   Choice for initial trust radius
   """
   Narrow = csleqp.SLEQP_INITIAL_TR_CHOICE_NARROW, "Narrow"
   Wide   = csleqp.SLEQP_INITIAL_TR_CHOICE_WIDE, "Wide"
 
+
+class AugJacMethod(_DocEnum):
+  """
+  Augmented Jacobian type
+  """
+  Auto = csleqp.SLEQP_AUG_JAC_AUTO, "Auto"
+  Standard = csleqp.SLEQP_AUG_JAC_STANDARD, "Standard"
+  Reduced = csleqp.SLEQP_AUG_JAC_REDUCED, "Reduced"
+  Direct = csleqp.SLEQP_AUG_JAC_DIRECT, "Direct"
+
+
 class ValueReason(_DocEnum):
   """
   The reason for setting a new function value
   """
   NoReason         = csleqp.SLEQP_VALUE_REASON_NONE, "No reason given"
   Init             = csleqp.SLEQP_VALUE_REASON_INIT, "Initialization"
   CheckingDeriv    = csleqp.SLEQP_VALUE_REASON_CHECKING_DERIV, "Derivative check"
```

### Comparing `sleqp-0.1.0/src/extension/working_set.pxi` & `sleqp-1.0.0/src/extension/working_set.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/_bounds.py` & `sleqp-1.0.0/src/sleqp/_bounds.py`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/_cons.py` & `sleqp-1.0.0/src/sleqp/_cons.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 
 from sleqp._bounds import create_constraint_bounds
 from sleqp._cons_func import create_constraint_func
 
 from sleqp._linear import (create_linear_constraints, LinearConstraints)
 
 
-@dataclass
 class GeneralConstraints:
-  lb: object = np.zeros((0,))
-  func: object = None
-  ub: object = np.zeros((0,))
+  def __init__(self,
+               cons_lb=np.zeros((0,)),
+               cons_func=None,
+               cons_ub=np.zeros((0,))):
+    self.lb = cons_lb
+    self.func = cons_func
+    self.ub = cons_ub
 
 
-@dataclass
 class Constraints:
-  general: object = GeneralConstraints()
-  linear: object = LinearConstraints()
+  def __init__(self,
+               general=GeneralConstraints(),
+               linear=LinearConstraints()):
+    self.general = general
+    self.linear = linear
 
 
 def split_linear_constraints(constraints):
   general = []
   linear = []
 
   for constraint in constraints:
```

### Comparing `sleqp-0.1.0/src/sleqp/_cons_func.py` & `sleqp-1.0.0/src/sleqp/_cons_func.py`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/_derivative.py` & `sleqp-1.0.0/src/sleqp/_derivative.py`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/_func.py` & `sleqp-1.0.0/src/sleqp/_func.py`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/_hessian.py` & `sleqp-1.0.0/src/sleqp/_hessian.py`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/_linear.py` & `sleqp-1.0.0/src/sleqp/_linear.py`

 * *Files identical despite different names*

### Comparing `sleqp-0.1.0/src/sleqp/minimize.py` & `sleqp-1.0.0/src/sleqp/minimize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import numpy as np
 from scipy.optimize import OptimizeResult
 
 import sleqp
 
 from sleqp._bounds import create_variable_bounds
 from sleqp._cons import create_constraints
@@ -18,17 +20,14 @@
     self.args = args
     self.num_variables = num_variables
 
     self._obj_val = None
     self._obj_grad = None
 
   def set_value(self, v, reason):
-    if (self.x == v).all():
-      return
-
     self.x[:] = v
 
     self.objective.set_value(self.x)
 
     if self.constraints:
       self.constraints.set_value(self.x)
 
@@ -58,36 +57,36 @@
       if self._obj_grad.ndim == 2:
         self._obj_grad = self._obj_grad[0,:]
 
   def obj_grad(self):
     self._eval_obj_grad()
     return self._obj_grad
 
-  def hess_prod(self, obj_dual, direction, cons_duals):
+  def hess_prod(self, direction, cons_duals):
     self._eval_obj_grad()
 
     prod = self.objective.hess_prod(direction,
                                     self.args)
 
-    prod *= obj_dual
-
     if self.constraints:
       cons_prod = self.constraints.hess_prod(direction,
                                              cons_duals,
                                              self.args)
       prod += cons_prod
 
     return prod
 
 
 def _create_result(solver):
   solution = solver.solution
 
   result = OptimizeResult()
 
+  result["mult_g"] = solution.cons_dual
+  result["mult_x"] = solution.vars_dual
   result["x"] = solution.primal
   result["success"] = (solver.status == sleqp.Status.Optimal)
   result["status"] = solver.status.value
   result["message"] = solver.status.desc
 
   result["fun"] = solution.obj_val
   result["jac"] = solution.obj_grad
@@ -105,15 +104,66 @@
     if abort is True:
       solver.abort()
 
   solver.add_callback(sleqp.SolverEvent.AcceptedIterate,
                       accepted_iterate)
 
 
-def minimize(fun, x0, args=(), jac=None, hess=None, hessp=None, bounds=None, constraints=None, callback=None):
+_handler = None
+_attached = False
+
+def _attach_handler():
+  global _handler, _attached
+
+  if _handler is None:
+    _handler = logging.StreamHandler()
+    _handler.setLevel(logging.INFO)
+
+  if not(_attached):
+    sleqp.logger.addHandler(_handler)
+    _attached = True
+
+
+def _detach_handler():
+  global _handler, _attached
+
+  if _handler is None:
+    return
+
+  if _attached:
+    sleqp.logger.removeHandler(_handler)
+    _attached = False
+
+
+class LogHelper:
+  def __init__(self, verbose):
+    self.verbose=verbose
+    self.old_level=None
+
+  def __enter__(self):
+    if not(self.verbose):
+      return
+
+    # Set level to at least INFO
+    if sleqp.logger.level < logging.INFO:
+      self.old_level = sleqp.logger.level
+      sleqp.logger.setLevel(logging.INFO)
+
+    _attach_handler()
+
+  def __exit__(self, exc_type, exc_value, exc_tb):
+    if self.verbose:
+      _detach_handler()
+
+    # Restore old level
+    if self.old_level is not None:
+      sleqp.logger.setLevel(self.old_level)
+
+
+def minimize(fun, x0, args=(), jac=None, hess=None, hessp=None, bounds=None, constraints=None, callback=None, **options):
   """
   A drop-in replacement for :func:`scipy.optimize.minimize`, minimizing a scalar function
   of one or more variables subjecting to constraints.
 
   :param fun:
       The objective function to be minimized.
       ``fun(x, *args) -> float``
@@ -135,14 +185,15 @@
         2. Sequence of ``(min, max)`` pairs for each element in `x`. ``None`` is used to specify no bound.
   :type bounds: sequence or :class:`scipy.optimize.Bounds`, optional
   :param callback:
         Called after each iteration. If callback returns True
         the algorithm execution is terminated. The signature is: ``callback(xk)``
         where ``xk`` is the current guess.
   :type callback: callable, optional
+
   :return: The optimization result
   :rtype: :class:`scipy.optimize.Optimizeresult`
   """
   if not isinstance(args, tuple):
     args = (args,)
 
   num_variables = len(x0)
@@ -151,44 +202,43 @@
   cons_ub = np.zeros((0,))
   cons_func = None
 
   constraints = create_constraints(num_variables, constraints)
 
   objective = create_func(fun, jac, hess, hessp)
 
-  options = sleqp.Options()
+  verbose = options.pop('verbose', False)
+
+  settings = sleqp.Settings(**options)
 
   if hessp is None and hess is None:
-    options.hessian_eval = sleqp.HessianEval.DampedBFGS
+    settings.hessian_eval = sleqp.HessianEval.DampedBFGS
 
   initial_sol = np.array(x0)
 
   (var_lb, var_ub) = create_variable_bounds(num_variables, bounds)
 
   min_func = _MinFunc(objective,
                       constraints.general.func,
                       args,
                       num_variables)
 
-  params = sleqp.Params()
-
   problem = sleqp.Problem(min_func,
-                          params,
                           var_lb,
                           var_ub,
                           constraints.general.lb,
                           constraints.general.ub,
+                          settings,
                           linear_coeffs=constraints.linear.coeffs,
                           linear_lb=constraints.linear.lb,
                           linear_ub=constraints.linear.ub)
 
   solver = sleqp.Solver(problem,
-                        params,
-                        options,
                         initial_sol)
 
   if callback is not None:
     _add_solver_callback(solver, callback)
 
-  solver.solve(100, 3600)
+  with LogHelper(verbose):
+    solver.solve()
 
   return _create_result(solver)
```

### Comparing `sleqp-0.1.0/src/sleqp.egg-info/PKG-INFO` & `sleqp-1.0.0/src/sleqp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleqp
-Version: 0.1.0
+Version: 1.0.0
 Summary: Active set-based NLP solver
 Author: Christoph Hansknecht
 Author-email: c.hansknecht@tu-braunschweig.de
 Classifier: Programming Language :: Cython
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: LICENSE.txt
```

### Comparing `sleqp-0.1.0/src/sleqp.egg-info/SOURCES.txt` & `sleqp-1.0.0/src/sleqp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 LICENSE.txt
 MANIFEST.in
 pyproject.toml
 requirements.txt
 setup.py
-src/sleqp.c
 src/extension/call.pxi
 src/extension/callback.pxi
 src/extension/cmp.pxi
 src/extension/csleqp.pxd
+src/extension/dyn.pxi
 src/extension/func.pxi
 src/extension/gil.pxi
 src/extension/hess_struct.pxi
 src/extension/iterate.pxi
 src/extension/log.pxi
 src/extension/lsq.pxi
-src/extension/options.pxi
-src/extension/params.pxi
 src/extension/problem.pxi
 src/extension/scale.pxi
-src/extension/sleqp.c
+src/extension/settings.pxi
 src/extension/sleqp.pyx
 src/extension/solver.pxi
 src/extension/sparse.pxi
 src/extension/sparse_matrix.pxi
 src/extension/types.pxi
 src/extension/version.pxi
 src/extension/working_set.pxi
```

