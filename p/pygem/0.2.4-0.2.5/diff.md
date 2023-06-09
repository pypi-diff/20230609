# Comparing `tmp/pygem-0.2.4.tar.gz` & `tmp/pygem-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygem-0.2.4.tar", last modified: Fri Jun  9 18:06:54 2023, max compression
+gzip compressed data, was "pygem-0.2.5.tar", last modified: Fri Jun  9 18:36:47 2023, max compression
```

## Comparing `pygem-0.2.4.tar` & `pygem-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.631522 pygem-0.2.4/
--rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2020-11-22 15:57:18.000000 pygem-0.2.4/.gitignore
--rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2020-11-22 15:57:18.000000 pygem-0.2.4/LICENSE
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.623151 pygem-0.2.4/LICENSES/
--rw-r--r--   0 drounce    (501) staff       (20)     1522 2023-06-07 04:01:43.000000 pygem-0.2.4/LICENSES/OGGM_LICENSE.txt
--rw-r--r--   0 drounce    (501) staff       (20)     2442 2023-06-09 18:06:54.631714 pygem-0.2.4/PKG-INFO
--rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 04:01:43.000000 pygem-0.2.4/README.md
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.625669 pygem-0.2.4/pygem/
--rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-09 18:06:11.000000 pygem-0.2.4/pygem/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    17559 2023-06-09 18:01:53.000000 pygem-0.2.4/pygem/class_climate.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    14035 2023-06-09 15:31:45.000000 pygem-0.2.4/pygem/gcmbiasadj.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 03:54:10.000000 pygem-0.2.4/pygem/glacierdynamics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 04:01:43.000000 pygem-0.2.4/pygem/massbalance.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 03:54:10.000000 pygem-0.2.4/pygem/oggm_compat.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    23592 2023-06-07 17:03:36.000000 pygem-0.2.4/pygem/pygem_modelsetup.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.628372 pygem-0.2.4/pygem/scraps/
--rwxr-xr-x   0 drounce    (501) staff       (20)      529 2020-11-22 15:57:18.000000 pygem-0.2.4/pygem/scraps/dummy_task_module.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2020-11-22 15:57:18.000000 pygem-0.2.4/pygem/scraps/run.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.629562 pygem-0.2.4/pygem/shop/
--rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2021-02-01 14:09:24.000000 pygem-0.2.4/pygem/shop/debris.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2021-09-23 17:13:56.000000 pygem-0.2.4/pygem/shop/icethickness.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12423 2023-06-09 18:04:23.000000 pygem-0.2.4/pygem/shop/mbdata.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.630581 pygem-0.2.4/pygem/tests/
--rwxr-xr-x   0 drounce    (501) staff       (20)        0 2020-11-22 15:57:18.000000 pygem-0.2.4/pygem/tests/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)      149 2020-11-22 15:57:18.000000 pygem-0.2.4/pygem/tests/test_basics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2020-11-22 15:57:18.000000 pygem-0.2.4/pygem/tests/test_oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.631215 pygem-0.2.4/pygem/utils/
--rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2021-01-10 16:41:45.000000 pygem-0.2.4/pygem/utils/_funcs.py
--rw-r--r--   0 drounce    (501) staff       (20)     2651 2022-06-13 02:59:07.000000 pygem-0.2.4/pygem/utils/_funcs_selectglaciers.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:06:54.627454 pygem-0.2.4/pygem.egg-info/
--rw-r--r--   0 drounce    (501) staff       (20)     2442 2023-06-09 18:06:54.000000 pygem-0.2.4/pygem.egg-info/PKG-INFO
--rw-r--r--   0 drounce    (501) staff       (20)      651 2023-06-09 18:06:54.000000 pygem-0.2.4/pygem.egg-info/SOURCES.txt
--rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-09 18:06:54.000000 pygem-0.2.4/pygem.egg-info/dependency_links.txt
--rw-r--r--   0 drounce    (501) staff       (20)       72 2023-06-09 18:06:54.000000 pygem-0.2.4/pygem.egg-info/requires.txt
--rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-09 18:06:54.000000 pygem-0.2.4/pygem.egg-info/top_level.txt
--rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-09 18:05:50.000000 pygem-0.2.4/pyproject.toml
--rwxr-xr-x   0 drounce    (501) staff       (20)     1008 2023-06-09 18:06:54.632364 pygem-0.2.4/setup.cfg
--rwxr-xr-x   0 drounce    (501) staff       (20)      539 2023-06-09 17:01:16.000000 pygem-0.2.4/setup.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.317629 pygem-0.2.5/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2020-11-22 15:57:18.000000 pygem-0.2.5/.gitignore
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2020-11-22 15:57:18.000000 pygem-0.2.5/LICENSE
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.307407 pygem-0.2.5/LICENSES/
+-rw-r--r--   0 drounce    (501) staff       (20)     1522 2023-06-07 04:01:43.000000 pygem-0.2.5/LICENSES/OGGM_LICENSE.txt
+-rw-r--r--   0 drounce    (501) staff       (20)     2442 2023-06-09 18:36:47.317839 pygem-0.2.5/PKG-INFO
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 04:01:43.000000 pygem-0.2.5/README.md
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.311444 pygem-0.2.5/pygem/
+-rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-09 18:35:31.000000 pygem-0.2.5/pygem/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    17559 2023-06-09 18:01:53.000000 pygem-0.2.5/pygem/class_climate.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    14055 2023-06-09 18:24:58.000000 pygem-0.2.5/pygem/gcmbiasadj.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    48927 2023-06-09 18:27:23.000000 pygem-0.2.5/pygem/glacierdynamics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    60877 2023-06-09 18:30:17.000000 pygem-0.2.5/pygem/massbalance.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12718 2023-06-09 18:31:01.000000 pygem-0.2.5/pygem/oggm_compat.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    23586 2023-06-09 18:31:25.000000 pygem-0.2.5/pygem/pygem_modelsetup.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.314629 pygem-0.2.5/pygem/scraps/
+-rwxr-xr-x   0 drounce    (501) staff       (20)      529 2020-11-22 15:57:18.000000 pygem-0.2.5/pygem/scraps/dummy_task_module.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2020-11-22 15:57:18.000000 pygem-0.2.5/pygem/scraps/run.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.315549 pygem-0.2.5/pygem/shop/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     7777 2023-06-09 18:31:50.000000 pygem-0.2.5/pygem/shop/debris.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     5057 2023-06-09 18:31:58.000000 pygem-0.2.5/pygem/shop/icethickness.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12423 2023-06-09 18:04:23.000000 pygem-0.2.5/pygem/shop/mbdata.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.316570 pygem-0.2.5/pygem/tests/
+-rwxr-xr-x   0 drounce    (501) staff       (20)        0 2020-11-22 15:57:18.000000 pygem-0.2.5/pygem/tests/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)      149 2020-11-22 15:57:18.000000 pygem-0.2.5/pygem/tests/test_basics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2020-11-22 15:57:18.000000 pygem-0.2.5/pygem/tests/test_oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.317242 pygem-0.2.5/pygem/utils/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2298 2023-06-09 18:32:57.000000 pygem-0.2.5/pygem/utils/_funcs.py
+-rw-r--r--   0 drounce    (501) staff       (20)     2651 2022-06-13 02:59:07.000000 pygem-0.2.5/pygem/utils/_funcs_selectglaciers.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 18:36:47.313898 pygem-0.2.5/pygem.egg-info/
+-rw-r--r--   0 drounce    (501) staff       (20)     2442 2023-06-09 18:36:47.000000 pygem-0.2.5/pygem.egg-info/PKG-INFO
+-rw-r--r--   0 drounce    (501) staff       (20)      651 2023-06-09 18:36:47.000000 pygem-0.2.5/pygem.egg-info/SOURCES.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-09 18:36:47.000000 pygem-0.2.5/pygem.egg-info/dependency_links.txt
+-rw-r--r--   0 drounce    (501) staff       (20)       72 2023-06-09 18:36:47.000000 pygem-0.2.5/pygem.egg-info/requires.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-09 18:36:47.000000 pygem-0.2.5/pygem.egg-info/top_level.txt
+-rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-09 18:35:05.000000 pygem-0.2.5/pyproject.toml
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1008 2023-06-09 18:36:47.318615 pygem-0.2.5/setup.cfg
+-rwxr-xr-x   0 drounce    (501) staff       (20)      539 2023-06-09 17:01:16.000000 pygem-0.2.5/setup.py
```

### Comparing `pygem-0.2.4/.gitignore` & `pygem-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/LICENSE` & `pygem-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/LICENSES/OGGM_LICENSE.txt` & `pygem-0.2.5/LICENSES/OGGM_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/PKG-INFO` & `pygem-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
 Home-page: https://github.com/drounce/PyGEM
 Author: David Rounce
 Author-email: David Rounce <drounce@cmu.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygem-0.2.4/README.md` & `pygem-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem/class_climate.py` & `pygem-0.2.5/pygem/class_climate.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem/gcmbiasadj.py` & `pygem-0.2.5/pygem/gcmbiasadj.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Run bias adjustments a given climate dataset"""
 
 # External libraries
 import numpy as np
 from scipy.ndimage import uniform_filter
-# Local libraries
-import pygem.pygem_input as pygem_prms
 
 
 #%% FUNCTIONS
 def annual_avg_2darray(x):
     """
     Annual average of dataset, where columns are a monthly timeseries (temperature)
     """
@@ -32,15 +30,16 @@
 def monthly_std_2darray(x):
     """
     Monthly standard deviation for a given 2d dataset where columns are monthly timeseries
     """
     return x.reshape(-1,12).transpose().reshape(-1,int(x.shape[1]/12)).std(1).reshape(12,-1).transpose()
 
     
-def temp_biasadj_HH2015(ref_temp, ref_elev, gcm_temp, dates_table_ref, dates_table):
+def temp_biasadj_HH2015(ref_temp, ref_elev, gcm_temp, dates_table_ref, dates_table, 
+                        ref_spinupyears=0, gcm_spinupyears=0):
     """
     Huss and Hock (2015) temperature bias correction based on mean and interannual variability
     
     Note: the mean over the reference period will only equal the mean of the gcm for the same time period when the GCM
     time series is run for the same period, i.e., due to the 25-year moving average, the mean gcm temps from 2000-2019
     will differ if using a reference period of 2000-2020 to bias adjust gcm temps from 2000-2100.
     
