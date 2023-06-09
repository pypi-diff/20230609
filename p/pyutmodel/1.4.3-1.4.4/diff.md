# Comparing `tmp/pyutmodel-1.4.3.tar.gz` & `tmp/pyutmodel-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutmodel-1.4.3.tar", last modified: Thu Apr 13 18:25:21 2023, max compression
+gzip compressed data, was "pyutmodel-1.4.4.tar", last modified: Fri Jun  9 21:14:38 2023, max compression
```

## Comparing `pyutmodel-1.4.3.tar` & `pyutmodel-1.4.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:25:21.845472 pyutmodel-1.4.3/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 pyutmodel-1.4.3/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2270 2023-04-13 18:25:21.845359 pyutmodel-1.4.3/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1939 2023-04-12 01:20:33.000000 pyutmodel-1.4.3/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:25:21.844572 pyutmodel-1.4.3/pyutmodel/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      174 2022-03-03 03:11:12.000000 pyutmodel-1.4.3/pyutmodel/DisplayMethodParameters.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-01-26 17:37:55.000000 pyutmodel-1.4.3/pyutmodel/ModelTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      485 2022-05-18 15:25:38.000000 pyutmodel-1.4.3/pyutmodel/PyutActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4721 2023-01-26 17:31:28.000000 pyutmodel-1.4.3/pyutmodel/PyutClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3270 2023-01-26 17:38:43.000000 pyutmodel-1.4.3/pyutmodel/PyutClassCommon.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2022-03-14 02:19:43.000000 pyutmodel-1.4.3/pyutmodel/PyutDisplayParameters.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2178 2023-02-07 02:28:42.000000 pyutmodel-1.4.3/pyutmodel/PyutField.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1300 2023-01-26 17:31:00.000000 pyutmodel-1.4.3/pyutmodel/PyutInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5259 2023-03-22 16:22:13.000000 pyutmodel-1.4.3/pyutmodel/PyutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1413 2022-03-27 17:27:56.000000 pyutmodel-1.4.3/pyutmodel/PyutLinkType.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3852 2023-01-26 17:32:44.000000 pyutmodel-1.4.3/pyutmodel/PyutLinkedObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8981 2023-02-06 15:37:30.000000 pyutmodel-1.4.3/pyutmodel/PyutMethod.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      828 2023-01-08 04:44:45.000000 pyutmodel-1.4.3/pyutmodel/PyutModifier.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1020 2023-01-26 16:44:25.000000 pyutmodel-1.4.3/pyutmodel/PyutNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2420 2022-03-15 21:36:23.000000 pyutmodel-1.4.3/pyutmodel/PyutObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2438 2023-02-07 16:16:50.000000 pyutmodel-1.4.3/pyutmodel/PyutParameter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2929 2022-05-18 01:48:45.000000 pyutmodel-1.4.3/pyutmodel/PyutSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6123 2023-03-11 02:14:00.000000 pyutmodel-1.4.3/pyutmodel/PyutSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2747 2023-02-05 20:11:42.000000 pyutmodel-1.4.3/pyutmodel/PyutStereotype.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      591 2022-05-18 15:25:38.000000 pyutmodel-1.4.3/pyutmodel/PyutText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      762 2022-03-14 02:23:07.000000 pyutmodel-1.4.3/pyutmodel/PyutType.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      184 2022-04-05 20:39:40.000000 pyutmodel-1.4.3/pyutmodel/PyutUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1512 2022-03-23 16:04:17.000000 pyutmodel-1.4.3/pyutmodel/PyutVisibilityEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-05-01 18:22:04.000000 pyutmodel-1.4.3/pyutmodel/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutmodel-1.4.3/pyutmodel/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:25:21.845164 pyutmodel-1.4.3/pyutmodel.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2270 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      837 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       10 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:25:21.845501 pyutmodel-1.4.3/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2023-04-13 17:50:57.000000 pyutmodel-1.4.3/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:14:38.518777 pyutmodel-1.4.4/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 pyutmodel-1.4.4/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2270 2023-06-09 21:14:38.518662 pyutmodel-1.4.4/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1939 2023-04-12 01:20:33.000000 pyutmodel-1.4.4/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:14:38.517992 pyutmodel-1.4.4/pyutmodel/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      174 2022-03-03 03:11:12.000000 pyutmodel-1.4.4/pyutmodel/DisplayMethodParameters.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-01-26 17:37:55.000000 pyutmodel-1.4.4/pyutmodel/ModelTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      485 2023-05-05 20:00:34.000000 pyutmodel-1.4.4/pyutmodel/PyutActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4721 2023-01-26 17:31:28.000000 pyutmodel-1.4.4/pyutmodel/PyutClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3270 2023-01-26 17:38:43.000000 pyutmodel-1.4.4/pyutmodel/PyutClassCommon.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2022-03-14 02:19:43.000000 pyutmodel-1.4.4/pyutmodel/PyutDisplayParameters.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2178 2023-02-07 02:28:42.000000 pyutmodel-1.4.4/pyutmodel/PyutField.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1300 2023-01-26 17:31:00.000000 pyutmodel-1.4.4/pyutmodel/PyutInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5259 2023-03-22 16:22:13.000000 pyutmodel-1.4.4/pyutmodel/PyutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1413 2022-03-27 17:27:56.000000 pyutmodel-1.4.4/pyutmodel/PyutLinkType.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3852 2023-01-26 17:32:44.000000 pyutmodel-1.4.4/pyutmodel/PyutLinkedObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8981 2023-02-06 15:37:30.000000 pyutmodel-1.4.4/pyutmodel/PyutMethod.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      828 2023-01-08 04:44:45.000000 pyutmodel-1.4.4/pyutmodel/PyutModifier.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1020 2023-01-26 16:44:25.000000 pyutmodel-1.4.4/pyutmodel/PyutNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2420 2023-05-05 20:00:34.000000 pyutmodel-1.4.4/pyutmodel/PyutObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2438 2023-02-07 16:16:50.000000 pyutmodel-1.4.4/pyutmodel/PyutParameter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2929 2022-05-18 01:48:45.000000 pyutmodel-1.4.4/pyutmodel/PyutSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6123 2023-03-11 02:14:00.000000 pyutmodel-1.4.4/pyutmodel/PyutSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2747 2023-02-05 20:11:42.000000 pyutmodel-1.4.4/pyutmodel/PyutStereotype.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      591 2022-05-18 15:25:38.000000 pyutmodel-1.4.4/pyutmodel/PyutText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      762 2022-03-14 02:23:07.000000 pyutmodel-1.4.4/pyutmodel/PyutType.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      184 2022-04-05 20:39:40.000000 pyutmodel-1.4.4/pyutmodel/PyutUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1512 2022-03-23 16:04:17.000000 pyutmodel-1.4.4/pyutmodel/PyutVisibilityEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-05-01 18:22:04.000000 pyutmodel-1.4.4/pyutmodel/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutmodel-1.4.4/pyutmodel/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:14:38.518520 pyutmodel-1.4.4/pyutmodel.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2270 2023-06-09 21:14:38.000000 pyutmodel-1.4.4/pyutmodel.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      837 2023-06-09 21:14:38.000000 pyutmodel-1.4.4/pyutmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 21:14:38.000000 pyutmodel-1.4.4/pyutmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 21:14:38.000000 pyutmodel-1.4.4/pyutmodel.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       10 2023-06-09 21:14:38.000000 pyutmodel-1.4.4/pyutmodel.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 21:14:38.518813 pyutmodel-1.4.4/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2023-06-09 21:11:20.000000 pyutmodel-1.4.4/setup.py
```

### Comparing `pyutmodel-1.4.3/LICENSE` & `pyutmodel-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/PKG-INFO` & `pyutmodel-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutmodel
-Version: 1.4.3
+Version: 1.4.4
 Summary: External Pyut Data Model
 Home-page: https://github.com/hasii2011/pyutmodel
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutmodel Version: 1.4.3 Summary: External Pyut
+Metadata-Version: 2.1 Name: pyutmodel Version: 1.4.4 Summary: External Pyut
 Data Model Home-page: https://github.com/hasii2011/pyutmodel Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/pyutmodel/tree/
