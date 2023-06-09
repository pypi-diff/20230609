# Comparing `tmp/element-calcium-imaging-0.7.2.tar.gz` & `tmp/element-calcium-imaging-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.7.2.tar", last modified: Fri Jun  9 05:17:35 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.7.3.tar", last modified: Fri Jun  9 05:30:34 2023, max compression
```

## Comparing `element-calcium-imaging-0.7.2.tar` & `element-calcium-imaging-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:17:35.696316 element-calcium-imaging-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 05:17:35.696316 element-calcium-imaging-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:17:35.692316 element-calcium-imaging-0.7.2/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    66523 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63721 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:17:35.696316 element-calcium-imaging-0.7.2/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:17:35.692316 element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 05:17:35.000000 element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-09 05:17:35.000000 element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:17:35.000000 element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 05:17:35.000000 element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 05:17:35.000000 element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:17:35.696316 element-calcium-imaging-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-09 05:17:28.000000 element-calcium-imaging-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:30:27.000000 element-calcium-imaging-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-09 05:30:27.000000 element-calcium-imaging-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.657798 element-calcium-imaging-0.7.3/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66523 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63721 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/setup.py
```

### Comparing `element-calcium-imaging-0.7.2/LICENSE` & `element-calcium-imaging-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/PKG-INFO` & `element-calcium-imaging-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.2
+Version: 0.7.3
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-calcium-imaging-0.7.2/README.md` & `element-calcium-imaging-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/analysis.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/analysis.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_no_curation.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_preprocess.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.7.3/element_calcium_imaging/scan.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/PKG-INFO` & `element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.2
+Version: 0.7.3
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-calcium-imaging-0.7.2/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.2/setup.py` & `element-calcium-imaging-0.7.3/setup.py`

 * *Files identical despite different names*

