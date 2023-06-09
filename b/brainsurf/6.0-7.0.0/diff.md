# Comparing `tmp/brainsurf-6.0.tar.gz` & `tmp/brainsurf-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsurf-6.0.tar", last modified: Tue May 30 17:14:54 2023, max compression
+gzip compressed data, was "brainsurf-7.0.0.tar", last modified: Fri Jun  9 04:11:56 2023, max compression
```

## Comparing `brainsurf-6.0.tar` & `brainsurf-7.0.0.tar`

### file list

```diff
@@ -1,71 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.864503 brainsurf-6.0/
--rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-6.0/LICENSE
--rw-rw-rw-   0        0        0     2152 2023-05-30 17:14:54.863547 brainsurf-6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.673360 brainsurf-6.0/brainsurf/
--rw-rw-rw-   0        0        0       68 2023-05-30 17:14:46.000000 brainsurf-6.0/brainsurf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.729464 brainsurf-6.0/brainsurf/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-6.0/brainsurf/analysis/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-05-23 17:17:31.000000 brainsurf-6.0/brainsurf/analysis/corelation_analysis.py
--rw-rw-rw-   0        0        0     3601 2023-04-29 05:21:32.000000 brainsurf-6.0/brainsurf/analysis/erp_analysis.py
--rw-rw-rw-   0        0        0     1455 2023-05-21 15:27:09.000000 brainsurf-6.0/brainsurf/analysis/find_range.py
--rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-6.0/brainsurf/analysis/multi_fractal.py
--rw-rw-rw-   0        0        0     1367 2023-04-29 04:19:06.000000 brainsurf-6.0/brainsurf/analysis/power_spectrum.py
--rw-rw-rw-   0        0        0     3087 2023-05-21 15:49:59.000000 brainsurf-6.0/brainsurf/analysis/stats_analysis.py
--rw-rw-rw-   0        0        0      493 2023-04-28 15:40:11.000000 brainsurf-6.0/brainsurf/analysis/time_frequency.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:11:03.000000 brainsurf-6.0/brainsurf/analysis/wavelet_transform.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.741023 brainsurf-6.0/brainsurf/cognitive_analysis_module/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-6.0/brainsurf/cognitive_analysis_module/__init__.py
--rw-rw-rw-   0        0        0    10182 2023-05-24 17:42:19.000000 brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py
--rw-rw-rw-   0        0        0     1028 2023-05-23 18:15:54.000000 brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.750570 brainsurf-6.0/brainsurf/comparitive_analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:51.000000 brainsurf-6.0/brainsurf/comparitive_analysis/__init__.py
--rw-rw-rw-   0        0        0     1307 2023-05-14 16:53:07.000000 brainsurf-6.0/brainsurf/comparitive_analysis/meditation_comparision.py
--rw-rw-rw-   0        0        0     1376 2023-05-23 17:05:32.000000 brainsurf-6.0/brainsurf/comparitive_analysis/t_test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.776957 brainsurf-6.0/brainsurf/data/
--rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-6.0/brainsurf/data/__init__.py
--rw-rw-rw-   0        0        0    21380 2023-05-29 16:47:53.000000 brainsurf-6.0/brainsurf/data/comparative_visualize.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-6.0/brainsurf/data/csv.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-6.0/brainsurf/data/edf.py
--rw-rw-rw-   0        0        0    11884 2023-05-23 18:39:23.000000 brainsurf-6.0/brainsurf/data/eeg_data.py
--rw-rw-rw-   0        0        0     2915 2023-05-21 15:27:09.000000 brainsurf-6.0/brainsurf/data/eeg_data_visualization.py
--rw-rw-rw-   0        0        0     1237 2023-05-17 18:40:22.000000 brainsurf-6.0/brainsurf/data/mff.py
--rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-6.0/brainsurf/data/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.801613 brainsurf-6.0/brainsurf/machine_learning/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-6.0/brainsurf/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-6.0/brainsurf/machine_learning/eeg_binary_classification.py
--rw-rw-rw-   0        0        0      764 2023-05-08 17:36:08.000000 brainsurf-6.0/brainsurf/machine_learning/meditative_non_meditative.py
--rw-rw-rw-   0        0        0     2470 2023-05-10 16:29:13.000000 brainsurf-6.0/brainsurf/machine_learning/rnn.py
--rw-rw-rw-   0        0        0     2428 2023-05-10 16:31:42.000000 brainsurf-6.0/brainsurf/machine_learning/rnn2.py
--rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-6.0/brainsurf/machine_learning/rnn_module.py
--rw-rw-rw-   0        0        0     2220 2023-05-08 16:44:59.000000 brainsurf-6.0/brainsurf/machine_learning/t2.py
--rw-rw-rw-   0        0        0     3385 2023-05-08 17:24:37.000000 brainsurf-6.0/brainsurf/machine_learning/time_series.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.815154 brainsurf-6.0/brainsurf/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-6.0/brainsurf/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-14 16:45:53.000000 brainsurf-6.0/brainsurf/preprocessing/artifact_removal.py
--rw-rw-rw-   0        0        0     2108 2023-05-10 15:28:37.000000 brainsurf-6.0/brainsurf/preprocessing/baseline.py
--rw-rw-rw-   0        0        0     1137 2023-05-10 15:30:11.000000 brainsurf-6.0/brainsurf/preprocessing/epoching.py
--rw-rw-rw-   0        0        0     4216 2023-05-17 19:24:17.000000 brainsurf-6.0/brainsurf/preprocessing/filtering.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.828732 brainsurf-6.0/brainsurf/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-6.0/brainsurf/utils/__init__.py
--rw-rw-rw-   0        0        0      943 2023-05-17 20:26:04.000000 brainsurf-6.0/brainsurf/utils/data.py
--rw-rw-rw-   0        0        0      879 2023-04-29 03:52:10.000000 brainsurf-6.0/brainsurf/utils/performance_eval.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.860944 brainsurf-6.0/brainsurf/visualization/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-6.0/brainsurf/visualization/__init__.py
--rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-6.0/brainsurf/visualization/plot_cluster.py
--rw-rw-rw-   0        0        0      510 2023-04-29 03:44:56.000000 brainsurf-6.0/brainsurf/visualization/plot_coherence.py
--rw-rw-rw-   0        0        0      420 2023-04-29 03:45:05.000000 brainsurf-6.0/brainsurf/visualization/plot_cross-correlation.py
--rw-rw-rw-   0        0        0      243 2023-05-21 15:27:09.000000 brainsurf-6.0/brainsurf/visualization/plot_eeg_signal.py
--rw-rw-rw-   0        0        0      262 2023-04-29 03:45:13.000000 brainsurf-6.0/brainsurf/visualization/plot_heatmap.py
--rw-rw-rw-   0        0        0     1013 2023-04-29 03:45:23.000000 brainsurf-6.0/brainsurf/visualization/plot_power_spectrum.py
--rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-6.0/brainsurf/visualization/plot_spectogram.py
--rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-6.0/brainsurf/visualization/plot_time_series.py
--rw-rw-rw-   0        0        0      623 2023-04-29 03:46:07.000000 brainsurf-6.0/brainsurf/visualization/plot_topomap.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.698239 brainsurf-6.0/brainsurf.egg-info/
--rw-rw-rw-   0        0        0     2152 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2109 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 17:14:54.865521 brainsurf-6.0/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-05-30 17:14:44.000000 brainsurf-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.777526 brainsurf-7.0.0/
+-rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-7.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2391 2023-06-09 04:11:56.776512 brainsurf-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-06-09 03:59:51.000000 brainsurf-7.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.435017 brainsurf-7.0.0/brainsurf/
+-rw-rw-rw-   0        0        0       70 2023-06-09 04:00:14.000000 brainsurf-7.0.0/brainsurf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.530573 brainsurf-7.0.0/brainsurf/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-7.0.0/brainsurf/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-06-08 16:28:08.000000 brainsurf-7.0.0/brainsurf/analysis/corelation_analysis.py
+-rw-rw-rw-   0        0        0     1756 2023-05-31 17:53:43.000000 brainsurf-7.0.0/brainsurf/analysis/erp_analysis.py
+-rw-rw-rw-   0        0        0     1388 2023-06-08 16:30:02.000000 brainsurf-7.0.0/brainsurf/analysis/frequency.py
+-rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-7.0.0/brainsurf/analysis/multi_fractal.py
+-rw-rw-rw-   0        0        0     6163 2023-06-08 18:09:22.000000 brainsurf-7.0.0/brainsurf/analysis/power_spectrum.py
+-rw-rw-rw-   0        0        0     3071 2023-06-08 22:36:24.000000 brainsurf-7.0.0/brainsurf/analysis/stats_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.554545 brainsurf-7.0.0/brainsurf/cognitive/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-7.0.0/brainsurf/cognitive/__init__.py
+-rw-rw-rw-   0        0        0    14202 2023-06-08 23:43:40.000000 brainsurf-7.0.0/brainsurf/cognitive/cognitive_comparision.py
+-rw-rw-rw-   0        0        0     4202 2023-06-08 16:35:05.000000 brainsurf-7.0.0/brainsurf/cognitive/cognitive_indexes.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.604570 brainsurf-7.0.0/brainsurf/io/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-7.0.0/brainsurf/io/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-7.0.0/brainsurf/io/csv.py
+-rw-rw-rw-   0        0        0      167 2023-06-08 16:03:18.000000 brainsurf-7.0.0/brainsurf/io/df.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-7.0.0/brainsurf/io/edf.py
+-rw-rw-rw-   0        0        0    13064 2023-06-09 01:08:35.000000 brainsurf-7.0.0/brainsurf/io/eeg_data.py
+-rw-rw-rw-   0        0        0      213 2023-06-03 12:32:49.000000 brainsurf-7.0.0/brainsurf/io/mff.py
+-rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-7.0.0/brainsurf/io/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.633976 brainsurf-7.0.0/brainsurf/machine_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-7.0.0/brainsurf/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-7.0.0/brainsurf/machine_learning/eeg_binary_classification.py
+-rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-7.0.0/brainsurf/machine_learning/rnn_module.py
+-rw-rw-rw-   0        0        0     2813 2023-05-31 18:17:21.000000 brainsurf-7.0.0/brainsurf/machine_learning/time_series.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.668982 brainsurf-7.0.0/brainsurf/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-7.0.0/brainsurf/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2406 2023-06-09 01:04:29.000000 brainsurf-7.0.0/brainsurf/preprocessing/artifact_removal.py
+-rw-rw-rw-   0        0        0     3877 2023-06-08 16:16:32.000000 brainsurf-7.0.0/brainsurf/preprocessing/baseline.py
+-rw-rw-rw-   0        0        0     2141 2023-06-08 16:13:30.000000 brainsurf-7.0.0/brainsurf/preprocessing/epoching.py
+-rw-rw-rw-   0        0        0     5481 2023-06-08 17:33:30.000000 brainsurf-7.0.0/brainsurf/preprocessing/filtering.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.684975 brainsurf-7.0.0/brainsurf/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-7.0.0/brainsurf/utils/__init__.py
+-rw-rw-rw-   0        0        0      654 2023-06-09 01:14:33.000000 brainsurf-7.0.0/brainsurf/utils/data.py
+-rw-rw-rw-   0        0        0     1442 2023-06-08 16:23:07.000000 brainsurf-7.0.0/brainsurf/utils/performance.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.773512 brainsurf-7.0.0/brainsurf/visualization/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-7.0.0/brainsurf/visualization/__init__.py
+-rw-rw-rw-   0        0        0    10693 2023-06-09 01:23:23.000000 brainsurf-7.0.0/brainsurf/visualization/comparative_visualize.py
+-rw-rw-rw-   0        0        0     3483 2023-05-30 19:11:59.000000 brainsurf-7.0.0/brainsurf/visualization/eeg_data_visualization.py
+-rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-7.0.0/brainsurf/visualization/plot_cluster.py
+-rw-rw-rw-   0        0        0     1805 2023-06-08 21:00:05.000000 brainsurf-7.0.0/brainsurf/visualization/plot_coherence.py
+-rw-rw-rw-   0        0        0     4274 2023-06-08 17:59:04.000000 brainsurf-7.0.0/brainsurf/visualization/plot_correlation.py
+-rw-rw-rw-   0        0        0      555 2023-06-06 16:53:17.000000 brainsurf-7.0.0/brainsurf/visualization/plot_eeg_signal.py
+-rw-rw-rw-   0        0        0      262 2023-06-08 17:56:49.000000 brainsurf-7.0.0/brainsurf/visualization/plot_heatmap.py
+-rw-rw-rw-   0        0        0     2077 2023-06-08 18:16:20.000000 brainsurf-7.0.0/brainsurf/visualization/plot_power_spectrum.py
+-rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-7.0.0/brainsurf/visualization/plot_spectogram.py
+-rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-7.0.0/brainsurf/visualization/plot_time_series.py
+-rw-rw-rw-   0        0        0      566 2023-06-08 16:41:38.000000 brainsurf-7.0.0/brainsurf/visualization/plot_topomap.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:11:56.469016 brainsurf-7.0.0/brainsurf.egg-info/
+-rw-rw-rw-   0        0        0     2391 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 04:11:56.000000 brainsurf-7.0.0/brainsurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 04:11:56.777526 brainsurf-7.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-06-09 04:00:27.000000 brainsurf-7.0.0/setup.py
```

### Comparing `brainsurf-6.0/LICENSE` & `brainsurf-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brainsurf-6.0/PKG-INFO` & `brainsurf-7.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 6.0
+Version: 7.0.0
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -34,24 +34,27 @@
 `cd esp`
 `pip install -r requirements.txt`
 `python setup.py install`
 
 
 # Usage
 ```python
-import brainsurf.data as data
-import brainsurf.preprocessing as pre
-import brainsurf.analysis as analysis
-import brainsurf.visualization as vis
+import brainsurf.io.mff as load_input
+import brainsurf.utils.data as util
+import brainsurf.utils.performance as performance
+import brainsurf.preprocessing.filtering as filter
+import brainsurf.preprocessing.artifact_removal as artifact
+import brainsurf.preprocessing.epoching as epoching
 
 #load EEG data from file
-eeg_data = data.read_edf_file('eeg_data.edf')
+suriya_baseline = load_input.convert_mff_to_eegdata("C:/Users/Preethi V Hiremath/Downloads/Meditators/Suriya/BS.mff")
 
-#preprocess the data
-preprocessed_data = pre.bandpass_filter(eeg_data, low_cutoff=1, high_cutoff=40)
 
-#analyze the data
-erp_data = analysis.compute_erp(preprocessed_data, event_markers=[1, 2, 3], epoch_duration=2)
+values = np.asarray(suriya_baseline['sec'], dtype=object)
+sampling_freq = util.estimate_sampling_frequency(values)
 
-#visualize the results
-vis.plot_erp(erp_data)
+
+pre_preprocessed_data = preprocess_eeg_data(suriya_baseline,sampling_freq)
+
+print(performance.calculate_memory_efficiency())
+performance.monitor_resource_usage()
```

