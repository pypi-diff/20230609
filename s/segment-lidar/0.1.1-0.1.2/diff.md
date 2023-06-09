# Comparing `tmp/segment-lidar-0.1.1.tar.gz` & `tmp/segment-lidar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-lidar-0.1.1.tar", last modified: Fri Jun  9 12:41:33 2023, max compression
+gzip compressed data, was "dist\segment-lidar-0.1.2.tar", last modified: Fri Jun  9 20:57:35 2023, max compression
```

## Comparing `segment-lidar-0.1.1.tar` & `segment-lidar-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:41:33.416669 segment-lidar-0.1.1/
--rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6072 2023-06-09 12:41:33.415667 segment-lidar-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5679 2023-06-09 11:48:47.000000 segment-lidar-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 12:41:33.383659 segment-lidar-0.1.1/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.1/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0     9739 2023-06-09 11:49:26.000000 segment-lidar-0.1.1/segment_lidar/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:41:33.414668 segment-lidar-0.1.1/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     6072 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-09 12:41:33.000000 segment-lidar-0.1.1/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 12:41:33.417667 segment-lidar-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-06-09 12:41:18.000000 segment-lidar-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:57:35.809617 segment-lidar-0.1.2/
+-rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6986 2023-06-09 20:57:35.808618 segment-lidar-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6442 2023-06-09 20:03:51.000000 segment-lidar-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 20:57:35.772617 segment-lidar-0.1.2/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.2/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0    10979 2023-06-09 20:54:31.000000 segment-lidar-0.1.2/segment_lidar/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:57:35.807622 segment-lidar-0.1.2/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     6986 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 20:57:35.000000 segment-lidar-0.1.2/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 20:57:35.810618 segment-lidar-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-06-09 20:51:09.000000 segment-lidar-0.1.2/setup.py
```

### Comparing `segment-lidar-0.1.1/LICENSE` & `segment-lidar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.1/PKG-INFO` & `segment-lidar-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: segment-lidar
-Version: 0.1.1
-Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
-Home-page: https://github.com/Yarroudh/segment-lidar
-Author: Anass Yarroudh
-Author-email: ayarroudh@uliege.be
-License: BSD 3-Clause "New" or "Revised" License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
 *Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
@@ -54,82 +43,98 @@
   --help  Show this message and exit.
 
 Commands:
   create-config  Create a configuration YAML file.
   segment        Segment LiDAR data.
 ```
 
-The package reads `.LAS` or `.LAZ` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
+The package reads `.las` or `.laz` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
 
 ```bash
 segment-lidar create-config -o config.yaml
 ```
 
 This will create a configuration file as follow:
 
 ```yaml
 algorithm: segment-geospatial
 classification: null
+csf_filter: true
+csf_params:
+  class_threshold: 0.5
+  cloth_resolution: 0.2
+  interations: 500
+  slope_smooth: false
 device: cuda:0
 image_path: raster.tif
 input_path: pointcloud.las
 model_path: sam_vit_h_4b8939.pth
 model_type: vit_h
 output_path: classified.las
 resolution: 0.15
 sam_geo:
   automatic: true
   box_threshold: 0.24
   erosion_kernel_size: 3
-  sam_kwargs: false
+  sam_kwargs: true
   text_prompt: null
   text_threshold: 0.3
 sam_kwargs:
   crop_n_layers: 1
   crop_n_points_downscale_factor: 1
-  min_mask_region_area: 10000
+  min_mask_region_area: 1000
   points_per_side: 32
-  pred_iou_thresh: 0.9
+  pred_iou_thresh: 0.95
   stability_score_thresh: 0.92
 ```
 
 The second step is to run the segmentation:
 
 ```bash
 segment-lidar segment --config config.yaml
 ```
 
 The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
 
+## Testing data
+
+For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
+
+This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
+
 ## Configuration
 
 - `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
 - `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
-- `model_type`: SAM model version [vit_h/vit_l/vit_b].
+- `model_type`: SAM model version [**vit_h/vit_l/vit_b**].
 - `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
