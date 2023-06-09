# Comparing `tmp/bboxconverter-0.1.8.tar.gz` & `tmp/bboxconverter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bboxconverter-0.1.8.tar", max compression
+gzip compressed data, was "bboxconverter-0.1.9.tar", max compression
```

## Comparing `bboxconverter-0.1.8.tar` & `bboxconverter-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2023-03-18 15:52:29.892549 bboxconverter-0.1.8/LICENSE
--rw-r--r--   0        0        0     4159 2023-03-18 15:52:29.892549 bboxconverter-0.1.8/README.md
--rw-r--r--   0        0        0     2084 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      715 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/__init__.py
--rw-r--r--   0        0        0       78 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/core/__init__.py
--rw-r--r--   0        0        0     8240 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/core/bbox.py
--rw-r--r--   0        0        0    10264 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/core/bbox_parser.py
--rw-r--r--   0        0        0        0 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/__init__.py
--rw-r--r--   0        0        0      634 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/api.py
--rw-r--r--   0        0        0     1279 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_coco.py
--rw-r--r--   0        0        0     1978 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_csv.py
--rw-r--r--   0        0        0     2823 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_manifest.py
--rw-r--r--   0        0        0       42 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_parquet.py
--rw-r--r--   0        0        0     2069 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_pascal_voc.py
--rw-r--r--   0        0        0      479 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_xml.py
--rw-r--r--   0        0        0       67 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/reader_yolo.py
--rw-r--r--   0        0        0     1841 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/writer_coco.py
--rw-r--r--   0        0        0     3096 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/writer_json_lines.py
--rw-r--r--   0        0        0      166 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/writer_pascal_voc.py
--rw-r--r--   0        0        0     1435 2023-03-18 15:52:30.044549 bboxconverter-0.1.8/src/bboxconverter/io/writer_yolo.py
--rw-r--r--   0        0        0     5615 1970-01-01 00:00:00.000000 bboxconverter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 21:46:45.640865 bboxconverter-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4946 2023-06-09 21:46:45.640865 bboxconverter-0.1.9/README.md
+-rw-r--r--   0        0        0     2110 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/core/__init__.py
+-rw-r--r--   0        0        0     8240 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/core/bbox.py
+-rw-r--r--   0        0        0    11774 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/core/bbox_parser.py
+-rw-r--r--   0        0        0      300 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/io/__init__.py
+-rw-r--r--   0        0        0      756 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/io/api.py
+-rw-r--r--   0        0        0     1460 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/io/reader_coco.py
+-rw-r--r--   0        0        0     1978 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/io/reader_csv.py
+-rw-r--r--   0        0        0     2823 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/io/reader_manifest.py
+-rw-r--r--   0        0        0       42 2023-06-09 21:46:45.824867 bboxconverter-0.1.9/src/bboxconverter/io/reader_parquet.py
+-rw-r--r--   0        0        0     2069 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/reader_pascal_voc.py
+-rw-r--r--   0        0        0      479 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/reader_xml.py
+-rw-r--r--   0        0        0       67 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/reader_yolo.py
+-rw-r--r--   0        0        0     1903 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/writer_coco.py
+-rw-r--r--   0        0        0     3096 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/writer_json_lines.py
+-rw-r--r--   0        0        0      166 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/writer_pascal_voc.py
+-rw-r--r--   0        0        0     1435 2023-06-09 21:46:45.828867 bboxconverter-0.1.9/src/bboxconverter/io/writer_yolo.py
+-rw-r--r--   0        0        0     6200 1970-01-01 00:00:00.000000 bboxconverter-0.1.9/PKG-INFO
```

### Comparing `bboxconverter-0.1.8/LICENSE` & `bboxconverter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/README.md` & `bboxconverter-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bboxconverter
+<img src="https://raw.githubusercontent.com/ODAncona/bboxconverter/main/docs/_static/logo.svg" alt="bbox logo" style="display: block; margin-left:auto; margin-right:auto;"></img>
 
 <p align="center">
     <a href="https://pypi.org/project/bboxconverter">
         <img src="https://img.shields.io/pypi/v/bboxconverter?color=blue" alt="Python versions">
     </a>
     <a href="https://pepy.tech/project/bboxconverter">
         <img src="https://pepy.tech/badge/bboxconverter" alt="Total downloads">
@@ -21,36 +21,40 @@
         <img src='https://readthedocs.org/projects/bboxconverter/badge/?version=latest' alt='Documentation Status'/>
     </a>
     <a href="https://codecov.io/gh/ODAncona/bboxconverter" > 
         <img src="https://codecov.io/gh/ODAncona/bboxconverter/branch/main/graph/badge.svg?token=BXGO9JZYWM"/> 
     </a>
 </p>
 
+# bboxconverter
+
+bboxconverter is a Python library that enables seamless conversion of bounding box formats between various types and file formats. It provides an easy-to-use syntax for reading and exporting bounding box files.
 
-    
 ## Introduction
 
 ### What is a bounding box?
 
 Bounding boxes are a crucial component of object detection algorithms, which are used to identify and classify objects within an image or video. A bounding box is a rectangle that surrounds an object of interest in the image, and is typically represented by a set of coordinates that define the box's position and size.
 
+<img src="https://raw.githubusercontent.com/ODAncona/bboxconverter/main/docs/_static/bbox.png" alt="Bounding box example" style="display: block; margin-left:auto; margin-right:auto;"></img>
+
 ### Various types and format
 
 When you work with bounding box you have severals things to consider.
 
 The bounding box could be stored in **different types** like:
 
 - Top-Left Bottom-Right (TLBR), (x_min, y_min, x_max, y_max)
 - Top-Left Width Height (TLWH), (x_min, y_min, width, height)
 - Center Width Height (CWH), (x_center, y_center, width, height)
 
 Which are popular among **different formats** like :
 
