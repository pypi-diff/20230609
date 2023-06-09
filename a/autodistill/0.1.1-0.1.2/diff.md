# Comparing `tmp/autodistill-0.1.1.tar.gz` & `tmp/autodistill-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-0.1.1.tar", last modified: Wed May 31 06:32:22 2023, max compression
+gzip compressed data, was "autodistill-0.1.2.tar", last modified: Fri Jun  9 17:07:49 2023, max compression
```

## Comparing `autodistill-0.1.1.tar` & `autodistill-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.647574 autodistill-0.1.1/
--rw-r--r--   0 james      (501) staff       (20)     1055 2023-05-30 17:10:38.000000 autodistill-0.1.1/LICENSE.md
--rw-r--r--   0 james      (501) staff       (20)     5598 2023-05-31 06:32:22.647421 autodistill-0.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5088 2023-05-30 17:10:38.000000 autodistill-0.1.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.644012 autodistill-0.1.1/autodistill/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-05-31 06:25:33.000000 autodistill-0.1.1/autodistill/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.645825 autodistill-0.1.1/autodistill/core/
--rw-r--r--   0 james      (501) staff       (20)      151 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/core/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      516 2023-05-30 17:13:34.000000 autodistill-0.1.1/autodistill/core/base_model.py
--rw-r--r--   0 james      (501) staff       (20)      114 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/core/ontology.py
--rw-r--r--   0 james      (501) staff       (20)      236 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/core/target_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.646871 autodistill-0.1.1/autodistill/detection/
--rw-r--r--   0 james      (501) staff       (20)      290 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/detection/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      580 2023-05-30 19:12:05.000000 autodistill-0.1.1/autodistill/detection/caption_ontology.py
--rw-r--r--   0 james      (501) staff       (20)     1760 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/detection/detection_base_model.py
--rw-r--r--   0 james      (501) staff       (20)      769 2023-05-30 17:23:36.000000 autodistill-0.1.1/autodistill/detection/detection_ontology.py
--rw-r--r--   0 james      (501) staff       (20)      366 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/detection/detection_target_model.py
--rw-r--r--   0 james      (501) staff       (20)     3258 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.644829 autodistill-0.1.1/autodistill.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     5598 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      605 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      142 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-05-31 06:32:22.647624 autodistill-0.1.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1265 2023-05-31 06:32:18.000000 autodistill-0.1.1/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.647074 autodistill-0.1.1/test/
--rw-r--r--   0 james      (501) staff       (20)       41 2023-05-30 17:10:38.000000 autodistill-0.1.1/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.730241 autodistill-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-07 11:34:42.000000 autodistill-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)    14015 2023-06-09 17:07:49.730047 autodistill-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    13503 2023-06-09 17:03:43.000000 autodistill-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.727619 autodistill-0.1.2/autodistill/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-06-09 17:04:08.000000 autodistill-0.1.2/autodistill/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.728978 autodistill-0.1.2/autodistill/core/
+-rw-r--r--   0 james      (501) staff       (20)      151 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      516 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      114 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      236 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/core/target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.729699 autodistill-0.1.2/autodistill/detection/
+-rw-r--r--   0 james      (501) staff       (20)      290 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      580 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/caption_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)     1760 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/detection_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      769 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/detection_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      366 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/detection/detection_target_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3258 2023-06-07 11:34:42.000000 autodistill-0.1.2/autodistill/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.728385 autodistill-0.1.2/autodistill.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)    14015 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      602 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      142 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-06-09 17:07:49.000000 autodistill-0.1.2/autodistill.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-09 17:07:49.730282 autodistill-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1261 2023-06-09 17:07:46.000000 autodistill-0.1.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 17:07:49.729845 autodistill-0.1.2/test/
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-06-07 11:34:42.000000 autodistill-0.1.2/test/test_hello.py
```

### Comparing `autodistill-0.1.1/autodistill/core/base_model.py` & `autodistill-0.1.2/autodistill/core/base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.1/autodistill/detection/caption_ontology.py` & `autodistill-0.1.2/autodistill/detection/caption_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.1/autodistill/detection/detection_base_model.py` & `autodistill-0.1.2/autodistill/detection/detection_base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.1/autodistill/detection/detection_ontology.py` & `autodistill-0.1.2/autodistill/detection/detection_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.1/autodistill/helpers.py` & `autodistill-0.1.2/autodistill/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.1/autodistill.egg-info/SOURCES.txt` & `autodistill-0.1.2/autodistill.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.md
+LICENSE
 README.md
 setup.py
 autodistill/__init__.py
 autodistill/helpers.py
 autodistill.egg-info/PKG-INFO
 autodistill.egg-info/SOURCES.txt
 autodistill.egg-info/dependency_links.txt
```

### Comparing `autodistill-0.1.1/setup.py` & `autodistill-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import setuptools
 from setuptools import find_packages
 import re
-import os
 
 with open("./autodistill/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autodistill",  
     version=version,
     author="Roboflow",
-    author_email="jacob@roboflow.com",
+    author_email="autodistill@roboflow.com",
     description="Distill large foundational models into smaller, domain-specific models for deployment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/autodistill/autodistill",
     install_requires=[
         "opencv-python>=4.6.0",
         "supervision",
```