@@ -64,16 +63,16 @@
     """
     # GCM subset to agree with reference time period to calculate bias corrections
     gcm_subset_idx_start = np.where(dates_table.date.values == dates_table_ref.date.values[0])[0][0]
     gcm_subset_idx_end = np.where(dates_table.date.values == dates_table_ref.date.values[-1])[0][0]
     gcm_temp_subset = gcm_temp[:,gcm_subset_idx_start:gcm_subset_idx_end+1]
 
     # Remove spinup years, so adjustment performed over calibration period
-    ref_temp_nospinup = ref_temp[:,pygem_prms.ref_spinupyears*12:]
-    gcm_temp_nospinup = gcm_temp_subset[:,pygem_prms.gcm_spinupyears*12:]
+    ref_temp_nospinup = ref_temp[:,ref_spinupyears*12:]
+    gcm_temp_nospinup = gcm_temp_subset[:,gcm_spinupyears*12:]
     
     # Roll months so they are aligned with simulation months
     roll_amt = -1*(12 - gcm_subset_idx_start%12)
     if roll_amt == -12:
         roll_amt = 0 
     
     # Mean monthly temperature
@@ -105,23 +104,24 @@
     gcm_temp_biasadj = t_m_Navg + (t_mt - t_m_Navg) * np.tile(variability_monthly_std, int(gcm_temp.shape[1]/12))
     
     # Update elevation
     gcm_elev_biasadj = ref_elev
     
     # Assert that mean temperatures for all the glaciers must be more-or-less equal
     gcm_temp_biasadj_subset = (
-            gcm_temp_biasadj[:,gcm_subset_idx_start:gcm_subset_idx_end+1][:,pygem_prms.ref_spinupyears*12:])
+            gcm_temp_biasadj[:,gcm_subset_idx_start:gcm_subset_idx_end+1][:,ref_spinupyears*12:])
     assert np.max(np.abs(np.mean(gcm_temp_biasadj_subset, axis=1) - 
-                         np.mean(ref_temp[:,pygem_prms.ref_spinupyears*12:], axis=1))) < 1, (
+                         np.mean(ref_temp[:,ref_spinupyears*12:], axis=1))) < 1, (
             'Error with gcm temperature bias adjustment: mean ref and gcm temps differ by more than 1 degree')
     
     return gcm_temp_biasadj, gcm_elev_biasadj
 
 
-def prec_biasadj_HH2015(ref_prec, ref_elev, gcm_prec, dates_table_ref, dates_table):
+def prec_biasadj_HH2015(ref_prec, ref_elev, gcm_prec, dates_table_ref, dates_table,
+                        ref_spinupyears=0, gcm_spinupyears=0):
     """
     Huss and Hock (2015) precipitation bias correction based on mean (multiplicative)
     
     Parameters
     ----------
     ref_prec : np.array
         time series of reference precipitation