### Comparing `brainsurf-6.0/brainsurf/analysis/multi_fractal.py` & `brainsurf-7.0.0/brainsurf/analysis/multi_fractal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-6.0/brainsurf/analysis/stats_analysis.py` & `brainsurf-7.0.0/brainsurf/preprocessing/artifact_removal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,78 @@
 import numpy as np
+from sklearn.preprocessing import StandardScaler
+import mne
 import pandas as pd
-from scipy import signal
+from sklearn.decomposition import PCA
 
-import nolds
+def reject_bad_channels(raw, signal1, signal2):
+    """
+    Reject bad channels from the raw data.
 
-def calculate_mean(data):
-    return np.nanmean(data)
+    Parameters:
+        raw (object): Raw data object.
+        signal1 (array-like): Signal 1 data.
+        signal2 (array-like): Signal 2 data.
 
-def calculate_variance(data):
-    return np.nanvar(data)
+    Returns:
+        object: Cleaned raw data object.
+    """
+    bad_channels = ['E127', 'E128']  # Specify the channels to exclude
+    raw.info['bads'] = bad_channels
+    clean_raw = raw.copy().drop_channels(bad_channels)
+    return clean_raw
 
-import numpy as np
 
-def calculate_skewness(data):
+def reject_artifacts(epochs):
     """
-    Calculates skewness of given data.
+    Reject epochs containing artifacts.
 
     Parameters:
-    data (ndarray): 1-D or 2-D array of data.
+        epochs (ndarray): Epochs data of shape (n_epochs, n_channels, n_samples).
 
     Returns:
-    float: Skewness value of the data.
+        ndarray: Artifact-free epochs data.
     """
