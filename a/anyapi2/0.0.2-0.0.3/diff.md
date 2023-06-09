# Comparing `tmp/anyapi2-0.0.2.tar.gz` & `tmp/anyapi2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyapi2-0.0.2.tar", last modified: Tue Oct  4 05:39:48 2022, max compression
+gzip compressed data, was "anyapi2-0.0.3.tar", last modified: Fri Jun  9 16:48:36 2023, max compression
```

## Comparing `anyapi2-0.0.2.tar` & `anyapi2-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 user      (1000) user      (1000)        0 2022-10-04 05:39:48.685027 anyapi2-0.0.2/
--rw-r--r--   0 user      (1000) user      (1000)     1084 2019-11-22 22:26:36.000000 anyapi2-0.0.2/LICENSE
--rw-rw----   0 user      (1000) user      (1000)     1210 2022-10-04 05:39:48.685027 anyapi2-0.0.2/PKG-INFO
--rw-rw----   0 user      (1000) user      (1000)      582 2022-09-26 21:27:44.000000 anyapi2-0.0.2/README.md
-drwxrwx---   0 user      (1000) user      (1000)        0 2022-10-04 05:39:48.685027 anyapi2-0.0.2/anyapi/
--rw-rw----   0 user      (1000) user      (1000)     2088 2022-09-30 19:52:28.000000 anyapi2-0.0.2/anyapi/__init__.py
--rw-rw----   0 user      (1000) user      (1000)      533 2022-09-27 14:24:22.000000 anyapi2-0.0.2/anyapi/cookies.py
-drwxrwx---   0 user      (1000) user      (1000)        0 2022-10-04 05:39:48.685027 anyapi2-0.0.2/anyapi2.egg-info/
--rw-rw----   0 user      (1000) user      (1000)     1210 2022-10-04 05:39:48.000000 anyapi2-0.0.2/anyapi2.egg-info/PKG-INFO
--rw-rw----   0 user      (1000) user      (1000)      217 2022-10-04 05:39:48.000000 anyapi2-0.0.2/anyapi2.egg-info/SOURCES.txt
--rw-rw----   0 user      (1000) user      (1000)        1 2022-10-04 05:39:48.000000 anyapi2-0.0.2/anyapi2.egg-info/dependency_links.txt
--rw-rw----   0 user      (1000) user      (1000)       33 2022-10-04 05:39:48.000000 anyapi2-0.0.2/anyapi2.egg-info/requires.txt
--rw-rw----   0 user      (1000) user      (1000)        7 2022-10-04 05:39:48.000000 anyapi2-0.0.2/anyapi2.egg-info/top_level.txt
--rw-rw----   0 user      (1000) user      (1000)       38 2022-10-04 05:39:48.685027 anyapi2-0.0.2/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1045 2022-10-04 05:39:01.000000 anyapi2-0.0.2/setup.py
+drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-09 16:48:36.882136 anyapi2-0.0.3/
+-rw-r--r--   0 user      (1000) user      (1000)     1084 2019-11-22 22:26:36.000000 anyapi2-0.0.3/LICENSE
+-rw-rw----   0 user      (1000) user      (1000)     1210 2023-06-09 16:48:36.882136 anyapi2-0.0.3/PKG-INFO
+-rw-rw----   0 user      (1000) user      (1000)      582 2022-09-26 21:27:44.000000 anyapi2-0.0.3/README.md
+drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-09 16:48:36.882136 anyapi2-0.0.3/anyapi/
+-rw-rw----   0 user      (1000) user      (1000)     2123 2023-06-09 16:46:01.000000 anyapi2-0.0.3/anyapi/__init__.py
+-rw-rw----   0 user      (1000) user      (1000)      533 2022-09-27 14:24:22.000000 anyapi2-0.0.3/anyapi/cookies.py
+drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-09 16:48:36.882136 anyapi2-0.0.3/anyapi2.egg-info/
+-rw-rw----   0 user      (1000) user      (1000)     1210 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/PKG-INFO
+-rw-rw----   0 user      (1000) user      (1000)      217 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/SOURCES.txt
+-rw-rw----   0 user      (1000) user      (1000)        1 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/dependency_links.txt
+-rw-rw----   0 user      (1000) user      (1000)       33 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/requires.txt
+-rw-rw----   0 user      (1000) user      (1000)        7 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/top_level.txt
+-rw-rw----   0 user      (1000) user      (1000)       38 2023-06-09 16:48:36.882136 anyapi2-0.0.3/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1045 2023-06-09 16:47:23.000000 anyapi2-0.0.3/setup.py
```

### Comparing `anyapi2-0.0.2/LICENSE` & `anyapi2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anyapi2-0.0.2/PKG-INFO` & `anyapi2-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyapi2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Boilerplate code for api integrations
 Home-page: https://github.com/c0ntribut0r/anyapi
 License: MIT
 Keywords: requests api
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anyapi2-0.0.2/README.md` & `anyapi2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `anyapi2-0.0.2/anyapi/__init__.py` & `anyapi2-0.0.3/anyapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from dataclasses import dataclass, field
 from logging import getLogger
 from pathlib import Path
 from typing import ClassVar
 
 import requests
 from tenacity import TryAgain, retry, retry_if_exception_type, stop_after_attempt, wait_incrementing
```

### Comparing `anyapi2-0.0.2/anyapi/cookies.py` & `anyapi2-0.0.3/anyapi/cookies.py`

 * *Files identical despite different names*

### Comparing `anyapi2-0.0.2/anyapi2.egg-info/PKG-INFO` & `anyapi2-0.0.3/anyapi2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyapi2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Boilerplate code for api integrations
 Home-page: https://github.com/c0ntribut0r/anyapi
 License: MIT
 Keywords: requests api
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anyapi2-0.0.2/setup.py` & `anyapi2-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 # # allow setup.py to be run from any path
 # os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='anyapi2',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     include_package_data=True,
     install_requires=['requests==2.28.1', 'tenacity==8.1.0'],
     license='MIT',
     description='Boilerplate code for api integrations',
     long_description=(Path(__file__).parent / 'README.md').read_text(),
     long_description_content_type="text/markdown",
```

