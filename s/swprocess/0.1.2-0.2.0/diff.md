# Comparing `tmp/swprocess-0.1.2.tar.gz` & `tmp/swprocess-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swprocess-0.1.2.tar", last modified: Tue Jun  6 14:01:56 2023, max compression
+gzip compressed data, was "swprocess-0.2.0.tar", last modified: Fri Jun  9 02:02:33 2023, max compression
```

## Comparing `swprocess-0.1.2.tar` & `swprocess-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    33246 2023-06-06 14:00:27.000000 swprocess-0.1.2/LICENSE.txt
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6471 2023-06-06 14:01:56.352237 swprocess-0.1.2/PKG-INFO
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     5357 2023-06-06 14:00:27.000000 swprocess-0.1.2/README.md
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      107 2023-06-06 14:01:56.352237 swprocess-0.1.2/setup.cfg
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2317 2023-06-06 14:00:27.000000 swprocess-0.1.2/setup.py
-drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/swprocess/
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1342 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/__init__.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    14158 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/activetimeseries.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    32276 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/array1d.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4438 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/interact.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2717 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/inversion.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    12409 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/masw.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    12992 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/maswworkflows.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      903 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/meta.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    23284 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/peaks.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    35081 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/peakssuite.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4628 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/regex.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1807 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/register.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     9629 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/sensor1c.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2234 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/snr.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2840 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/source.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     5736 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/spaccurve.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    11584 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/spaccurvesuite.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    16726 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/stats.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6940 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/utils.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    27082 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/wavefieldtransforms.py
-drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/swprocess.egg-info/
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6471 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/PKG-INFO
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1051 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/SOURCES.txt
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)        1 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/dependency_links.txt
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      112 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/requires.txt
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)       10 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/top_level.txt
-drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/test/
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    17719 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_activetimeseries.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    25801 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_array1d.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1683 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_interact.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2260 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_masw.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    13372 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_maswworkflows.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    24157 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_peaks.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    32638 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_peakssuite.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1403 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_regex.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2267 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_register.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6248 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_sensor1c.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2935 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_snr.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2453 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_source.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4268 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_spaccurve.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     3297 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_spaccurvesuite.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     8024 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_stats.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     3168 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_utils.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     8321 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_wavefieldtransforms.py
--rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1909 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/testtools.py
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-09 02:02:33.299425 swprocess-0.2.0/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    33246 2023-06-06 14:00:27.000000 swprocess-0.2.0/LICENSE.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6471 2023-06-09 02:02:33.299425 swprocess-0.2.0/PKG-INFO
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     5357 2023-06-06 14:00:27.000000 swprocess-0.2.0/README.md
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      107 2023-06-09 02:02:33.299425 swprocess-0.2.0/setup.cfg
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2331 2023-06-09 01:59:09.000000 swprocess-0.2.0/setup.py
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-09 02:02:33.289424 swprocess-0.2.0/swprocess/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1342 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/__init__.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    14158 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/activetimeseries.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    32276 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/array1d.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4438 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/interact.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2717 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/inversion.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    12409 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/masw.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    12992 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/maswworkflows.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1197 2023-06-09 01:59:09.000000 swprocess-0.2.0/swprocess/meta.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    23766 2023-06-09 01:59:09.000000 swprocess-0.2.0/swprocess/peaks.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    35432 2023-06-09 01:59:09.000000 swprocess-0.2.0/swprocess/peakssuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4566 2023-06-09 01:59:09.000000 swprocess-0.2.0/swprocess/regex.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1807 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/register.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     9629 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/sensor1c.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2234 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/snr.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2840 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/source.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     5736 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/spaccurve.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    11584 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/spaccurvesuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    16726 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/stats.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6940 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/utils.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    27082 2023-06-06 14:00:27.000000 swprocess-0.2.0/swprocess/wavefieldtransforms.py
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-09 02:02:33.289424 swprocess-0.2.0/swprocess.egg-info/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6471 2023-06-09 02:02:33.000000 swprocess-0.2.0/swprocess.egg-info/PKG-INFO
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1051 2023-06-09 02:02:33.000000 swprocess-0.2.0/swprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)        1 2023-06-09 02:02:33.000000 swprocess-0.2.0/swprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      123 2023-06-09 02:02:33.000000 swprocess-0.2.0/swprocess.egg-info/requires.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)       10 2023-06-09 02:02:33.000000 swprocess-0.2.0/swprocess.egg-info/top_level.txt
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-09 02:02:33.299425 swprocess-0.2.0/test/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    17719 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_activetimeseries.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    25801 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_array1d.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1683 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_interact.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2260 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_masw.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    13372 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_maswworkflows.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    24157 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_peaks.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    32638 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_peakssuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1403 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_regex.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2267 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_register.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6248 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_sensor1c.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2935 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_snr.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2453 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_source.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4268 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_spaccurve.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     3297 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_spaccurvesuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     8024 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_stats.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     3168 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_utils.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     8321 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/test_wavefieldtransforms.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1909 2023-06-06 14:00:27.000000 swprocess-0.2.0/test/testtools.py
```

### Comparing `swprocess-0.1.2/LICENSE.txt` & `swprocess-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/PKG-INFO` & `swprocess-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swprocess
-Version: 0.1.2
+Version: 0.2.0
 Summary: Package for Surface Wave Processing
 Home-page: https://github.com/jpvantassel/swprocess
 Author: Joseph P. Vantassel
 Author-email: joseph.p.vantassel@gmail.com
 Project-URL: Bug Reports, https://github.com/jpvantassel/swprocess/issues
 Project-URL: Source, https://github.com/jpvantassel/swprocess
 Project-URL: Docs, https://swprocess.readthedocs.io/en/latest/?badge=latest
