# Comparing `tmp/cardo-python-utils-0.2.0.tar.gz` & `tmp/cardo-python-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardo-python-utils-0.2.0.tar", last modified: Fri Jun  9 16:11:51 2023, max compression
+gzip compressed data, was "cardo-python-utils-0.2.1.tar", last modified: Fri Jun  9 17:06:47 2023, max compression
```

## Comparing `cardo-python-utils-0.2.0.tar` & `cardo-python-utils-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 16:11:51.857722 cardo-python-utils-0.2.0/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-09 16:11:51.857722 cardo-python-utils-0.2.0/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.0/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 16:11:51.853722 cardo-python-utils-0.2.0/cardo_python_utils.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-09 16:11:51.000000 cardo-python-utils-0.2.0/cardo_python_utils.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-06-09 16:11:51.000000 cardo-python-utils-0.2.0/cardo_python_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-09 16:11:51.000000 cardo-python-utils-0.2.0/cardo_python_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-06-09 16:11:51.000000 cardo-python-utils-0.2.0/cardo_python_utils.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-06-09 16:11:51.000000 cardo-python-utils-0.2.0/cardo_python_utils.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 16:11:51.857722 cardo-python-utils-0.2.0/python_utils/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.0/python_utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/data_structures.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/db.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/django_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    14224 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.0/python_utils/esma_choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/imports.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/math.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/pandas_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/rest.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/text.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/time.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/python_utils/types_hinting.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-06-09 16:11:51.857722 cardo-python-utils-0.2.0/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.0/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.1/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 17:06:47.086227 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/python_utils/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.1/python_utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/data_structures.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/db.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/django_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    14223 2023-06-09 17:06:36.000000 cardo-python-utils-0.2.1/python_utils/esma_choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/imports.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/math.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/pandas_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/rest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/text.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/time.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/types_hinting.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/setup.py
```

### Comparing `cardo-python-utils-0.2.0/LICENSE` & `cardo-python-utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/PKG-INFO` & `cardo-python-utils-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.0/README.rst` & `cardo-python-utils-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/cardo_python_utils.egg-info/PKG-INFO` & `cardo-python-utils-0.2.1/cardo_python_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.0/cardo_python_utils.egg-info/SOURCES.txt` & `cardo-python-utils-0.2.1/cardo_python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/choices.py` & `cardo-python-utils-0.2.1/python_utils/choices.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/data_structures.py` & `cardo-python-utils-0.2.1/python_utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/django_utils.py` & `cardo-python-utils-0.2.1/python_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/esma_choices.py` & `cardo-python-utils-0.2.1/python_utils/esma_choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     EQUP = 17, "Equipment"
     PROP = 18, "Property"
     OTHR = 100, "Other"
 
 
 class InterestRateTypeChoices(ChoiceEnum):
     FLIF = 1, "Floating rate underlying exposure (for life)"
-    FINX = 2, "Floating rate underlying exposure linked to one index that will revert to another index in the future",
+    FINX = 2, "Floating rate underlying exposure linked to one index that will revert to another index in the future"
     FXRL = 3, "Fixed rate underlying exposure (for life)"
     FXPR = 4, "Fixed with future periodic resets"
     FLCF = 5, "Fixed rate underlying exposure with compulsory future switch to floating"
     FLFL = 6, "Floating rate underlying exposure with floor"
     CAPP = 7, "Floating rate underlying exposure with cap)"
     FLCA = 8, "Floating rate underlying exposure with both floor and cap"
     DISC = 9, "Discount"
```

### Comparing `cardo-python-utils-0.2.0/python_utils/exceptions.py` & `cardo-python-utils-0.2.1/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/imports.py` & `cardo-python-utils-0.2.1/python_utils/imports.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/math.py` & `cardo-python-utils-0.2.1/python_utils/math.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/pandas_utils.py` & `cardo-python-utils-0.2.1/python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/rest.py` & `cardo-python-utils-0.2.1/python_utils/rest.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/text.py` & `cardo-python-utils-0.2.1/python_utils/text.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/python_utils/time.py` & `cardo-python-utils-0.2.1/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.0/setup.cfg` & `cardo-python-utils-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardo-python-utils
-version = 0.2.0
+version = 0.2.1
 description = Python library enhanced with a wide range of functions for different scenarios.
 long_description = file: README.rst
 url = https://github.com/CardoAI/cardo-python-utils
 author = Kristi Kotini
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

