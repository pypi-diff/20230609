# Comparing `tmp/segment-lidar-0.1.2.tar.gz` & `tmp/segment-lidar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\segment-lidar-0.1.2.tar", last modified: Fri Jun  9 20:57:35 2023, max compression
+gzip compressed data, was "dist\segment-lidar-0.1.3.tar", last modified: Fri Jun  9 21:04:11 2023, max compression
```

## Comparing `segment-lidar-0.1.2.tar` & `segment-lidar-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:57:35.809617 segment-lidar-0.1.2/
--rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6986 2023-06-09 20:57:35.808618 segment-lidar-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6442 2023-06-09 20:03:51.000000 segment-lidar-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 20:57:35.772617 segment-lidar-0.1.2/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.2/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0    10979 2023-06-09 20:54:31.000000 segment-lidar-0.1.2/segment_lidar/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:57:35.807622 segment-lidar-0.1.2/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     6986 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 20:57:35.810618 segment-lidar-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-06-09 20:51:09.000000 segment-lidar-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:04:11.274541 segment-lidar-0.1.3/
+-rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6986 2023-06-09 21:04:11.273541 segment-lidar-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6442 2023-06-09 20:03:51.000000 segment-lidar-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 21:04:11.232538 segment-lidar-0.1.3/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.3/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0    11014 2023-06-09 21:03:38.000000 segment-lidar-0.1.3/segment_lidar/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:04:11.272541 segment-lidar-0.1.3/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     6986 2023-06-09 21:04:10.000000 segment-lidar-0.1.3/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-09 21:04:11.000000 segment-lidar-0.1.3/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 21:04:10.000000 segment-lidar-0.1.3/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-09 21:04:10.000000 segment-lidar-0.1.3/segment_lidar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2023-06-09 21:04:10.000000 segment-lidar-0.1.3/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 21:04:10.000000 segment-lidar-0.1.3/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 21:04:11.274541 segment-lidar-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-06-09 21:03:57.000000 segment-lidar-0.1.3/setup.py
```

### Comparing `segment-lidar-0.1.2/LICENSE` & `segment-lidar-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.2/PKG-INFO` & `segment-lidar-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `segment-lidar-0.1.2/README.md` & `segment-lidar-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.2/segment_lidar/main.py` & `segment-lidar-0.1.3/segment_lidar/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Copyright (c) 2023 - University of Liège
 # Author : Anass Yarroudh (ayarroudh@uliege.be), Geomatics Unit of ULiege
 # This file is distributed under the BSD-3 licence. See LICENSE file for complete text of the license.
 
 import os
 
-os.system('pip install git+https://github.com/jianboqi/CSF.git')
+try:
+    import CSF
+except ImportError:
+    os.system('pip install git+https://github.com/jianboqi/CSF.git')
 
 import yaml
 import click
 import time
 import torch
 import cv2
 import numpy as np
 import supervision as sv
 from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
 from samgeo import SamGeo
 from samgeo.text_sam import LangSAM
 import rasterio
-import CSF
 import laspy
 
 
 def cloud_to_image(points, minx, maxx, miny, maxy, resolution):
     width = int((maxx - minx) / resolution) + 1
     height = int((maxy - miny) / resolution) + 1
```

### Comparing `segment-lidar-0.1.2/segment_lidar.egg-info/PKG-INFO` & `segment-lidar-0.1.3/segment_lidar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `segment-lidar-0.1.2/setup.py` & `segment-lidar-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="segment-lidar",
-    version='0.1.2',
+    version='0.1.3',
     description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause "New" or "Revised" License',
     author='Anass Yarroudh',
     author_email='ayarroudh@uliege.be',
     url='https://github.com/Yarroudh/segment-lidar',
```

