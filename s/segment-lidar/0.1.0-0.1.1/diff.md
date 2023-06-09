# Comparing `tmp/segment-lidar-0.1.0.tar.gz` & `tmp/segment-lidar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-lidar-0.1.0.tar", last modified: Thu Jun  8 13:28:53 2023, max compression
+gzip compressed data, was "segment-lidar-0.1.1.tar", last modified: Fri Jun  9 12:41:33 2023, max compression
```

## Comparing `segment-lidar-0.1.0.tar` & `segment-lidar-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:28:53.666510 segment-lidar-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-06-08 12:35:26.000000 segment-lidar-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4586 2023-06-08 13:28:53.665513 segment-lidar-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4221 2023-06-08 12:33:06.000000 segment-lidar-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 13:28:53.647512 segment-lidar-0.1.0/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.0/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0     8941 2023-06-08 12:35:00.000000 segment-lidar-0.1.0/segment_lidar/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:28:53.664517 segment-lidar-0.1.0/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     4586 2023-06-08 13:28:53.000000 segment-lidar-0.1.0/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-08 13:28:53.000000 segment-lidar-0.1.0/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:28:53.000000 segment-lidar-0.1.0/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-08 13:28:53.000000 segment-lidar-0.1.0/segment_lidar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2023-06-08 13:28:53.000000 segment-lidar-0.1.0/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 13:28:53.000000 segment-lidar-0.1.0/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 13:28:53.666510 segment-lidar-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-06-08 13:13:29.000000 segment-lidar-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:41:33.416669 segment-lidar-0.1.1/
+-rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6072 2023-06-09 12:41:33.415667 segment-lidar-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5679 2023-06-09 11:48:47.000000 segment-lidar-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 12:41:33.383659 segment-lidar-0.1.1/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.1/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0     9739 2023-06-09 11:49:26.000000 segment-lidar-0.1.1/segment_lidar/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:41:33.414668 segment-lidar-0.1.1/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     6072 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-09 12:41:33.000000 segment-lidar-0.1.1/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 12:41:32.000000 segment-lidar-0.1.1/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 12:41:33.417667 segment-lidar-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-06-09 12:41:18.000000 segment-lidar-0.1.1/setup.py
```

### Comparing `segment-lidar-0.1.0/PKG-INFO` & `segment-lidar-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
-License: MIT License
+License: BSD 3-Clause "New" or "Revised" License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
-*A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
-![results](https://github.com/Yarroudh/segment-lidar/results.gif)
+![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
+
 
 ## Installation
 
-We recommand using `python==3.9`.
-To install `segment-lidar` from source, you need to run the following commands:
+We recommand using `python==3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
+
+Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
+
+```bash
+pip install segment-lidar
+```
+
+Or, you can install it from source by running the following commands:
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
 ## Usage of the package
 
 After installation, you have a small program called <code>segment-lidar</code>. Use <code>segment-lidar --help</code> to see the detailed help:
 
-```bash
+```
 Usage: segment-lidar [OPTIONS] COMMAND [ARGS]...
 
   A package for segmenting LiDAR data using Segment-Anything from Meta AI
   Research.
 
 Options:
   --help  Show this message and exit.
@@ -88,24 +96,40 @@
 
 ```bash
 segment-lidar segment --config config.yaml
 ```
 
 The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
 
+## Configuration
+
+- `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
+- `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
+- `model_type`: SAM model version [vit_h/vit_l/vit_b].
+- `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
+- `input_path`: path to your input LAS/LAZ file.
+- `output_path`: path to your output LAS/LAZ file. The results will be saved in this file.
+- `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
+- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified class.
+- `resolution`: resolution of the image created from the point cloud.
+- `sam_kwargs`: refer to **segment-anything** for additionnal information.
+- `sam_geo`: refer to **segment-geospatial** for additionnal information.
+
+Please note that the actual version is a pre-release and it's under tests. If you find any issue or bug, please report it in **issues** section. The second version will have more advanced features.
+
 ## Related repositories
 
 - [Segment Anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
 ## Documentation
 
 Coming soon.
 
 ## License
 
-This software is under the MIT License, a permissive license that grants you extensive freedom to use, modify, and distribute the software, provided that you include the MIT copyright and license notice in all copies or substantial portions of the software. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
+This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
 ## Author
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

### Comparing `segment-lidar-0.1.0/README.md` & `segment-lidar-0.1.1/segment_lidar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,54 @@
+Metadata-Version: 2.1
+Name: segment-lidar
+Version: 0.1.1
+Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
+Home-page: https://github.com/Yarroudh/segment-lidar
+Author: Anass Yarroudh
+Author-email: ayarroudh@uliege.be
+License: BSD 3-Clause "New" or "Revised" License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
-*A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
-![results](https://github.com/Yarroudh/segment-lidar/results.gif)
+![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
+
 
 ## Installation
 
-We recommand using `python==3.9`.
-To install `segment-lidar` from source, you need to run the following commands:
+We recommand using `python==3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
+
+Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
+
+```bash
+pip install segment-lidar
+```
+
+Or, you can install it from source by running the following commands:
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
 ## Usage of the package
 
 After installation, you have a small program called <code>segment-lidar</code>. Use <code>segment-lidar --help</code> to see the detailed help:
 
-```bash
+```
 Usage: segment-lidar [OPTIONS] COMMAND [ARGS]...
 
   A package for segmenting LiDAR data using Segment-Anything from Meta AI
   Research.
 
 Options:
   --help  Show this message and exit.
@@ -77,24 +96,40 @@
 
 ```bash
 segment-lidar segment --config config.yaml
 ```
 
 The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
 
+## Configuration
+
+- `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
+- `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
+- `model_type`: SAM model version [vit_h/vit_l/vit_b].
+- `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
+- `input_path`: path to your input LAS/LAZ file.
+- `output_path`: path to your output LAS/LAZ file. The results will be saved in this file.
+- `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
+- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified class.
+- `resolution`: resolution of the image created from the point cloud.
+- `sam_kwargs`: refer to **segment-anything** for additionnal information.
+- `sam_geo`: refer to **segment-geospatial** for additionnal information.
+
+Please note that the actual version is a pre-release and it's under tests. If you find any issue or bug, please report it in **issues** section. The second version will have more advanced features.
+
 ## Related repositories
 
 - [Segment Anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
 ## Documentation
 
 Coming soon.
 
 ## License
 
-This software is under the MIT License, a permissive license that grants you extensive freedom to use, modify, and distribute the software, provided that you include the MIT copyright and license notice in all copies or substantial portions of the software. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
+This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
 ## Author
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

### Comparing `segment-lidar-0.1.0/segment_lidar/main.py` & `segment-lidar-0.1.1/segment_lidar/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,260 +1,275 @@
-import os
-import yaml
-import click
-import time
-import torch
-import cv2
-import numpy as np
-import supervision as sv
-from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
-from samgeo import SamGeo
-from samgeo.text_sam import LangSAM
-import rasterio
-import laspy
-
-
-def cloud_to_image(points, minx, maxx, miny, maxy, resolution):
-    width = int((maxx - minx) / resolution) + 1
-    height = int((maxy - miny) / resolution) + 1
-
-    image = np.zeros((height, width, 3), dtype=np.uint8)
-    for point in points:
-        if points.shape[1] == 3:
-            x, y, *_ = point
-            r, g, b = (255, 255, 255)
-            pixel_x = int((x - minx) / resolution)
-            pixel_y = int((maxy - y) / resolution)
-            image[pixel_y, pixel_x] = [r, g, b]
-        else:
-            x, y, *_ = point
-            r, g, b = point[-3:]
-            pixel_x = int((x - minx) / resolution)
-            pixel_y = int((maxy - y) / resolution)
-            image[pixel_y, pixel_x] = [r, g, b]
-
-    return image
-
-
-def image_to_cloud(points, minx, maxy, image, resolution):
-    segment_ids = []
-    unique_values = {}
-    image = np.asarray(image)
-
-    for point in points:
-        x, y, *_ = point
-        pixel_x = int((x - minx) / resolution)
-        pixel_y = int((maxy - y) / resolution)
-        if not (0 <= pixel_x < image.shape[1]) or not (0 <= pixel_y < image.shape[0]):
-            segment_ids.append(-1)
-            continue
-        rgb = image[pixel_y, pixel_x]
-
-        if rgb not in unique_values:
-            unique_values[rgb] = len(unique_values)
-
-        id = unique_values[rgb]
-        segment_ids.append(id)
-
-    return segment_ids
-
-
-@click.group(help="A package for segmenting LiDAR data using Segment-Anything from Meta AI Research.")
-def cli():
-    pass
-
-
-@click.command()
-@click.option('--output', '-o', type=click.Path(exists=False), required=False, help='Output path')
-
-def create_config(output):
-    '''
-    Create a configuration YAML file.
-    '''
-    configuration = {
-        "device": "cuda:0",
-        "algorithm": "segment-geospatial",
-        "model_type": "vit_h",
-        "model_path": "sam_vit_h_4b8939.pth",
-        "sam_kwargs": {
-            "points_per_side": 32,
-            "pred_iou_thresh": 0.9,
-            "stability_score_thresh": 0.92,
-            "crop_n_layers": 1,
-            "crop_n_points_downscale_factor": 1,
-            "min_mask_region_area": 10000
-        },
-        "sam_geo": {
-            "automatic": True,
-            "erosion_kernel_size": 3,
-            "sam_kwargs": False,
-            "text_prompt": None,
-            "box_threshold": 0.24,
-            "text_threshold": 0.30
-        },
-        "input_path": "pointcloud.las",
-        "output_path": "classified.las",
-        "classification": None,
-        "image_path": "raster.tif",
-        "resolution": 0.15
-    }
-
-    yaml_data = yaml.dump(configuration)
-    output = output if output else 'config.yaml'
-
-    with open(output, 'w') as file:
-        file.write(yaml_data)
-
-    print(f'Configuration file created at {output}.')
-
-
-@cli.command()
-@click.option('--input', '-i', type=click.Path(exists=True), required=False, help='Input LiDAR data')
-@click.option('--output', '-o', type=click.Path(exists=False), required=False, help='Output file')
-@click.option('--config', '-c', type=click.Path(exists=True), required=True, help='Configuration file')
-
-def segment(input, output, config):
-    '''
-    Segment LiDAR data.
-    '''
-    start = time.time()
-
-    # Read configuration file
-    cnfg = yaml.load(open(config, 'r'), Loader=yaml.FullLoader)
-    device = cnfg['device']
-    model_type = cnfg['model_type']
-    model_path = cnfg['model_path']
-    mask = cnfg['sam_kwargs']
-
-    # Set environment variables and device
-    os.environ['KMP_DUPLICATE_LIB_OK'] = 'True'
-    DEVICE = torch.device('cuda:0') if device == 'cuda:0' and torch.cuda.is_available() else torch.device('cpu')
-
-    # Read input LiDAR data
-    input_path = input if input else cnfg['input_path']
-
-    # 3D point cloud to 2D image
-    image_path = cnfg['image_path']
-    resolution = cnfg['resolution']
-    extension = os.path.splitext(input_path)[1]
-
-    try:
-        if extension not in ['.laz', '.las']:
-            raise ValueError(f'The input file format {extension} is not supported.\nThe file format should be [.las/.laz].')
-    except ValueError as error:
-        error_message = str(error)
-        error_lines = error_message.split('\n')
-        print(error_lines[-2])
-        print(error_lines[-1])
-        exit()
-
-    extension = '.las' if extension == '.laz' else extension
-
-    lidar = laspy.read(input_path)
-    if hasattr(lidar, 'red') and hasattr(lidar, 'green') and hasattr(lidar, 'blue'):
-        points = np.vstack((lidar.x, lidar.y, lidar.z, lidar.red / 255.0, lidar.green / 255.0, lidar.blue / 255.0)).transpose()
-    else:
-        points = np.vstack((lidar.x, lidar.y, lidar.z)).transpose()
-
-    minx = np.min(points[:, 0])
-    maxx = np.max(points[:, 0])
-    miny = np.min(points[:, 1])
-    maxy = np.max(points[:, 1])
-    image = cloud_to_image(points, minx, maxx, miny, maxy, resolution)
-    image = np.asarray(image).astype(np.uint8)
-
-    with rasterio.open(
-        image_path,
-        'w',
-        driver='GTiff',
-        width=image.shape[1],
-        height=image.shape[0],
-        count=3,
-        dtype=image.dtype
-    ) as dst:
-        for i in range(3):
-            dst.write(image[:, :, i], i + 1)
-
-    # Instance segmentation
-    with rasterio.open(image_path, 'r') as src:
-        image_rgb = src.read()
-
-    output_path = output if output else cnfg['output_path']
-    if cnfg['algorithm'] == 'segment-anything':
-        # Load model
-        sam = sam_model_registry[model_type](checkpoint=model_path)
-        sam.to(device=DEVICE)
-
-        # Set mask generator
-        mask_generator = SamAutomaticMaskGenerator(
-            model=sam,
-            points_per_side=mask['points_per_side'],
-            pred_iou_thresh=mask['pred_iou_thresh'],
-            stability_score_thresh=mask['stability_score_thresh'],
-            crop_n_layers=mask['crop_n_layers'],
-            crop_n_points_downscale_factor=mask['crop_n_points_downscale_factor'],
-            min_mask_region_area=mask['min_mask_region_area']
-        )
-
-        image_rgb = image_rgb.reshape((image_rgb.shape[1], image_rgb.shape[2], image_rgb.shape[0]))
-        result = mask_generator.generate(image_rgb)
-        mask_annotator = sv.MaskAnnotator()
-        detections = sv.Detections.from_sam(result)
-        annotated_image = mask_annotator.annotate(image_rgb, detections)
-
-        # Save annotated image
-        cv2.imwrite(f"{os.path.dirname(output_path)}/labeled.tif", annotated_image)
-
-    elif cnfg['algorithm'] == 'segment-geospatial':
-        # Parameters
-        sam_kwargs = mask if cnfg['sam_geo']['sam_kwargs'] else None
-        automatic = cnfg['sam_geo']['automatic']
-        text_prompt = cnfg['sam_geo']['text_prompt']
-        box_threshold = cnfg['sam_geo']['box_threshold']
-        text_threshold = cnfg['sam_geo']['text_threshold']
-        erosion_kernel = (cnfg['sam_geo']['erosion_kernel_size'], cnfg['sam_geo']['erosion_kernel_size']) if cnfg['sam_geo']['erosion_kernel_size'] else None
-
-        # Segmentation
-        if text_prompt is not None:
-            sam = LangSAM()
-            sam.predict(image=image_path, text_prompt=text_prompt, box_threshold=box_threshold, text_threshold=text_threshold, output=f"{os.path.dirname(output_path)}/labeled.tif",)
-
-        else:
-            sam = SamGeo(
-                model_type=model_type,
-                checkpoint=model_path,
-                automatic=automatic,
-                sam_kwargs=sam_kwargs
-            )
-            sam.generate(source=image_path, output=f"{os.path.dirname(output_path)}/labeled.tif", erosion_kernel=erosion_kernel, foreground=True, unique=True)
-
-    # Project results on point cloud
-    extension = os.path.splitext(output_path)[1]
-    try:
-        if extension not in ['.laz', '.las']:
-            raise ValueError(f'The output file format {extension} is not supported.\nThe file format should be [.las/.laz].')
-    except ValueError as error:
-        error_message = str(error)
-        error_lines = error_message.split('\n')
-        print(error_lines[-2])
-        print(error_lines[-1])
-        exit()
-
-    with rasterio.open(os.path.dirname(output_path) + "/labeled.tif", 'r') as src:
-        segmented_image = src.read()
-        segmented_image = np.squeeze(segmented_image)
-
-    segment_ids = image_to_cloud(points, minx, maxy, segmented_image, resolution)
-    lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
-    lidar.segment_id = segment_ids
-
-    lidar.write(output_path)
-
-    end = time.time()
-    print(f'Point cloud segmentation completed in {np.round(end - start, 2)} seconds.')
-
-
-cli.add_command(create_config)
-cli.add_command(segment)
-
-if __name__ == '__main__':
+# Copyright (c) 2023 - University of Liège
+# Author : Anass Yarroudh (ayarroudh@uliege.be), Geomatics Unit of ULiege
+# This file is distributed under the BSD-3 licence. See LICENSE file for complete text of the license.
+
+import os
+import yaml
+import click
+import time
+import torch
+import cv2
+import numpy as np
+import supervision as sv
+from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
+from samgeo import SamGeo
+from samgeo.text_sam import LangSAM
+import rasterio
+import laspy
+
+
+def cloud_to_image(points, minx, maxx, miny, maxy, resolution):
+    width = int((maxx - minx) / resolution) + 1
+    height = int((maxy - miny) / resolution) + 1
+
+    image = np.zeros((height, width, 3), dtype=np.uint8)
+    for point in points:
+        if points.shape[1] == 3:
+            x, y, *_ = point
+            r, g, b = (255, 255, 255)
+            pixel_x = int((x - minx) / resolution)
+            pixel_y = int((maxy - y) / resolution)
+            image[pixel_y, pixel_x] = [r, g, b]
+        else:
+            x, y, *_ = point
+            r, g, b = point[-3:]
+            pixel_x = int((x - minx) / resolution)
+            pixel_y = int((maxy - y) / resolution)
+            image[pixel_y, pixel_x] = [r, g, b]
+
+    return image
+
+
+def image_to_cloud(points, minx, maxy, image, resolution):
+    segment_ids = []
+    unique_values = {}
+    image = np.asarray(image)
+
+    for point in points:
+        x, y, *_ = point
+        pixel_x = int((x - minx) / resolution)
+        pixel_y = int((maxy - y) / resolution)
+        if not (0 <= pixel_x < image.shape[1]) or not (0 <= pixel_y < image.shape[0]):
+            segment_ids.append(-1)
+            continue
+        rgb = image[pixel_y, pixel_x]
+
+        if rgb not in unique_values:
+            unique_values[rgb] = len(unique_values)
+
+        id = unique_values[rgb]
+        segment_ids.append(id)
+
+    return segment_ids
+
+
+@click.group(help="A package for segmenting LiDAR data using Segment-Anything from Meta AI Research.")
+def cli():
+    pass
+
+
+@click.command()
+@click.option('--output', '-o', type=click.Path(exists=False), required=False, help='Output path')
+
+def create_config(output):
+    '''
+    Create a configuration YAML file.
+    '''
+    configuration = {
+        "device": "cuda:0",
+        "algorithm": "segment-geospatial",
+        "model_type": "vit_h",
+        "model_path": "sam_vit_h_4b8939.pth",
+        "sam_kwargs": {
+            "points_per_side": 32,
+            "pred_iou_thresh": 0.9,
+            "stability_score_thresh": 0.92,
+            "crop_n_layers": 1,
+            "crop_n_points_downscale_factor": 1,
+            "min_mask_region_area": 10000
+        },
+        "sam_geo": {
+            "automatic": True,
+            "erosion_kernel_size": 3,
+            "sam_kwargs": False,
+            "text_prompt": None,
+            "box_threshold": 0.24,
+            "text_threshold": 0.30
+        },
+        "input_path": "pointcloud.las",
+        "output_path": "classified.las",
+        "classification": None,
+        "image_path": "raster.tif",
+        "resolution": 0.15
+    }
+
+    yaml_data = yaml.dump(configuration)
+    output = output if output else 'config.yaml'
+
+    with open(output, 'w') as file:
+        file.write(yaml_data)
+
+    print(f'Configuration file created at {output}.')
+
+
+@cli.command()
+@click.option('--input', '-i', type=click.Path(exists=True), required=False, help='Input LiDAR data')
+@click.option('--output', '-o', type=click.Path(exists=False), required=False, help='Output file')
+@click.option('--config', '-c', type=click.Path(exists=True), required=True, help='Configuration file')
+
+def segment(input, output, config):
+    '''
+    Segment LiDAR data.
+    '''
+    start = time.time()
+
+    # Read configuration file
+    cnfg = yaml.load(open(config, 'r'), Loader=yaml.FullLoader)
+    device = cnfg['device']
+    model_type = cnfg['model_type']
+    model_path = cnfg['model_path']
+    mask = cnfg['sam_kwargs']
+
+    # Set environment variables and device
+    os.environ['KMP_DUPLICATE_LIB_OK'] = 'True'
+    DEVICE = torch.device('cuda:0') if device == 'cuda:0' and torch.cuda.is_available() else torch.device('cpu')
+
+    # Read input LiDAR data
+    input_path = input if input else cnfg['input_path']
+
+    # 3D point cloud to 2D image
+    image_path = cnfg['image_path']
+    resolution = cnfg['resolution']
+    classification = cnfg['classification']
+    extension = os.path.splitext(input_path)[1]
+
+    try:
+        if extension not in ['.laz', '.las']:
+            raise ValueError(f'The input file format {extension} is not supported.\nThe file format should be [.las/.laz].')
+    except ValueError as error:
+        error_message = str(error)
+        error_lines = error_message.split('\n')
+        print(error_lines[-2])
+        print(error_lines[-1])
+        exit()
+
+    extension = '.las' if extension == '.laz' else extension
+
+    lidar = laspy.read(input_path)
+
+    # Filter points based on classification value
+    if classification == None:
+        pcd = lidar.points
+    else:
+        pcd = lidar.points[lidar.classification == classification]
+
+    # Store points in a numpy array
+    if hasattr(lidar, 'red') and hasattr(lidar, 'green') and hasattr(lidar, 'blue'):
+        points = np.vstack((pcd.x, pcd.y, pcd.z, pcd.red / 255.0, pcd.green / 255.0, pcd.blue / 255.0)).transpose()
+    else:
+        points = np.vstack((pcd.x, pcd.y, pcd.z)).transpose()
+
+    # Convert points to image
+    minx = np.min(points[:, 0])
+    maxx = np.max(points[:, 0])
+    miny = np.min(points[:, 1])
+    maxy = np.max(points[:, 1])
+    image = cloud_to_image(points, minx, maxx, miny, maxy, resolution)
+    image = np.asarray(image).astype(np.uint8)
+
+    with rasterio.open(
+        image_path,
+        'w',
+        driver='GTiff',
+        width=image.shape[1],
+        height=image.shape[0],
+        count=3,
+        dtype=image.dtype
+    ) as dst:
+        for i in range(3):
+            dst.write(image[:, :, i], i + 1)
+
+    # Instance segmentation
+    with rasterio.open(image_path, 'r') as src:
+        image_rgb = src.read()
+
+    output_path = output if output else cnfg['output_path']
+    if cnfg['algorithm'] == 'segment-anything':
+        # Load model
+        sam = sam_model_registry[model_type](checkpoint=model_path)
+        sam.to(device=DEVICE)
+
+        # Set mask generator
+        mask_generator = SamAutomaticMaskGenerator(
+            model=sam,
+            points_per_side=mask['points_per_side'],
+            pred_iou_thresh=mask['pred_iou_thresh'],
+            stability_score_thresh=mask['stability_score_thresh'],
+            crop_n_layers=mask['crop_n_layers'],
+            crop_n_points_downscale_factor=mask['crop_n_points_downscale_factor'],
+            min_mask_region_area=mask['min_mask_region_area']
+        )
+
+        image_rgb = image_rgb.reshape((image_rgb.shape[1], image_rgb.shape[2], image_rgb.shape[0]))
+        result = mask_generator.generate(image_rgb)
+        mask_annotator = sv.MaskAnnotator()
+        detections = sv.Detections.from_sam(result)
+        annotated_image = mask_annotator.annotate(image_rgb, detections)
+
+        # Save annotated image
+        cv2.imwrite(f"{os.path.dirname(output_path)}/labeled.tif", annotated_image)
+
+    elif cnfg['algorithm'] == 'segment-geospatial':
+        # Parameters
+        sam_kwargs = mask if cnfg['sam_geo']['sam_kwargs'] else None
+        automatic = cnfg['sam_geo']['automatic']
+        text_prompt = cnfg['sam_geo']['text_prompt']
+        box_threshold = cnfg['sam_geo']['box_threshold']
+        text_threshold = cnfg['sam_geo']['text_threshold']
+        erosion_kernel = (cnfg['sam_geo']['erosion_kernel_size'], cnfg['sam_geo']['erosion_kernel_size']) if cnfg['sam_geo']['erosion_kernel_size'] else None
+
+        # Segmentation
+        if text_prompt is not None:
+            sam = LangSAM()
+            sam.predict(image=image_path, text_prompt=text_prompt, box_threshold=box_threshold, text_threshold=text_threshold, output=f"{os.path.dirname(output_path)}/labeled.tif",)
+
+        else:
+            sam = SamGeo(
+                model_type=model_type,
+                checkpoint=model_path,
+                automatic=automatic,
+                sam_kwargs=sam_kwargs
+            )
+            sam.generate(source=image_path, output=f"{os.path.dirname(output_path)}/labeled.tif", erosion_kernel=erosion_kernel, foreground=True, unique=True)
+
+    # Project results on point cloud
+    extension = os.path.splitext(output_path)[1]
+    try:
+        if extension not in ['.laz', '.las']:
+            raise ValueError(f'The output file format {extension} is not supported.\nThe file format should be [.las/.laz].')
+    except ValueError as error:
+        error_message = str(error)
+        error_lines = error_message.split('\n')
+        print(error_lines[-2])
+        print(error_lines[-1])
+        exit()
+
+    with rasterio.open(os.path.dirname(output_path) + "/labeled.tif", 'r') as src:
+        segmented_image = src.read()
+        segmented_image = np.squeeze(segmented_image)
+
+    segment_ids = image_to_cloud(points, minx, maxy, segmented_image, resolution)
+    lidar.points = pcd
+    lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
+    lidar.segment_id = segment_ids
+
+    lidar.write(output_path)
+
+    end = time.time()
+    print(f'Point cloud segmentation completed in {np.round(end - start, 2)} seconds.')
+
+
+cli.add_command(create_config)
+cli.add_command(segment)
+
+if __name__ == '__main__':
     cli(prog_name='segment-lidar')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `segment-lidar-0.1.0/segment_lidar.egg-info/PKG-INFO` & `segment-lidar-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-Metadata-Version: 2.1
-Name: segment-lidar
-Version: 0.1.0
-Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
-Home-page: https://github.com/Yarroudh/segment-lidar
-Author: Anass Yarroudh
-Author-email: ayarroudh@uliege.be
-License: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
-*A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
-![results](https://github.com/Yarroudh/segment-lidar/results.gif)
+![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
+
 
 ## Installation
 
-We recommand using `python==3.9`.
-To install `segment-lidar` from source, you need to run the following commands:
+We recommand using `python==3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
+
+Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
+
+```bash
+pip install segment-lidar
+```
+
+Or, you can install it from source by running the following commands:
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
 ## Usage of the package
 
 After installation, you have a small program called <code>segment-lidar</code>. Use <code>segment-lidar --help</code> to see the detailed help:
 
-```bash
+```
 Usage: segment-lidar [OPTIONS] COMMAND [ARGS]...
 
   A package for segmenting LiDAR data using Segment-Anything from Meta AI
   Research.
 
 Options:
   --help  Show this message and exit.
@@ -88,24 +85,40 @@
 
 ```bash
 segment-lidar segment --config config.yaml
 ```
 
 The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
 
+## Configuration
+
+- `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
+- `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
+- `model_type`: SAM model version [vit_h/vit_l/vit_b].
+- `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
+- `input_path`: path to your input LAS/LAZ file.
+- `output_path`: path to your output LAS/LAZ file. The results will be saved in this file.
+- `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
+- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified class.
+- `resolution`: resolution of the image created from the point cloud.
+- `sam_kwargs`: refer to **segment-anything** for additionnal information.
+- `sam_geo`: refer to **segment-geospatial** for additionnal information.
+
+Please note that the actual version is a pre-release and it's under tests. If you find any issue or bug, please report it in **issues** section. The second version will have more advanced features.
+
 ## Related repositories
 
 - [Segment Anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
 ## Documentation
 
 Coming soon.
 
 ## License
 
-This software is under the MIT License, a permissive license that grants you extensive freedom to use, modify, and distribute the software, provided that you include the MIT copyright and license notice in all copies or substantial portions of the software. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
+This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
 ## Author
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

### Comparing `segment-lidar-0.1.0/setup.py` & `segment-lidar-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="segment-lidar",
-    version='0.1.0',
+    version='0.1.1',
     description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    license='MIT License',
+    license='BSD 3-Clause "New" or "Revised" License',
     author = 'Anass Yarroudh',
     author_email = 'ayarroudh@uliege.be',
     url = 'https://github.com/Yarroudh/segment-lidar',
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "segment-lidar=segment_lidar.main:cli"
         ]
     }
-)
+)
```