-- `input_path`: path to your input LAS/LAZ file.
-- `output_path`: path to your output LAS/LAZ file. The results will be saved in this file.
+- `input_path`: path to your input **.las/.laz** file.
+- `output_path`: path to your output .las/.laz file. The results will be saved in this file.
 - `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
-- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified class.
+- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified **class**.
+- `csf_filter`: apply ground filtering using cloth simulation filter.
+- `csf_params`: refer to [Cloth Simulation Filer](http://ramm.bnu.edu.cn/projects/CSF) for additional information.
 - `resolution`: resolution of the image created from the point cloud.
-- `sam_kwargs`: refer to **segment-anything** for additionnal information.
-- `sam_geo`: refer to **segment-geospatial** for additionnal information.
+- `sam_kwargs`: refer to **segment-anything** for additional information.
+- `sam_geo`: refer to **segment-geospatial** for additional information.
 
-Please note that the actual version is a pre-release and it's under tests. If you find any issue or bug, please report it in **issues** section. The second version will have more advanced features.
+Please note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
 ## Related repositories
 
-- [Segment Anything](https://github.com/facebookresearch/segment-anything)
+We would like to express our acknowledgments to the creators of:
+
+- [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
 ## Documentation
 
 Coming soon.
 
 ## License
 
 This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
 ## Author
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
-For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

### Comparing `segment-lidar-0.1.1/README.md` & `segment-lidar-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: segment-lidar
+Version: 0.1.2
+Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
+Home-page: https://github.com/Yarroudh/segment-lidar
+Author: Anass Yarroudh
+Author-email: ayarroudh@uliege.be
+License: BSD 3-Clause "New" or "Revised" License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
 *Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
@@ -43,75 +57,91 @@
   --help  Show this message and exit.
 
 Commands:
   create-config  Create a configuration YAML file.
   segment        Segment LiDAR data.
 ```
 
-The package reads `.LAS` or `.LAZ` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
+The package reads `.las` or `.laz` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
 
 ```bash
 segment-lidar create-config -o config.yaml
 ```
 
 This will create a configuration file as follow:
 
 ```yaml
 algorithm: segment-geospatial
 classification: null
+csf_filter: true
+csf_params:
+  class_threshold: 0.5
+  cloth_resolution: 0.2
+  interations: 500
+  slope_smooth: false
 device: cuda:0
 image_path: raster.tif
 input_path: pointcloud.las
 model_path: sam_vit_h_4b8939.pth
 model_type: vit_h
 output_path: classified.las
 resolution: 0.15
 sam_geo:
   automatic: true
   box_threshold: 0.24
   erosion_kernel_size: 3
-  sam_kwargs: false
+  sam_kwargs: true
   text_prompt: null
   text_threshold: 0.3
 sam_kwargs:
   crop_n_layers: 1
   crop_n_points_downscale_factor: 1
-  min_mask_region_area: 10000
+  min_mask_region_area: 1000
   points_per_side: 32
-  pred_iou_thresh: 0.9
+  pred_iou_thresh: 0.95
   stability_score_thresh: 0.92
 ```
 
 The second step is to run the segmentation:
 
 ```bash
 segment-lidar segment --config config.yaml
 ```
 
 The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
 
+## Testing data
+
+For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
+
+This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
+
 ## Configuration
 
 - `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
 - `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
-- `model_type`: SAM model version [vit_h/vit_l/vit_b].
+- `model_type`: SAM model version [**vit_h/vit_l/vit_b**].
 - `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
-- `input_path`: path to your input LAS/LAZ file.
-- `output_path`: path to your output LAS/LAZ file. The results will be saved in this file.
+- `input_path`: path to your input **.las/.laz** file.
+- `output_path`: path to your output .las/.laz file. The results will be saved in this file.
 - `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
-- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified class.
+- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified **class**.
+- `csf_filter`: apply ground filtering using cloth simulation filter.
+- `csf_params`: refer to [Cloth Simulation Filer](http://ramm.bnu.edu.cn/projects/CSF) for additional information.
 - `resolution`: resolution of the image created from the point cloud.
-- `sam_kwargs`: refer to **segment-anything** for additionnal information.
-- `sam_geo`: refer to **segment-geospatial** for additionnal information.
+- `sam_kwargs`: refer to **segment-anything** for additional information.
+- `sam_geo`: refer to **segment-geospatial** for additional information.
 
-Please note that the actual version is a pre-release and it's under tests. If you find any issue or bug, please report it in **issues** section. The second version will have more advanced features.
+Please note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
 ## Related repositories
 
-- [Segment Anything](https://github.com/facebookresearch/segment-anything)
+We would like to express our acknowledgments to the creators of:
+
+- [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
 ## Documentation
 
 Coming soon.
 
 ## License
```

### Comparing `segment-lidar-0.1.1/segment_lidar/main.py` & `segment-lidar-0.1.2/segment_lidar/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Copyright (c) 2023 - University of Liège
 # Author : Anass Yarroudh (ayarroudh@uliege.be), Geomatics Unit of ULiege
 # This file is distributed under the BSD-3 licence. See LICENSE file for complete text of the license.
 
 import os
+
+os.system('pip install git+https://github.com/jianboqi/CSF.git')
+
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
+import CSF
 import laspy
 
 
 def cloud_to_image(points, minx, maxx, miny, maxy, resolution):
     width = int((maxx - minx) / resolution) + 1
     height = int((maxy - miny) / resolution) + 1
 