-    if data.ndim == 1:
-        mean = np.nanmean(data)
-        std = np.nanstd(data)
-        skewness = np.nanmean((data - mean) ** 3) / std ** 3
-    elif data.ndim == 2:
-        mean = np.nanmean(data, axis=1)
-        std = np.nanstd(data, axis=1)
-        skewness = np.nanmean(((data - mean[:, np.newaxis]) ** 3), axis=1) / (std ** 3)
-    else:
-        raise ValueError('Data must be 1-D or 2-D array.')
-    return skewness
+    artifact_threshold = 50  # Arbitrary threshold for artifact detection
+    artifact_free_epochs = epochs[np.max(np.abs(epochs), axis=1) < artifact_threshold]
+    return artifact_free_epochs
 
 
-def calculate_kurtosis(data):
+def signal_averaging(data):
     """
-    Calculates kurtosis of given data.
+    Perform signal averaging to remove random noise or artifacts.
+    """
+    averaged_signal = np.mean(data, axis=0)
+    return averaged_signal
 
-    Parameters:
-    data (ndarray): 1-D or 2-D array of data.
 
-    Returns:
-    float: Kurtosis value of the data.
+
+def artifact_subspace_reconstruction(data, artifact_components):
     """
-    if data.ndim == 1:
-        mean = np.nanmean(data)
-        std = np.nanstd(data)
-        kurtosis = np.nanmean((data - mean) ** 4) / std ** 4
-    elif data.ndim == 2:
-        mean = np.nanmean(data, axis=1)
-        std = np.nanstd(data, axis=1)
-        kurtosis = np.nanmean(((data - mean[:, np.newaxis]) ** 4), axis=1) / (std ** 4)
-    else:
-        raise ValueError('Data must be 1-D or 2-D array.')
-    return kurtosis
-
-
-def calculate_coherence(data1, data2, fs):
-    freqs, psd_data1 = signal.welch(data1, fs=fs, nperseg=1024)
-    freqs, psd_data2 = signal.welch(data2, fs=fs, nperseg=1024)
-    freqs, csd = signal.csd(data1, data2, fs=fs, nperseg=1024)
-    coh = np.abs(csd)**2 / (psd_data1 * psd_data2)
-    return freqs, coh
-
-
-def calculate_max(data):
-    return np.max(data, axis=1)
-
-def calculate_min(data):
-    return np.min(data, axis=1)
-
-def calculate_relative_power(freqs, psd):
-    delta_mask = (freqs >= 0.5) & (freqs <= 4)
-    theta_mask = (freqs >= 4) & (freqs <= 8)
-    alpha_mask = (freqs >= 8) & (freqs <= 13)
-    beta_mask = (freqs >= 13) & (freqs <= 30)
-
-    delta_power = np.trapz(psd[delta_mask], freqs[delta_mask])
-    theta_power = np.trapz(psd[theta_mask], freqs[theta_mask])
-    alpha_power = np.trapz(psd[alpha_mask], freqs[alpha_mask])
-    beta_power = np.trapz(psd[beta_mask], freqs[beta_mask])
-
-    total_power = delta_power + theta_power + alpha_power + beta_power
-
-    delta_power=delta_power / total_power
-    theta_power=theta_power / total_power
-    alpha_power=alpha_power / total_power
-    beta_power=beta_power / total_power
-    return {
-        "delta": delta_power / total_power,
-        "theta": theta_power / total_power,
-        "alpha": alpha_power / total_power,
-        "beta": beta_power / total_power
-    }
-
-def calc_ap_entropy(data, m=2, r=0.2):
-    ae = nolds.sampen(data, emb_dim=m, tolerance=r)
-    return ae
-
-def calc_fractal_dimension(data):
-    fd = nolds.dfa(data)
-    return fd
+    Perform artifact subspace reconstruction to remove artifacts modeled as a subspace.
+    """
+    artifact_components = StandardScaler().fit_transform(artifact_components)
+    data_projected = data - np.dot(np.dot(data, artifact_components.T), artifact_components)
+    return data_projected
+
+
+def regression_based_removal(data, regressor, artifacts):
+    """
+    Apply regression-based artifact removal by modeling artifacts as a function of other variables.
+    """
+    predicted_artifacts = regressor.predict(data)
+    cleaned_data = data - predicted_artifacts.reshape(-1, 1)
+    return cleaned_data
+
+def template_subtraction(data, template):
+    """
+    Perform template subtraction to remove artifacts with a consistent shape or waveform.
+    """
+    cleaned_data = data - template
+    return cleaned_data
+
+def remove_artifacts(raw):
+    ica = mne.preprocessing.ICA(n_components=30, random_state=42)
+    ica.fit(raw)
+    cleaned_raw = raw.copy()
+    ica.apply(cleaned_raw)
+    return cleaned_raw
```

### Comparing `brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py` & `brainsurf-7.0.0/brainsurf/cognitive/cognitive_comparision.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,79 @@
 import numpy as np
 from scipy.stats import ttest_rel, wilcoxon
