# Comparing `tmp/RoxiLib-0.3.0.dev0.tar.gz` & `tmp/RoxiLib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoxiLib-0.3.0.dev0.tar", last modified: Thu Jun  8 12:39:18 2023, max compression
+gzip compressed data, was "RoxiLib-0.5.0.tar", last modified: Fri Jun  9 09:42:27 2023, max compression
```

## Comparing `RoxiLib-0.3.0.dev0.tar` & `RoxiLib-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:39:18.820083 RoxiLib-0.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-08 12:39:18.820083 RoxiLib-0.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:39:18.820083 RoxiLib-0.3.0.dev0/RoxiLib/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/RoxiLib/RoxiCommunication.py
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/RoxiLib/RoxiStateHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/RoxiLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151393 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/RoxiLib/bt_data.h
--rw-r--r--   0 runner    (1001) docker     (123)  2241536 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/RoxiLib/libRoxi.dll
--rw-r--r--   0 runner    (1001) docker     (123)    37562 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/RoxiLib/roxi_api_wdk.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:39:18.820083 RoxiLib-0.3.0.dev0/RoxiLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-08 12:39:18.000000 RoxiLib-0.3.0.dev0/RoxiLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 12:39:18.000000 RoxiLib-0.3.0.dev0/RoxiLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:39:18.000000 RoxiLib-0.3.0.dev0/RoxiLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 12:39:18.000000 RoxiLib-0.3.0.dev0/RoxiLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:39:18.820083 RoxiLib-0.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-08 12:39:08.000000 RoxiLib-0.3.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:42:27.731018 RoxiLib-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-09 09:42:27.731018 RoxiLib-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 09:42:27.000000 RoxiLib-0.5.0/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:42:27.731018 RoxiLib-0.5.0/RoxiLib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/RoxiLib/RoxiCommunication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/RoxiLib/RoxiStateHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/RoxiLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151393 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/RoxiLib/bt_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2241536 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/RoxiLib/libRoxi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    37562 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/RoxiLib/roxi_api_wdk.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:42:27.731018 RoxiLib-0.5.0/RoxiLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-09 09:42:27.000000 RoxiLib-0.5.0/RoxiLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-09 09:42:27.000000 RoxiLib-0.5.0/RoxiLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:42:27.000000 RoxiLib-0.5.0/RoxiLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 09:42:27.000000 RoxiLib-0.5.0/RoxiLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:42:27.731018 RoxiLib-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-09 09:42:19.000000 RoxiLib-0.5.0/version.py
```

### Comparing `RoxiLib-0.3.0.dev0/PKG-INFO` & `RoxiLib-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoxiLib
-Version: 0.3.0.dev0
+Version: 0.5.0
 Summary: Python API for Roxi lib
 Home-page: https://github.com/wavingroup/allinclusive_API
 Author: Wavin T&I
 Author-email: support@wavin.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RoxiLib-0.3.0.dev0/RoxiLib/RoxiCommunication.py` & `RoxiLib-0.5.0/RoxiLib/RoxiCommunication.py`

 * *Files identical despite different names*

### Comparing `RoxiLib-0.3.0.dev0/RoxiLib/RoxiStateHandler.py` & `RoxiLib-0.5.0/RoxiLib/RoxiStateHandler.py`

 * *Files identical despite different names*

### Comparing `RoxiLib-0.3.0.dev0/RoxiLib/bt_data.h` & `RoxiLib-0.5.0/RoxiLib/bt_data.h`

 * *Files identical despite different names*

### Comparing `RoxiLib-0.3.0.dev0/RoxiLib/libRoxi.dll` & `RoxiLib-0.5.0/RoxiLib/libRoxi.dll`

 * *Files identical despite different names*

### Comparing `RoxiLib-0.3.0.dev0/RoxiLib/roxi_api_wdk.h` & `RoxiLib-0.5.0/RoxiLib/roxi_api_wdk.h`

 * *Files identical despite different names*

### Comparing `RoxiLib-0.3.0.dev0/RoxiLib.egg-info/PKG-INFO` & `RoxiLib-0.5.0/RoxiLib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoxiLib
-Version: 0.3.0.dev0
+Version: 0.5.0
 Summary: Python API for Roxi lib
 Home-page: https://github.com/wavingroup/allinclusive_API
 Author: Wavin T&I
 Author-email: support@wavin.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RoxiLib-0.3.0.dev0/setup.py` & `RoxiLib-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import io
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup, Distribution
+from version import get_git_version
 
 def read(filename):
     filename = os.path.join(os.path.dirname(__file__), filename)
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 class BinaryDistribution(Distribution):
     """Distribution which always forces a binary package with platform name"""
     def has_ext_modules(foo):
         return True
 
+try:
+    import multiprocessing
+except ImportError:
+    pass
+
 setup(
     name="RoxiLib",
     url="https://github.com/wavingroup/allinclusive_API",
     license='MIT',
 
     author="Wavin T&I",
     author_email="support@wavin.com",
@@ -28,15 +34,15 @@
     description="Python API for Roxi lib",
     
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
 
     packages=['RoxiLib'],
     package_data={'': ['*.dll', '*.h']}, #package DLL and Header files
-    version="0.3.0-dev",
+    version=get_git_version(),
 
     #install_requires=['pymodbus>=3.1.0'],
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
```

