# Comparing `tmp/man_etl-1.0.1.tar.gz` & `tmp/man_etl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "man_etl-1.0.1.tar", last modified: Fri Jun  9 00:32:54 2023, max compression
+gzip compressed data, was "man_etl-1.0.2.tar", last modified: Fri Jun  9 13:36:53 2023, max compression
```

## Comparing `man_etl-1.0.1.tar` & `man_etl-1.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:50.859559 man_etl-1.0.1/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-09 12:37:50.852559 man_etl-1.0.1/PKG-INFO
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2199 2023-06-09 08:21:22.000000 man_etl-1.0.1/README.md
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:49.257300 man_etl-1.0.1/man_etl/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-1.0.1/man_etl/__init__.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:50.005282 man_etl-1.0.1/man_etl/etl_pipelines/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:46:59.000000 man_etl-1.0.1/man_etl/etl_pipelines/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      783 2023-06-09 09:46:43.000000 man_etl-1.0.1/man_etl/etl_pipelines/arctic_to_arrowflight.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1163 2023-06-08 17:11:20.000000 man_etl-1.0.1/man_etl/etl_pipelines/arctic_transform.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1227 2023-06-09 12:25:06.000000 man_etl-1.0.1/man_etl/etl_pipelines/arctic_transform_rf.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:50.426270 man_etl-1.0.1/man_etl/etl_pipelines/core/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      593 2023-06-08 17:31:07.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/base.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2877 2023-06-09 09:46:43.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/extractors.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      648 2023-06-08 17:10:22.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/pipeline.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1827 2023-06-09 12:37:20.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/rf_extractor.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1516 2023-06-09 12:22:59.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/rf_storer.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1832 2023-06-09 09:46:43.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/storers.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1173 2023-06-09 12:22:56.000000 man_etl-1.0.1/man_etl/etl_pipelines/core/transformers.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1062 2023-06-08 17:15:55.000000 man_etl-1.0.1/man_etl/etl_pipelines/csv_to_arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      706 2023-06-09 12:23:44.000000 man_etl-1.0.1/man_etl/etl_pipelines/ons_arctic_to_arrowflight_rf.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      747 2023-06-09 09:59:37.000000 man_etl-1.0.1/man_etl/etl_pipelines/ons_to_arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      727 2023-06-09 12:24:00.000000 man_etl-1.0.1/man_etl/etl_pipelines/ons_to_arctic_rf.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 11:35:52.000000 man_etl-1.0.1/man_etl/etl_pipelines/ons_to_arrowflight.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:50.623310 man_etl-1.0.1/man_etl/etl_pipelines/util/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:44:11.000000 man_etl-1.0.1/man_etl/etl_pipelines/util/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       25 2023-06-08 13:36:53.000000 man_etl-1.0.1/man_etl/etl_pipelines/util/definitions.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1369 2023-06-08 13:36:53.000000 man_etl-1.0.1/man_etl/etl_pipelines/util/transforms.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       97 2023-06-09 08:21:51.000000 man_etl-1.0.1/man_etl/etl_pipelines/util/utils.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1156 2023-06-09 12:25:29.000000 man_etl-1.0.1/man_etl/etl_pipelines/yf_arctic_to_arrowflight_rf.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      848 2023-06-09 06:21:44.000000 man_etl-1.0.1/man_etl/etl_pipelines/yf_to_arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      647 2023-06-09 12:26:25.000000 man_etl-1.0.1/man_etl/etl_pipelines/yf_to_arctic_rf.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-1.0.1/man_etl/generate_db.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:50.810334 man_etl-1.0.1/man_etl/python/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-1.0.1/man_etl/python/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      103 2023-06-08 17:30:09.000000 man_etl-1.0.1/man_etl/python/app.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      749 2023-06-08 17:30:09.000000 man_etl-1.0.1/man_etl/python/pyarrow_client.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 09:46:43.000000 man_etl-1.0.1/man_etl/python/signal_constructor.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:37:49.473701 man_etl-1.0.1/man_etl.egg-info/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-09 12:37:45.000000 man_etl-1.0.1/man_etl.egg-info/PKG-INFO
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1399 2023-06-09 12:37:47.000000 man_etl-1.0.1/man_etl.egg-info/SOURCES.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-09 12:37:45.000000 man_etl-1.0.1/man_etl.egg-info/dependency_links.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      828 2023-06-09 12:37:45.000000 man_etl-1.0.1/man_etl.egg-info/entry_points.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       30 2023-06-09 12:37:45.000000 man_etl-1.0.1/man_etl.egg-info/requires.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-09 12:37:45.000000 man_etl-1.0.1/man_etl.egg-info/top_level.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-09 12:37:50.861559 man_etl-1.0.1/setup.cfg
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1186 2023-06-09 12:37:36.000000 man_etl-1.0.1/setup.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:55.650448 man_etl-1.0.2/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-09 14:02:55.634392 man_etl-1.0.2/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2199 2023-06-09 08:21:22.000000 man_etl-1.0.2/README.md
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:52.630628 man_etl-1.0.2/man_etl/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-1.0.2/man_etl/__init__.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:54.028710 man_etl-1.0.2/man_etl/etl_pipelines/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:46:59.000000 man_etl-1.0.2/man_etl/etl_pipelines/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      783 2023-06-09 09:46:43.000000 man_etl-1.0.2/man_etl/etl_pipelines/arctic_to_arrowflight.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1163 2023-06-08 17:11:20.000000 man_etl-1.0.2/man_etl/etl_pipelines/arctic_transform.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1227 2023-06-09 12:25:06.000000 man_etl-1.0.2/man_etl/etl_pipelines/arctic_transform_rf.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:54.880870 man_etl-1.0.2/man_etl/etl_pipelines/core/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      593 2023-06-08 17:31:07.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/base.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2877 2023-06-09 09:46:43.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/extractors.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      648 2023-06-08 17:10:22.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/pipeline.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1827 2023-06-09 12:37:20.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/rf_extractor.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1516 2023-06-09 12:22:59.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/rf_storer.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1832 2023-06-09 09:46:43.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/storers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1173 2023-06-09 12:22:56.000000 man_etl-1.0.2/man_etl/etl_pipelines/core/transformers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1062 2023-06-08 17:15:55.000000 man_etl-1.0.2/man_etl/etl_pipelines/csv_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      730 2023-06-09 14:02:02.000000 man_etl-1.0.2/man_etl/etl_pipelines/ons_arctic_to_arrowflight_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      747 2023-06-09 09:59:37.000000 man_etl-1.0.2/man_etl/etl_pipelines/ons_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      727 2023-06-09 12:24:00.000000 man_etl-1.0.2/man_etl/etl_pipelines/ons_to_arctic_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 11:35:52.000000 man_etl-1.0.2/man_etl/etl_pipelines/ons_to_arrowflight.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:55.260355 man_etl-1.0.2/man_etl/etl_pipelines/util/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:44:11.000000 man_etl-1.0.2/man_etl/etl_pipelines/util/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       25 2023-06-08 13:36:53.000000 man_etl-1.0.2/man_etl/etl_pipelines/util/definitions.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1369 2023-06-08 13:36:53.000000 man_etl-1.0.2/man_etl/etl_pipelines/util/transforms.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       97 2023-06-09 08:21:51.000000 man_etl-1.0.2/man_etl/etl_pipelines/util/utils.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1156 2023-06-09 12:25:29.000000 man_etl-1.0.2/man_etl/etl_pipelines/yf_arctic_to_arrowflight_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      848 2023-06-09 06:21:44.000000 man_etl-1.0.2/man_etl/etl_pipelines/yf_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      647 2023-06-09 12:26:25.000000 man_etl-1.0.2/man_etl/etl_pipelines/yf_to_arctic_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-1.0.2/man_etl/generate_db.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:55.569111 man_etl-1.0.2/man_etl/python/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-1.0.2/man_etl/python/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      103 2023-06-08 17:30:09.000000 man_etl-1.0.2/man_etl/python/app.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      749 2023-06-08 17:30:09.000000 man_etl-1.0.2/man_etl/python/pyarrow_client.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 09:46:43.000000 man_etl-1.0.2/man_etl/python/signal_constructor.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 14:02:52.959517 man_etl-1.0.2/man_etl.egg-info/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-09 14:02:46.000000 man_etl-1.0.2/man_etl.egg-info/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1399 2023-06-09 14:02:49.000000 man_etl-1.0.2/man_etl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-09 14:02:46.000000 man_etl-1.0.2/man_etl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      828 2023-06-09 14:02:46.000000 man_etl-1.0.2/man_etl.egg-info/entry_points.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       30 2023-06-09 14:02:47.000000 man_etl-1.0.2/man_etl.egg-info/requires.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-09 14:02:47.000000 man_etl-1.0.2/man_etl.egg-info/top_level.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-09 14:02:55.651557 man_etl-1.0.2/setup.cfg
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1186 2023-06-09 14:02:36.000000 man_etl-1.0.2/setup.py
```

### Comparing `man_etl-1.0.1/README.md` & `man_etl-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/arctic_to_arrowflight.py` & `man_etl-1.0.2/man_etl/etl_pipelines/arctic_to_arrowflight.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/arctic_transform.py` & `man_etl-1.0.2/man_etl/etl_pipelines/arctic_transform.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/arctic_transform_rf.py` & `man_etl-1.0.2/man_etl/etl_pipelines/arctic_transform_rf.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/arctic.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/base.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/base.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/extractors.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/extractors.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/pipeline.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/rf_extractor.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/rf_extractor.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/rf_storer.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/rf_storer.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/storers.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/storers.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/core/transformers.py` & `man_etl-1.0.2/man_etl/etl_pipelines/core/transformers.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/csv_to_arctic.py` & `man_etl-1.0.2/man_etl/etl_pipelines/csv_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/ons_arctic_to_arrowflight_rf.py` & `man_etl-1.0.2/man_etl/etl_pipelines/ons_to_arctic_rf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from man_etl.etl_pipelines.core.rf_extractor import ArrowFlightExtractor
 from man_etl.etl_pipelines.core.rf_storer import ArrowFlightStorer
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('Logger')
 
