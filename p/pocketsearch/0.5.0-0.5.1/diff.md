# Comparing `tmp/pocketsearch-0.5.0.tar.gz` & `tmp/pocketsearch-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.5.0.tar", last modified: Fri Jun  9 16:23:23 2023, max compression
+gzip compressed data, was "pocketsearch-0.5.1.tar", last modified: Fri Jun  9 16:31:10 2023, max compression
```

## Comparing `pocketsearch-0.5.0.tar` & `pocketsearch-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:23.444374 pocketsearch-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 16:23:14.000000 pocketsearch-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-09 16:23:23.444374 pocketsearch-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-09 16:23:14.000000 pocketsearch-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:23:23.444374 pocketsearch-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-09 16:23:14.000000 pocketsearch-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:23.444374 pocketsearch-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:23.444374 pocketsearch-0.5.0/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 16:23:14.000000 pocketsearch-0.5.0/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 16:23:14.000000 pocketsearch-0.5.0/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:23.444374 pocketsearch-0.5.0/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-09 16:23:23.000000 pocketsearch-0.5.0/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 16:23:23.000000 pocketsearch-0.5.0/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:23:23.000000 pocketsearch-0.5.0/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 16:23:23.000000 pocketsearch-0.5.0/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.249450 pocketsearch-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-09 16:31:10.245450 pocketsearch-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:31:10.249450 pocketsearch-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.241450 pocketsearch-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.245450 pocketsearch-0.5.1/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.245450 pocketsearch-0.5.1/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.5.0/LICENSE` & `pocketsearch-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.0/PKG-INFO` & `pocketsearch-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.0
+Version: 0.5.1
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
-Home-page: https://github.com/kaykay-dv/pypermint
+Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pocketsearch-0.5.0/README.md` & `pocketsearch-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.0/setup.py` & `pocketsearch-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.5.0",
+    version = "0.5.1",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/kaykay-dv/pypermint",
+    url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
         "Bug Tracker": "https://github.com/kaykay-dv/pocketsearch/issues",
     },
     classifiers = [
         "Development Status :: 4 - Beta",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
```

### Comparing `pocketsearch-0.5.0/src/pocketsearch/__init__.py` & `pocketsearch-0.5.1/src/pocketsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.0/src/pocketsearch/tests.py` & `pocketsearch-0.5.1/src/pocketsearch/tests.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.0/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.5.1/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.0
+Version: 0.5.1
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
-Home-page: https://github.com/kaykay-dv/pypermint
+Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