-# from .cognitive_indexes import calculate_pe,calculate_band_power,calculate_arousal_index, calculate_neural_activity,calculate_engagement
+import pandas as pd
+from scipy import stats
+from brainsurf.cognitive.cognitive_indexes import calculate_arousal_index, calculate_band_power, calculate_engagement, calculate_neural_activity, calculate_pe
+import pandas as pd
+import scipy.stats as stats
+
+import numpy as np
+
+# def calculate_cognitive_indexes(data_before, data_after):
+#     """
+#     Calculate cognitive indexes from EEG data to assess attention, mental workload, or cognitive performance.
+#     Examples of cognitive indexes include response time, error rates, or other relevant measures.
+
+#     Args:
+#     - data_before (pandas.DataFrame or dict): EEG data before meditation.
+#     - data_after (pandas.DataFrame or dict): EEG data after meditation.
+
+#     Returns:
+#     - cognitive_indexes_before (numpy.ndarray): Cognitive indexes calculated from data_before.
+#     - cognitive_indexes_after (numpy.ndarray): Cognitive indexes calculated from data_after.
+#     """
+
+#     # Convert data_before and data_after to pandas DataFrames if they are dictionaries
+#     if isinstance(data_before, dict):
+#         data_before = pd.DataFrame(data_before)
+#     if isinstance(data_after, dict):
+#         data_after = pd.DataFrame(data_after)
+
+#     # Extract the necessary data columns from data_before
+#     alpha_power_before = data_before[0]['alpha']
+#     beta_power_before = data_before[0]['beta']
+#     delta_power_before = data_before[0]['delta']
+#     theta_power_before = data_before[0]['theta']
+
+#     # Define the frequency bands for calculation
+#     bands = {
+#         'delta': (0.5, 4),
+#         'theta': (4, 8),
+#         'alpha': (8, 13),
+#         'beta': (13, 30)
+#     }
+#     print(alpha_power_before, beta_power_before)
+#     # Calculate cognitive indexes before meditation
+#     pe_before = calculate_pe(alpha_power_before, beta_power_before)
+#     ai_before = calculate_arousal_index(alpha_power_before, theta_power_before)
+#     na_before = calculate_neural_activity(
+#         delta_power_before, theta_power_before, alpha_power_before, beta_power_before
+#     )
+#     eng_before = calculate_engagement(alpha_power_before, theta_power_before, delta_power_before)
+
+#     # Extract the necessary data columns from data_after
+#     alpha_power_after = data_after[0]['alpha']
+#     beta_power_after = data_after[0]['beta']
+#     delta_power_after = data_after[0]['delta']
+#     theta_power_after = data_after[0]['theta']
+    
+#     # Calculate cognitive indexes after meditation
+#     pe_after = calculate_pe(alpha_power_after, beta_power_after)
+#     ai_after = calculate_arousal_index(alpha_power_after, theta_power_after)
+#     na_after = calculate_neural_activity(
+#         delta_power_after, theta_power_after, alpha_power_after, beta_power_after
+#     )
+#     eng_after = calculate_engagement(alpha_power_after, theta_power_after, delta_power_after)
+
+#     # Compare the cognitive indexes before and after meditation using paired t-test
+#     cognitive_indexes_before = np.array([pe_before, ai_before, na_before, eng_before])
+#     cognitive_indexes_after = np.array([pe_after, ai_after, na_after, eng_after])
+
+#     # Perform the paired t-test
+#     return cognitive_indexes_before, cognitive_indexes_after
 
 def calculate_cognitive_indexes(data_before, data_after):
     """
     Calculate cognitive indexes from EEG data to assess attention, mental workload, or cognitive performance.
     Examples of cognitive indexes include response time, error rates, or other relevant measures.
 
     Args:
@@ -12,38 +81,14 @@
     - data_after (pandas.DataFrame): EEG data after meditation.
 
     Returns:
     - cognitive_indexes_before (numpy.ndarray): Cognitive indexes calculated from data_before.
     - cognitive_indexes_after (numpy.ndarray): Cognitive indexes calculated from data_after.
     """
 
-    def calculate_band_power(freqs, power, bands):
-        band_power = {}
-        for band, f_range in bands.items():
-            idx = np.logical_and(freqs >= f_range[0], freqs <= f_range[1])
-            band_power[band] = np.trapz(power[idx], freqs[idx])
-
-        return band_power
-
-    def calculate_pe(alpha_power, beta_power):
-        pe = beta_power / alpha_power
-        return pe
-
-    def calculate_arousal_index(alpha_power, theta_power):
-        ai = alpha_power / theta_power
-        return ai
-
-    def calculate_neural_activity(delta_power, theta_power, alpha_power, beta_power):
-        na = (delta_power + theta_power) / (alpha_power + beta_power)
-        return na
-
-    def calculate_engagement(alpha_power, theta_power, delta_power):
-        eng = (alpha_power + theta_power) / delta_power
-        return eng
-
     # Extract the necessary data columns from data_before
     freqs_before = data_before['sec']
     alpha_power_before = data_before['alpha']
     beta_power_before = data_before['beta']
     delta_power_before = data_before['delta']
     theta_power_before = data_before['theta']
 
@@ -110,67 +155,115 @@
         # Perform Wilcoxon signed-rank test
         test_statistic, p_value = wilcoxon(cognitive_indexes_before, cognitive_indexes_after)
     else:
         raise ValueError("Invalid test_type. Options: 'paired_ttest', 'wilcoxon'")
 
     return test_statistic, p_value
 
+
+
+# def compare_eeg_data_stats(pre_merged, post_merged):
+#     # Extract the relevant feature columns
+#     pre_eeg_raw = pre_merged['raw']
+#     pre_alpha = pre_merged['alpha']
+#     pre_beta = pre_merged['beta']
+#     pre_theta = pre_merged['theta']
+#     pre_delta = pre_merged['delta']
+
+#     post_eeg_raw = post_merged['raw']
+#     post_alpha = post_merged['alpha']
+#     post_beta = post_merged['beta']
+#     post_theta = post_merged['theta']
+#     post_delta = post_merged['delta'] 
+#     # Perform t-tests for each feature
+#     t_statistic_raw, p_value_raw = stats.ttest_ind(pre_eeg_raw, post_eeg_raw)
+#     t_statistic_alpha, p_value_alpha = stats.ttest_ind(pre_alpha, post_alpha)
+#     t_statistic_beta, p_value_beta = stats.ttest_ind(pre_beta, post_beta)
+#     t_statistic_theta, p_value_theta = stats.ttest_ind(pre_theta, post_theta)
+#     t_statistic_delta, p_value_delta = stats.ttest_ind(pre_delta, post_delta)
+#     # Perform ANOVA for each feature
+#     f_statistic_raw, p_value_anova_raw = stats.f_oneway(pre_eeg_raw, post_eeg_raw)
+#     f_statistic_alpha, p_value_anova_alpha = stats.f_oneway(pre_alpha, post_alpha)
+#     f_statistic_beta, p_value_anova_beta = stats.f_oneway(pre_beta, post_beta)
+#     f_statistic_theta, p_value_anova_theta = stats.f_oneway(pre_theta, post_theta)
+#     f_statistic_delta, p_value_anova_delta = stats.f_oneway(pre_delta, post_delta)
+
+#     # Calculate effect sizes (Cohen's d) for each feature
+#     effect_size_raw = abs(pre_eeg_raw.mean() - post_eeg_raw.mean()) / pre_eeg_raw.std()
+#     effect_size_alpha = abs(pre_alpha.mean() - post_alpha.mean()) / pre_alpha.std()
+#     effect_size_beta = abs(pre_beta.mean() - post_beta.mean()) / pre_beta.std()
+#     effect_size_theta = abs(pre_theta.mean() - post_theta.mean()) / pre_theta.std()
+#     effect_size_delta = abs(pre_delta.mean() - post_delta.mean()) / pre_delta.std()
+
+#     # Create a DataFrame to store the results
+#     results = pd.DataFrame({
+#         'Feature': ['EEG', 'Alpha', 'Beta', 'Theta', 'Delta'],
+#         'T-Stat': [t_statistic_raw, t_statistic_alpha, t_statistic_beta, t_statistic_theta, t_statistic_delta],
+#         'P-Value (T-Test)': [p_value_raw, p_value_alpha, p_value_beta, p_value_theta, p_value_delta],
+#         'F-Stat': [f_statistic_raw, f_statistic_alpha, f_statistic_beta, f_statistic_theta, f_statistic_delta],
+#         'P-Value (ANOVA)': [p_value_anova_raw, p_value_anova_alpha, p_value_anova_beta, p_value_anova_theta, p_value_anova_delta],
+#         'Effect Size': [effect_size_raw, effect_size_alpha, effect_size_beta, effect_size_theta, effect_size_delta]
+#     })
+#     return results
+
+import pandas as pd
+from scipy import stats
 import pandas as pd
 from scipy import stats
 