@@ -141,16 +141,16 @@
     """
     # GCM subset to agree with reference time period to calculate bias corrections
     gcm_subset_idx_start = np.where(dates_table.date.values == dates_table_ref.date.values[0])[0][0]
     gcm_subset_idx_end = np.where(dates_table.date.values == dates_table_ref.date.values[-1])[0][0]
     gcm_prec_subset = gcm_prec[:,gcm_subset_idx_start:gcm_subset_idx_end+1]
     
     # Remove spinup years, so adjustment performed over calibration period
-    ref_prec_nospinup = ref_prec[:,pygem_prms.ref_spinupyears*12:]
-    gcm_prec_nospinup = gcm_prec_subset[:,pygem_prms.gcm_spinupyears*12:]
+    ref_prec_nospinup = ref_prec[:,ref_spinupyears*12:]
+    gcm_prec_nospinup = gcm_prec_subset[:,gcm_spinupyears*12:]
     
     # Roll months so they are aligned with simulation months
     roll_amt = -1*(12 - gcm_subset_idx_start%12)
     
     # PRECIPITATION BIAS CORRECTIONS
     # Monthly mean precipitation
     ref_prec_monthly_avg = np.roll(monthly_avg_2darray(ref_prec_nospinup), roll_amt, axis=1)
@@ -160,25 +160,26 @@
     gcm_prec_biasadj = gcm_prec * np.tile(bias_adj_prec_monthly, int(gcm_prec.shape[1]/12))
     
     # Update elevation
     gcm_elev_biasadj = ref_elev
     
     # Assertion that bias adjustment does not drastically modify the precipitation and are reasonable
     gcm_prec_biasadj_subset = (
-            gcm_prec_biasadj[:,gcm_subset_idx_start:gcm_subset_idx_end+1][:,pygem_prms.gcm_spinupyears*12:])
+            gcm_prec_biasadj[:,gcm_subset_idx_start:gcm_subset_idx_end+1][:,gcm_spinupyears*12:])
     gcm_prec_biasadj_frac = gcm_prec_biasadj_subset.sum(axis=1) / ref_prec_nospinup.sum(axis=1)
     assert np.min(gcm_prec_biasadj_frac) > 0.5 and np.max(gcm_prec_biasadj_frac) < 2, (
             'Error with gcm precipitation bias adjustment: total ref and gcm prec differ by more than factor of 2')
     assert gcm_prec_biasadj.max() <= 10, 'gcm_prec_adj (precipitation bias adjustment) too high, needs to be modified'
     assert gcm_prec_biasadj.min() >= 0, 'gcm_prec_adj is producing a negative precipitation value'   
     
     return gcm_prec_biasadj, gcm_elev_biasadj
 
 
-def prec_biasadj_opt1(ref_prec, ref_elev, gcm_prec, dates_table_ref, dates_table):
+def prec_biasadj_opt1(ref_prec, ref_elev, gcm_prec, dates_table_ref, dates_table,
+                        ref_spinupyears=0, gcm_spinupyears=0):
     """
     Precipitation bias correction based on mean with limited maximum
     
     Parameters
     ----------
     ref_prec : np.array
         time series of reference precipitation
