# Comparing `tmp/pspy-1.6.1.tar.gz` & `tmp/pspy-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspy-1.6.1.tar", last modified: Thu May 11 11:55:20 2023, max compression
+gzip compressed data, was "pspy-1.6.2.tar", last modified: Fri Jun  9 10:52:37 2023, max compression
```

## Comparing `pspy-1.6.1.tar` & `pspy-1.6.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-11 11:55:12.000000 pspy-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 11:55:12.000000 pspy-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 11:55:20.488767 pspy-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-11 11:55:12.000000 pspy-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/pspy/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 11:55:20.488767 pspy-1.6.1/pspy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/cov_fortran/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/cov_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/cov_fortran/cov_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/flat_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/mcm_fortran/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/mcm_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/mcm_fortran/mcm_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/pspy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    35346 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_map_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_mcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/so_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/sph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.472767 pspy-1.6.1/pspy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/tests/data/generate_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-11 11:55:12.000000 pspy-1.6.1/pspy/tests/data/parameters_test_data.yml
--rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/data/test_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_pspy_namaster.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_so_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_so_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/tests/test_so_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/pspy/wigner3j/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/wigner3j/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-05-11 11:55:13.000000 pspy-1.6.1/pspy/wigner3j/wigner3j_sub.f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.468767 pspy-1.6.1/pspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 11:55:20.000000 pspy-1.6.1/pspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:55:20.488767 pspy-1.6.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-05-11 11:55:13.000000 pspy-1.6.1/scripts/test-pspy
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-11 11:55:20.488767 pspy-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-11 11:55:13.000000 pspy-1.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-11 11:55:13.000000 pspy-1.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-09 10:52:30.000000 pspy-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 10:52:30.000000 pspy-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-09 10:52:37.503988 pspy-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-09 10:52:30.000000 pspy-1.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/pspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 10:52:37.503988 pspy-1.6.2/pspy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/cov_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/cov_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/cov_fortran/cov_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/flat_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/mcm_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/mcm_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/mcm_fortran/mcm_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/pspy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39436 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_map_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_mcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/sph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/generate_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/parameters_test_data.yml
+-rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/test_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_pspy_namaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_so_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/pspy/wigner3j/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/wigner3j/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/wigner3j/wigner3j_sub.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-06-09 10:52:30.000000 pspy-1.6.2/scripts/test-pspy
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 10:52:37.503988 pspy-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-09 10:52:30.000000 pspy-1.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-09 10:52:30.000000 pspy-1.6.2/versioneer.py
```

### Comparing `pspy-1.6.1/LICENSE` & `pspy-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/PKG-INFO` & `pspy-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
```

### Comparing `pspy-1.6.1/README.rst` & `pspy-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/cov_fortran/cov_fortran.f90` & `pspy-1.6.2/pspy/cov_fortran/cov_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/flat_tools.py` & `pspy-1.6.2/pspy/flat_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/mcm_fortran/mcm_fortran.f90` & `pspy-1.6.2/pspy/mcm_fortran/mcm_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/pspy_utils.py` & `pspy-1.6.2/pspy/pspy_utils.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_config.py` & `pspy-1.6.2/pspy/so_config.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_consistency.py` & `pspy-1.6.2/pspy/so_consistency.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_cov.py` & `pspy-1.6.2/pspy/so_cov.py`

 * *Files 5% similar despite different names*

```diff
@@ -430,15 +430,16 @@
                   coupling_dict,
                   binning_file,
                   lmax,
                   mbb_inv_ab,
                   mbb_inv_cd,
                   binned_mcm=True,
                   cov_T_E_only=True,