-def analyze_eeg_data(pre_merged, post_merged):
-    # Extract the relevant feature columns
-    pre_eeg_raw = pre_merged['raw']
-    pre_alpha = pre_merged['alpha']
-    pre_beta = pre_merged['beta']
-    pre_theta = pre_merged['theta']
-    pre_delta = pre_merged['delta']
-
-    post_eeg_raw = post_merged['raw']
-    post_alpha = post_merged['alpha']
-    post_beta = post_merged['beta']
-    post_theta = post_merged['theta']
-    post_delta = post_merged['delta']
-
-    # Perform t-tests for each feature
-    t_statistic_raw, p_value_raw = stats.ttest_ind(pre_eeg_raw, post_eeg_raw)
-    t_statistic_alpha, p_value_alpha = stats.ttest_ind(pre_alpha, post_alpha)
-    t_statistic_beta, p_value_beta = stats.ttest_ind(pre_beta, post_beta)
-    t_statistic_theta, p_value_theta = stats.ttest_ind(pre_theta, post_theta)
-    t_statistic_delta, p_value_delta = stats.ttest_ind(pre_delta, post_delta)
-
-    # Perform ANOVA for each feature
-    f_statistic_raw, p_value_anova_raw = stats.f_oneway(pre_eeg_raw, post_eeg_raw)
-    f_statistic_alpha, p_value_anova_alpha = stats.f_oneway(pre_alpha, post_alpha)
-    f_statistic_beta, p_value_anova_beta = stats.f_oneway(pre_beta, post_beta)
-    f_statistic_theta, p_value_anova_theta = stats.f_oneway(pre_theta, post_theta)
-    f_statistic_delta, p_value_anova_delta = stats.f_oneway(pre_delta, post_delta)
-
-    # Calculate effect sizes (Cohen's d) for each feature
-    effect_size_raw = abs(pre_eeg_raw.mean() - post_eeg_raw.mean()) / pre_eeg_raw.std()
-    effect_size_alpha = abs(pre_alpha.mean() - post_alpha.mean()) / pre_alpha.std()
-    effect_size_beta = abs(pre_beta.mean() - post_beta.mean()) / pre_beta.std()
-    effect_size_theta = abs(pre_theta.mean() - post_theta.mean()) / pre_theta.std()
-    effect_size_delta = abs(pre_delta.mean() - post_delta.mean()) / pre_delta.std()
-
-    # Create a DataFrame to store the results
-    results = pd.DataFrame({
-        'Feature': ['EEG', 'Alpha', 'Beta', 'Theta', 'Delta'],
-        'T-Stat': [t_statistic_raw, t_statistic_alpha, t_statistic_beta, t_statistic_theta, t_statistic_delta],
-        'P-Value (T-Test)': [p_value_raw, p_value_alpha, p_value_beta, p_value_theta, p_value_delta],
-        'F-Stat': [f_statistic_raw, f_statistic_alpha, f_statistic_beta, f_statistic_theta, f_statistic_delta],
-        'P-Value (ANOVA)': [p_value_anova_raw, p_value_anova_alpha, p_value_anova_beta, p_value_anova_theta, p_value_anova_delta],
-        'Effect Size': [effect_size_raw, effect_size_alpha, effect_size_beta, effect_size_theta, effect_size_delta]
-    })
 
+def compare_eeg_data_stats(pre_merged, post_merged, feature_columns):
+    results = pd.DataFrame(columns=['Feature', 'T-Stat', 'P-Value (T-Test)', 'F-Stat', 'P-Value (ANOVA)', 'Effect Size'])
+    
+    for feature in feature_columns:
+        pre_data = pre_merged[feature]
+        post_data = post_merged[feature]
+        
+        t_statistic, p_value_ttest = stats.ttest_ind(pre_data, post_data)
+        f_statistic, p_value_anova = stats.f_oneway(pre_data, post_data)
+        
+        effect_size = abs(pre_data.mean() - post_data.mean()) / pre_data.std()
+        
+        result = pd.DataFrame({
+            'Feature': [feature],
+            'T-Stat': [t_statistic],
+            'P-Value (T-Test)': [p_value_ttest],
+            'F-Stat': [f_statistic],
+            'P-Value (ANOVA)': [p_value_anova],
+            'Effect Size': [effect_size]
+        })
+        
+        results = pd.concat([results, result], ignore_index=True)
+    
     return results
 
 
-import pandas as pd
-import numpy as np
+
+
+def perform_ttest(data_before, data_after):
+    t_stat, p_value = stats.ttest_rel(data_before, data_after)
+    return t_stat, p_value
+
+def calculate_ttest_results(df):
+    variables = ['Arousal Index', 'Neural Activity', 'Performance Index', 'Engagement']
+    columns = ['t-statistic', 'p-value']
+    results = []
+
+    for variable in variables:
+        data_before = df[f'{variable} Before']
+        data_after = df[f'{variable} After']
+        t_stat, p_value = perform_ttest(data_before, data_after)
+        results.append([t_stat, p_value])
+
+    ttest_results_df = pd.DataFrame(results, index=variables, columns=columns)
+    return ttest_results_df
+
+# # Example usage:
+# ttest_results_df = calculate_ttest_results(df)
+
 
 def analyze_stroop_data(data):
     # Convert the data to a pandas DataFrame for easier analysis
     df = pd.DataFrame(data, columns=["Color 1", "Color 2", "Congruent", "Response Time", "Accuracy", "Block", "Trial"])
 
     # Calculate average response time for congruent and incongruent trials
     congruent_rt = df[df["Congruent"] == 1]["Response Time"]
@@ -188,23 +281,28 @@
 
     avg_congruent_acc = np.mean(congruent_acc)
     avg_incongruent_acc = np.mean(incongruent_acc)
 
     # Perform t-test for accuracy (without using scipy)
     t_value_acc, p_value_acc = independent_ttest(congruent_acc, incongruent_acc)
 
-    # Print the results
-    print("Response Time Analysis:")
-    print("Average Response Time - Congruent: {:.2f}".format(avg_congruent_rt))
-    print("Average Response Time - Incongruent: {:.2f}".format(avg_incongruent_rt))
-    print("T-Test - Response Time: t-value = {:.2f}, p-value = {:.4f}".format(t_value, p_value))
-    print("\nAccuracy Analysis:")
-    print("Average Accuracy - Congruent: {:.2f}%".format(avg_congruent_acc * 100))
-    print("Average Accuracy - Incongruent: {:.2f}%".format(avg_incongruent_acc * 100))
-    print("T-Test - Accuracy: t-value = {:.2f}, p-value = {:.4f}".format(t_value_acc, p_value_acc))
+    # Store the results in a dictionary
+    results = {
+        "Average Response Time - Congruent": avg_congruent_rt,
+        "Average Response Time - Incongruent": avg_incongruent_rt,
+        "T-Test - Response Time - t-value": t_value,
+        "T-Test - Response Time - p-value": p_value,
+        "Average Accuracy - Congruent": avg_congruent_acc,
+        "Average Accuracy - Incongruent": avg_incongruent_acc,
+        "T-Test - Accuracy - t-value": t_value_acc,
+        "T-Test - Accuracy - p-value": p_value_acc
+    }
+
+    return results
+
 
 def independent_ttest(x, y):
     # Calculate the t-value and p-value for two independent samples
     mean_diff = np.mean(x) - np.mean(y)
     var_x = np.var(x, ddof=1)
     var_y = np.var(y, ddof=1)
     n_x = len(x)
```

### Comparing `brainsurf-6.0/brainsurf/data/eeg_data.py` & `brainsurf-7.0.0/brainsurf/io/eeg_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 import pandas as pd
 import pyedflib
-import h5py 
+import mne
 import numpy as np
 from scipy.signal import welch
-
-
 class EEGData:
     def __init__(self, **kwargs):
         self.data = pd.DataFrame(kwargs)
 
     def __len__(self):
         return len(self.data)
+    def drop_columns(self, columns):
+        """
+        Drop specified columns from the EEGData object.
 
+        Parameters:
+            columns (str or list): The column(s) to drop.
+
+        Returns:
+            None
+        """
+        if isinstance(columns, str):
+            columns = [columns]  # Convert single column name to a list
+
+        existing_columns = list(self.data.columns)
+        columns_to_drop = [col for col in columns if col in existing_columns]
+
+        if columns_to_drop:
+            self.data.drop(columns=columns_to_drop, inplace=True)
+        else:
+            print("Specified column(s) not found in the EEGData object.")
     def get_data(self):
         return self.data
 
     def data_length(self):
         length = 0
         for value in self.data.values():
             if isinstance(value, list):