@@ -198,16 +199,16 @@
     """
     # GCM subset to agree with reference time period to calculate bias corrections
     gcm_subset_idx_start = np.where(dates_table.date.values == dates_table_ref.date.values[0])[0][0]
     gcm_subset_idx_end = np.where(dates_table.date.values == dates_table_ref.date.values[-1])[0][0]
     gcm_prec_subset = gcm_prec[:,gcm_subset_idx_start:gcm_subset_idx_end+1]
     
     # Remove spinup years, so adjustment performed over calibration period
-    ref_prec_nospinup = ref_prec[:,pygem_prms.ref_spinupyears*12:]
-    gcm_prec_nospinup = gcm_prec_subset[:,pygem_prms.gcm_spinupyears*12:]
+    ref_prec_nospinup = ref_prec[:,ref_spinupyears*12:]
+    gcm_prec_nospinup = gcm_prec_subset[:,gcm_spinupyears*12:]
     
     # Roll months so they are aligned with simulation months
     roll_amt = -1*(12 - gcm_subset_idx_start%12)
     
     # PRECIPITATION BIAS CORRECTIONS
     # Monthly mean precipitation
     ref_prec_monthly_avg = np.roll(monthly_avg_2darray(ref_prec_nospinup), roll_amt, axis=1)
@@ -249,15 +250,15 @@
             outlier_replacement[gcm_prec_biasadj > gcm_prec_max_check_adj])
     
     # Update elevation
     gcm_elev_biasadj = ref_elev
     
     # Assertion that bias adjustment does not drastically modify the precipitation and are reasonable
     gcm_prec_biasadj_subset = (
-            gcm_prec_biasadj[:,gcm_subset_idx_start:gcm_subset_idx_end+1][:,pygem_prms.gcm_spinupyears*12:])
+            gcm_prec_biasadj[:,gcm_subset_idx_start:gcm_subset_idx_end+1][:,gcm_spinupyears*12:])
     gcm_prec_biasadj_frac = gcm_prec_biasadj_subset.sum(axis=1) / ref_prec_nospinup.sum(axis=1)
     assert np.min(gcm_prec_biasadj_frac) > 0.5 and np.max(gcm_prec_biasadj_frac) < 2, (
             'Error with gcm precipitation bias adjustment: total ref and gcm prec differ by more than factor of 2')
     assert gcm_prec_biasadj.max() <= 10, 'gcm_prec_adj (precipitation bias adjustment) too high, needs to be modified'
     assert gcm_prec_biasadj.min() >= 0, 'gcm_prec_adj is producing a negative precipitation value'   
     
     return gcm_prec_biasadj, gcm_elev_biasadj
```

### Comparing `pygem-0.2.4/pygem/glacierdynamics.py` & `pygem-0.2.5/pygem/glacierdynamics.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #import netCDF4
 import xarray as xr
 
 from oggm import cfg, utils
 from oggm.core.flowline import FlowlineModel
 from oggm.exceptions import InvalidParamsError
 from oggm import __version__
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 
 cfg.initialize()
 
 
 #%%
 class MassRedistributionCurveModel(FlowlineModel):
     """Glacier geometry updated using mass redistribution curves; also known as the "delta-h method"
