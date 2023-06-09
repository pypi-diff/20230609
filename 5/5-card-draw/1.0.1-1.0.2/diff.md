# Comparing `tmp/5_card_draw-1.0.1.tar.gz` & `tmp/5_card_draw-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5_card_draw-1.0.1.tar", last modified: Thu Jun  8 23:56:53 2023, max compression
+gzip compressed data, was "5_card_draw-1.0.2.tar", last modified: Fri Jun  9 00:08:31 2023, max compression
```

## Comparing `5_card_draw-1.0.1.tar` & `5_card_draw-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 23:56:53.842376 5_card_draw-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-08 23:56:53.831426 5_card_draw-1.0.1/5_card_draw/
--rw-rw-rw-   0        0        0      458 2023-06-04 18:40:07.000000 5_card_draw-1.0.1/5_card_draw/video_poker.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:56:53.841378 5_card_draw-1.0.1/5_card_draw.egg-info/
--rw-rw-rw-   0        0        0      671 2023-06-08 23:56:53.000000 5_card_draw-1.0.1/5_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-08 23:56:53.000000 5_card_draw-1.0.1/5_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:56:53.000000 5_card_draw-1.0.1/5_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 23:56:53.000000 5_card_draw-1.0.1/5_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:56:53.000000 5_card_draw-1.0.1/5_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 5_card_draw-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      671 2023-06-08 23:56:53.842376 5_card_draw-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6553 2023-06-08 23:40:24.000000 5_card_draw-1.0.1/README.md
--rw-rw-rw-   0        0        0      302 2023-06-08 23:56:53.844372 5_card_draw-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-06-08 23:56:40.000000 5_card_draw-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:08:31.700708 5_card_draw-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:08:31.684752 5_card_draw-1.0.2/5_card_draw/
+-rw-rw-rw-   0        0        0      458 2023-06-04 18:40:07.000000 5_card_draw-1.0.2/5_card_draw/video_poker.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:08:31.699724 5_card_draw-1.0.2/5_card_draw.egg-info/
+-rw-rw-rw-   0        0        0      671 2023-06-09 00:08:31.000000 5_card_draw-1.0.2/5_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-09 00:08:31.000000 5_card_draw-1.0.2/5_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:08:31.000000 5_card_draw-1.0.2/5_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 00:08:31.000000 5_card_draw-1.0.2/5_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:08:31.000000 5_card_draw-1.0.2/5_card_draw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 5_card_draw-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      671 2023-06-09 00:08:31.700708 5_card_draw-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6553 2023-06-08 23:40:24.000000 5_card_draw-1.0.2/README.md
+-rw-rw-rw-   0        0        0      308 2023-06-09 00:08:31.701706 5_card_draw-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1681 2023-06-09 00:08:10.000000 5_card_draw-1.0.2/setup.py
```

### Comparing `5_card_draw-1.0.1/5_card_draw.egg-info/PKG-INFO` & `5_card_draw-1.0.2/5_card_draw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 5-card-draw
-Version: 1.0.1
+Version: 1.0.2
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/VideoPoker-5CardRedraw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `5_card_draw-1.0.1/LICENSE.txt` & `5_card_draw-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `5_card_draw-1.0.1/PKG-INFO` & `5_card_draw-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 5_card_draw
-Version: 1.0.1
+Version: 1.0.2
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/VideoPoker-5CardRedraw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `5_card_draw-1.0.1/README.md` & `5_card_draw-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `5_card_draw-1.0.1/setup.py` & `5_card_draw-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 
 '''
 import os
 from pathlib import Path
 import setuptools
 
 requires = [
-    'tkinter',
-    'pathlib',
+    'tk',
+    'pathlib'
 ]
 
 scripts = [
     str(Path('5_card_draw','video_poker.py'))
 ]
 
 #Package setuptools pypi install for local developer installs
 setuptools.setup(
     name = '5_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.1'),
+    version = os.getenv('PACKAGE_VERSION', '1.0.2'),
     description = 'Video Poker application for 5 Card Draw Poker',
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
     packages = setuptools.find_packages(),
     install_requires = requires,
     scripts = scripts,
     classifiers = [
```