@@ -185,23 +202,66 @@
 
             
             # Repeat the above code for other frequency bands (beta, theta, delta, gamma)
             # Adjust the frequency ranges and feature extraction accordingly
             
         else:
             raise ValueError("Required keys 'raw' and 'sec' are missing in the EEGData object.")
+        
+    def apply_ica(self, n_components=20, random_state=None):
+        
+        if 'raw' in self.data:
+            raw_data = self.data['raw']
+            
+            # Convert raw data to MNE Raw object
+            info = mne.create_info(ch_names=raw_data.columns.tolist(), sfreq=128)  # Adjust sfreq as per your data
+            raw = mne.io.RawArray(raw_data.T.values, info)
+            
+            # Apply ICA
+            ica = mne.preprocessing.ICA(n_components=n_components, random_state=random_state)
+            ica.fit(raw)
+            
+            # Apply ICA to raw data
+            ica_raw = ica.apply(raw)
+            
+            # Update raw data in EEGData object with cleaned data
+            self.data['raw'] = pd.DataFrame(ica_raw.get_data().T, columns=raw_data.columns)
+        else:
+            raise ValueError("Required key 'raw' is missing in the EEGData object.")
+        
+    def apply_car(self):
+        """
+        Apply Common Average Reference (CAR) to the EEG data.
+
+        Returns:
+            None
+        """
+        if 'raw' in self.data:
+            raw_data = self.data['raw']
+            
+            # Apply CAR
+            car_data = raw_data - np.mean(raw_data, axis=1, keepdims=True)
+            
+            # Update raw data in EEGData object with CAR data
+            self.data['raw'] = pd.DataFrame(car_data, columns=raw_data.columns)
+        else:
+            raise ValueError("Required key 'raw' is missing in the EEGData object.")
 
 
 
 
 class EEGDataFactory:
     def create_eeg_data(self, input_file):
-
+        if isinstance(input_file, pd.DataFrame):
+            eeg_data = EEGData()
+            for column in input_file.columns:
+                eeg_data.add_data(column, input_file[column])
+            return eeg_data
         #CSV
-        if input_file.endswith('.csv'):
+        elif input_file.endswith('.csv'):
             data = self.parse_csv(input_file)
             if 'sec' in data.columns and 'EEG' in data.columns and 'alpha' in data.columns and 'beta' in data.columns and 'delta' in data.columns and 'theta ' in data.columns:
                 # CSV data with sec, alpha, beta,  delta and theta columns            
                 return EEGData(sec=data['sec'], raw=data['EEG'], alpha=data['alpha'], beta=data['beta'], theta=data['theta '], delta =data['delta'])
             elif 'sec' in data.columns:
                 # CSV data with raw and sec columns
                 return EEGData(sec=data['sec'], raw=data['EEG'])
@@ -213,27 +273,20 @@
             # Parse EDF data
             data = self.parse_edf(input_file)
             channel_names = data['channel_names']
             raw_data = data['raw_data']
             return EEGData(channel_names=channel_names, raw_data=raw_data)
     
         elif input_file.endswith('.mff'):
-            data = self.parse_mff(input_file)
-           
-            if 'sec' in data.columns and 'EEG' in data.columns and 'alpha' in data.columns and 'beta' in data.columns and 'delta' in data.columns and 'theta ' in data.columns:
-                    # CSV data with sec, alpha, beta, and gamma columns            
-                    return EEGData(sec=data['sec'], raw=data['EEG'], alpha=data['alpha'], beta=data['beta'], theta=data['theta '], delta =data['delta'])
-            elif 'sec' in data.columns:
-                    # CSV data with raw and time columns
-                    return EEGData(time=data['sec'], raw=data['EEG'])
-            elif 'EEG' in data.col:
-                    # CSV data with only raw data
-                    return EEGData(raw=data['EEG'])
-            else:
-                return EEGData(sec=data['time'], raw=data['EEG'], channel_names=channel_names)
+            raw = mne.io.read_raw_egi(input_file)
+            eeg_data = raw.get_data()
+            time_points = raw.times
+            baseline = pd.DataFrame(data=eeg_data.T, columns=raw.ch_names)
+            baseline['sec'] = time_points
+            return baseline
             # Create EEGData object with the extracted data           
         
         elif input_file.endswith('.xlsx'):
             data = self.parse_xlsx(input_file)
             # Extract relevant information from the XLSX data
             if 'sec' in data.columns and 'EEG' in data.columns and 'alpha' in data.columns and 'beta' in data.columns and 'delta' in data.columns and 'theta ' in data.columns:
                     # CSV data with sec, alpha, beta, and gamma columns            
@@ -242,25 +295,16 @@
                     # CSV data with raw and time columns
                     return EEGData(sec=data['sec'], raw=data['EEG'])
             else:
                     # CSV data with only raw data
                     return EEGData(raw=data['EEG'])
         else:
             raise ValueError("Invalid file format. Only CSV, EDF, MFF, and XLSX files are supported.")
- 
-  
-    def parse_mff(self, input_file):
-        # Implement your MFF file parsing logic here
-        with h5py.File(input_file, 'r') as f:
-            sec = f['/path/to/timestamps'][()]  # Replace '/path/to/timestamps' with the actual dataset path
-            eeg_signals = f['/path/to/eeg_signals'][()]  # Replace '/path/to/eeg_signals' with the actual dataset path
-            channel_names = f['/path/to/channel_names'][()]  # Replace '/path/to/channel_names' with the actual dataset path
-        
-        data = {'sec': sec, 'eeg_signals': eeg_signals, 'channel_names': channel_names}
-        return data
+    
+    
 
     def parse_csv(self, input_file):
         data = pd.read_csv(input_file)
         return data
 
     def parse_edf(self, input_file):
         f = pyedflib.EdfReader(input_file)
```

### Comparing `brainsurf-6.0/brainsurf/data/eeg_data_visualization.py` & `brainsurf-7.0.0/brainsurf/visualization/eeg_data_visualization.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,48 +6,54 @@
 from scipy.signal import coherence
 from scipy.signal import correlate2d
 
 class EEGVisualizationFactory:
     def __init__(self, data):
         self.data = data
 
-    def plot_eeg_signal(self):
+    def plot_eeg_signal(self, x_label='Time [sec]', y_label='EEG', title='EEG Signal'):
         sec = self.data['sec']
-        EEG = self.data['raw']
-        plt.plot(sec, EEG)
-        plt.xlabel('Time [sec]')
-        plt.ylabel('EEG')
-        plt.title('EEG Signal')
+        eeg = self.data['raw']
+        plt.plot(sec, eeg)
+        plt.xlabel(x_label)
+        plt.ylabel(y_label)
+        plt.title(title)
         plt.show()
 
-    def plot_spectrogram(self, channel):
+    def plot_spectrogram(self, channel, fs=None, window='hann', nperseg=256, noverlap=None,
+                         cmap='RdBu_r', scaling='density', x_label='Time [sec]', y_label='Frequency [Hz]',
+                         title=None):
         sec = self.data['sec']
-        data = self.data[channel]
-        fs = 1.0 / (sec[1] - sec[0])
-        window = 'hann'
-        nperseg = 256
-        noverlap = None
-        cmap = 'RdBu_r'
-        scaling = 'density'
-        f, t, Sxx = spectrogram(data, fs=fs, window=window, nperseg=nperseg, noverlap=noverlap, scaling=scaling)
+        channel_data = self.data[channel]
+        if fs is None:
+            fs = 1.0 / (sec[1] - sec[0])
+        f, t, Sxx = spectrogram(channel_data, fs=fs, window=window, nperseg=nperseg, noverlap=noverlap, scaling=scaling)
         plt.pcolormesh(t, f, Sxx, cmap=cmap)