```

### Comparing `swprocess-0.1.2/README.md` & `swprocess-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/setup.py` & `swprocess-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     keywords='surface-wave dispersion processing geopsy active passive masw mam',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=["numpy", "scipy", "matplotlib",
                       "obspy", "sigpropy>=1.0.0", "pandas",
                       "swprepost", "PyQt5"],
     extras_require={
-        'dev': ['coverage', 'tox', 'sphinx', 'sphinx_rtd_theme'],
+        'dev': ['coverage', 'tox', 'sphinx', 'sphinx_rtd_theme', 'jupyterlab'],
     },
     package_data={
     },
     data_files=[
     ],
     entry_points={
     },
```

### Comparing `swprocess-0.1.2/swprocess/__init__.py` & `swprocess-0.2.0/swprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/activetimeseries.py` & `swprocess-0.2.0/swprocess/activetimeseries.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/array1d.py` & `swprocess-0.2.0/swprocess/array1d.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/interact.py` & `swprocess-0.2.0/swprocess/interact.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/inversion.py` & `swprocess-0.2.0/swprocess/inversion.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/masw.py` & `swprocess-0.2.0/swprocess/masw.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/maswworkflows.py` & `swprocess-0.2.0/swprocess/maswworkflows.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/meta.py` & `swprocess-0.2.0/swprocess/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,16 @@
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <https: //www.gnu.org/licenses/>.
 
 """Metadata for swprocess."""
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
+
+SUPPORTED_GEOPSY_VERSIONS = ["3.2.0"]
+
+def check_geopsy_version(version):            
+    if version not in SUPPORTED_GEOPSY_VERSIONS:
+        msg = f"geopsy version {version} is not supported; "
+        msg += f"use {SUPPORTED_GEOPSY_VERSIONS} instead."
+        raise ValueError(msg)
```

### Comparing `swprocess-0.1.2/swprocess/peaks.py` & `swprocess-0.2.0/swprocess/peaks.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import json
 import warnings
 import logging
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-from .regex import get_process_type, get_peak_from_max, get_all, get_nmaxima
+from .regex import get_wavetype, get_process_type, get_peak_from_max, get_all, get_nmaxima, get_geopsy_version
+from .meta import check_geopsy_version
 
 logger = logging.getLogger("swprocess.peaks")
 
 
 class Peaks():
     """Class for handling dispersion peaks.
 
@@ -140,70 +141,78 @@
     @property
     def extended_attrs(self):
         """List of available Peaks attributes, including calculated."""
         others = ["wavelength", "slowness", "wavenumber"]
         return self.attrs + others
 
     @classmethod
-    def _parse_peaks(cls, peak_data, wavetype="rayleigh", start_time=None, frequencies=None, nmaxima=None, process_type=None):
+    def _parse_peaks(cls, peak_data, wavetype="rayleigh", start_time=None, frequencies=None, nmaxima=None):
         """Parse data for a given blockset."""
-        if process_type is None:
-            regex = get_process_type()
-            process_type, *_ = regex.search(peak_data).groups()
+        regex = get_wavetype()
+        wavetype_from_file = regex.search(peak_data).groups()[0]
+        if wavetype == "rayleigh" and wavetype_from_file == "Vertical":
+            wavetype = "vertical"
+
+        regex = get_process_type()
+        process_type = regex.search(peak_data).groups()[0]
+        if process_type.lower() == "rtbf" and wavetype_from_file == "Vertical":
+            process_type = "capon"
+        else:
+            process_type = process_type.lower()
 
         if start_time is None:
-            regex = get_peak_from_max(wavetype=wavetype, process_type=process_type)
+            regex = get_peak_from_max(wavetype=wavetype)
             start_time, *_ = regex.search(peak_data).groups()
 
         if frequencies is None:
-            regex = get_peak_from_max(time=start_time, wavetype=wavetype, process_type=process_type)
+            regex = get_peak_from_max(time=start_time, wavetype=wavetype)
             frequencies = []
             for match in regex.finditer(peak_data):
                 _, f, *_ = match.groups()
                 if f in frequencies:
                     continue
                 else:
                     frequencies.append(f)
         nfrequencies = len(frequencies)
 
         if nmaxima is None:
             regex = get_nmaxima()
             nmaxima = int(regex.search(peak_data).groups()[0])
-            nmaxima = 1 if nmaxima <= 0 else nmaxima
+            nmaxima = max(1, nmaxima)
+            nmaxima = min(100, nmaxima)
 
         frqs = np.full((nmaxima, nfrequencies), fill_value=np.nan, dtype=float)
         vels = np.full_like(frqs, fill_value=np.nan, dtype=float)
         azis = np.full_like(frqs, fill_value=np.nan, dtype=float)
         ells = np.full_like(frqs, fill_value=np.nan, dtype=float)
         nois = np.full_like(frqs, fill_value=np.nan, dtype=float)
         pwrs = np.full_like(frqs, fill_value=np.nan, dtype=float)
 
         for col, frequency in enumerate(frequencies):
-            getpeak = get_peak_from_max(time=start_time, wavetype=wavetype,
-                                        frequency=frequency, process_type=process_type)
+            getpeak = get_peak_from_max(time=start_time, frequency=frequency,
+                                        wavetype=wavetype)
 
             for row, match in enumerate(getpeak.finditer(peak_data)):
                 _, _frq, _slo, _azi, _ell, _noi, _pwr = match.groups()
 
                 frqs[row, col] = float(_frq)
                 vels[row, col] = 1/float(_slo)
                 azis[row, col] = float(_azi)
                 ells[row, col] = float(_ell)
                 nois[row, col] = float(_noi)
                 pwrs[row, col] = float(_pwr)
 
         # Include for "belt and suspenders".
-        wavetype = wavetype if process_type.lower() == "rtbf" else None
         getall = get_all(time=start_time, wavetype=wavetype)
         count = len(getall.findall(peak_data))
         if np.sum(~np.isnan(frqs)) != count:  # pragma: no cover
             msg = f"Missing {count - len(frqs)} dispersion peaks."
             raise ValueError(msg)
 
-        return cls(frqs, vels, identifier=start_time, azimuth=azis,
+        return cls(frqs, vels, identifier=f"{start_time}-{process_type}", azimuth=azis,
                    ellipticity=ells, noise=nois, power=pwrs)
 
     def plot(self, xtype="frequency", ytype="velocity", plot_kwargs=None,
              mask=None):
         """Plot dispersion data in `Peaks` object.
 
         Parameters