-FILEPATH = "ons_arctic/cpi.parquet"
+VENDOR_FILEPATH = "vendor_ons/cpi.parquet"
 
 @click.command()
-@click.option("--library", prompt="Enter library name", default="ons")
+@click.option("--library", prompt="Enter library name", default="ons_arctic")
 def ons_to_arctic_rf(library):
-    extractor_data = ArrowFlightExtractor.parquet(filepath=FILEPATH).extract()
+    extractor_data = ArrowFlightExtractor.parquet(filepath=VENDOR_FILEPATH).extract()
     payload = {"cpi": extractor_data}
     logger.info("Storing data in S3")
     storer = ArrowFlightStorer.parquet(to_store=payload, library_name=library)
     storer.store()
 
 if __name__ == "__main__":
     ons_to_arctic_rf()
```

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/ons_to_arctic.py` & `man_etl-1.0.2/man_etl/etl_pipelines/ons_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/ons_to_arctic_rf.py` & `man_etl-1.0.2/man_etl/etl_pipelines/ons_arctic_to_arrowflight_rf.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from man_etl.etl_pipelines.core.rf_extractor import ArrowFlightExtractor
 from man_etl.etl_pipelines.core.rf_storer import ArrowFlightStorer
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('Logger')
 
-VENDOR_FILEPATH = "vendor_ons/cpi.parquet"
+FILEPATH = "ons_arctic/cpi.parquet"
 
 @click.command()
-@click.option("--library", prompt="Enter library name", default="ons_arctic")
-def ons_to_arctic_rf(library):
-    extractor_data = ArrowFlightExtractor.parquet(filepath=VENDOR_FILEPATH).extract()
+@click.option("--library", prompt="Enter library name", default="ons")
+def ons_arctic_to_arrowflight_rf(library):
+    extractor_data = ArrowFlightExtractor.parquet(filepath=FILEPATH).extract()
     payload = {"cpi": extractor_data}
     logger.info("Storing data in S3")
     storer = ArrowFlightStorer.parquet(to_store=payload, library_name=library)
     storer.store()
 
 if __name__ == "__main__":
-    ons_to_arctic_rf()
+    ons_arctic_to_arrowflight_rf()
```

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/util/transforms.py` & `man_etl-1.0.2/man_etl/etl_pipelines/util/transforms.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/yf_arctic_to_arrowflight_rf.py` & `man_etl-1.0.2/man_etl/etl_pipelines/yf_arctic_to_arrowflight_rf.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/yf_to_arctic.py` & `man_etl-1.0.2/man_etl/etl_pipelines/yf_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/etl_pipelines/yf_to_arctic_rf.py` & `man_etl-1.0.2/man_etl/etl_pipelines/yf_to_arctic_rf.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl/python/pyarrow_client.py` & `man_etl-1.0.2/man_etl/python/pyarrow_client.py`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl.egg-info/SOURCES.txt` & `man_etl-1.0.2/man_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/man_etl.egg-info/entry_points.txt` & `man_etl-1.0.2/man_etl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `man_etl-1.0.1/setup.py` & `man_etl-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="man_etl",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     include_package_dapta=True,
     install_requires=[
         "Click",
         "pandas",
         "yfinance",
         "pyarrow"
```