@@ -71,39 +75,46 @@
 @click.option('--output', '-o', type=click.Path(exists=False), required=False, help='Output path')
 
 def create_config(output):
     '''
     Create a configuration YAML file.
     '''
     configuration = {
-        "device": "cuda:0",
         "algorithm": "segment-geospatial",
-        "model_type": "vit_h",
-        "model_path": "sam_vit_h_4b8939.pth",
-        "sam_kwargs": {
-            "points_per_side": 32,
-            "pred_iou_thresh": 0.9,
-            "stability_score_thresh": 0.92,
-            "crop_n_layers": 1,
-            "crop_n_points_downscale_factor": 1,
-            "min_mask_region_area": 10000
+        "classification": None,
+        "csf_filter": True,
+        "csf_params": {
+            "slope_smooth": False,
+            "cloth_resolution": 0.2,
+            "class_threshold": 0.5,
+            "interations": 500
         },
+        "device": "cuda:0",
+        "image_path": "raster.tif",
+        "input_path": "pointcloud.las",
+        "model_path": "sam_vit_h_4b8939.pth",
+        "model_type": "vit_h",
+        "output_path": "classified.las",
+        "resolution": 0.15,
         "sam_geo": {
             "automatic": True,
+            "box_threshold": 0.24,
             "erosion_kernel_size": 3,
-            "sam_kwargs": False,
+            "sam_kwargs": True,
             "text_prompt": None,
-            "box_threshold": 0.24,
-            "text_threshold": 0.30
+            "text_threshold": 0.3
         },
-        "input_path": "pointcloud.las",
-        "output_path": "classified.las",
-        "classification": None,
-        "image_path": "raster.tif",
-        "resolution": 0.15
+        "sam_kwargs": {
+            "crop_n_layers": 1,
+            "crop_n_points_downscale_factor": 1,
+            "min_mask_region_area": 1000,
+            "points_per_side": 32,
+            "pred_iou_thresh": 0.95,
+            "stability_score_thresh": 0.92
+        }
     }
 
     yaml_data = yaml.dump(configuration)
     output = output if output else 'config.yaml'
 
     with open(output, 'w') as file:
         file.write(yaml_data)
@@ -131,14 +142,16 @@
 
     # Set environment variables and device
     os.environ['KMP_DUPLICATE_LIB_OK'] = 'True'
     DEVICE = torch.device('cuda:0') if device == 'cuda:0' and torch.cuda.is_available() else torch.device('cpu')
 
     # Read input LiDAR data
     input_path = input if input else cnfg['input_path']
+    lidar = laspy.read(input_path)
+
 
     # 3D point cloud to 2D image
     image_path = cnfg['image_path']
     resolution = cnfg['resolution']
     classification = cnfg['classification']
     extension = os.path.splitext(input_path)[1]
 
@@ -150,28 +163,40 @@
         error_lines = error_message.split('\n')
         print(error_lines[-2])
         print(error_lines[-1])
         exit()
 
     extension = '.las' if extension == '.laz' else extension
 
-    lidar = laspy.read(input_path)
-
     # Filter points based on classification value
     if classification == None:
         pcd = lidar.points
     else:
         pcd = lidar.points[lidar.classification == classification]
 
     # Store points in a numpy array
     if hasattr(lidar, 'red') and hasattr(lidar, 'green') and hasattr(lidar, 'blue'):
         points = np.vstack((pcd.x, pcd.y, pcd.z, pcd.red / 255.0, pcd.green / 255.0, pcd.blue / 255.0)).transpose()
     else:
         points = np.vstack((pcd.x, pcd.y, pcd.z)).transpose()
 
+    # Filter ground points if required
+    if cnfg['csf_filter']:
+        csf = CSF.CSF()
+        csf.params.bSloopSmooth = cnfg['csf_params']['slope_smooth']
+        csf.params.cloth_resolution = cnfg['csf_params']['cloth_resolution']
+        csf.params.interations = cnfg['csf_params']['iterations']
+        csf.params.class_threshold = cnfg['csf_params']['class_threshold']
+        csf.setPointCloud(points[:, :3])
+
+        ground = CSF.VecInt()
+        non_ground = CSF.VecInt()
+        csf.do_filtering(ground, non_ground)
+        points = points[non_ground, :]
+
     # Convert points to image
     minx = np.min(points[:, 0])
     maxx = np.max(points[:, 0])
     miny = np.min(points[:, 1])
     maxy = np.max(points[:, 1])
     image = cloud_to_image(points, minx, maxx, miny, maxy, resolution)
     image = np.asarray(image).astype(np.uint8)
@@ -254,20 +279,30 @@
         exit()
 
     with rasterio.open(os.path.dirname(output_path) + "/labeled.tif", 'r') as src:
         segmented_image = src.read()
         segmented_image = np.squeeze(segmented_image)
 
     segment_ids = image_to_cloud(points, minx, maxy, segmented_image, resolution)
-    lidar.points = pcd
-    lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
-    lidar.segment_id = segment_ids
+
+    # Save point cloud
+    if cnfg['csf_filter']:
+        points = np.concatenate((non_ground, ground))
+        lidar.points = pcd[points]
+        segment_ids = np.append(segment_ids, np.full(len(ground), -1))
+        lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
+        lidar.segment_id = segment_ids
+    else:
+        lidar.points = pcd
+        lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
+        lidar.segment_id = segment_ids
 
     lidar.write(output_path)
 
+
     end = time.time()
     print(f'Point cloud segmentation completed in {np.round(end - start, 2)} seconds.')
 
 
 cli.add_command(create_config)
 cli.add_command(segment)
```

### Comparing `segment-lidar-0.1.1/segment_lidar.egg-info/PKG-INFO` & `segment-lidar-0.1.2/segment_lidar.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
@@ -54,75 +57,91 @@
   --help  Show this message and exit.
 
 Commands:
   create-config  Create a configuration YAML file.
   segment        Segment LiDAR data.
 ```
 
-The package reads `.LAS` or `.LAZ` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
+The package reads `.las` or `.laz` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
 
 ```bash
 segment-lidar create-config -o config.yaml
 ```
 
 This will create a configuration file as follow:
 
 ```yaml
 algorithm: segment-geospatial
 classification: null
+csf_filter: true
+csf_params:
+  class_threshold: 0.5
+  cloth_resolution: 0.2
+  interations: 500
+  slope_smooth: false
 device: cuda:0
 image_path: raster.tif
 input_path: pointcloud.las
 model_path: sam_vit_h_4b8939.pth
 model_type: vit_h
 output_path: classified.las
 resolution: 0.15
 sam_geo:
   automatic: true
   box_threshold: 0.24
   erosion_kernel_size: 3
-  sam_kwargs: false
+  sam_kwargs: true
   text_prompt: null
   text_threshold: 0.3
 sam_kwargs:
   crop_n_layers: 1
   crop_n_points_downscale_factor: 1
-  min_mask_region_area: 10000
+  min_mask_region_area: 1000
   points_per_side: 32
-  pred_iou_thresh: 0.9
+  pred_iou_thresh: 0.95
   stability_score_thresh: 0.92
 ```
 
 The second step is to run the segmentation:
 
 ```bash
 segment-lidar segment --config config.yaml
 ```
 
 The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
 
+## Testing data
+
+For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
+
+This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
+
 ## Configuration
 
 - `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
 - `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
-- `model_type`: SAM model version [vit_h/vit_l/vit_b].
+- `model_type`: SAM model version [**vit_h/vit_l/vit_b**].
 - `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
-- `input_path`: path to your input LAS/LAZ file.
-- `output_path`: path to your output LAS/LAZ file. The results will be saved in this file.
+- `input_path`: path to your input **.las/.laz** file.
+- `output_path`: path to your output .las/.laz file. The results will be saved in this file.
 - `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
-- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified class.
+- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified **class**.
+- `csf_filter`: apply ground filtering using cloth simulation filter.
+- `csf_params`: refer to [Cloth Simulation Filer](http://ramm.bnu.edu.cn/projects/CSF) for additional information.
 - `resolution`: resolution of the image created from the point cloud.
-- `sam_kwargs`: refer to **segment-anything** for additionnal information.
-- `sam_geo`: refer to **segment-geospatial** for additionnal information.
+- `sam_kwargs`: refer to **segment-anything** for additional information.
+- `sam_geo`: refer to **segment-geospatial** for additional information.
 
-Please note that the actual version is a pre-release and it's under tests. If you find any issue or bug, please report it in **issues** section. The second version will have more advanced features.
+Please note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
 ## Related repositories
 
-- [Segment Anything](https://github.com/facebookresearch/segment-anything)
+We would like to express our acknowledgments to the creators of:
+
+- [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
 ## Documentation
 
 Coming soon.
 
 ## License
```

### Comparing `segment-lidar-0.1.1/setup.py` & `segment-lidar-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="segment-lidar",
-    version='0.1.1',
+    version='0.1.2',
     description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause "New" or "Revised" License',
-    author = 'Anass Yarroudh',
-    author_email = 'ayarroudh@uliege.be',
-    url = 'https://github.com/Yarroudh/segment-lidar',
+    author='Anass Yarroudh',
+    author_email='ayarroudh@uliege.be',
+    url='https://github.com/Yarroudh/segment-lidar',
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "segment-lidar=segment_lidar.main:cli"
         ]
-    }
-)
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+    ],
+)
```