-- [COCO]((http://cocodataset.org/)) (Common Objects in Context)
-- [Pascal VOC]((http://host.robots.ox.ac.uk/pascal/VOC/)) (Visual Object Classes)
+- [COCO](<(http://cocodataset.org/)>) (Common Objects in Context)
+- [Pascal VOC](<(http://host.robots.ox.ac.uk/pascal/VOC/)>) (Visual Object Classes)
 - [YOLO](https://albumentations.ai/docs/getting_started/bounding_boxes_augmentation/#yolo) (You Only Look Once)
 
 Furthermore, the bounding box could be stored in **different file formats** like:
 
 - csv
 - xml
 - json
@@ -68,15 +72,15 @@
 
 ```bash
 git clone https://github.com/ODAncona/bboxconverter.git
 cd bboxconverter
 poetry install
 ```
 
-See the [installation](./docs/guides/installation.md) guide for more informations.
+See the [installation](https://bboxconverter.readthedocs.io/en/latest/guides/installation.html) guide for more informations.
 
 ## Usage
 
 The goal of this library is to seamlessly convert bounding box format using easy syntax.
 
 It should be a breeze like...
 
@@ -110,21 +114,26 @@
 parser.export(output_path=output_path, format='yolo')
 ```
 
 ## Documentation
 
 You can find the documention online at [bboxconvert.readthedoc.io](https://bboxconverter.readthedocs.io/en/latest/index.html)
 
+## Changelog
+
+See the [CHANGELOG](https://github.com/ODAncona/bboxconverter/blob/main/CHANGELOG.md) file for details.
+
 ## Contributing
 
 Contributions are welcome! Please read the [contributing guidelines](https://github.com/ODAncona/bboxconverter/blob/main/CONTRIBUTING.md) first.
 
 ## License
 
 This project is licensed under the GPLV3 License - see the [LICENSE](https://github.com/ODAncona/bboxconverter/blob/main/LICENSE) file for details.
 
 ## Acknowledgments
 
 - [Pascal VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
 - [COCO](http://cocodataset.org/#home)
 - [YOLO](https://pjreddie.com/darknet/yolo/)
 - [Albumentation](https://albumentations.ai/)
+- [Pyodi](https://github.com/Gradiant/pyodi)
```

#### html2text {}

```diff
@@ -1,43 +1,50 @@
-# bboxconverter
+[bbox logo]
   [Python_versions] [Total_downloads] [Monthly_downloads] [Python_versions]
 [https://github.com/ODAncona/bboxconverter/actions/workflows/ci.yml/badge.svg]
  [Documentation_Status] [https://codecov.io/gh/ODAncona/bboxconverter/branch/
                     main/graph/badge.svg?token=BXGO9JZYWM]
-## Introduction ### What is a bounding box? Bounding boxes are a crucial
-component of object detection algorithms, which are used to identify and
-classify objects within an image or video. A bounding box is a rectangle that
-surrounds an object of interest in the image, and is typically represented by a
-set of coordinates that define the box's position and size. ### Various types
-and format When you work with bounding box you have severals things to
-consider. The bounding box could be stored in **different types** like: - Top-
-Left Bottom-Right (TLBR), (x_min, y_min, x_max, y_max) - Top-Left Width Height
-(TLWH), (x_min, y_min, width, height) - Center Width Height (CWH), (x_center,
-y_center, width, height) Which are popular among **different formats** like : -
-[COCO]((http://cocodataset.org/)) (Common Objects in Context) - [Pascal VOC](
-(http://host.robots.ox.ac.uk/pascal/VOC/)) (Visual Object Classes) - [YOLO]
-(https://albumentations.ai/docs/getting_started/bounding_boxes_augmentation/
-#yolo) (You Only Look Once) Furthermore, the bounding box could be stored in
-**different file formats** like: - csv - xml - json - manifest - parquet -
-pickle ## Installation ```bash pip install bboxconverter ``` or ```bash git
-clone https://github.com/ODAncona/bboxconverter.git cd bboxconverter poetry
-install ``` See the [installation](./docs/guides/installation.md) guide for
-more informations. ## Usage The goal of this library is to seamlessly convert
-bounding box format using easy syntax. It should be a breeze like... ```python
-import bboxconverter as bc # Input file path input_path = './examples/
-example.csv' # Output file path output_path = './examples/output/example.json'
-# Mapping between the input file and the bboxconverter format bbox_map = dict
-( class_name='class', file_path='name', x_min='top_left_x', y_min='top_left_y',
-width='w', height='h', image_width='img_size_x', image_height='img_size_y', ) #
-Read the input file parser = bc.read_csv(input_path, mapping=bbox_map) # Export
-the file to the desired format parser.export(output_path=output_path,
-format='coco') parser.export(output_path=output_path, format='voc')
-parser.export(output_path=output_path, format='yolo') ``` ## Documentation You
-can find the documention online at [bboxconvert.readthedoc.io](https://
-bboxconverter.readthedocs.io/en/latest/index.html) ## Contributing
+# bboxconverter bboxconverter is a Python library that enables seamless
+conversion of bounding box formats between various types and file formats. It
+provides an easy-to-use syntax for reading and exporting bounding box files. ##
+Introduction ### What is a bounding box? Bounding boxes are a crucial component
+of object detection algorithms, which are used to identify and classify objects
+within an image or video. A bounding box is a rectangle that surrounds an
+object of interest in the image, and is typically represented by a set of
+coordinates that define the box's position and size. [Bounding box example] ###
+Various types and format When you work with bounding box you have severals
+things to consider. The bounding box could be stored in **different types**
+like: - Top-Left Bottom-Right (TLBR), (x_min, y_min, x_max, y_max) - Top-Left
+Width Height (TLWH), (x_min, y_min, width, height) - Center Width Height (CWH),
+(x_center, y_center, width, height) Which are popular among **different
+formats** like : - [COCO](<(http://cocodataset.org/)>) (Common Objects in
+Context) - [Pascal VOC](<(http://host.robots.ox.ac.uk/pascal/VOC/)>) (Visual
+Object Classes) - [YOLO](https://albumentations.ai/docs/getting_started/
+bounding_boxes_augmentation/#yolo) (You Only Look Once) Furthermore, the
+bounding box could be stored in **different file formats** like: - csv - xml -
+json - manifest - parquet - pickle ## Installation ```bash pip install
+bboxconverter ``` or ```bash git clone https://github.com/ODAncona/
+bboxconverter.git cd bboxconverter poetry install ``` See the [installation]
+(https://bboxconverter.readthedocs.io/en/latest/guides/installation.html) guide
+for more informations. ## Usage The goal of this library is to seamlessly
+convert bounding box format using easy syntax. It should be a breeze like...
+```python import bboxconverter as bc # Input file path input_path = './
+examples/example.csv' # Output file path output_path = './examples/output/
+example.json' # Mapping between the input file and the bboxconverter format
+bbox_map = dict( class_name='class', file_path='name', x_min='top_left_x',
+y_min='top_left_y', width='w', height='h', image_width='img_size_x',
+image_height='img_size_y', ) # Read the input file parser = bc.read_csv
+(input_path, mapping=bbox_map) # Export the file to the desired format
+parser.export(output_path=output_path, format='coco') parser.export
+(output_path=output_path, format='voc') parser.export(output_path=output_path,
+format='yolo') ``` ## Documentation You can find the documention online at
+[bboxconvert.readthedoc.io](https://bboxconverter.readthedocs.io/en/latest/
+index.html) ## Changelog See the [CHANGELOG](https://github.com/ODAncona/
+bboxconverter/blob/main/CHANGELOG.md) file for details. ## Contributing
 Contributions are welcome! Please read the [contributing guidelines](https://
 github.com/ODAncona/bboxconverter/blob/main/CONTRIBUTING.md) first. ## License
 This project is licensed under the GPLV3 License - see the [LICENSE](https://
 github.com/ODAncona/bboxconverter/blob/main/LICENSE) file for details. ##
 Acknowledgments - [Pascal VOC](http://host.robots.ox.ac.uk/pascal/VOC/) -
 [COCO](http://cocodataset.org/#home) - [YOLO](https://pjreddie.com/darknet/
-yolo/) - [Albumentation](https://albumentations.ai/)
+yolo/) - [Albumentation](https://albumentations.ai/) - [Pyodi](https://
+github.com/Gradiant/pyodi)
```

### Comparing `bboxconverter-0.1.8/pyproject.toml` & `bboxconverter-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bboxconverter"
-version = "0.1.8"
+version = "0.1.9"
 description = "Converting bounding box annotations to popular formats like a breeze."
 readme = "README.md"
 license = "GLP-3.0"
 keywords = [
     "bbox converter",
     "bbox",
     "converter",
@@ -45,14 +45,16 @@
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.0.0"
 myst-nb = {version = "^0.17.1", python = "^3.8"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.2.0"
+scikit-image = "^0.21.0"
+
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
```

### Comparing `bboxconverter-0.1.8/src/bboxconverter/__init__.py` & `bboxconverter-0.1.9/src/bboxconverter/__init__.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/src/bboxconverter/core/bbox.py` & `bboxconverter-0.1.9/src/bboxconverter/core/bbox.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/src/bboxconverter/core/bbox_parser.py` & `bboxconverter-0.1.9/src/bboxconverter/core/bbox_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 FORMAT : list
     List of supported formats. Can be one of the following: 'voc', 'coco', 'yolo', 'jsonlines'
 
 TYPES : list
     List of supported bounding box types. Can be one of the following: 'tlbr', 'tlwh', 'cwh'
 """
 from pandas.core.frame import DataFrame
-from sklearn.model_selection import GroupShuffleSplit
+from sklearn.model_selection import GroupShuffleSplit, GroupKFold
 from bboxconverter.core.bbox import BBox, TLBR_BBox, TLWH_BBox, CWH_BBox
 from bboxconverter.io.writer_coco import to_coco
 from bboxconverter.io.writer_yolo import to_yolo
 from bboxconverter.io.writer_pascal_voc import to_pascal_voc
 from pathlib import Path
 from shutil import copy
 
-FORMAT = ['voc', 'coco', 'yolo', 'jsonlines']
-TYPES = ['tlbr', 'tlwh', 'cwh']
+FORMAT = ["voc", "coco", "yolo", "jsonlines"]
+TYPES = ["tlbr", "tlwh", "cwh"]
 
 
-class BboxParser():
+class BboxParser:
     """
     The BboxParser class is used to ingest bounding boxes from various format into a pandas dataframe and output them in various formats.
     """
 
     data: DataFrame = None
     bbox_type: str = None
 
@@ -65,186 +65,228 @@
         Parameters
         ----------
         bbox_type : str
             Type of bounding box. Can be one of the following: 'tlbr', 'tlwh', 'cwh'
         **kwargs : dict
             Dictionary of parameters for bounding box
         """
-        if bbox_type == 'tlbr':
+        if bbox_type == "tlbr":
             return TLBR_BBox(**kwargs)
-        if bbox_type == 'tlwh':
+        if bbox_type == "tlwh":
             return TLWH_BBox(**kwargs)
-        if bbox_type == 'cwh':
+        if bbox_type == "cwh":
             return CWH_BBox(**kwargs)
         return None
 
-    def create_data_splits(self,
-                           ds_path,
-                           train_size=0.8,
-                           val_size=0.1,
-                           test_size=0.1,
-                           save_func=to_coco,
-                           ) -> None:
-
+    def create_data_splits(
+        self,
+        ds_path,
+        train_size=0.8,
+        val_size=0.1,
+        test_size=0.1,
+        save_func=to_coco,
+    ) -> None:
         if train_size + val_size + test_size != 1:
-            raise ValueError(
-                'train_size + val_size + test_size must equal 1.0')
-        
-        ds_path = Path(ds_path).parent
+            raise ValueError("train_size + val_size + test_size must equal 1.0")
+
+        ds_path = Path(ds_path)
 
         # Group split
         splitter1 = GroupShuffleSplit(
             train_size=train_size + val_size,
             test_size=test_size,
             n_splits=1,
-            random_state=7
+            random_state=7,
         )
-        split = splitter1.split(self.data, groups=self.data['file_path'])
+        split = splitter1.split(self.data, groups=self.data["file_path"])
         temp_inds, test_inds = next(split)
         temp = self.data.iloc[temp_inds]
         test = self.data.iloc[test_inds]
 
         # Split temp into train and val
         splitter2 = GroupShuffleSplit(
             train_size=train_size / (train_size + val_size),
             test_size=val_size / (train_size + val_size),
             n_splits=1,
-            random_state=7
+            random_state=7,
         )
-        split = splitter2.split(temp, groups=temp['file_path'])
+        split = splitter2.split(temp, groups=temp["file_path"])
         train_inds, val_inds = next(split)
         train = temp.iloc[train_inds]
         val = temp.iloc[val_inds]
 
         # Management
         splits = dict(
-            train=dict(
-                ds=train,
-                path=ds_path / 'train',
-                output_name='train.json'
-            ),
-            val=dict(
-                ds=val,
-                path=ds_path / 'val',
-                output_name='val.json'
-            ),
-            test=dict(
-                ds=test,
-                path=ds_path / 'test',
-                output_name='test.json'
-            )
+            train=dict(ds=train, path=ds_path / "train", output_name="train.json"),
+            val=dict(ds=val, path=ds_path / "val", output_name="val.json"),
+            test=dict(ds=test, path=ds_path / "test", output_name="test.json"),
         )
 
         for split in splits.values():
             # Create directories
-            split_path = split['path']
-            img_folder = split_path / 'images'
+            split_path = split["path"]
+            img_folder = split_path / "images"
             split_path.mkdir(parents=True, exist_ok=True)
             img_folder.mkdir(parents=True, exist_ok=True)
 
             # Copy images
-            for img in split['ds']['file_path'].unique():
-                copy(
-                    ds_path / img,
-                    img_folder / Path(img).name
-                )
+            for img in split["ds"]["file_path"].unique():
+                copy(ds_path / img, img_folder / Path(img).name)
 
             # Save annotations
-            save_func(split['ds'], str(split['path'] / split['output_name']))
+            save_func(split["ds"], str(split["path"] / split["output_name"]))
+
+    def create_kfold_splits(
+        self,
+        ds_path,
+        kfold,
+        train_size=0.8,
+        test_size=0.2,
+        save_func=to_coco,
+    ) -> None:
+        """
+        Create kfold splits of the dataset and save them in the specified format
+
+        Parameters
+        ----------
+        ds_path : str | Path
+            Path to dataset
+        kfold : int
+            Number of folds
+        train_size : float
+            Size of the train split
+        test_size : float
+            Size of the test split
+        save_func : function
+            Function to convert bbox
+        """
+        ds_path = Path(ds_path)
+
+        group_kfold = GroupKFold(n_splits=kfold)
+
+        for i, (train_index, test_index) in enumerate(
+            group_kfold.split(self.data, groups=self.data["file_path"]), start=1
+        ):
+            print(f"Creating fold {i} of {kfold}")
+            # Create directories
+            split_path = ds_path / f"fold_{i}"
+            split_path.mkdir(parents=True, exist_ok=True)
+
+            # Create train and test splits
+            train = self.data.iloc[train_index]
+            test = self.data.iloc[test_index]
+
+            # Management
+            splits = dict(
+                train=dict(ds=train, path=split_path / "train", output_name="train.json"),
+                test=dict(ds=test, path=split_path / "test", output_name="test.json"),
+            )
 
-    def export(self,
-               output_path: "str | Path",
-               format: str,
-               split=False,
-               train_size=0.8,
-               test_size=0.1,
-               val_size=0.1) -> None:
+            for split in splits.values():
+                # Create directories
+                split_path = split["path"]
+                split_path.mkdir(parents=True, exist_ok=True)
+
+                # Save annotations
+                save_func(split["ds"], str(split["path"] / split["output_name"]))
+
+    def export(
+        self,
+        output_path: "str | Path",
+        format: str,
+        split=False,
+        train_size=0.8,
+        test_size=0.1,
+        val_size=0.1,
+        kfold=None,
+    ) -> None:
         """
         Export bounding boxes to a popular file format:
 
-        - "voc" => Pascal VOC 
+        - "voc" => Pascal VOC
         - "coco" => COCO
         - "yolo" => YOLO
         - "jsonlines" => Sagemaker
 
         If split is False, the output file will contain all bounding boxes. If split is True, the output file will contain the train and test split of the dataset.
 
+        If kfold is not None, the output folder will contain the kfold split of the dataset.
+
         Parameters
         ----------
         output_path : str | Path
-            Path to output file. The path should include the file name and extension.
+            Path to output folder. It will add the file name and extension automatically.
         format : str
             Format of output file. Can be one of the following: 'voc', 'coco', 'yolo', 'sagemaker'
         type : str
             Type of bounding box. Can be one of the following: 'tlbr', 'tlwh', 'cwh'
         split : bool
             Split the dataset into train and test using scikit-learn train_test_split function.
         train_size : float
             If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the test split. If int, represents the absolute number of test samples. If None, the value is set to the complement of the train size.
         test_size : float
             If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the train split. If int, represents the absolute number of train samples. If None, the value is automatically set to the complement of the test size.
+        kfold : int
+            Number of folds to split the dataset into. If None, the dataset will not be split into folds.
 
         """
+        df_bbox = self.data.copy()
+
         # Check if bounding box type is set
         type = self.bbox_type
         assert type is not None
         if type not in TYPES:
             raise ValueError(f"Invalid bbox type: {type}")
 
         # Set export to file function
-        save_func = {
-            'coco': to_coco,
-            'voc': to_pascal_voc,
-            'yolo': to_yolo
-        }.get(format, None)
+        save_func = {"coco": to_coco, "voc": to_pascal_voc, "yolo": to_yolo}.get(
+            format, None
+        )
         if save_func is None:
             raise ValueError(f"Invalid save function: {format}")
 
-        format_type = {'coco': 'tlwh', 'voc': 'tlbr', 'yolo': 'cwh'}
-
-        # Check if conversion is needed
-        if type == format_type[format]:
-            if split:
-                self.create_data_splits(output_path, train_size, test_size, val_size,
-                                        save_func)
-            else:
-                save_func(self.data, output_path)
-            return
+        format_type = {"coco": "tlwh", "voc": "tlbr", "yolo": "cwh"}
 
-        # Set conversion function
-        format_map = {
-            ('voc', 'tlwh'): TLBR_BBox.from_TLWH,
-            ('voc', 'cwh'): TLBR_BBox.from_CWH,
-            ('coco', 'tlbr'): TLWH_BBox.from_TLBR,
-            ('coco', 'cwh'): TLWH_BBox.from_CWH,
-            ('yolo', 'tlbr'): CWH_BBox.from_TLBR,
-            ('yolo', 'tlwh'): CWH_BBox.from_TLWH,
-        }
-
-        # Get conversion function
-        convert_func = format_map.get((format.lower(), self.bbox_type))
-        if convert_func is None:
-            raise ValueError(f"Invalid export format: {format}")
-
-        # Transform data to bounding boxes
-        bboxes = self.data.drop(
-            columns=['image_channel'], errors='ignore').apply(
-                lambda x: self.create_bbox(self.bbox_type, **x.to_dict()),
-                axis=1)
+        # Check if we need to convert bounding boxes
+        if type != format_type[format]:
+            # Set conversion function
+            format_map = {
+                ("voc", "tlwh"): TLBR_BBox.from_TLWH,
+                ("voc", "cwh"): TLBR_BBox.from_CWH,
+                ("coco", "tlbr"): TLWH_BBox.from_TLBR,
+                ("coco", "cwh"): TLWH_BBox.from_CWH,
+                ("yolo", "tlbr"): CWH_BBox.from_TLBR,
+                ("yolo", "tlwh"): CWH_BBox.from_TLWH,
+            }
+
+            # Get conversion function
+            convert_func = format_map.get((format.lower(), type))
+            if convert_func is None:
+                raise ValueError(f"Invalid export format: {format}")
+
+            # Transform data to bounding boxes
+            bboxes = df_bbox.drop(columns=["image_channel"], errors="ignore").apply(
+                lambda x: self.create_bbox(self.bbox_type, **x.to_dict()), axis=1
+            )
 
-        # Serialize bounding boxes
-        bboxes = bboxes.apply(lambda x: convert_func(x).to_dict())
-        df_bbox = DataFrame.from_records(bboxes)
+            # Serialize bounding boxes
+            bboxes = bboxes.apply(lambda x: convert_func(x).to_dict())
+            df_bbox = DataFrame.from_records(bboxes)
 
         # Save to file
         if split:
-            self.create_data_splits(output_path, train_size, test_size, val_size,
-                                    save_func)
+            self.create_data_splits(
+                output_path, train_size, test_size, val_size, save_func
+            )
+        if kfold:
+            self.create_kfold_splits(
+                output_path, kfold, train_size, test_size, save_func
+            )
         else:
-            save_func(df_bbox, output_path)
+            save_func(df_bbox, Path(output_path) / "annotations.json")
 
     def to_csv(self, output_path: "str | Path", type) -> None:
         """
         Export bounding boxes to a csv file.
 
         Parameters
         ----------
@@ -256,38 +298,37 @@
         assert self.bbox_type is not None
         if type not in TYPES:
             raise ValueError(f"Invalid bbox type: {type}")
 
         # Conversion function map (output_type, input_bbox_type)
         # Each type should have two functions to convert from TLBR, TLWH, CWH
         type_map = {
-            ('tlbr', 'tlwh'): TLBR_BBox.from_TLWH,
-            ('tlbr', 'cwh'): TLBR_BBox.from_CWH,
-            ('tlwh', 'tlbr'): TLWH_BBox.from_TLBR,
-            ('tlwh', 'cwh'): TLWH_BBox.from_CWH,
-            ('cwh', 'tlbr'): CWH_BBox.from_TLBR,
-            ('cwh', 'tlwh'): CWH_BBox.from_TLWH,
+            ("tlbr", "tlwh"): TLBR_BBox.from_TLWH,
+            ("tlbr", "cwh"): TLBR_BBox.from_CWH,
+            ("tlwh", "tlbr"): TLWH_BBox.from_TLBR,
+            ("tlwh", "cwh"): TLWH_BBox.from_CWH,
+            ("cwh", "tlbr"): CWH_BBox.from_TLBR,
+            ("cwh", "tlwh"): CWH_BBox.from_TLWH,
         }
 
         if type == self.bbox_type:
             # No conversion needed
             self.data.to_csv(output_path, index=False)
             return
 
         # Get conversion function
         convert_func = type_map.get((type, self.bbox_type))
 
         if convert_func is None:
             raise ValueError(f"Invalid bbox type: {type}")
 
         # Transform data to bounding boxes
-        bboxes = self.data.drop(
-            columns=['image_channel'], errors='ignore').apply(
-                lambda x: self.create_bbox(self.bbox_type, **x.to_dict()),
-                axis=1)
+        bboxes = self.data.drop(columns=["image_channel"], errors="ignore").apply(
+            lambda x: self.create_bbox(self.bbox_type, **x.to_dict()), axis=1
+        )
 
         # Serialize bounding boxes
         bboxes = bboxes.apply(lambda x: convert_func(x).to_dict())
 
         # Save to file
         DataFrame.from_records(bboxes).to_csv(output_path, index=False)
```

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/api.py` & `bboxconverter-0.1.9/src/bboxconverter/io/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module imports all the input / output functions for the bboxconverter package who could be used by the user.
+"""
 from bboxconverter.io.reader_coco import read_coco
 from bboxconverter.io.reader_csv import read_csv
 from bboxconverter.io.reader_manifest import read_manifest
 from bboxconverter.io.reader_pascal_voc import read_pascal_voc
 from bboxconverter.io.reader_xml import read_xml
 from bboxconverter.io.writer_coco import to_coco
 from bboxconverter.io.writer_pascal_voc import to_pascal_voc
```

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/reader_coco.py` & `bboxconverter-0.1.9/src/bboxconverter/io/reader_coco.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         images = {img['id']: img for img in data['images']}
         df_bbox = DataFrame(data['annotations'])
         df_bbox['class_name'] = df_bbox['category_id'].map(categories)
         df_bbox['file_path'] = df_bbox['image_id'].map(lambda x: images[x]['file_name'])
         df_bbox['image_width'] = df_bbox['image_id'].map(lambda x: images[x]['width'])
         df_bbox['image_height'] = df_bbox['image_id'].map(lambda x: images[x]['height'])
         df_bbox[['x_min','y_min','width','height']] = DataFrame(df_bbox['bbox'].tolist(), index=df_bbox.index)
-        df_bbox.drop(columns=['category_id', 'image_id','ignore','iscrowd','area','id','segmentation','bbox'], inplace=True)
+        #df_bbox.drop(columns=['category_id', 'image_id','ignore','iscrowd','area','id','bbox'], inplace=True)
+        cols_to_drop = ['category_id', 'image_id', 'ignore', 'iscrowd', 'area', 'id', 'bbox']
+        df_bbox.drop(columns=[col for col in cols_to_drop if col in df_bbox.columns], inplace=True)
+
 
     return BboxParser(df_bbox, 'tlwh')
```

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/reader_csv.py` & `bboxconverter-0.1.9/src/bboxconverter/io/reader_csv.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/reader_manifest.py` & `bboxconverter-0.1.9/src/bboxconverter/io/reader_manifest.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/reader_pascal_voc.py` & `bboxconverter-0.1.9/src/bboxconverter/io/reader_pascal_voc.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/writer_coco.py` & `bboxconverter-0.1.9/src/bboxconverter/io/writer_coco.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     cat_id = {cat['name']:cat['id'] for cat in categories}
 
     annotations = df_bbox.apply(
         lambda row: {
             'id': row.name,
             'image_id': image_id[row['file_path']],
             'category_id': cat_id[row['class_name']],
-            'segmentation': [],
+            'segmentation': row['segmentation'] if 'segmentation' in df_bbox.columns else [],
             'bbox': [row['x_min'], row['y_min'], row['width'], row['height']],
             'area': row['width'] * row['height'],
             'iscrowd': 0,
             'ignore': 0,
         },
         axis=1).tolist()
```

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/writer_json_lines.py` & `bboxconverter-0.1.9/src/bboxconverter/io/writer_json_lines.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/src/bboxconverter/io/writer_yolo.py` & `bboxconverter-0.1.9/src/bboxconverter/io/writer_yolo.py`

 * *Files identical despite different names*

### Comparing `bboxconverter-0.1.8/PKG-INFO` & `bboxconverter-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bboxconverter
-Version: 0.1.8
+Version: 0.1.9
 Summary: Converting bounding box annotations to popular formats like a breeze.
 License: GLP-3.0
 Keywords: bbox converter,bbox,converter,bounding box,annotation,coco,yolo,voc,object detection,bboxtools,bboxutils,train,test,split
 Author: Olivier D'Ancona
 Author-email: olivier_dancona@hotmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
@@ -13,27 +13,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Project-URL: documentation, https://bboxconverter.readthedocs.io/en/latest/index.html
 Project-URL: repository, https://github.com/ODAncona/bboxconverter.git
 Description-Content-Type: text/markdown
 
-# bboxconverter
+<img src="https://raw.githubusercontent.com/ODAncona/bboxconverter/main/docs/_static/logo.svg" alt="bbox logo" style="display: block; margin-left:auto; margin-right:auto;"></img>
 
 <p align="center">
     <a href="https://pypi.org/project/bboxconverter">
         <img src="https://img.shields.io/pypi/v/bboxconverter?color=blue" alt="Python versions">
     </a>
     <a href="https://pepy.tech/project/bboxconverter">
         <img src="https://pepy.tech/badge/bboxconverter" alt="Total downloads">
@@ -52,36 +48,40 @@
         <img src='https://readthedocs.org/projects/bboxconverter/badge/?version=latest' alt='Documentation Status'/>
     </a>
     <a href="https://codecov.io/gh/ODAncona/bboxconverter" > 
         <img src="https://codecov.io/gh/ODAncona/bboxconverter/branch/main/graph/badge.svg?token=BXGO9JZYWM"/> 
     </a>
 </p>
 
+# bboxconverter
+
+bboxconverter is a Python library that enables seamless conversion of bounding box formats between various types and file formats. It provides an easy-to-use syntax for reading and exporting bounding box files.
 
-    
 ## Introduction
 
 ### What is a bounding box?
 
 Bounding boxes are a crucial component of object detection algorithms, which are used to identify and classify objects within an image or video. A bounding box is a rectangle that surrounds an object of interest in the image, and is typically represented by a set of coordinates that define the box's position and size.
 
+<img src="https://raw.githubusercontent.com/ODAncona/bboxconverter/main/docs/_static/bbox.png" alt="Bounding box example" style="display: block; margin-left:auto; margin-right:auto;"></img>
+
 ### Various types and format
 
 When you work with bounding box you have severals things to consider.
 
 The bounding box could be stored in **different types** like:
 
 - Top-Left Bottom-Right (TLBR), (x_min, y_min, x_max, y_max)
 - Top-Left Width Height (TLWH), (x_min, y_min, width, height)
 - Center Width Height (CWH), (x_center, y_center, width, height)
 
 Which are popular among **different formats** like :
 
-- [COCO]((http://cocodataset.org/)) (Common Objects in Context)
-- [Pascal VOC]((http://host.robots.ox.ac.uk/pascal/VOC/)) (Visual Object Classes)
+- [COCO](<(http://cocodataset.org/)>) (Common Objects in Context)
+- [Pascal VOC](<(http://host.robots.ox.ac.uk/pascal/VOC/)>) (Visual Object Classes)
 - [YOLO](https://albumentations.ai/docs/getting_started/bounding_boxes_augmentation/#yolo) (You Only Look Once)
 
 Furthermore, the bounding box could be stored in **different file formats** like:
 
 - csv
 - xml
 - json
@@ -99,15 +99,15 @@
 
 ```bash
 git clone https://github.com/ODAncona/bboxconverter.git
 cd bboxconverter
 poetry install
 ```
 
-See the [installation](./docs/guides/installation.md) guide for more informations.
+See the [installation](https://bboxconverter.readthedocs.io/en/latest/guides/installation.html) guide for more informations.
 
 ## Usage
 
 The goal of this library is to seamlessly convert bounding box format using easy syntax.
 
 It should be a breeze like...
 
@@ -141,22 +141,27 @@
 parser.export(output_path=output_path, format='yolo')
 ```
 
 ## Documentation
 
 You can find the documention online at [bboxconvert.readthedoc.io](https://bboxconverter.readthedocs.io/en/latest/index.html)
 
+## Changelog
+
+See the [CHANGELOG](https://github.com/ODAncona/bboxconverter/blob/main/CHANGELOG.md) file for details.
+
 ## Contributing
 
 Contributions are welcome! Please read the [contributing guidelines](https://github.com/ODAncona/bboxconverter/blob/main/CONTRIBUTING.md) first.
 
 ## License
 
 This project is licensed under the GPLV3 License - see the [LICENSE](https://github.com/ODAncona/bboxconverter/blob/main/LICENSE) file for details.
 
 ## Acknowledgments
 
 - [Pascal VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
 - [COCO](http://cocodataset.org/#home)
 - [YOLO](https://pjreddie.com/darknet/yolo/)
 - [Albumentation](https://albumentations.ai/)
+- [Pyodi](https://github.com/Gradiant/pyodi)
```

#### html2text {}

```diff
@@ -1,63 +1,67 @@
-Metadata-Version: 2.1 Name: bboxconverter Version: 0.1.8 Summary: Converting
+Metadata-Version: 2.1 Name: bboxconverter Version: 0.1.9 Summary: Converting
 bounding box annotations to popular formats like a breeze. License: GLP-3.0
 Keywords: bbox converter,bbox,converter,bounding
 box,annotation,coco,yolo,voc,object
 detection,bboxtools,bboxutils,train,test,split Author: Olivier D'Ancona Author-
 email: olivier_dancona@hotmail.com Requires-Python: >=3.8 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.1,<2.0.0) Project-URL: documentation, https:
-//bboxconverter.readthedocs.io/en/latest/index.html Project-URL: repository,
-https://github.com/ODAncona/bboxconverter.git Description-Content-Type: text/
-markdown # bboxconverter
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist:
+pandas (>=1.5.2,<2.0.0) Requires-Dist: scikit-learn (>=1.2.1,<2.0.0) Project-
+URL: documentation, https://bboxconverter.readthedocs.io/en/latest/index.html
+Project-URL: repository, https://github.com/ODAncona/bboxconverter.git
+Description-Content-Type: text/markdown [bbox logo]
   [Python_versions] [Total_downloads] [Monthly_downloads] [Python_versions]
 [https://github.com/ODAncona/bboxconverter/actions/workflows/ci.yml/badge.svg]
  [Documentation_Status] [https://codecov.io/gh/ODAncona/bboxconverter/branch/
                     main/graph/badge.svg?token=BXGO9JZYWM]
-## Introduction ### What is a bounding box? Bounding boxes are a crucial
-component of object detection algorithms, which are used to identify and
-classify objects within an image or video. A bounding box is a rectangle that
-surrounds an object of interest in the image, and is typically represented by a
-set of coordinates that define the box's position and size. ### Various types
-and format When you work with bounding box you have severals things to
-consider. The bounding box could be stored in **different types** like: - Top-
-Left Bottom-Right (TLBR), (x_min, y_min, x_max, y_max) - Top-Left Width Height
-(TLWH), (x_min, y_min, width, height) - Center Width Height (CWH), (x_center,
-y_center, width, height) Which are popular among **different formats** like : -
-[COCO]((http://cocodataset.org/)) (Common Objects in Context) - [Pascal VOC](
-(http://host.robots.ox.ac.uk/pascal/VOC/)) (Visual Object Classes) - [YOLO]
-(https://albumentations.ai/docs/getting_started/bounding_boxes_augmentation/
-#yolo) (You Only Look Once) Furthermore, the bounding box could be stored in
-**different file formats** like: - csv - xml - json - manifest - parquet -
-pickle ## Installation ```bash pip install bboxconverter ``` or ```bash git
-clone https://github.com/ODAncona/bboxconverter.git cd bboxconverter poetry
-install ``` See the [installation](./docs/guides/installation.md) guide for
-more informations. ## Usage The goal of this library is to seamlessly convert
-bounding box format using easy syntax. It should be a breeze like... ```python
-import bboxconverter as bc # Input file path input_path = './examples/
-example.csv' # Output file path output_path = './examples/output/example.json'
-# Mapping between the input file and the bboxconverter format bbox_map = dict
-( class_name='class', file_path='name', x_min='top_left_x', y_min='top_left_y',
-width='w', height='h', image_width='img_size_x', image_height='img_size_y', ) #
-Read the input file parser = bc.read_csv(input_path, mapping=bbox_map) # Export
-the file to the desired format parser.export(output_path=output_path,
-format='coco') parser.export(output_path=output_path, format='voc')
-parser.export(output_path=output_path, format='yolo') ``` ## Documentation You
-can find the documention online at [bboxconvert.readthedoc.io](https://
-bboxconverter.readthedocs.io/en/latest/index.html) ## Contributing
+# bboxconverter bboxconverter is a Python library that enables seamless
+conversion of bounding box formats between various types and file formats. It
+provides an easy-to-use syntax for reading and exporting bounding box files. ##
+Introduction ### What is a bounding box? Bounding boxes are a crucial component
+of object detection algorithms, which are used to identify and classify objects
+within an image or video. A bounding box is a rectangle that surrounds an
+object of interest in the image, and is typically represented by a set of
+coordinates that define the box's position and size. [Bounding box example] ###
+Various types and format When you work with bounding box you have severals
+things to consider. The bounding box could be stored in **different types**
+like: - Top-Left Bottom-Right (TLBR), (x_min, y_min, x_max, y_max) - Top-Left
+Width Height (TLWH), (x_min, y_min, width, height) - Center Width Height (CWH),
+(x_center, y_center, width, height) Which are popular among **different
+formats** like : - [COCO](<(http://cocodataset.org/)>) (Common Objects in
+Context) - [Pascal VOC](<(http://host.robots.ox.ac.uk/pascal/VOC/)>) (Visual
+Object Classes) - [YOLO](https://albumentations.ai/docs/getting_started/
+bounding_boxes_augmentation/#yolo) (You Only Look Once) Furthermore, the
+bounding box could be stored in **different file formats** like: - csv - xml -
+json - manifest - parquet - pickle ## Installation ```bash pip install
+bboxconverter ``` or ```bash git clone https://github.com/ODAncona/
+bboxconverter.git cd bboxconverter poetry install ``` See the [installation]
+(https://bboxconverter.readthedocs.io/en/latest/guides/installation.html) guide
+for more informations. ## Usage The goal of this library is to seamlessly
+convert bounding box format using easy syntax. It should be a breeze like...
+```python import bboxconverter as bc # Input file path input_path = './
+examples/example.csv' # Output file path output_path = './examples/output/
+example.json' # Mapping between the input file and the bboxconverter format
+bbox_map = dict( class_name='class', file_path='name', x_min='top_left_x',
+y_min='top_left_y', width='w', height='h', image_width='img_size_x',
+image_height='img_size_y', ) # Read the input file parser = bc.read_csv
+(input_path, mapping=bbox_map) # Export the file to the desired format
+parser.export(output_path=output_path, format='coco') parser.export
+(output_path=output_path, format='voc') parser.export(output_path=output_path,
+format='yolo') ``` ## Documentation You can find the documention online at
+[bboxconvert.readthedoc.io](https://bboxconverter.readthedocs.io/en/latest/
+index.html) ## Changelog See the [CHANGELOG](https://github.com/ODAncona/
+bboxconverter/blob/main/CHANGELOG.md) file for details. ## Contributing
 Contributions are welcome! Please read the [contributing guidelines](https://
 github.com/ODAncona/bboxconverter/blob/main/CONTRIBUTING.md) first. ## License
 This project is licensed under the GPLV3 License - see the [LICENSE](https://
 github.com/ODAncona/bboxconverter/blob/main/LICENSE) file for details. ##
 Acknowledgments - [Pascal VOC](http://host.robots.ox.ac.uk/pascal/VOC/) -
 [COCO](http://cocodataset.org/#home) - [YOLO](https://pjreddie.com/darknet/
-yolo/) - [Albumentation](https://albumentations.ai/)
+yolo/) - [Albumentation](https://albumentations.ai/) - [Pyodi](https://
+github.com/Gradiant/pyodi)
```