-        plt.ylabel('Frequency [Hz]')
-        plt.xlabel('Time [sec]')
-        plt.title(f'Spectrogram ({channel})')
+        plt.ylabel(y_label)
+        plt.xlabel(x_label)
+        if title is not None:
+            plt.title(title)
+        else:
+            plt.title(f'Spectrogram ({channel})')
         plt.colorbar()
         plt.show()
 
-    def plot_power_spectrum(self, channel):
+    def plot_power_spectrum(self, channel, fs=None, x_label='Frequency [Hz]', y_label='Power Spectral Density',
+                            title=None):
         sec = self.data['sec']
-        data = self.data[channel]
-        fs = 1.0 / (sec[1] - sec[0])
-        f, Pxx = plt.psd(data, Fs=fs)
-        plt.xlabel('Frequency [Hz]')
-        plt.ylabel('Power Spectral Density')
-        plt.title(f'Power Spectrum ({channel})')
+        channel_data = self.data[channel]
+        if fs is None:
+            fs = 1.0 / (sec[1] - sec[0])
+        f, Pxx = plt.psd(channel_data, Fs=fs)
+        plt.xlabel(x_label)
+        plt.ylabel(y_label)
+        if title is not None:
+            plt.title(title)
+        else:
+            plt.title(f'Power Spectrum ({channel})')
         plt.show()
 
     def plot_coherence(self, channel1, channel2, freq_range=None):
         sec = self.data['sec']
         data1 = self.data[channel1]
         data2 = self.data[channel2]
         fs = 1.0 / (sec[1] - sec[0])
@@ -73,18 +79,22 @@
         plt.plot(corr)
         plt.xlabel('Time')
         plt.ylabel('Cross-Correlation')
         plt.title(f'Cross-Correlation ({channel1} vs {channel2})')
         plt.show()
 
     def plot_heatmap(self):
-       corr_matrix = self.data.corr()
-       plt.figure(figsize=(10, 8))
-       sns.heatmap(corr_matrix, cmap='RdBu_r', annot=True, fmt=".2f", vmin=-1, vmax=1)
-       plt.title('EEG Data Heatmap')
-       plt.xticks(rotation=90)
-       plt.yticks(rotation=0)
-       plt.show()
+        eeg_df = pd.DataFrame(self.data)
+        # Calculate the correlation matrix
+        corr_matrix = eeg_df.corr()
+        # Plot the correlation heatmap
+        plt.figure(figsize=(10, 8))
+        sns.heatmap(corr_matrix, cmap='RdBu_r', annot=True, fmt=".2f", vmin=-1, vmax=1)
+        plt.title('EEG Data Heatmap')
+        plt.xticks(rotation=90)
+        plt.yticks(rotation=0)
+        plt.show()
+
```

### Comparing `brainsurf-6.0/brainsurf/machine_learning/eeg_binary_classification.py` & `brainsurf-7.0.0/brainsurf/machine_learning/eeg_binary_classification.py`

 * *Files identical despite different names*

### Comparing `brainsurf-6.0/brainsurf/machine_learning/rnn_module.py` & `brainsurf-7.0.0/brainsurf/machine_learning/rnn_module.py`

 * *Files identical despite different names*

### Comparing `brainsurf-6.0/brainsurf/machine_learning/time_series.py` & `brainsurf-7.0.0/brainsurf/machine_learning/time_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import numpy as np
 import pandas as pd
 from sklearn.metrics import r2_score
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler
-from sklearn.metrics import accuracy_score, mean_squared_error
-from sklearn.model_selection import GridSearchCV
-from sklearn.linear_model import LinearRegression
-from sklearn.tree import DecisionTreeRegressor
+from sklearn.metrics import mean_squared_error
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.ensemble import RandomForestRegressor
 import matplotlib.pyplot as plt
-
 def load_data(filepath):
     data = pd.read_csv(filepath)
     print(data.head())
     return data
 
 def preprocess_data(data):
     """
@@ -93,15 +89,7 @@
     axs[0, 0].legend()
     axs[0, 1].legend()
     axs[1, 0].legend()
     axs[1, 1].legend()
 
     plt.show()
 
-
-if __name__ == '__main__':
-    data = load_data('C:/Users/Preethi V Hiremath/OneDrive/Desktop/Projects/esp/brainsurf/data/eeg_data/sample_data2.csv')
-    preprocessed_data = preprocess_data(data)
-    X_train, X_test, y_train, y_test = split_data(preprocessed_data)
-    model = train_model(X_train, y_train)
-    evaluate_model(model, X_test, y_test)
-    visualize_predictions(model, X_test, y_test)
```

### Comparing `brainsurf-6.0/brainsurf/preprocessing/filtering.py` & `brainsurf-7.0.0/brainsurf/preprocessing/filtering.py`

 * *Files 20% similar despite different names*

```diff
@@ -57,63 +57,94 @@
     """
     nyq = 0.5 * fs
     cutoff = cutoff_freq / nyq
     b, a = butter(order, cutoff, btype='low')
     y = lfilter(b, a, data)
     return y
 
+def apply_highpass_filter(raw, highpass_freq):
+    """
+    Apply a high-pass filter to the raw data.
+
+    Parameters:
+        raw (Raw object): The raw data to be filtered.
+        highpass_freq (float): The cut-off frequency for the high-pass filter.
+
+    Returns:
+        Raw object: The filtered raw data.
+
+    """
+    raw.filter(l_freq=highpass_freq, h_freq=None)
+    return raw
+
+def apply_lowpass_filter(raw, lowpass_freq):
+    """
+    Apply a low-pass filter to the raw data.
+
+    Parameters:
+        raw (Raw object): The raw data to be filtered.
+        lowpass_freq (float): The cut-off frequency for the low-pass filter.
+
+    Returns:
+        Raw object: The filtered raw data.
+
+    """
+    raw.filter(l_freq=None, h_freq=lowpass_freq)
+    return raw
+
+
 def highpass_filter(data, cutoff_freq, fs, order):
     """
     Apply a high-pass filter to the input data.
 
     Parameters:
-        data (array-like): Input data to be filtered.
-        cutoff_freq (float): Cut-off frequency of the filter.
-        fs (float): Sampling frequency of the data.
-        order (int): Order of the Butterworth filter.
+        data (array-like): The input data to be filtered.
+        cutoff_freq (float): The cut-off frequency of the filter.
+        fs (float): The sampling frequency of the data.
+        order (int): The order of the Butterworth filter.
 
     Returns:
-        array-like: Filtered data.
+        array-like: The filtered data.
 
     """
     nyq = 0.5 * fs
     cutoff = cutoff_freq / nyq
     b, a = butter(order, cutoff, btype='high')
     y = lfilter(b, a, data)
     return y
 
 def comb_filter(data, delay, gain):
     """
     Apply a comb filter to the input data.
 
     Parameters:
-        data (array-like): Input data to be filtered.
-        delay (int): Delay value for the comb filter.
-        gain (float): Gain value for the comb filter.
+        data (array-like): The input data to be filtered.
+        delay (int): The delay parameter of the comb filter.
+        gain (float): The gain parameter of the comb filter.
 
     Returns:
-        array-like: Filtered data.
+        array-like: The filtered data.
 
     """
     y = np.zeros_like(data)
     for i in range(delay, len(data)):
         y[i] = data[i] + gain * data[i - delay]
     return y
 
 def adaptive_filter(data, reference, order):
     """
     Apply an adaptive filter to the input data.
 
     Parameters:
-        data (array-like): Input data to be filtered.
-        reference (array-like): Reference data for the adaptive filter.
-        order (int): Order of the adaptive filter.
+        data (array-like): The input data to be filtered.
+        reference (array-like): The reference signal for the adaptive filter.
+        order (int): The order of the adaptive filter.
 
     Returns:
-        array-like: Filtered data.
+        array-like: The filtered data.
 
     """
     y = np.zeros_like(data)
     w = np.zeros(order)
     for i in range(order, len(data)):
         x = data[i-order:i][::-1]
         y[i] = np.dot(w, x)
