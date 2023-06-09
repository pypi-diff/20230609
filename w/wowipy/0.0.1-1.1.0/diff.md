# Comparing `tmp/wowipy-0.0.1.tar.gz` & `tmp/wowipy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-0.0.1.tar", last modified: Fri Jun  9 09:29:45 2023, max compression
+gzip compressed data, was "wowipy-1.1.0.tar", last modified: Fri Jun  9 09:33:10 2023, max compression
```

## Comparing `wowipy-0.0.1.tar` & `wowipy-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:45.908788 wowipy-0.0.1/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-0.0.1/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-06-09 09:29:45.908788 wowipy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 09:29:45.909788 wowipy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-06-09 09:25:26.000000 wowipy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:45.900810 wowipy-0.0.1/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:29:19.000000 wowipy-0.0.1/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-0.0.1/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    34007 2023-06-09 08:48:32.000000 wowipy-0.0.1/wowipy/models.py
--rw-rw-rw-   0        0        0     4515 2023-06-06 12:53:23.000000 wowipy-0.0.1/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    33020 2023-06-09 09:08:56.000000 wowipy-0.0.1/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:45.907791 wowipy-0.0.1/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-06-09 09:29:45.000000 wowipy-0.0.1/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-09 09:29:45.000000 wowipy-0.0.1/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:29:45.000000 wowipy-0.0.1/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-09 09:29:45.000000 wowipy-0.0.1/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 09:29:45.000000 wowipy-0.0.1/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 09:33:10.019625 wowipy-1.1.0/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.0/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-06-09 09:33:10.019625 wowipy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:33:10.019625 wowipy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-06-09 09:33:03.000000 wowipy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:33:10.008653 wowipy-1.1.0/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.0/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.0/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    34007 2023-06-09 08:48:32.000000 wowipy-1.1.0/wowipy/models.py
+-rw-rw-rw-   0        0        0     4515 2023-06-06 12:53:23.000000 wowipy-1.1.0/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    33020 2023-06-09 09:08:56.000000 wowipy-1.1.0/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:33:10.018651 wowipy-1.1.0/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-0.0.1/COPYING` & `wowipy-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-0.0.1/LICENSE` & `wowipy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-0.0.1/PKG-INFO` & `wowipy-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 0.0.1
+Version: 1.1.0
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-0.0.1/setup.py` & `wowipy-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='0.0.1',
+    version='1.1.0',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-0.0.1/wowipy/models.py` & `wowipy-1.1.0/wowipy/models.py`

 * *Files identical despite different names*

### Comparing `wowipy-0.0.1/wowipy/rest_adapter.py` & `wowipy-1.1.0/wowipy/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `wowipy-0.0.1/wowipy/wowipy.py` & `wowipy-1.1.0/wowipy/wowipy.py`

 * *Files identical despite different names*

### Comparing `wowipy-0.0.1/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.0/wowipy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 0.0.1
+Version: 1.1.0
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

