# Comparing `tmp/pyspk-1.4.tar.gz` & `tmp/pyspk-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspk-1.4.tar", last modified: Fri Jun  9 16:28:32 2023, max compression
+gzip compressed data, was "pyspk-1.5.tar", last modified: Fri Jun  9 17:01:36 2023, max compression
```

## Comparing `pyspk-1.4.tar` & `pyspk-1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 16:28:32.856931 pyspk-1.4/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.4/LICENSE.md
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.4/MANIFEST.in
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 16:28:32.856725 pyspk-1.4/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8667 2023-06-09 16:28:12.000000 pyspk-1.4/README.md
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 16:28:32.855882 pyspk-1.4/pyspk/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/__init__.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/fit_vals.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/model.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/stat_errors_200.csv
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/stat_errors_500.csv
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 16:28:32.856549 pyspk-1.4/pyspk.egg-info/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      288 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/SOURCES.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/dependency_links.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/requires.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/top_level.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-09 16:28:32.856965 pyspk-1.4/setup.cfg
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-09 16:28:12.000000 pyspk-1.4/setup.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 17:01:36.912228 pyspk-1.5/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.5/LICENSE.md
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.5/MANIFEST.in
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 17:01:36.912026 pyspk-1.5/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     8667 2023-06-09 16:28:12.000000 pyspk-1.5/README.md
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 17:01:36.910767 pyspk-1.5/pyspk/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/__init__.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/fit_vals.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2023-06-09 16:47:49.000000 pyspk-1.5/pyspk/model.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/stat_errors_200.csv
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/stat_errors_500.csv
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 17:01:36.911880 pyspk-1.5/pyspk.egg-info/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      288 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/SOURCES.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/dependency_links.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/requires.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/top_level.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-09 17:01:36.912266 pyspk-1.5/setup.cfg
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-09 17:01:19.000000 pyspk-1.5/setup.py
```

### Comparing `pyspk-1.4/LICENSE.md` & `pyspk-1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.4/PKG-INFO` & `pyspk-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.4
+Version: 1.5
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyspk-1.4/README.md` & `pyspk-1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.4/pyspk/fit_vals.py` & `pyspk-1.5/pyspk/fit_vals.py`

 * *Files identical despite different names*

### Comparing `pyspk-1.4/pyspk/model.py` & `pyspk-1.5/pyspk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """
     y = vals[2] * _np.power(x, 2) + vals[1] * x + vals[0] 
     return y
 
 
 def _optimal_mass_funct(k, params):
     """
-    Optimal mass function defined in eq.(2) in Salcido et al. (2022).
+    Optimal mass function defined in eq.(2) in Salcido et al. (2023).
 
     Parameters
     ----------
     k : array of float
         co-moving wavenumber in units [h/Mpc]
     prams : dict
         dictionary containing the best fitting parameters of the SP(k) model at a specific redshift. 
@@ -71,15 +71,15 @@
     output = params['alpha'] - (params['alpha'] - params['beta']) * _np.power(k, params['gamma'])
     return output
 
 
 def optimal_mass(SO, z, k, verbose=False):
     """
     Optimal mass function as a function of scale and redshift for a specific 
-    spherical over-density. Defined in eq.(2) in Salcido et al. (2022).
+    spherical over-density. Defined in eq.(2) in Salcido et al. (2023).
 
     Parameters
     ----------
     SO : int
         spherical over-density. Only accepts 200 or 500
     z : float
         redshift z. Only accepts values of z <= 3
@@ -104,15 +104,15 @@
     params = _get_params(SO, z)
     output = params['alpha'] - (params['alpha'] - params['beta']) * _np.power(k, params['gamma'])
     return _np.power(10, output)
 
 
 def _lambda_funct(x, params):
     """
