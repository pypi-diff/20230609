# Comparing `tmp/PyTextProMax-1.5.tar.gz` & `tmp/PyTextProMax-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTextProMax-1.5.tar", last modified: Fri Jun  9 12:51:22 2023, max compression
+gzip compressed data, was "PyTextProMax-2.0.tar", last modified: Fri Jun  9 13:08:25 2023, max compression
```

## Comparing `PyTextProMax-1.5.tar` & `PyTextProMax-2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:51:22.161562 PyTextProMax-1.5/
--rw-rw-rw-   0        0        0     1079 2023-06-09 11:34:23.000000 PyTextProMax-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      649 2023-06-09 12:51:22.161562 PyTextProMax-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 12:51:22.160561 PyTextProMax-1.5/PyTextProMax.egg-info/
--rw-rw-rw-   0        0        0      649 2023-06-09 12:51:21.000000 PyTextProMax-1.5/PyTextProMax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-09 12:51:22.000000 PyTextProMax-1.5/PyTextProMax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:51:21.000000 PyTextProMax-1.5/PyTextProMax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-09 12:51:21.000000 PyTextProMax-1.5/PyTextProMax.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:51:21.000000 PyTextProMax-1.5/PyTextProMax.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5046 2023-06-09 12:51:00.000000 PyTextProMax-1.5/README.md
--rw-rw-rw-   0        0        0     3531 2023-06-09 12:50:59.000000 PyTextProMax-1.5/__init__.py
--rw-rw-rw-   0        0        0       86 2023-06-09 12:51:22.162561 PyTextProMax-1.5/setup.cfg
--rw-rw-rw-   0        0        0      821 2023-06-09 12:51:01.000000 PyTextProMax-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:08:25.267845 PyTextProMax-2.0/
+-rw-rw-rw-   0        0        0     1079 2023-06-09 11:34:23.000000 PyTextProMax-2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      649 2023-06-09 13:08:25.267845 PyTextProMax-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 13:08:25.265845 PyTextProMax-2.0/PyTextProMax.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-06-09 13:08:25.000000 PyTextProMax-2.0/PyTextProMax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-06-09 13:08:25.000000 PyTextProMax-2.0/PyTextProMax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:08:25.000000 PyTextProMax-2.0/PyTextProMax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-09 13:08:25.000000 PyTextProMax-2.0/PyTextProMax.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 13:08:25.000000 PyTextProMax-2.0/PyTextProMax.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5046 2023-06-09 12:51:00.000000 PyTextProMax-2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-09 13:08:25.269846 PyTextProMax-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      824 2023-06-09 13:07:59.000000 PyTextProMax-2.0/setup.py
```

### Comparing `PyTextProMax-1.5/LICENSE.txt` & `PyTextProMax-2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTextProMax-1.5/PKG-INFO` & `PyTextProMax-2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTextProMax
-Version: 1.5
+Version: 2.0
 Summary: A python library that can help categorize sentences.
 Home-page: https://github.com/CittiTheBozo/PyTextProMax
 Download-URL: https://github.com/CittiTheBozo/PyTextProMax/releases/tag/v1.0.0/
 Author: Cittidabozo
 Author-email: diabetolover@gmail.com
 License: MIT
 Keywords: text,handling,useful,emotion
```

### Comparing `PyTextProMax-1.5/PyTextProMax.egg-info/PKG-INFO` & `PyTextProMax-2.0/PyTextProMax.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTextProMax
-Version: 1.5
+Version: 2.0
 Summary: A python library that can help categorize sentences.
 Home-page: https://github.com/CittiTheBozo/PyTextProMax
 Download-URL: https://github.com/CittiTheBozo/PyTextProMax/releases/tag/v1.0.0/
 Author: Cittidabozo
 Author-email: diabetolover@gmail.com
 License: MIT
 Keywords: text,handling,useful,emotion
```

### Comparing `PyTextProMax-1.5/README.md` & `PyTextProMax-2.0/README.md`

 * *Files identical despite different names*

### Comparing `PyTextProMax-1.5/setup.py` & `PyTextProMax-2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 setup(
   name = 'PyTextProMax',
-  version = '1.5',
+  py_modules=['PyTextProMax'],
+  version = '2.0',
   license='MIT',
-  scripts= ['__init__.py'],
   description = 'A python library that can help categorize sentences.',
   author = 'Cittidabozo',
   author_email = 'diabetolover@gmail.com',
   url = 'https://github.com/CittiTheBozo/PyTextProMax',
   download_url = 'https://github.com/CittiTheBozo/PyTextProMax/releases/tag/v1.0.0/',
   keywords = ['text', 'handling', 'useful', 'emotion'],
   install_requires=[
```