```

### Comparing `pyutmodel-1.4.3/README.md` & `pyutmodel-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutClass.py` & `pyutmodel-1.4.4/pyutmodel/PyutClass.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutClassCommon.py` & `pyutmodel-1.4.4/pyutmodel/PyutClassCommon.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutDisplayParameters.py` & `pyutmodel-1.4.4/pyutmodel/PyutDisplayParameters.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutField.py` & `pyutmodel-1.4.4/pyutmodel/PyutField.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutInterface.py` & `pyutmodel-1.4.4/pyutmodel/PyutInterface.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutLink.py` & `pyutmodel-1.4.4/pyutmodel/PyutLink.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutLinkType.py` & `pyutmodel-1.4.4/pyutmodel/PyutLinkType.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutLinkedObject.py` & `pyutmodel-1.4.4/pyutmodel/PyutLinkedObject.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutMethod.py` & `pyutmodel-1.4.4/pyutmodel/PyutMethod.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutModifier.py` & `pyutmodel-1.4.4/pyutmodel/PyutModifier.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutNote.py` & `pyutmodel-1.4.4/pyutmodel/PyutNote.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutObject.py` & `pyutmodel-1.4.4/pyutmodel/PyutObject.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutParameter.py` & `pyutmodel-1.4.4/pyutmodel/PyutParameter.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutSDInstance.py` & `pyutmodel-1.4.4/pyutmodel/PyutSDInstance.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutSDMessage.py` & `pyutmodel-1.4.4/pyutmodel/PyutSDMessage.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutStereotype.py` & `pyutmodel-1.4.4/pyutmodel/PyutStereotype.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutText.py` & `pyutmodel-1.4.4/pyutmodel/PyutText.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutType.py` & `pyutmodel-1.4.4/pyutmodel/PyutType.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel/PyutVisibilityEnum.py` & `pyutmodel-1.4.4/pyutmodel/PyutVisibilityEnum.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/pyutmodel.egg-info/PKG-INFO` & `pyutmodel-1.4.4/pyutmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutmodel
-Version: 1.4.3
+Version: 1.4.4
 Summary: External Pyut Data Model
 Home-page: https://github.com/hasii2011/pyutmodel
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutmodel Version: 1.4.3 Summary: External Pyut
+Metadata-Version: 2.1 Name: pyutmodel Version: 1.4.4 Summary: External Pyut
 Data Model Home-page: https://github.com/hasii2011/pyutmodel Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/pyutmodel/tree/
```

### Comparing `pyutmodel-1.4.3/pyutmodel.egg-info/SOURCES.txt` & `pyutmodel-1.4.4/pyutmodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.3/setup.py` & `pyutmodel-1.4.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="pyutmodel",
-    version="1.4.3",
+    version="1.4.4",
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Data Model',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hasii2011/pyutmodel",
     packages=[
         'pyutmodel',
     ],
     package_data={
         'pyutmodel': ['py.typed'],
     },
-    install_requires=['hasiihelper~=0.2.0', 'Deprecated==1.2.13'],
+    install_requires=['hasiihelper~=0.2.1', 'Deprecated==1.2.14'],
 )
```