@@ -626,14 +635,19 @@
         file, as is most often the case, this method ignores all but the
         first instance found.
 
         """
         with open(fname, "r") as f:
             peak_data = f.read()
 
+        regex = get_geopsy_version()
+        major, minor, micro = regex.search(peak_data).groups()
+        version = f"{major}.{minor}.{micro}"
+        check_geopsy_version(version)
+
         return cls._parse_peaks(peak_data, wavetype=wavetype)
 
     def __eq__(self, other):
         if not isinstance(other, Peaks):
             return False
 
         # Check non-iterable attributes
```

### Comparing `swprocess-0.1.2/swprocess/peakssuite.py` & `swprocess-0.2.0/swprocess/peakssuite.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 import numpy as np
 from scipy.interpolate import interp1d
 from matplotlib.widgets import Cursor
 import matplotlib.pyplot as plt
 
 from .wavefieldtransforms import AbstractWavefieldTransform as AWTransform
 from .peaks import Peaks
-from .regex import get_process_type, get_nmaxima, get_peak_from_max
+from .regex import get_nmaxima, get_peak_from_max, get_geopsy_version, get_wavetype
+from .meta import check_geopsy_version
 
 logger = logging.getLogger("swprocess.peakssuite")
 
 
 class PeaksSuite():
 
     def __init__(self, peaks):
@@ -813,31 +814,39 @@
             fnames = [str(fnames)]
 
         peaks = []
         for fname in fnames:
             with open(fname, "r") as f:
                 peak_data = f.read()
 
-            regex = get_process_type()
-            process_type = regex.search(peak_data).groups()[0]
+            regex = get_geopsy_version()
+            major, minor, micro = regex.search(peak_data).groups()
+            version = f"{major}.{minor}.{micro}"
+            check_geopsy_version(version)
+
+            regex = get_wavetype()
+            wavetype_from_file = regex.search(peak_data).groups()[0]
+            if wavetype == "rayleigh" and wavetype_from_file == "Vertical":
+                wavetype = "vertical"
 
             regex = get_nmaxima()
             nmaxima = int(regex.search(peak_data).groups()[0])
-            nmaxima = 1 if nmaxima <= 0 else nmaxima
+            nmaxima = max(1, nmaxima)
+            nmaxima = min(100, nmaxima)
 
-            regex = get_peak_from_max(wavetype=wavetype, process_type=process_type)
+            regex = get_peak_from_max(wavetype=wavetype)
             frequencies = []
             for match in regex.finditer(peak_data):
                 _, f, *_ = match.groups()
                 if f in frequencies:
                     continue
                 else:
                     frequencies.append(f)
 
-            regex = get_peak_from_max(wavetype=wavetype, process_type=process_type)
+            regex = get_peak_from_max(wavetype=wavetype)
             found_times = []
             for found in regex.finditer(peak_data):
                 start_time = found.groups()[0]
                 if start_time in found_times:
                     continue
                 found_times.append(start_time)
                 peak = Peaks._parse_peaks(peak_data,
```

### Comparing `swprocess-0.1.2/swprocess/regex.py` & `swprocess-0.2.0/swprocess/regex.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 """Regular expression definitions."""
 
 import re
 
 __all__ = ["get_peak_from_max", "get_nmaxima",  "get_all", "get_spac_ratio", "get_spac_ring"]
 
+DEFAULT_TIME = "\d+\.?\d*"
+DEFAULT_FREQUENCY = "-?\d+.?\d*[eE]?[+-]?\d*"
 NUMBER = "-?\d+.?\d*[eE]?[+-]?\d*"
 
 
-def get_peak_from_max(time="\d+\.?\d*", wavetype="rayleigh", process_type="rtbf",
-                      frequency="-?\d+.?\d*[eE]?[+-]?\d*"):
+def get_peak_from_max(time=DEFAULT_TIME, frequency=DEFAULT_FREQUENCY, wavetype="rayleigh"):
     """Compile regular expression to extract peaks from a `.max` file.
 
     Parameters
     ----------
     wavetype : {'rayleigh', 'love', 'vertical', 'radial', 'transverse'}, optional
         Define a specific wavetype to extract, default is `'rayleigh'`.
     time : str, optional
