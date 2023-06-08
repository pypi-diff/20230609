# Comparing `tmp/5_card_draw-0.0.dev0.tar.gz` & `tmp/5_card_draw-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5_card_draw-0.0.dev0.tar", last modified: Thu Jun  8 23:24:47 2023, max compression
+gzip compressed data, was "5_card_draw-1.0.0.tar", last modified: Thu Jun  8 23:38:50 2023, max compression
```

## Comparing `5_card_draw-0.0.dev0.tar` & `5_card_draw-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 23:24:47.855268 5_card_draw-0.0.dev0/
-drwxrwxrwx   0        0        0        0 2023-06-08 23:24:47.840308 5_card_draw-0.0.dev0/5_card_draw/
--rw-rw-rw-   0        0        0      458 2023-06-04 18:40:07.000000 5_card_draw-0.0.dev0/5_card_draw/video_poker.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:24:47.854278 5_card_draw-0.0.dev0/5_card_draw.egg-info/
--rw-rw-rw-   0        0        0      674 2023-06-08 23:24:47.000000 5_card_draw-0.0.dev0/5_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-08 23:24:47.000000 5_card_draw-0.0.dev0/5_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:24:47.000000 5_card_draw-0.0.dev0/5_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 23:24:47.000000 5_card_draw-0.0.dev0/5_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:24:47.000000 5_card_draw-0.0.dev0/5_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 5_card_draw-0.0.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0      674 2023-06-08 23:24:47.855268 5_card_draw-0.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     6553 2023-06-08 23:22:16.000000 5_card_draw-0.0.dev0/README.md
--rw-rw-rw-   0        0        0      312 2023-06-08 23:24:47.857262 5_card_draw-0.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1721 2023-06-08 23:19:50.000000 5_card_draw-0.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:38:50.131375 5_card_draw-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-08 23:38:50.120427 5_card_draw-1.0.0/5_card_draw/
+-rw-rw-rw-   0        0        0      458 2023-06-04 18:40:07.000000 5_card_draw-1.0.0/5_card_draw/video_poker.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:38:50.130377 5_card_draw-1.0.0/5_card_draw.egg-info/
+-rw-rw-rw-   0        0        0      671 2023-06-08 23:38:50.000000 5_card_draw-1.0.0/5_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-08 23:38:50.000000 5_card_draw-1.0.0/5_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 23:38:50.000000 5_card_draw-1.0.0/5_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 23:38:50.000000 5_card_draw-1.0.0/5_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 23:38:50.000000 5_card_draw-1.0.0/5_card_draw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 5_card_draw-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      671 2023-06-08 23:38:50.131375 5_card_draw-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6553 2023-06-08 23:22:16.000000 5_card_draw-1.0.0/README.md
+-rw-rw-rw-   0        0        0      312 2023-06-08 23:38:50.133369 5_card_draw-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1687 2023-06-08 23:38:11.000000 5_card_draw-1.0.0/setup.py
```

### Comparing `5_card_draw-0.0.dev0/5_card_draw.egg-info/PKG-INFO` & `5_card_draw-1.0.0/5_card_draw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 5-card-draw
-Version: 0.0.dev0
+Version: 1.0.0
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/VideoPoker-5CardRedraw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `5_card_draw-0.0.dev0/LICENSE.txt` & `5_card_draw-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `5_card_draw-0.0.dev0/README.md` & `5_card_draw-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `5_card_draw-0.0.dev0/setup.py` & `5_card_draw-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 OR
 Developer Install: "py -m pip install -e ." from this folder.
 
 Publish a Pip Version to PyPi:
 0. Create an account https://pypi.org/account/register/
 1. Install Prequisites: py -m pip install --upgrade pip setuptools wheel twine build
 2. py setup.py sdist bdist_wheel
-3. python -m twine upload — repository testpypi dist/*
+3. py twine upload dist/*
 
 '''
 import os
 from pathlib import Path
 import setuptools
 
 requires = [
@@ -26,15 +26,15 @@
 scripts = [
     str(Path('5_card_draw','video_poker.py'))
 ]
 
 #Package setuptools pypi install for local developer installs
 setuptools.setup(
     name = '5_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '0.0.dev0'),
+    version = os.getenv('PACKAGE_VERSION', '1.0.0'),
     description = 'Video Poker application for 5 Card Draw Poker',
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
     packages = setuptools.find_packages(),
     install_requires = requires,
     scripts = scripts,
     classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