@@ -30,15 +30,15 @@
     """
 
     def __init__(self, flowlines, mb_model=None, y0=0.,
                  glen_a=None, fs=0., is_tidewater=False, water_level=0, 
 #                 calving_k=0,
                  inplace=False,
                  debug=True,
-                 option_areaconstant=False, spinupyears=pygem_prms.ref_spinupyears, 
+                 option_areaconstant=False, spinupyears=0, 
                  constantarea_years=0,
                  **kwargs):
         """ Instanciate the model.
         
         Parameters
         ----------
         flowlines : list
```

### Comparing `pygem-0.2.4/pygem/massbalance.py` & `pygem-0.2.5/pygem/massbalance.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: davidrounce
 """
 # External libraries
 import numpy as np
 # Local libraries
 from oggm.core.massbalance import MassBalanceModel
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 from pygem.utils._funcs import annualweightedmean_array
 
 #%%
 class PyGEMMassBalance(MassBalanceModel):
     """Mass-balance computed from the Python Glacier Evolution Model.
 
     This mass balance accounts for ablation, accumulation, and refreezing.
```

### Comparing `pygem-0.2.4/pygem/oggm_compat.py` & `pygem-0.2.5/pygem/oggm_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ PYGEM-OGGGM COMPATIBILITY FUNCTIONS """
 # External libraries
 import numpy as np
 import pandas as pd
 import netCDF4
 # Local libraries
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 from oggm import cfg, utils
 from oggm import workflow
 #from oggm import tasks
 from oggm.cfg import SEC_IN_YEAR
 from oggm.core.massbalance import MassBalanceModel
 #from oggm.shop import rgitopo
 from pygem.shop import debris, mbdata, icethickness
```

### Comparing `pygem-0.2.4/pygem/pygem_modelsetup.py` & `pygem-0.2.5/pygem/pygem_modelsetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Built-in libaries
 import os
 # External libraries
 import pandas as pd
 import numpy as np
 from datetime import datetime
 # Local libraries
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 
 
 def datesmodelrun(startyear=pygem_prms.ref_startyear, endyear=pygem_prms.ref_endyear, 
                   spinupyears=pygem_prms.ref_spinupyears, option_wateryear=pygem_prms.ref_wateryear):
     """
     Create table of year, month, day, water year, season and number of days in the month.