@@ -38,32 +39,31 @@
     Return
     ------
     Compiled Regular Expression
         To extract peaks from a `.max` file.
 
     """
     # abs_time frequency polarization slowness azimuth ellipticity noise power valid
-    process_type = process_type.lower()
-    if process_type=="rtbf":
-        wavetype = validate_wavetypes(wavetype)
-        pattern = f"({time}) ({frequency}) {wavetype} ({NUMBER}) ({NUMBER}) ({NUMBER}) ({NUMBER}|-?inf|nan) ({NUMBER}) 1"
-    elif process_type in ["conventional", "capon"]:
-        pattern = f"({time}) ({frequency}) ({NUMBER}) ({NUMBER}) ({NUMBER}|-?inf|nan) ({NUMBER}|-?inf|nan) ({NUMBER}) 1"
-    else:
-        raise ValueError(f"process_type = {process_type} is unknown.")
+    wavetype = validate_wavetypes(wavetype)
+    pattern = f"({time}) ({frequency}) {wavetype} ({NUMBER}) ({NUMBER}) ({NUMBER}) ({NUMBER}|-?inf|nan) ({NUMBER}) 1"
+    return re.compile(pattern)
+
+def get_geopsy_version():
+    return re.compile("geopsypack-(\d+).(\d+).(\d+)")
 
+def get_wavetype():
+    pattern = f"{DEFAULT_TIME} {DEFAULT_FREQUENCY} (\S+) {NUMBER} {NUMBER} {NUMBER} {NUMBER}|-?inf|nan {NUMBER} 1"
     return re.compile(pattern)
 
 def get_process_type():
     return re.compile("PROCESS_TYPE=(\S+)")
 
 def get_nmaxima():
     return re.compile("N_MAXIMA=(\d+)")
 
-
 def get_all(wavetype="rayleigh", time="(\d+\.?\d*)"):
     """Compile regular expression to identify peaks from a `.max` file.
 
     Parameters
     ----------
     wavetype : {'rayleigh', 'love', 'vertical', 'radial', 'transverse'}, optional
         Define a specific wavetype to extract, default is `'rayleigh'`.