-                  dtype=np.float64):
+                  dtype=np.float64,
+                  old_way=False):
                   
     """From the two point functions and the coupling kernel construct the T and E analytical covariance matrix of <(C_ab- Clth)(C_cd-Clth)>
 
     Parameters
     ----------
 
     Clth_dict: dictionnary
@@ -491,39 +492,50 @@
             M = Cl0Cl1 * coupling_dict[id0 + id1]
             M += Cl2Cl3 * coupling_dict[id2 + id3]
 
             full_analytic_cov[i * n_ell:(i + 1) * n_ell, j * n_ell:(j + 1) * n_ell] = M
     
     full_analytic_cov = np.triu(full_analytic_cov) + np.tril(full_analytic_cov.T, -1)
     
-    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype)
-    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype)
-
-    if binned_mcm == True:
-        analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
-        analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
+    if old_way == True:
+        mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype)
+        mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype)
+        if binned_mcm == True:
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
+            analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
+        else:
+            full_analytic_cov = mbb_inv_ab @ full_analytic_cov @ mbb_inv_cd.T
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
     else:
-        full_analytic_cov = mbb_inv_ab @ full_analytic_cov @ mbb_inv_cd.T
-        analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
+        slices, mbb_inv_ab_list = extract_mbb_list(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype, transpose=False)
+        slices, mbb_inv_cd_list = extract_mbb_list(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype, transpose=True)
+        if binned_mcm == True:
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
+            analytic_cov = block_diagonal_mult(slices, mbb_inv_ab_list, mbb_inv_cd_list, analytic_cov)
+        else:
+            full_analytic_cov = block_diagonal_mult(slices, mbb_inv_ab_list, mbb_inv_cd_list, full_analytic_cov)
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
 
     return analytic_cov
 
+
 def generalized_cov_spin0and2(coupling_dict,
                               id_element,
                               ns,
                               ps_all,
                               nl_all,
                               lmax,
                               binning_file,
                               mbb_inv_ab,
                               mbb_inv_cd,
                               binned_mcm=True,
                               return_full_cov=False,
                               cov_T_E_only=True,
-                              dtype=np.float64):
+                              dtype=np.float64,
+                              old_way=False):
 
     """
     This routine deserves some explanation
     We want to compute the covariance between two power spectra
     C1 = Wa * Xb, C2 =  Yc * Zd
     Here W, X, Y, Z can be either T or E and a,b,c,d will be an index
     corresponding to the survey and array we consider so for example a = s17&pa5_150 or a = dr6&pa4_090
@@ -588,27 +600,34 @@
                 id3 = id3.replace(field, "P")
 
         
             M = coupling_dict[id0 + id1] * chi(na, nc, nb, nd, ns, ps_all, nl_all, W + Y + X + Z)
             M += coupling_dict[id2 + id3] * chi(na, nd, nb, nc, ns, ps_all, nl_all, W + Z + X + Y)
             full_analytic_cov[i * n_ell: (i + 1) * n_ell, j * n_ell: (j + 1) * n_ell] = M
 
-    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype)
-    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype)
-
-    if binned_mcm == True:
-        analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
-        analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
+    if old_way == True:
+        mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype)
+        mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype)
+        if binned_mcm == True:
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
+            analytic_cov = mbb_inv_ab @ analytic_cov @ mbb_inv_cd.T
+        else:
+            full_analytic_cov = mbb_inv_ab @ full_analytic_cov @ mbb_inv_cd.T
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
     else:
-        full_analytic_cov = mbb_inv_ab @ full_analytic_cov @ mbb_inv_cd.T
-        if return_full_cov == True:
-            return full_analytic_cov
-
-        analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
-
+        slices, mbb_inv_ab_list = extract_mbb_list(mbb_inv_ab, cov_T_E_only=cov_T_E_only, dtype=dtype, transpose=False)
+        slices, mbb_inv_cd_list = extract_mbb_list(mbb_inv_cd, cov_T_E_only=cov_T_E_only, dtype=dtype, transpose=True)
+        if binned_mcm == True:
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
+            analytic_cov = block_diagonal_mult(slices, mbb_inv_ab_list, mbb_inv_cd_list, analytic_cov)
+        else:
+            full_analytic_cov = block_diagonal_mult(slices, mbb_inv_ab_list, mbb_inv_cd_list, full_analytic_cov)
+            analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
+            
+            
     return analytic_cov
 
 
 def covariance_element_beam(id_element,
                             ps_all,
                             norm_beam_cov,
                             binning_file,
@@ -668,22 +687,107 @@
             M *=  np.outer(ps_all[na, nb, spec1], ps_all[nc, nd, spec2])
         
             analytic_cov_from_beam[i * nbins: (i + 1) * nbins, j * nbins: (j + 1) * nbins] = bin_mat(M, binning_file, lmax)
 
     return analytic_cov_from_beam
 
 
+def block_diagonal_mult(slices, mbb_inv_ab_list, mbb_inv_cd_list, analytic_cov):
+
+    """Suggestion by adrien to do an operation of the type A M B, where A and B are block diagonal matrix
+    Parameters
+    ----------
+    slices: list of tuple of integer
+        give the min and max indices of each block
+    mbb_inv_ab_list: list of 2d array
+        list of the inverse of the mode coupling matrix
+    mbb_inv_cd_list: list of 2d array
+        list of the transpose of the inverse of the mode coupling matrix
+    analytic_cov: 2d array
+        analytic covariance matrix
+    
+    """
+    nblocks = len(slices)
+    
+    for i in range(nblocks):
+        for j in range(nblocks):
+        
+            min_i, max_i = slices[i]
+            min_j, max_j = slices[j]
+
+            analytic_cov[min_i: max_i, min_j: max_j] = mbb_inv_ab_list[i] @ analytic_cov[min_i: max_i, min_j: max_j] @ mbb_inv_cd_list[j]
+            
+    return analytic_cov
+
+def extract_mbb_list(mbb_inv,
+                     cov_T_E_only=True,
+                     dtype=np.float64,
+                     transpose=False):
+                     
+    """extract a list of inverse mode coupling matrix, you can optionnaly choose the dtype, if you want only the TT-TE-ET-EE part,
+    and if you want to transpose it
+
+    Parameters
+    ----------
+
+    mbb_inv: dict of 2d arrays
+      the inverse spin0 and 2 mode coupling matrix
+    cov_T_E_only: boolean
+        if true don't do B
+    dtype: np dtype
+        choose the type to save memory
+    transpose: boolean
+        wether to transpose it or not
+    """
+
+
+    nbins = mbb_inv["spin0xspin0"].shape[0]
+    slices = []
+    
+    if cov_T_E_only == False:
+
+        nblocks = 6
+        for i in range(nblocks - 1):
+            slices += [(i * nbins, (i + 1) * nbins)]
+        slices += [(5 * nbins, 9 * nbins)] # the EE-EB-BE-BB block
+
+        mbb_list = [mbb_inv["spin0xspin0"],
+                    mbb_inv["spin0xspin2"],
+                    mbb_inv["spin0xspin2"],
+                    mbb_inv["spin2xspin0"],
+                    mbb_inv["spin2xspin0"],
+                    mbb_inv["spin2xspin2"]]
+    else:
+    
+        nblocks = 4
+        for i in range(nblocks):
+            slices += [(i * nbins, (i + 1) * nbins)]
+
+        mbb_list = [mbb_inv["spin0xspin0"],
+                    mbb_inv["spin0xspin2"],
+                    mbb_inv["spin2xspin0"],
+                    mbb_inv["spin2xspin2"][0:nbins, 0:nbins]]
+
+    for i in range(nblocks):
+        if mbb_list[i].dtype != dtype:
+            mbb_list[i] = mbb_list[i].astype(dtype)
+        if transpose == True:
+            mbb_list[i] = mbb_list[i].T
+    
+    return slices, mbb_list
+
+
+
 def extract_mbb(mbb_inv, cov_T_E_only=True, dtype=np.float64):
-    """The mode coupling marix is computed for T,E,B but for now we only construct analytical covariance matrix for T and E
-    The B modes is complex with important E->B leakage, this routine extract the T and E part of the mode coupling matrix
+    """The mode coupling marix is computed for T,E,B but for if cov_T_E_only=True we only construct analytical covariance matrix for T and E
 
     Parameters
     ----------
 
-    mbb_inv: 2d array
+    mbb_inv: dict of 2d arrays
       the inverse spin0 and 2 mode coupling matrix
     cov_T_E_only: boolean
         if true don't do B
     """
     nbins = mbb_inv["spin0xspin0"].shape[0]
     if cov_T_E_only:
         mbb_inv_array = np.zeros((4*nbins, 4*nbins), dtype=dtype)
```

### Comparing `pspy-1.6.1/pspy/so_dict.py` & `pspy-1.6.2/pspy/so_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,13 +70,12 @@
         f.close()
 
     readFromFile = read_from_file
 
     def write_to_file(self, filename, mode="w"):
         f = open(filename, mode)
         keys = self.keys()
-        keys.sort()
         for key in keys:
             f.write("%s = %s\n" % (key, repr(self[key])))
         f.close()
 
     writeToFile = write_to_file
```

### Comparing `pspy-1.6.1/pspy/so_map.py` & `pspy-1.6.2/pspy/so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_map_preprocessing.py` & `pspy-1.6.2/pspy/so_map_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_mcm.py` & `pspy-1.6.2/pspy/so_mcm.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_misc.py` & `pspy-1.6.2/pspy/so_misc.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_mpi.py` & `pspy-1.6.2/pspy/so_mpi.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_spectra.py` & `pspy-1.6.2/pspy/so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/so_window.py` & `pspy-1.6.2/pspy/so_window.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/sph_tools.py` & `pspy-1.6.2/pspy/sph_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat` & `pspy-1.6.2/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/tests/data/generate_test_data.py` & `pspy-1.6.2/pspy/tests/data/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/tests/data/test_data.pkl` & `pspy-1.6.2/pspy/tests/data/test_data.pkl`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/tests/test_pspy_namaster.py` & `pspy-1.6.2/pspy/tests/test_pspy_namaster.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Tests pspy versus namaster."""
 import os
 import tempfile
+import time
 import unittest
 
 import healpy as hp
 import numpy as np
+import pspy
 from pspy import pspy_utils, so_map, so_mcm, so_spectra, so_window, sph_tools
 
 
 def _assert_import(pkg_name):
     try:
         import importlib
 
@@ -111,19 +113,27 @@
     Clb["ET"] = Clb["TE"]
     Clb["BT"] = Clb["TB"]
     return lb, Clb
 
 
 class SOPspyNamasterTests(unittest.TestCase):
     def setUp(self):
+        print(f"pspy current version : {pspy.__version__}")
+        # This sould be fixed see https://github.com/LSSTDESC/NaMaster/issues/172
+        # print(f"namaster current version : {nmt.__version__}")
         pass
 
     def test_pspy_namaster(self):
+        t0 = time.time()
         lb_pspy, Clb_pspy = run_pspy()
+        print(f"pspy runs in {time.time() - t0:.2f} seconds")
+
+        t0 = time.time()
         lb_nmt, Clb_nmt = run_namaster()
+        print(f"namaster runs in {time.time() - t0:.2f} seconds")
 
         decimal = 12
         for spec in spectra:
             msg = f"Testing {spec} spectrum"
             np.testing.assert_almost_equal(
                 Clb_pspy[spec], Clb_nmt[spec], err_msg=msg, decimal=decimal
             )
```

### Comparing `pspy-1.6.1/pspy/tests/test_so_dict.py` & `pspy-1.6.2/pspy/tests/test_so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/tests/test_so_map.py` & `pspy-1.6.2/pspy/tests/test_so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/tests/test_so_spectra.py` & `pspy-1.6.2/pspy/tests/test_so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy/wigner3j/wigner3j_sub.f` & `pspy-1.6.2/pspy/wigner3j/wigner3j_sub.f`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/pspy.egg-info/PKG-INFO` & `pspy-1.6.2/pspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
```

### Comparing `pspy-1.6.1/pspy.egg-info/SOURCES.txt` & `pspy-1.6.2/pspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/setup.py` & `pspy-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.1/versioneer.py` & `pspy-1.6.2/versioneer.py`

 * *Files identical despite different names*

