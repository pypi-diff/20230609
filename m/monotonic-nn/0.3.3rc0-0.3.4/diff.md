# Comparing `tmp/monotonic-nn-0.3.3rc0.tar.gz` & `tmp/monotonic-nn-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.3.3rc0.tar", last modified: Fri Jun  9 12:43:56 2023, max compression
+gzip compressed data, was "monotonic-nn-0.3.4.tar", last modified: Fri Jun  9 13:12:22 2023, max compression
```

## Comparing `monotonic-nn-0.3.3rc0.tar` & `monotonic-nn-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/
--rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.3rc0/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.3rc0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)    10875 2023-06-09 05:52:52.000000 monotonic-nn-0.3.3rc0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)      406 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31838 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    10242 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14180 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      639 2023-06-09 12:43:15.000000 monotonic-nn-0.3.3rc0/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-09 12:43:56.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-09 12:43:56.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-09 12:43:56.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-09 12:43:56.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-09 12:43:56.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-09 12:43:56.000000 monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      919 2023-06-09 12:37:52.000000 monotonic-nn-0.3.3rc0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-09 12:43:56.554793 monotonic-nn-0.3.3rc0/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-09 12:37:02.000000 monotonic-nn-0.3.3rc0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.4/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.4/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12016 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10875 2023-06-09 05:52:52.000000 monotonic-nn-0.3.4/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      403 2023-06-09 13:12:11.000000 monotonic-nn-0.3.4/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:11.000000 monotonic-nn-0.3.4/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-09 13:12:10.000000 monotonic-nn-0.3.4/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31838 2023-06-09 13:12:11.000000 monotonic-nn-0.3.4/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10242 2023-06-09 13:12:11.000000 monotonic-nn-0.3.4/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:11.000000 monotonic-nn-0.3.4/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14180 2023-06-09 13:12:10.000000 monotonic-nn-0.3.4/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      369 2023-06-09 13:12:11.000000 monotonic-nn-0.3.4/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12016 2023-06-09 13:12:22.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-09 13:12:22.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-09 13:12:22.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-09 13:12:22.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-09 13:12:22.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-09 13:12:22.000000 monotonic-nn-0.3.4/monotonic_nn.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      916 2023-06-09 13:12:07.000000 monotonic-nn-0.3.4/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-09 13:12:22.867623 monotonic-nn-0.3.4/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-09 12:37:02.000000 monotonic-nn-0.3.4/setup.py
```

### Comparing `monotonic-nn-0.3.3rc0/LICENSE` & `monotonic-nn-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.3rc0/PKG-INFO` & `monotonic-nn-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.3rc0
+Version: 0.3.4
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.3rc0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.4 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.3rc0/README.md` & `monotonic-nn-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.3rc0/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.3.4/airt/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.3rc0/airt/_modidx.py` & `monotonic-nn-0.3.4/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.3rc0/airt/keras/experiments.py` & `monotonic-nn-0.3.4/airt/keras/experiments.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.3rc0/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.3.4/monotonic_nn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.3rc0
+Version: 0.3.4
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.3rc0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.4 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.3rc0/settings.ini` & `monotonic-nn-0.3.4/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.3.3rc0
+version = 0.3.4
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.3.3rc0/setup.py` & `monotonic-nn-0.3.4/setup.py`

 * *Files identical despite different names*