```

### Comparing `swprocess-0.1.2/swprocess/register.py` & `swprocess-0.2.0/swprocess/register.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/sensor1c.py` & `swprocess-0.2.0/swprocess/sensor1c.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/snr.py` & `swprocess-0.2.0/swprocess/snr.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/source.py` & `swprocess-0.2.0/swprocess/source.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/spaccurve.py` & `swprocess-0.2.0/swprocess/spaccurve.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/spaccurvesuite.py` & `swprocess-0.2.0/swprocess/spaccurvesuite.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/stats.py` & `swprocess-0.2.0/swprocess/stats.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/utils.py` & `swprocess-0.2.0/swprocess/utils.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess/wavefieldtransforms.py` & `swprocess-0.2.0/swprocess/wavefieldtransforms.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/swprocess.egg-info/PKG-INFO` & `swprocess-0.2.0/swprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swprocess
-Version: 0.1.2
+Version: 0.2.0
 Summary: Package for Surface Wave Processing
 Home-page: https://github.com/jpvantassel/swprocess
 Author: Joseph P. Vantassel
 Author-email: joseph.p.vantassel@gmail.com
 Project-URL: Bug Reports, https://github.com/jpvantassel/swprocess/issues
 Project-URL: Source, https://github.com/jpvantassel/swprocess
 Project-URL: Docs, https://swprocess.readthedocs.io/en/latest/?badge=latest
```

### Comparing `swprocess-0.1.2/swprocess.egg-info/SOURCES.txt` & `swprocess-0.2.0/swprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_activetimeseries.py` & `swprocess-0.2.0/test/test_activetimeseries.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_array1d.py` & `swprocess-0.2.0/test/test_array1d.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_interact.py` & `swprocess-0.2.0/test/test_interact.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_masw.py` & `swprocess-0.2.0/test/test_masw.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_maswworkflows.py` & `swprocess-0.2.0/test/test_maswworkflows.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_peaks.py` & `swprocess-0.2.0/test/test_peaks.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_peakssuite.py` & `swprocess-0.2.0/test/test_peakssuite.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_regex.py` & `swprocess-0.2.0/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_register.py` & `swprocess-0.2.0/test/test_register.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_sensor1c.py` & `swprocess-0.2.0/test/test_sensor1c.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_snr.py` & `swprocess-0.2.0/test/test_snr.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_source.py` & `swprocess-0.2.0/test/test_source.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_spaccurve.py` & `swprocess-0.2.0/test/test_spaccurve.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_spaccurvesuite.py` & `swprocess-0.2.0/test/test_spaccurvesuite.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_stats.py` & `swprocess-0.2.0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_utils.py` & `swprocess-0.2.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/test_wavefieldtransforms.py` & `swprocess-0.2.0/test/test_wavefieldtransforms.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.2/test/testtools.py` & `swprocess-0.2.0/test/testtools.py`

 * *Files identical despite different names*

