# Comparing `tmp/rapidpe_rift_pipe-0.4.0.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.4.0.tar", last modified: Thu Jun  1 21:14:03 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.0.tar", last modified: Thu Jun  8 21:22:34 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.4.0.tar` & `rapidpe_rift_pipe-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.178728 rapidpe_rift_pipe-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-01 21:14:03.178728 rapidpe_rift_pipe-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.156727 rapidpe_rift_pipe-0.4.0/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.168728 rapidpe_rift_pipe-0.4.0/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-01 21:14:03.179728 rapidpe_rift_pipe-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.157727 rapidpe_rift_pipe-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.175728 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-01 21:04:40.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44671 2023-05-31 13:19:09.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18503 2023-05-18 18:03:43.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.176728 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 21:13:50.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.177728 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 21:13:50.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31454 2023-05-30 22:21:02.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-06-01 17:09:14.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.177728 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 21:13:50.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:14:03.176728 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-01 21:14:03.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-06-01 21:14:03.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 21:14:03.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-01 21:14:03.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-01 21:14:03.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 21:14:03.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 21:14:02.000000 rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.999214 rapidpe_rift_pipe-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-08 21:22:33.999214 rapidpe_rift_pipe-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.991214 rapidpe_rift_pipe-0.5.0/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.994214 rapidpe_rift_pipe-0.5.0/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2023-06-08 21:22:34.000214 rapidpe_rift_pipe-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.992214 rapidpe_rift_pipe-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.997214 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47425 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.998214 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.999214 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31454 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.999214 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-06-08 21:22:24.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:22:33.998214 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:22:33.000000 rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.4.0/COPYING` & `rapidpe_rift_pipe-0.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/PKG-INFO` & `rapidpe_rift_pipe-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.4.0/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.0/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.0/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.0/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.0/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.0/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/setup.cfg` & `rapidpe_rift_pipe-0.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 install_requires = 
 	numpy
 	matplotlib
 	h5py
 	tabulate
 	astropy
 	lalsuite
+	gwpy>=3.0.4
 	rift==0.0.15.8
 	rapid_pe>=0.1.0,<0.2.0
 scripts = 
 	bin/postscripts/convert_result_to_txt.py
 	bin/postscripts/create_summarypage.py
 	bin/postscripts/compute_posterior.py
 	bin/postscripts/plot_skymap.py
