# Comparing `tmp/five_card_draw-1.0.0.tar.gz` & `tmp/five_card_draw-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.0.tar", last modified: Fri Jun  9 00:30:57 2023, max compression
+gzip compressed data, was "five_card_draw-1.0.1.tar", last modified: Fri Jun  9 00:32:44 2023, max compression
```

## Comparing `five_card_draw-1.0.0.tar` & `five_card_draw-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 00:30:57.404479 five_card_draw-1.0.0/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      663 2023-06-09 00:30:57.404479 five_card_draw-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 00:30:57.389518 five_card_draw-1.0.0/five_card_draw/
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.0/five_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15612 2023-06-09 00:26:57.000000 five_card_draw-1.0.0/five_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.0/five_card_draw/five_card_draw.py
-drwxrwxrwx   0        0        0        0 2023-06-09 00:30:57.403481 five_card_draw-1.0.0/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0      663 2023-06-09 00:30:57.000000 five_card_draw-1.0.0/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-06-09 00:30:57.000000 five_card_draw-1.0.0/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 00:30:57.000000 five_card_draw-1.0.0/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 00:30:57.000000 five_card_draw-1.0.0/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 00:30:57.000000 five_card_draw-1.0.0/five_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      308 2023-06-09 00:30:57.406473 five_card_draw-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1784 2023-06-09 00:30:04.000000 five_card_draw-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:32:44.656040 five_card_draw-1.0.1/
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      663 2023-06-09 00:32:44.657037 five_card_draw-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 00:32:44.645068 five_card_draw-1.0.1/five_card_draw/
+-rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.1/five_card_draw/fcd_bank.txt
+-rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.1/five_card_draw/fcd_functions.py
+-rw-rw-rw-   0        0        0    15612 2023-06-09 00:26:57.000000 five_card_draw-1.0.1/five_card_draw/fcd_pagegui.py
+-rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.1/five_card_draw/five_card_draw.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:32:44.656040 five_card_draw-1.0.1/five_card_draw.egg-info/
+-rw-rw-rw-   0        0        0      663 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      308 2023-06-09 00:32:44.658034 five_card_draw-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1832 2023-06-09 00:32:33.000000 five_card_draw-1.0.1/setup.py
```

### Comparing `five_card_draw-1.0.0/LICENSE.txt` & `five_card_draw-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.0/PKG-INFO` & `five_card_draw-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five_card_draw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `five_card_draw-1.0.0/README.md` & `five_card_draw-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.0/five_card_draw/fcd_functions.py` & `five_card_draw-1.0.1/five_card_draw/fcd_functions.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.0/five_card_draw/fcd_pagegui.py` & `five_card_draw-1.0.1/five_card_draw/fcd_pagegui.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.0/five_card_draw.egg-info/PKG-INFO` & `five_card_draw-1.0.1/five_card_draw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five-card-draw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `five_card_draw-1.0.0/setup.py` & `five_card_draw-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     'pathlib'
 ]
 
 scripts = [
     str(Path('five_card_draw','five_card_draw.py')),
     str(Path('five_card_draw','fcd_pagegui.py')),
     str(Path('five_card_draw','fcd_functions.py')),
+    str(Path('five_card_draw','fcd_bank.txt'))
 ]
 
 #Package setuptools pypi install for local developer installs
 setuptools.setup(
     name = 'five_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.0'),
+    version = os.getenv('PACKAGE_VERSION', '1.0.1'),
     description = 'Video Poker application for 5 Card Draw Poker',
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
     packages = setuptools.find_packages(),
     install_requires = requires,
     scripts = scripts,
     classifiers = [
```

