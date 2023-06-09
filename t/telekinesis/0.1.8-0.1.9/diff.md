# Comparing `tmp/telekinesis-0.1.8.tar.gz` & `tmp/telekinesis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telekinesis-0.1.8.tar", last modified: Fri Jun 11 05:28:58 2021, max compression
+gzip compressed data, was "telekinesis-0.1.9.tar", last modified: Fri Jun 11 08:51:43 2021, max compression
```

## Comparing `telekinesis-0.1.8.tar` & `telekinesis-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 05:28:58.942626 telekinesis-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-11 05:28:51.000000 telekinesis-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-11 05:28:58.942626 telekinesis-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-06-11 05:28:51.000000 telekinesis-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-11 05:28:58.942626 telekinesis-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      813 2021-06-11 05:28:51.000000 telekinesis-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 05:28:58.942626 telekinesis-0.1.8/telekinesis/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-06-11 05:28:51.000000 telekinesis-0.1.8/telekinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27480 2021-06-11 05:28:51.000000 telekinesis-0.1.8/telekinesis/broker.py
--rw-r--r--   0 runner    (1001) docker     (121)    24725 2021-06-11 05:28:51.000000 telekinesis-0.1.8/telekinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-06-11 05:28:51.000000 telekinesis-0.1.8/telekinesis/cryptography.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-06-11 05:28:51.000000 telekinesis-0.1.8/telekinesis/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    40593 2021-06-11 05:28:51.000000 telekinesis-0.1.8/telekinesis/telekinesis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 05:28:58.942626 telekinesis-0.1.8/telekinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-11 05:28:58.000000 telekinesis-0.1.8/telekinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-06-11 05:28:58.000000 telekinesis-0.1.8/telekinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-11 05:28:58.000000 telekinesis-0.1.8/telekinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-11 05:28:58.000000 telekinesis-0.1.8/telekinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-11 05:28:58.000000 telekinesis-0.1.8/telekinesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 05:28:58.942626 telekinesis-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-06-11 05:28:51.000000 telekinesis-0.1.8/test/test_00_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-06-11 05:28:51.000000 telekinesis-0.1.8/test/test_01_subscribe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2021-06-11 05:28:51.000000 telekinesis-0.1.8/test/test_02_garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-06-11 05:28:51.000000 telekinesis-0.1.8/test/test_03_request_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-06-11 05:28:51.000000 telekinesis-0.1.8/test/test_04_state_diffing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.629891 telekinesis-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-11 08:51:33.000000 telekinesis-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-11 08:51:43.629891 telekinesis-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-06-11 08:51:33.000000 telekinesis-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-11 08:51:43.629891 telekinesis-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2021-06-11 08:51:33.000000 telekinesis-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.625891 telekinesis-0.1.9/telekinesis/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27480 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24725 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40593 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/telekinesis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.629891 telekinesis-0.1.9/telekinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.629891 telekinesis-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_00_walkthrough.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_01_subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_02_garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_03_request_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_04_state_diffing.py
```

### Comparing `telekinesis-0.1.8/LICENSE` & `telekinesis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/PKG-INFO` & `telekinesis-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telekinesis
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Source, End-to-End Encrypted, Anywhere-to-Anywhere, Remote Procedure Calls.
 Home-page: https://github.com/telekinesis-cloud/telekinesis
 Author: Telekinesis, Inc.
 Author-email: support@telekinesis.cloud
 License: UNKNOWN
 Description: # Telekinesis - Python Package
```

### Comparing `telekinesis-0.1.8/setup.py` & `telekinesis-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telekinesis",
-    version="0.1.8",
+    version="0.1.9",
     author="Telekinesis, Inc.",
     author_email="support@telekinesis.cloud",
     description="Open Source, End-to-End Encrypted, Anywhere-to-Anywhere, Remote Procedure Calls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/telekinesis-cloud/telekinesis",
     packages=setuptools.find_packages(),
```

### Comparing `telekinesis-0.1.8/telekinesis/__init__.py` & `telekinesis-0.1.9/telekinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/telekinesis/broker.py` & `telekinesis-0.1.9/telekinesis/broker.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/telekinesis/client.py` & `telekinesis-0.1.9/telekinesis/client.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/telekinesis/cryptography.py` & `telekinesis-0.1.9/telekinesis/cryptography.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/telekinesis/helpers.py` & `telekinesis-0.1.9/telekinesis/helpers.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/telekinesis/telekinesis.py` & `telekinesis-0.1.9/telekinesis/telekinesis.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/telekinesis.egg-info/PKG-INFO` & `telekinesis-0.1.9/telekinesis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telekinesis
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Source, End-to-End Encrypted, Anywhere-to-Anywhere, Remote Procedure Calls.
 Home-page: https://github.com/telekinesis-cloud/telekinesis
 Author: Telekinesis, Inc.
 Author-email: support@telekinesis.cloud
 License: UNKNOWN
 Description: # Telekinesis - Python Package
```

### Comparing `telekinesis-0.1.8/test/test_00_walkthrough.py` & `telekinesis-0.1.9/test/test_00_walkthrough.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/test/test_01_subscribe.py` & `telekinesis-0.1.9/test/test_01_subscribe.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/test/test_02_garbage_collection.py` & `telekinesis-0.1.9/test/test_02_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/test/test_03_request_forwarding.py` & `telekinesis-0.1.9/test/test_03_request_forwarding.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.8/test/test_04_state_diffing.py` & `telekinesis-0.1.9/test/test_04_state_diffing.py`

 * *Files identical despite different names*

