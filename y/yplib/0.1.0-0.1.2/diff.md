# Comparing `tmp/yplib-0.1.0.tar.gz` & `tmp/yplib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.0.tar", last modified: Fri Jun  9 00:23:14 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.2.tar", last modified: Fri Jun  9 02:18:56 2023, max compression
```

## Comparing `yplib-0.1.0.tar` & `yplib-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 00:23:14.359233 yplib-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 00:23:14.359233 yplib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 00:23:14.360378 yplib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 00:22:47.000000 yplib-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 00:23:14.356319 yplib-0.1.0/yplib/
--rw-rw-rw-   0        0        0     4343 2023-06-09 00:21:38.000000 yplib-0.1.0/yplib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 00:23:14.358346 yplib-0.1.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 00:23:14.000000 yplib-0.1.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-06-09 00:23:14.000000 yplib-0.1.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 00:23:14.000000 yplib-0.1.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 00:23:14.000000 yplib-0.1.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 02:18:56.775154 yplib-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:18:56.774637 yplib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:18:56.775154 yplib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 02:18:27.000000 yplib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:18:56.772016 yplib-0.1.2/yplib/
+-rw-rw-rw-   0        0        0     8130 2023-06-09 02:18:08.000000 yplib-0.1.2/yplib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:18:56.774137 yplib-0.1.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.0/LICENSE` & `yplib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.0/PKG-INFO` & `yplib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.0
+Version: 0.1.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.0/setup.py` & `yplib-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.0",
+  version="0.1.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.0/yplib.egg-info/PKG-INFO` & `yplib-0.1.2/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.0
+Version: 0.1.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

