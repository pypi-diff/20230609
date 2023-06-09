# Comparing `tmp/btweb-0.1.1.tar.gz` & `tmp/btweb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btweb-0.1.1.tar", last modified: Fri Jun  9 20:26:04 2023, max compression
+gzip compressed data, was "btweb-0.1.2.tar", last modified: Fri Jun  9 20:27:26 2023, max compression
```

## Comparing `btweb-0.1.1.tar` & `btweb-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:26:04.756611 btweb-0.1.1/
--rw-r--r--   0 etejeda    (501) staff       (20)     1347 2023-05-11 11:43:48.000000 btweb-0.1.1/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-05-11 11:43:48.000000 btweb-0.1.1/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-05-11 11:43:48.000000 btweb-0.1.1/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      224 2023-05-11 11:43:48.000000 btweb-0.1.1/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     2910 2023-06-09 20:26:04.756818 btweb-0.1.1/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1955 2023-05-11 11:58:32.000000 btweb-0.1.1/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:26:04.754365 btweb-0.1.1/btweb/
--rw-r--r--   0 etejeda    (501) staff       (20)     3598 2023-05-12 20:19:16.000000 btweb-0.1.1/btweb/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      759 2023-06-09 20:25:07.000000 btweb-0.1.1/btweb/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:26:04.756280 btweb-0.1.1/btweb.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2910 2023-06-09 20:26:04.000000 btweb-0.1.1/btweb.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      302 2023-06-09 20:26:04.000000 btweb-0.1.1/btweb.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-09 20:26:04.000000 btweb-0.1.1/btweb.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:38:15.000000 btweb-0.1.1/btweb.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       58 2023-06-09 20:26:04.000000 btweb-0.1.1/btweb.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        6 2023-06-09 20:26:04.000000 btweb-0.1.1/btweb.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:43:48.000000 btweb-0.1.1/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1183 2023-06-09 20:26:04.757529 btweb-0.1.1/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-05-11 11:43:48.000000 btweb-0.1.1/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-05-11 11:43:48.000000 btweb-0.1.1/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:27:26.908688 btweb-0.1.2/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1347 2023-05-11 11:43:48.000000 btweb-0.1.2/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-05-11 11:43:48.000000 btweb-0.1.2/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-05-11 11:43:48.000000 btweb-0.1.2/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      224 2023-05-11 11:43:48.000000 btweb-0.1.2/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     2910 2023-06-09 20:27:26.908910 btweb-0.1.2/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1955 2023-05-11 11:58:32.000000 btweb-0.1.2/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:27:26.906673 btweb-0.1.2/btweb/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3598 2023-05-12 20:19:16.000000 btweb-0.1.2/btweb/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      769 2023-06-09 20:26:43.000000 btweb-0.1.2/btweb/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:27:26.908402 btweb-0.1.2/btweb.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2910 2023-06-09 20:27:26.000000 btweb-0.1.2/btweb.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      302 2023-06-09 20:27:26.000000 btweb-0.1.2/btweb.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-09 20:27:26.000000 btweb-0.1.2/btweb.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:38:15.000000 btweb-0.1.2/btweb.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       58 2023-06-09 20:27:26.000000 btweb-0.1.2/btweb.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        6 2023-06-09 20:27:26.000000 btweb-0.1.2/btweb.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:43:48.000000 btweb-0.1.2/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1183 2023-06-09 20:27:26.909715 btweb-0.1.2/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-05-11 11:43:48.000000 btweb-0.1.2/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-05-11 11:43:48.000000 btweb-0.1.2/tox.ini
```

### Comparing `btweb-0.1.1/.gitignore` & `btweb-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `btweb-0.1.1/LICENSE` & `btweb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `btweb-0.1.1/PKG-INFO` & `btweb-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btweb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility library for fronting requests functionality
 Home-page: https://github.com/berttejeda/bert.webadapter.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: requests,https,get,python,remote,file,download
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btweb-0.1.1/README.md` & `btweb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `btweb-0.1.1/btweb/__init__.py` & `btweb-0.1.2/btweb/__init__.py`

 * *Files identical despite different names*

### Comparing `btweb-0.1.1/btweb/logger.py` & `btweb-0.1.2/btweb/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import logging.handlers
+import os
 import sys
 
 class Logger:
 
   def __init__(self, **kwargs):
     self.debug = kwargs.get('debug', False)
```

### Comparing `btweb-0.1.1/btweb.egg-info/PKG-INFO` & `btweb-0.1.2/btweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btweb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility library for fronting requests functionality
 Home-page: https://github.com/berttejeda/bert.webadapter.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: requests,https,get,python,remote,file,download
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btweb-0.1.1/setup.cfg` & `btweb-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btweb
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Utility library for fronting requests functionality
-version = 0.1.1
+version = 0.1.2
 url = https://github.com/berttejeda/bert.webadapter.git
 keywords = 
 	requests
 	https
 	get
 	python
 	remote
```