```

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     convert_list_string_to_dict,
     correct_list_string_formatting_if_list_string,
     transform_s1zs2z_chi,
 )
 from rapidpe_rift_pipe.search_bias_bounds import parse_search_bias_bounds
 from rapid_pe import amrlib
 
+
+import gwpy.timeseries
 from ligo.lw import ligolw
 from ligo.lw import lsctables
 from ligo.lw import utils as ligolw_utils
 from rapidpe_rift_pipe.config import Config
 from sklearn.neighbors import BallTree
 
 
@@ -63,14 +65,26 @@
     "o3replay": {
         "H1": "GDS-CALIB_STRAIN_INJ1_O3Replay",
         "L1": "GDS-CALIB_STRAIN_INJ1_O3Replay",
         "V1": "Hrec_hoft_16384Hz_INJ1_O3Replay",
     },
 }
 
+shm_basedir = "/dev/shm/kafka/"
+
+_run_mode_to_shm_dir = {}
+_run_mode_to_shm_dir["online"] = {
+    ifo: os.path.join(shm_basedir, ifo)
+    for ifo in ["H1", "L1", "V1"]
+}
+_run_mode_to_shm_dir["o3replay"] = {
+    ifo: os.path.join(shm_basedir, f"{ifo}_O3ReplayMDC")
+    for ifo in ["H1", "L1", "V1"]
+}
+
 
 def make_parser():
     parser = ArgumentParser()
 
     parser.add_argument(
         "config",
         help="Configuration file.",
@@ -464,35 +478,21 @@
                 t_duration_buffer = 50
                 data_start_time = int(t_event - t_before_cache)
                 data_end_time = int(t_event + t_after_cache)
 
                 event_info['data_start_time'] = int(t_event - t_duration_buffer)
                 event_info['data_end_time'] = int(t_event + t_mr_buffer)
 
-                data_type = config.event.frame_data_types[ifo]
-                # TODO: We should import gwdatafind and call the underlying
-                #       functions directly.
-                raw_cache_file_path = os.path.join(output_dir,f"{ifo[0]}_raw.cache")
-                dcmd = (
-                    "python -m gwdatafind -u file "
-                    f"-o {ifo[0]} -t {data_type} -s {data_start_time} "
-                    f"-e {data_end_time} > {raw_cache_file_path}"
+                cache_fname = cache_data(
+                    config,
+                    ifo=ifo, channel=channel,
+                    start_time=data_start_time, end_time=data_end_time,
                 )
-                logging.info(dcmd)
-                retry_times = [1] + [5] + [500]*2
-                for retry_time in retry_times:
-                    exit_status = os.system(dcmd)
-                    if exit_status == 0 and os.stat(raw_cache_file_path).st_size != 0:
-                        break
-                    else:
-                        logging.error(f"There is no data at the time when this triggered. Retry in {retry_time} seconds")
-                        time.sleep(retry_time)
-                else:
-                    logging.error(f"data not found after {sum(retry_times)} seconds")
-                    sys.exit(1)
+                # TODO: Use `cache_fname` when creating Condor submit files to
+                #       pass the data without relying on NFS.
                 num_ifos += 1
 
             if num_ifos == 0:
                 logging.error("Failed to load data from any IFOs.")
 
             # path2cache always assumes data is in output_dir, so that path
             # needs to be removed before passing output to data.cache
@@ -1007,9 +1007,101 @@
             "ERROR: Only non-cbc event(s) for this (super)event. "
             f"Can't submit rapidpe. gids={other_gids}"
         )
     else:
         return gid
 
 
+def cache_data(config, *, ifo, channel, start_time, end_time):
+    output_dir = os.path.abspath(config.output_parent_directory)
+    raw_cache_file_path = os.path.join(output_dir, f"{ifo[0]}_raw.cache")
+
+    data_type = config.event.frame_data_types[ifo]
+
+    channel = f"{ifo}:{channel}"
+    if config.event.query_shm:
+        try:
+            shm_dir = _run_mode_to_shm_dir[config.event.run_mode]
+            data = get_data_shm(shm_dir=shm_dir[ifo],
+                                ifo=ifo,
+                                channel=channel, data_type=data_type,
+                                start_time=start_time, end_time=end_time)
+
+        except FileNotFoundError:
+            logging.info(
+                "Shared-memory data unavailable for %s between %s and %s",
+                ifo, start_time, end_time,
+            )
+
+            data = get_data_gwpy(channel=channel, data_type=data_type,
+                                 start_time=start_time, end_time=end_time)
+    else:
+        data = get_data_gwpy(channel=channel, data_type=data_type,
+                             start_time=start_time, end_time=end_time)
+
+    if data is None:
+        logging.error("Failed to fetch data for IFO %s", ifo)
+        return
+
+    actual_start = data.times[0].value
+    actual_duration = data.duration.value
+
+    # NOTE: Copied this from Bilby, seems a little wonky.
+    #       Converts float to int, but only if it's equivalent.
+    if int(actual_duration) == actual_duration:
+        actual_duration = int(actual_duration)
+
+    output_gwf_path = os.path.join(
+        output_dir,
+        f"{ifo[0]}-{data_type}-{actual_start}-{actual_duration}.gwf"
+    )
+    data.write(output_gwf_path)
+    logging.info("Wrote %s data to %s", ifo, output_gwf_path)
+
+    with open(raw_cache_file_path, "w") as cache_file:
+        cache_file.write(output_gwf_path)
+
+    return raw_cache_file_path
+
+
+def get_data_shm(*, shm_dir, ifo, channel, data_type, start_time, end_time):
+    segments = []
+    for time in range(start_time, end_time):
+        gwf_path = os.path.join(shm_dir,
+                                f"{ifo[0]}-{data_type}-{time}-1.gwf")
+
+        logging.info("Attempting to load data from %s", gwf_path)
+
+        segments.append(
+            gwpy.timeseries.TimeSeries.read(gwf_path, channel=channel)
+        )
+
+    return gwpy.timeseries.TimeSeriesList(*segments).join()
+
+
+gwpy_retry_times = [30]*2 + [60]*2
+def get_data_gwpy(*, channel, data_type, start_time, end_time):
+    for retry_time in gwpy_retry_times:
+        try:
+            logging.info(
+                "Attempting to fetch %s from %s to %s with GWpy discovery",
+                channel, start_time, end_time,
+            )
+            return gwpy.timeseries.TimeSeries.get(
+                channel=channel, frametype=data_type,
+                start=start_time, end=end_time,
+            )
+        except RuntimeError:
+            logging.exception(
+                "Failed to discover data with GWpy, retrying in %s sec",
+                retry_time,
+            )
+            time.sleep(retry_time)
+
+    logging.error(
+        "Failed to discover data with GWpy after %s attempts in %s sec",
+        len(gwpy_retry_times), sum(gwpy_retry_times),
+    )
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,14 +430,18 @@
         "gracedb_id" : {
             "parser" : parse_str,
         },
         "run_mode" : {
             "parser" : parse_str,
             "fallback" : "online",
         },
+        "query_shm": {
+            "parser" : parse_bool,
+            "fallback" : False,
+        },
         "mdc_event_injection_file" : {
             "parser": parse_str,
             "fallback": None
         },
         "mdc_time_offset" : {
             "parser" : parse_str,
             "fallback" : None
@@ -447,14 +451,18 @@
         "superevent_id" : {
             "parser" : parse_str,
         },
         "run_mode" : {
             "parser" : parse_str,
             "fallback" : "online",
         },
+        "query_shm": {
+            "parser" : parse_bool,
+            "fallback" : False,
+        },
         "mdc_event_injection_file" : {
             "parser": parse_str,
             "fallback": None
         },
         "mdc_time_offset" : {
             "parser" : parse_str,
             "fallback" : None
```

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.4.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