@@ -122,27 +153,42 @@
     return y
 
 def kalman_filter(data, measurement_noise, process_noise):
     """
     Apply a Kalman filter to the input data.
 
     Parameters:
-        data (array-like): Input data to be filtered.
-        measurement_noise (float): Measurement noise covariance.
-        process_noise (float): Process noise covariance.
+        data (array-like): The input data to be filtered.
+        measurement_noise (float): The measurement noise of the Kalman filter.
+        process_noise (float): The process noise of the Kalman filter.
 
     Returns:
-        array-like: Filtered data.
+        array-like: The filtered data.
 
     """
     n = len(data)
     x = np.zeros(n)
     P = np.zeros(n)
     x[0] = data[0]
     P[0] = measurement_noise
     for i in range(1, n):
         x_priori = x[i-1]
         P_priori = P[i-1] + process_noise
         K = P_priori / (P_priori + measurement_noise)
         x[i] = x_priori + K * (data[i] - x_priori)
         P[i] = (1 - K) * P_priori
     return x
+
+
+def apply_spatial_filter(epochs):
+    """
+    Apply a spatial filter to the input epochs.
+
+    Parameters:
+        epochs (Epochs object): The epochs data to be filtered.
+
+    Returns:
+        Epochs object: The spatially filtered epochs.
+
+    """
+    spatial_filtered_epochs = epochs  # Placeholder, implement as required
+    return spatial_filtered_epochs
```

### Comparing `brainsurf-6.0/brainsurf/visualization/plot_time_series.py` & `brainsurf-7.0.0/brainsurf/visualization/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-6.0/brainsurf/visualization/plot_topomap.py` & `brainsurf-7.0.0/brainsurf/visualization/plot_topomap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-# cannot visualize as we dont have positional information
+
 def plot_topomap(data, pos, vmin=None, vmax=None, cmap='viridis', show=True):
     fig, ax = plt.subplots()
     sc = ax.scatter(pos[:, 0], pos[:, 1], c=data, cmap=cmap, vmin=vmin, vmax=vmax)
     plt.colorbar(sc, ax=ax)
     ax.set_xlim([np.min(pos[:, 0]) - 0.1, np.max(pos[:, 0]) + 0.1])
     ax.set_ylim([np.min(pos[:, 1]) - 0.1, np.max(pos[:, 1]) + 0.1])
     ax.set_title('Topographic Map')
```

### Comparing `brainsurf-6.0/brainsurf.egg-info/PKG-INFO` & `brainsurf-7.0.0/brainsurf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 6.0
+Version: 7.0.0
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -34,24 +34,27 @@
 `cd esp`
 `pip install -r requirements.txt`
 `python setup.py install`
 
 
 # Usage
 ```python
-import brainsurf.data as data
-import brainsurf.preprocessing as pre
-import brainsurf.analysis as analysis
-import brainsurf.visualization as vis
+import brainsurf.io.mff as load_input
+import brainsurf.utils.data as util
+import brainsurf.utils.performance as performance
+import brainsurf.preprocessing.filtering as filter
+import brainsurf.preprocessing.artifact_removal as artifact
+import brainsurf.preprocessing.epoching as epoching
 
 #load EEG data from file
-eeg_data = data.read_edf_file('eeg_data.edf')
+suriya_baseline = load_input.convert_mff_to_eegdata("C:/Users/Preethi V Hiremath/Downloads/Meditators/Suriya/BS.mff")
 
-#preprocess the data
-preprocessed_data = pre.bandpass_filter(eeg_data, low_cutoff=1, high_cutoff=40)
 
-#analyze the data
-erp_data = analysis.compute_erp(preprocessed_data, event_markers=[1, 2, 3], epoch_duration=2)
+values = np.asarray(suriya_baseline['sec'], dtype=object)
+sampling_freq = util.estimate_sampling_frequency(values)
 
-#visualize the results
-vis.plot_erp(erp_data)
+
+pre_preprocessed_data = preprocess_eeg_data(suriya_baseline,sampling_freq)
+
+print(performance.calculate_memory_efficiency())
+performance.monitor_resource_usage()
```

### Comparing `brainsurf-6.0/brainsurf.egg-info/SOURCES.txt` & `brainsurf-7.0.0/brainsurf.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -6,53 +6,45 @@
 brainsurf.egg-info/SOURCES.txt
 brainsurf.egg-info/dependency_links.txt
 brainsurf.egg-info/requires.txt
 brainsurf.egg-info/top_level.txt
 brainsurf/analysis/__init__.py
 brainsurf/analysis/corelation_analysis.py
 brainsurf/analysis/erp_analysis.py
-brainsurf/analysis/find_range.py
+brainsurf/analysis/frequency.py
 brainsurf/analysis/multi_fractal.py
 brainsurf/analysis/power_spectrum.py
 brainsurf/analysis/stats_analysis.py
-brainsurf/analysis/time_frequency.py
-brainsurf/analysis/wavelet_transform.py
-brainsurf/cognitive_analysis_module/__init__.py
-brainsurf/cognitive_analysis_module/cognitive_comparision.py
-brainsurf/cognitive_analysis_module/cognitive_indexes.py
-brainsurf/comparitive_analysis/__init__.py
-brainsurf/comparitive_analysis/meditation_comparision.py
-brainsurf/comparitive_analysis/t_test.py
-brainsurf/data/__init__.py
-brainsurf/data/comparative_visualize.py
-brainsurf/data/csv.py
-brainsurf/data/edf.py
-brainsurf/data/eeg_data.py
-brainsurf/data/eeg_data_visualization.py
-brainsurf/data/mff.py
-brainsurf/data/xlsx.py
+brainsurf/cognitive/__init__.py
+brainsurf/cognitive/cognitive_comparision.py
+brainsurf/cognitive/cognitive_indexes.py
+brainsurf/io/__init__.py
+brainsurf/io/csv.py
+brainsurf/io/df.py
+brainsurf/io/edf.py
+brainsurf/io/eeg_data.py
+brainsurf/io/mff.py
+brainsurf/io/xlsx.py
 brainsurf/machine_learning/__init__.py
 brainsurf/machine_learning/eeg_binary_classification.py
-brainsurf/machine_learning/meditative_non_meditative.py
-brainsurf/machine_learning/rnn.py
-brainsurf/machine_learning/rnn2.py
 brainsurf/machine_learning/rnn_module.py
-brainsurf/machine_learning/t2.py
 brainsurf/machine_learning/time_series.py
 brainsurf/preprocessing/__init__.py
 brainsurf/preprocessing/artifact_removal.py
 brainsurf/preprocessing/baseline.py
 brainsurf/preprocessing/epoching.py
 brainsurf/preprocessing/filtering.py
 brainsurf/utils/__init__.py
 brainsurf/utils/data.py
-brainsurf/utils/performance_eval.py
+brainsurf/utils/performance.py
 brainsurf/visualization/__init__.py
+brainsurf/visualization/comparative_visualize.py
+brainsurf/visualization/eeg_data_visualization.py
 brainsurf/visualization/plot_cluster.py
 brainsurf/visualization/plot_coherence.py
-brainsurf/visualization/plot_cross-correlation.py
+brainsurf/visualization/plot_correlation.py
 brainsurf/visualization/plot_eeg_signal.py
 brainsurf/visualization/plot_heatmap.py
 brainsurf/visualization/plot_power_spectrum.py
 brainsurf/visualization/plot_spectogram.py
 brainsurf/visualization/plot_time_series.py
 brainsurf/visualization/plot_topomap.py
```

### Comparing `brainsurf-6.0/setup.py` & `brainsurf-7.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='brainsurf',
-    version='6.0',
+    version='7.0.0',
     description='EEG Signal Processing Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='preethivhiremath',
     author_email='preethivhiremath.vh@gmail.com',
     url='https://github.com/preethihiremath/brainsurf',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'mne',
         'pyabf',
         'nolds',
+        'pytest',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