```

### Comparing `pygem-0.2.4/pygem/scraps/dummy_task_module.py` & `pygem-0.2.5/pygem/scraps/dummy_task_module.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem/scraps/run.py` & `pygem-0.2.5/pygem/scraps/run.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem/shop/debris.py` & `pygem-0.2.5/pygem/shop/debris.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import rasterio
 import xarray as xr
 
 from oggm import cfg
 from oggm.utils import entity_task
 from oggm.core.gis import rasterio_to_gdir
 from oggm.utils import ncDataset
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 
 """
 To-do list:
   - Add binned debris-covered area to flowlines
   - Fabien may have better way of processing debris rasters to gridded data without exporting .tif
 """
```

### Comparing `pygem-0.2.4/pygem/shop/icethickness.py` & `pygem-0.2.5/pygem/shop/icethickness.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import rasterio
 import xarray as xr
 
 from oggm import cfg
 from oggm.utils import entity_task
 from oggm.core.gis import rasterio_to_gdir
 from oggm.utils import ncDataset
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 
 if not 'consensus_mass' in cfg.BASENAMES:
     cfg.BASENAMES['consensus_mass'] = ('consensus_mass.pkl', 'Glacier mass from consensus ice thickness data')
 if not 'consensus_h' in cfg.BASENAMES:
     cfg.BASENAMES['consensus_h'] = ('consensus_h.tif', 'Raster of consensus ice thickness data')
 
 # Module logger
```

### Comparing `pygem-0.2.4/pygem/shop/mbdata.py` & `pygem-0.2.5/pygem/shop/mbdata.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem/tests/test_oggm_compat.py` & `pygem-0.2.5/pygem/tests/test_oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem/utils/_funcs.py` & `pygem-0.2.5/pygem/utils/_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Functions that didn't fit into other modules
 """
-import pygem.pygem_input as pygem_prms
+import pygem_input as pygem_prms
 import numpy as np
 
 
 def annualweightedmean_array(var, dates_table):
     """
     Calculate annual mean of variable according to the timestep.
```

### Comparing `pygem-0.2.4/pygem/utils/_funcs_selectglaciers.py` & `pygem-0.2.5/pygem/utils/_funcs_selectglaciers.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pygem.egg-info/PKG-INFO` & `pygem-0.2.5/pygem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
 Home-page: https://github.com/drounce/PyGEM
 Author: David Rounce
 Author-email: David Rounce <drounce@cmu.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygem-0.2.4/pygem.egg-info/SOURCES.txt` & `pygem-0.2.5/pygem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygem-0.2.4/pyproject.toml` & `pygem-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "wheel",
 ]
 
 [tool.setuptools_scm]
 
 [project]
 name = "pygem"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="David Rounce", email="drounce@cmu.edu" },
 ]
 description = "Python Glacier Evolution Model for large-scale glacier modeling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygem-0.2.4/setup.cfg` & `pygem-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygem
-version = 0.2.4
+version = 0.2.5
 description = Python Glacier Evolution Model
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/drounce/PyGEM
 author = David Rounce
 author_email = drounce@cmu.edu
 license = MIT
```

### Comparing `pygem-0.2.4/setup.py` & `pygem-0.2.5/setup.py`

 * *Files identical despite different names*

