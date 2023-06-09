# Comparing `tmp/artus-0.2.0.tar.gz` & `tmp/artus-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artus-0.2.0.tar", last modified: Wed Jun  7 12:13:28 2023, max compression
+gzip compressed data, was "artus-0.2.1.tar", last modified: Fri Jun  9 11:49:39 2023, max compression
```

## Comparing `artus-0.2.0.tar` & `artus-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.291770 artus-0.2.0/
--rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 12:13:28.291770 artus-0.2.0/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)     2427 2023-06-07 10:43:24.000000 artus-0.2.0/README.md
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.2.0/artus/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/evaluate_model/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/evaluate_model/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.2.0/artus/evaluate_model/coco_stats.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.2.0/artus/evaluate_model/evaluate.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.2.0/artus/evaluate_model/write_eval_results.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/inference/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/inference/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.2.0/artus/inference/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.2.0/artus/inference/deploy_unlabeled_dataset.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.2.0/artus/inference/predict.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/prepare/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/prepare/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.2.0/artus/prepare/coco_splitting.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.2.0/artus/prepare/crs_settings.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.2.0/artus/prepare/tile.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.2.0/artus/prepare/transform_geoson_to_coco.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.291770 artus-0.2.0/artus/spatialize/
--rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.2.0/artus/spatialize/GeoCOCOExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.2.0/artus/spatialize/GeoFiftyoneExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.2.0/artus/spatialize/LocationImporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/spatialize/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.291770 artus-0.2.0/artus/train/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/train/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.2.0/artus/train/build_trainer.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.2.0/artus/train/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.2.0/artus/train/data_augmentation.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.2.0/artus/train/train.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.2.0/artus/train/validation_hook.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus.egg-info/
--rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)      909 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/SOURCES.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/dependency_links.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/requires.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/top_level.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)     1331 2023-06-07 12:06:56.000000 artus-0.2.0/pyproject.toml
--rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 12:13:28.291770 artus-0.2.0/setup.cfg
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/
+-rw-rw-r--   0 justine   (1000) justine   (1000)    11357 2023-06-08 12:27:48.000000 artus-0.2.1/LICENSE
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-09 11:49:39.847981 artus-0.2.1/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2514 2023-06-08 12:28:48.000000 artus-0.2.1/README.md
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.2.1/artus/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/evaluate_model/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/evaluate_model/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.2.1/artus/evaluate_model/coco_stats.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.2.1/artus/evaluate_model/evaluate.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-09 07:01:26.000000 artus-0.2.1/artus/evaluate_model/write_eval_results.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/inference/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/inference/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.2.1/artus/inference/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.2.1/artus/inference/deploy_unlabeled_dataset.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.2.1/artus/inference/predict.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/prepare/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/prepare/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.2.1/artus/prepare/coco_splitting.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.2.1/artus/prepare/crs_settings.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.2.1/artus/prepare/tile.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.2.1/artus/prepare/transform_geojson_to_coco.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/spatialize/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.2.1/artus/spatialize/GeoCOCOExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.2.1/artus/spatialize/GeoFiftyoneExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.2.1/artus/spatialize/LocationImporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/spatialize/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/train/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/train/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.2.1/artus/train/build_trainer.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.2.1/artus/train/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.2.1/artus/train/data_augmentation.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.2.1/artus/train/train.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.2.1/artus/train/validation_hook.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus.egg-info/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)      918 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/SOURCES.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/dependency_links.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)      426 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/requires.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/top_level.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1356 2023-06-09 11:49:12.000000 artus-0.2.1/pyproject.toml
+-rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-09 11:49:39.847981 artus-0.2.1/setup.cfg
```

### Comparing `artus-0.2.0/PKG-INFO` & `artus-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.2.0
+Version: 0.2.1
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
 
 <img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
