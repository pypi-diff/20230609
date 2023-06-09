# Comparing `tmp/hasiihelper-0.2.0.tar.gz` & `tmp/hasiihelper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasiihelper-0.2.0.tar", last modified: Tue Apr 11 20:37:40 2023, max compression
+gzip compressed data, was "hasiihelper-0.2.1.tar", last modified: Fri Jun  9 15:46:13 2023, max compression
```

## Comparing `hasiihelper-0.2.0.tar` & `hasiihelper-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:37:40.266367 hasiihelper-0.2.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-03-26 16:04:54.000000 hasiihelper-0.2.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2030 2023-04-11 20:37:40.266243 hasiihelper-0.2.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1663 2023-04-11 01:32:43.000000 hasiihelper-0.2.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:37:40.265457 hasiihelper-0.2.0/hasiihelper/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2022-04-25 21:01:57.000000 hasiihelper-0.2.0/hasiihelper/Dimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      694 2021-03-31 01:16:10.000000 hasiihelper-0.2.0/hasiihelper/Position.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1123 2023-04-04 01:18:09.000000 hasiihelper-0.2.0/hasiihelper/ResourceManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5601 2023-03-08 18:43:42.000000 hasiihelper-0.2.0/hasiihelper/SemanticVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1832 2022-11-20 03:20:07.000000 hasiihelper-0.2.0/hasiihelper/Singleton.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2369 2023-04-10 20:04:39.000000 hasiihelper-0.2.0/hasiihelper/UnitTestBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiihelper-0.2.0/hasiihelper/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiihelper-0.2.0/hasiihelper/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:37:40.266083 hasiihelper-0.2.0/hasiihelper.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2030 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      410 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       19 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-11 20:37:40.000000 hasiihelper-0.2.0/hasiihelper.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-11 20:37:40.266401 hasiihelper-0.2.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      806 2023-04-10 18:38:31.000000 hasiihelper-0.2.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 15:46:13.243570 hasiihelper-0.2.1/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-03-26 16:04:54.000000 hasiihelper-0.2.1/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2030 2023-06-09 15:46:13.243452 hasiihelper-0.2.1/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1663 2023-04-11 01:32:43.000000 hasiihelper-0.2.1/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 15:46:13.242733 hasiihelper-0.2.1/hasiihelper/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2022-04-25 21:01:57.000000 hasiihelper-0.2.1/hasiihelper/Dimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      694 2021-03-31 01:16:10.000000 hasiihelper-0.2.1/hasiihelper/Position.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1123 2023-04-04 01:18:09.000000 hasiihelper-0.2.1/hasiihelper/ResourceManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5601 2023-03-08 18:43:42.000000 hasiihelper-0.2.1/hasiihelper/SemanticVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1832 2022-11-20 03:20:07.000000 hasiihelper-0.2.1/hasiihelper/Singleton.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2369 2023-04-10 20:04:39.000000 hasiihelper-0.2.1/hasiihelper/UnitTestBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiihelper-0.2.1/hasiihelper/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiihelper-0.2.1/hasiihelper/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 15:46:13.243286 hasiihelper-0.2.1/hasiihelper.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2030 2023-06-09 15:46:13.000000 hasiihelper-0.2.1/hasiihelper.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      410 2023-06-09 15:46:13.000000 hasiihelper-0.2.1/hasiihelper.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 15:46:13.000000 hasiihelper-0.2.1/hasiihelper.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       19 2023-06-09 15:46:13.000000 hasiihelper-0.2.1/hasiihelper.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-09 15:46:13.000000 hasiihelper-0.2.1/hasiihelper.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 15:46:13.243604 hasiihelper-0.2.1/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      806 2023-06-09 15:43:14.000000 hasiihelper-0.2.1/setup.py
```

### Comparing `hasiihelper-0.2.0/LICENSE` & `hasiihelper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/PKG-INFO` & `hasiihelper-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasiihelper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Humberto`s Helper Classes
 Home-page: https://github.com/hasii2011/hasiihelper
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hasiihelper Version: 0.2.0 Summary: Humberto`s
+Metadata-Version: 2.1 Name: hasiihelper Version: 0.2.1 Summary: Humberto`s
 Helper Classes Home-page: https://github.com/hasii2011/hasiihelper Author:
 Humberto A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II Maintainer-email:
 humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./developer/agpl-license-web-badge-version-2-256x48.png]
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/hasiihelper/
 tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/
```

### Comparing `hasiihelper-0.2.0/README.md` & `hasiihelper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper/Dimensions.py` & `hasiihelper-0.2.1/hasiihelper/Dimensions.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper/Position.py` & `hasiihelper-0.2.1/hasiihelper/Position.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper/ResourceManager.py` & `hasiihelper-0.2.1/hasiihelper/ResourceManager.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper/SemanticVersion.py` & `hasiihelper-0.2.1/hasiihelper/SemanticVersion.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper/Singleton.py` & `hasiihelper-0.2.1/hasiihelper/Singleton.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper/UnitTestBase.py` & `hasiihelper-0.2.1/hasiihelper/UnitTestBase.py`

 * *Files identical despite different names*

### Comparing `hasiihelper-0.2.0/hasiihelper.egg-info/PKG-INFO` & `hasiihelper-0.2.1/hasiihelper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasiihelper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Humberto`s Helper Classes
 Home-page: https://github.com/hasii2011/hasiihelper
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hasiihelper Version: 0.2.0 Summary: Humberto`s
+Metadata-Version: 2.1 Name: hasiihelper Version: 0.2.1 Summary: Humberto`s
 Helper Classes Home-page: https://github.com/hasii2011/hasiihelper Author:
 Humberto A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II Maintainer-email:
 humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./developer/agpl-license-web-badge-version-2-256x48.png]
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/hasiihelper/
 tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/
```

### Comparing `hasiihelper-0.2.0/setup.py` & `hasiihelper-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="hasiihelper",
-    version="0.2.0",
+    version="0.2.1",
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Humberto`s Helper Classes',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -22,9 +22,9 @@
     package_data={
         'hasiihelper':  ['py.typed'],
     },
 
     packages=[
         'hasiihelper',
     ],
-    install_requires=['Deprecated~=1.2.13'],
+    install_requires=['Deprecated~=1.2.14'],
 )
```