-    lambda function for a specific redshift. Defined in eq.(6) in Salcido et al. (2022).
+    lambda function for a specific redshift. Defined in eq.(6) in Salcido et al. (2023).
 
     Parameters
     ----------
     k : array of float
         co-moving wavenumber in units [h/Mpc]
     prams : dict
         dictionary containing the best fitting parameters of the SP(k) model at a specific redshift. 
@@ -124,15 +124,15 @@
     """
     output = 1 + params['lambda_a'] * _np.exp(params['lambda_b'] * x)
     return output
 
 
 def _mu_funct(x, params):
     """
-    mu function for a specific redshift. Defined in eq.(7) in Salcido et al. (2022).
+    mu function for a specific redshift. Defined in eq.(7) in Salcido et al. (2023).
 
     Parameters
     ----------
     k : array of float
         co-moving wavenumber in units [h/Mpc]
     prams : dict
         dictionary containing the best fitting parameters of the SP(k) model at a specific redshift. 
@@ -147,15 +147,15 @@
     C = 1 + _np.exp(params['mu_b'] * x + params['mu_c'])
     output = A + (B / C)
     return output
 
 
 def _nu_func(x, params):
     """
-    nu function for a specific redshift. Defined in eq.(8) in Salcido et al. (2022).
+    nu function for a specific redshift. Defined in eq.(8) in Salcido et al. (2023).
 
     Parameters
     ----------
     k : array of float
         co-moving wavenumber in units [h/Mpc]
     prams : dict
         dictionary containing the best fitting parameters of the SP(k) model at a specific redshift. 
@@ -308,15 +308,15 @@
         sets the Akino power law redshift dependence. 
     cosmo: astropy cosmology object, optional
         astropy cosmology object with the desired cosmology
     k_min : float, default 0.1
         minimum co-moving wavenumber in units [h/Mpc]
     k_max : float, default 8, max 12
         maximum co-moving wavenumber in units [h/Mpc]. Default is set to the Nyquist frequency of the Antilles
-        simulations (see Salcido et al. 2022). 
+        simulations (see Salcido et al. 2023). 
     n : int, default 100
         number of equally spaced co-moving wavenumber in log-spaced between k_min and k_max.
     errors : boolean, default False
         enables additional output with the bootstrapped 68% and 95% confidence intervals from statistical errors.
     verbose : boolean, default True
         run in verbose mode
         
@@ -334,15 +334,15 @@
         array with the -2 sigma confidence interval 
     error_95_p : array of float, optional
         array with the +2 sigma confidence interval 
 
     Notes
     ----------
     The maximum co-moving wavenumber in units [h/Mpc] is set to the Nyquist frequency of the Antilles simulations 
-    (see Salcido et al. 2022). Although SP(k) was fitted up to k = 12 [h/Mpc], we caution the user that setting 
+    (see Salcido et al. 2023). Although SP(k) was fitted up to k = 12 [h/Mpc], we caution the user that setting 
     𝑘 > 𝑘Ny (8 [h/Mpc]) might not be representative of the true uncertainties in the data. 
     """
 
     if z < 0:
         raise Exception('\033[91mIncorrect redshift.\033[0m') from None
         
     if z > 3:
```

### Comparing `pyspk-1.4/pyspk/stat_errors_200.csv` & `pyspk-1.5/pyspk/stat_errors_200.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.4/pyspk/stat_errors_500.csv` & `pyspk-1.5/pyspk/stat_errors_500.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.4/pyspk.egg-info/PKG-INFO` & `pyspk-1.5/pyspk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.4
+Version: 1.5
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyspk-1.4/setup.py` & `pyspk-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     print(long_description)
 
 setuptools.setup(
     name="pyspk",
-    version=1.4,
+    version=1.5,
     description="Python package to predict the suppression of the total matter power spectrum due to baryonic physics",
     url="https://github.com/jemme07/pyspk",
     author="Jaime Salcido",
     author_email="j.salcidonegrete@ljmu.ac.uk",
     packages=['pyspk'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