-</div>
-
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
+[![PyPI version](https://badge.fury.io/py/artus.svg)](https://badge.fury.io/py/artus)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7852855.svg)](https://doi.org/10.5281/zenodo.7852855)
 
+</div>
+
+
 Artus is a python package to automatically produce maps thanks to deep learning models. With artus, you can train deep learning learning models (neural network)
 on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported to a GeoJson format and uploaded in your favourite GIS software.
 
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
```

### Comparing `artus-0.2.0/README.md` & `artus-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 <div align="center">
 
 <img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
-</div>
-
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
+[![PyPI version](https://badge.fury.io/py/artus.svg)](https://badge.fury.io/py/artus)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7852855.svg)](https://doi.org/10.5281/zenodo.7852855)
 
+</div>
+
+
 Artus is a python package to automatically produce maps thanks to deep learning models. With artus, you can train deep learning learning models (neural network)
 on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported to a GeoJson format and uploaded in your favourite GIS software.
 
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
```

### Comparing `artus-0.2.0/artus/evaluate_model/coco_stats.py` & `artus-0.2.1/artus/evaluate_model/coco_stats.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/evaluate_model/evaluate.py` & `artus-0.2.1/artus/evaluate_model/evaluate.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/evaluate_model/write_eval_results.py` & `artus-0.2.1/artus/evaluate_model/write_eval_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         Returns:
             A plotly interactive barplot that can be seen with Python(fig.show())
         """
         metrics = self.process_csv()
 
         fig = px.bar(metrics, x="model", y="Average precision", color="model", barmode="relative",
              facet_col="variable", facet_col_wrap=5, facet_row_spacing=0.04, facet_col_spacing=0.04,
-             height=2000, width = 1500, title= self.title)
+             height=1500, width = 1500, title= self.title)
         
         fig.for_each_annotation(lambda a: a.update(text=a.text.split("=")[-1]))
 
         return fig
 
     def export_plots(self):
         """Export the plots in html format. Plots are interactives."""
```

### Comparing `artus-0.2.0/artus/inference/config.py` & `artus-0.2.1/artus/inference/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/inference/deploy_unlabeled_dataset.py` & `artus-0.2.1/artus/inference/deploy_unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/inference/predict.py` & `artus-0.2.1/artus/inference/predict.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/prepare/coco_splitting.py` & `artus-0.2.1/artus/prepare/coco_splitting.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/prepare/crs_settings.py` & `artus-0.2.1/artus/prepare/crs_settings.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/prepare/tile.py` & `artus-0.2.1/artus/prepare/tile.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/prepare/transform_geoson_to_coco.py` & `artus-0.2.1/artus/prepare/transform_geojson_to_coco.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/spatialize/GeoCOCOExporter.py` & `artus-0.2.1/artus/spatialize/GeoCOCOExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/spatialize/GeoFiftyoneExporter.py` & `artus-0.2.1/artus/spatialize/GeoFiftyoneExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/spatialize/LocationImporter.py` & `artus-0.2.1/artus/spatialize/LocationImporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/train/build_trainer.py` & `artus-0.2.1/artus/train/build_trainer.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/train/config.py` & `artus-0.2.1/artus/train/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/train/data_augmentation.py` & `artus-0.2.1/artus/train/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/train/train.py` & `artus-0.2.1/artus/train/train.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus/train/validation_hook.py` & `artus-0.2.1/artus/train/validation_hook.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.0/artus.egg-info/PKG-INFO` & `artus-0.2.1/artus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.2.0
+Version: 0.2.1
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
 
 <img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
-</div>
-
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
+[![PyPI version](https://badge.fury.io/py/artus.svg)](https://badge.fury.io/py/artus)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7852855.svg)](https://doi.org/10.5281/zenodo.7852855)
 
+</div>
+
+
 Artus is a python package to automatically produce maps thanks to deep learning models. With artus, you can train deep learning learning models (neural network)
 on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported to a GeoJson format and uploaded in your favourite GIS software.
 
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
```

### Comparing `artus-0.2.0/artus.egg-info/SOURCES.txt` & `artus-0.2.1/artus.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 artus/__init__.py
 artus.egg-info/PKG-INFO
 artus.egg-info/SOURCES.txt
 artus.egg-info/dependency_links.txt
 artus.egg-info/requires.txt
@@ -14,15 +15,15 @@
 artus/inference/config.py
 artus/inference/deploy_unlabeled_dataset.py
 artus/inference/predict.py
 artus/prepare/__init__.py
 artus/prepare/coco_splitting.py
 artus/prepare/crs_settings.py
 artus/prepare/tile.py
-artus/prepare/transform_geoson_to_coco.py
+artus/prepare/transform_geojson_to_coco.py
 artus/spatialize/GeoCOCOExporter.py
 artus/spatialize/GeoFiftyoneExporter.py
 artus/spatialize/LocationImporter.py
 artus/spatialize/__init__.py
 artus/train/__init__.py
 artus/train/build_trainer.py
 artus/train/config.py
```

### Comparing `artus-0.2.0/pyproject.toml` & `artus-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "artus"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Justine Talpaert Daudon", email="justine.daudon@protonmail.com" },
 ]
 description = "A geoAI package to train and predict spatial occurences on rasters or georeferenced images."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,14 +16,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "fiftyone>=0.19.1",
     "torch>=1.12.1",
     "torchmetrics>=0.9.3",
     "torchvision>=0.13.1",
+    "geopandas>=0.13.0",
     "Fiona==1.8.22",
     "importlib-metadata==6.1.0",
     "importlib-resources==5.7.1",
     "joblib==1.2.0",
     "matplotlib>=3.5.0",
     "numpy>=1.18.1",
     "opencv-python>4.6.0",
```

