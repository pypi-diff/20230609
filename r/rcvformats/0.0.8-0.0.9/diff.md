# Comparing `tmp/rcvformats-0.0.8.tar.gz` & `tmp/rcvformats-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcvformats-0.0.8.tar", last modified: Tue Jan 19 02:32:09 2021, max compression
+gzip compressed data, was "rcvformats-0.0.9.tar", last modified: Tue Jan 19 02:48:25 2021, max compression
```

## Comparing `rcvformats-0.0.8.tar` & `rcvformats-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.253192 rcvformats-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2021-01-19 02:32:09.249192 rcvformats-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-01-19 02:31:51.000000 rcvformats-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.249192 rcvformats-0.0.8/rcvformats/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.249192 rcvformats-0.0.8/rcvformats/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/common/electionbuddyparser.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.249192 rcvformats-0.0.8/rcvformats/conversions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/conversions/automatic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8742 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/conversions/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/conversions/electionbuddy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/conversions/opavote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.249192 rcvformats-0.0.8/rcvformats/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/schemas/electionbuddy.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/schemas/opavote.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/schemas/universaltabulator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.249192 rcvformats-0.0.8/rcvformats/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/test/testconversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-01-19 02:31:51.000000 rcvformats-0.0.8/rcvformats/test/testschema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:32:09.249192 rcvformats-0.0.8/rcvformats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2021-01-19 02:32:09.000000 rcvformats-0.0.8/rcvformats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-01-19 02:32:09.000000 rcvformats-0.0.8/rcvformats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-01-19 02:32:09.000000 rcvformats-0.0.8/rcvformats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-01-19 02:32:09.000000 rcvformats-0.0.8/rcvformats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-01-19 02:32:09.253192 rcvformats-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      818 2021-01-19 02:31:51.000000 rcvformats-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.196628 rcvformats-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2021-01-19 02:48:25.196628 rcvformats-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-01-19 02:48:01.000000 rcvformats-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.192628 rcvformats-0.0.9/rcvformats/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.196628 rcvformats-0.0.9/rcvformats/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/common/electionbuddyparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.196628 rcvformats-0.0.9/rcvformats/conversions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/conversions/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8742 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/conversions/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/conversions/electionbuddy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/conversions/opavote.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.196628 rcvformats-0.0.9/rcvformats/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/schemas/electionbuddy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/schemas/opavote.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/schemas/universaltabulator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.196628 rcvformats-0.0.9/rcvformats/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/test/testconversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-01-19 02:48:01.000000 rcvformats-0.0.9/rcvformats/test/testschema.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 02:48:25.192628 rcvformats-0.0.9/rcvformats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2021-01-19 02:48:25.000000 rcvformats-0.0.9/rcvformats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2021-01-19 02:48:25.000000 rcvformats-0.0.9/rcvformats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-01-19 02:48:25.000000 rcvformats-0.0.9/rcvformats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-01-19 02:48:25.000000 rcvformats-0.0.9/rcvformats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-01-19 02:48:25.196628 rcvformats-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2021-01-19 02:48:01.000000 rcvformats-0.0.9/setup.py
```

### Comparing `rcvformats-0.0.8/PKG-INFO` & `rcvformats-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcvformats
-Version: 0.0.8
+Version: 0.0.9
 Summary: Schema validations, migrations, and conversions to standardize the Ranked Choice Voting ecosystem
 Home-page: https://github.com/artoonie/rcvformats
 Author: Armin Samii
 Author-email: armin.samii@gmail.com
 License: UNKNOWN
 Description: ![Python package](https://github.com/artoonie/rcvformats/workflows/Python%20package/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/rcvformats/badge/?version=latest)](https://rcvformats.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `rcvformats-0.0.8/README.md` & `rcvformats-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/common/electionbuddyparser.py` & `rcvformats-0.0.9/rcvformats/common/electionbuddyparser.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/conversions/automatic.py` & `rcvformats-0.0.9/rcvformats/conversions/automatic.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/conversions/base.py` & `rcvformats-0.0.9/rcvformats/conversions/base.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/conversions/electionbuddy.py` & `rcvformats-0.0.9/rcvformats/conversions/electionbuddy.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/conversions/opavote.py` & `rcvformats-0.0.9/rcvformats/conversions/opavote.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/schemas/base.py` & `rcvformats-0.0.9/rcvformats/schemas/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Loads supported schemas (currently only one: the Universal Tabulator schema)
 """
 
 import abc
 import json
+import os
+
 import jsonschema
 
 from rcvformats.common import utils
 
 
 class Schema(abc.ABC):
     """
@@ -64,19 +66,24 @@
     @property
     @abc.abstractmethod
     def schema_filename(self):
         """ The JSON Schema filename """
 
     def __init__(self):
         filename = self.schema_filename
-        with open(filename, 'r') as file_object:
+        filepath = os.path.join(self._get_jsonschema_directory(), filename)
+        with open(filepath, 'r') as file_object:
             self.schema = json.load(file_object)
 
         super().__init__()
 
+    @classmethod
+    def _get_jsonschema_directory(cls):
+        return os.path.join(os.path.dirname(__file__), '..', 'jsonschemas')
+
     def _validate_file_object(self, file_object):
         """ Opens the file and runs :func:`~validate_data` """
         try:
             data = json.load(file_object)
         except json.decoder.JSONDecodeError as error:
             self._last_error = error
             return False
```

### Comparing `rcvformats-0.0.8/rcvformats/schemas/electionbuddy.py` & `rcvformats-0.0.9/rcvformats/schemas/electionbuddy.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/test/testconversions.py` & `rcvformats-0.0.9/rcvformats/test/testconversions.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats/test/testschema.py` & `rcvformats-0.0.9/rcvformats/test/testschema.py`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/rcvformats.egg-info/PKG-INFO` & `rcvformats-0.0.9/rcvformats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcvformats
-Version: 0.0.8
+Version: 0.0.9
 Summary: Schema validations, migrations, and conversions to standardize the Ranked Choice Voting ecosystem
 Home-page: https://github.com/artoonie/rcvformats
 Author: Armin Samii
 Author-email: armin.samii@gmail.com
 License: UNKNOWN
 Description: ![Python package](https://github.com/artoonie/rcvformats/workflows/Python%20package/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/rcvformats/badge/?version=latest)](https://rcvformats.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `rcvformats-0.0.8/rcvformats.egg-info/SOURCES.txt` & `rcvformats-0.0.9/rcvformats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcvformats-0.0.8/setup.py` & `rcvformats-0.0.9/setup.py`

 * *Files identical despite different names*

