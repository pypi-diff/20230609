# Comparing `tmp/wkcuber-0.9.8.tar.gz` & `tmp/wkcuber-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkcuber-0.9.8.tar", max compression
+gzip compressed data, was "wkcuber-0.9.9.tar", max compression
```

## Comparing `wkcuber-0.9.8.tar` & `wkcuber-0.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    34520 2022-02-28 14:24:50.045027 wkcuber-0.9.8/LICENSE
--rw-r--r--   0        0        0     7646 2022-02-28 14:24:50.045027 wkcuber-0.9.8/README.md
--rw-r--r--   0        0        0      954 2022-02-28 14:25:06.029244 wkcuber-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      373 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/__init__.py
--rw-r--r--   0        0        0     3668 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/__main__.py
--rw-r--r--   0        0        0      221 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/__init__.py
--rw-r--r--   0        0        0      105 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/bounding_box.py
--rw-r--r--   0        0        0       99 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/dataset.py
--rw-r--r--   0        0        0       97 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/layer.py
--rw-r--r--   0        0        0      108 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/layer_categories.py
--rw-r--r--   0        0        0      100 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/mag_view.py
--rw-r--r--   0        0        0      102 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/properties.py
--rw-r--r--   0        0        0       96 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/api/view.py
--rw-r--r--   0        0        0     5332 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/check_equality.py
--rw-r--r--   0        0        0     3017 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/compress.py
--rw-r--r--   0        0        0      106 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/compress_utils.py
--rw-r--r--   0        0        0     7126 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/convert_image_stack_to_wkw.py
--rw-r--r--   0        0        0     3459 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/convert_knossos.py
--rw-r--r--   0        0        0    10505 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/convert_nifti.py
--rw-r--r--   0        0        0     6988 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/convert_raw.py
--rw-r--r--   0        0        0     6603 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/convert_zarr.py
--rw-r--r--   0        0        0    20091 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/converter.py
--rw-r--r--   0        0        0    15088 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/cubing.py
--rw-r--r--   0        0        0     5371 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/downsampling.py
--rw-r--r--   0        0        0      199 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/downsampling_utils.py
--rw-r--r--   0        0        0     4398 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/export_wkw_as_nifti.py
--rw-r--r--   0        0        0     9775 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/export_wkw_as_tiff.py
--rw-r--r--   0        0        0    32047 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/image_readers.py
--rw-r--r--   0        0        0     4305 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/knossos.py
--rw-r--r--   0        0        0       96 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/mag.py
--rw-r--r--   0        0        0    15001 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/metadata.py
--rw-r--r--   0        0        0        0 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/py.typed
--rw-r--r--   0        0        0     5328 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/recubing.py
--rw-r--r--   0        0        0    15437 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/tile_cubing.py
--rw-r--r--   0        0        0     2105 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/upload.py
--rw-r--r--   0        0        0     4524 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/upsampling.py
--rw-r--r--   0        0        0      108 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/upsampling_utils.py
--rw-r--r--   0        0        0     8367 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/utils.py
--rw-r--r--   0        0        0        0 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/vendor/__init__.py
--rw-r--r--   0        0        0    30205 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/vendor/dm3.py
--rw-r--r--   0        0        0    11172 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/vendor/dm4.py
--rw-r--r--   0        0        0       22 2022-02-28 14:25:05.561243 wkcuber-0.9.8/wkcuber/version.py
--rw-r--r--   0        0        0      711 2022-02-28 14:24:50.341027 wkcuber-0.9.8/wkcuber/versioning.py
--rw-r--r--   0        0        0     9057 2022-02-28 14:25:06.659557 wkcuber-0.9.8/setup.py
--rw-r--r--   0        0        0     8930 2022-02-28 14:25:06.660207 wkcuber-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    34520 2022-01-28 15:48:11.603553 wkcuber-0.9.9/LICENSE
+-rw-r--r--   0        0        0     7646 2022-03-02 13:46:28.700438 wkcuber-0.9.9/README.md
+-rw-r--r--   0        0        0      954 2022-03-03 15:42:02.566305 wkcuber-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      373 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/__init__.py
+-rw-r--r--   0        0        0     3668 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/__main__.py
+-rw-r--r--   0        0        0      221 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/__init__.py
+-rw-r--r--   0        0        0      105 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/bounding_box.py
+-rw-r--r--   0        0        0       99 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/dataset.py
+-rw-r--r--   0        0        0       97 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/layer.py
+-rw-r--r--   0        0        0      108 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/layer_categories.py
+-rw-r--r--   0        0        0      100 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/mag_view.py
+-rw-r--r--   0        0        0      102 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/properties.py
+-rw-r--r--   0        0        0       96 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/api/view.py
+-rw-r--r--   0        0        0     5332 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/check_equality.py
+-rw-r--r--   0        0        0     3017 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/compress.py
+-rw-r--r--   0        0        0      106 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/compress_utils.py
+-rw-r--r--   0        0        0     7126 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/convert_image_stack_to_wkw.py
+-rw-r--r--   0        0        0     3459 2022-01-28 15:48:11.863556 wkcuber-0.9.9/wkcuber/convert_knossos.py
+-rw-r--r--   0        0        0    10505 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/convert_nifti.py
+-rw-r--r--   0        0        0     6988 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/convert_raw.py
+-rw-r--r--   0        0        0     6603 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/convert_zarr.py
+-rw-r--r--   0        0        0    20091 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/converter.py
+-rw-r--r--   0        0        0    15088 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/cubing.py
+-rw-r--r--   0        0        0     5371 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/downsampling.py
+-rw-r--r--   0        0        0      199 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/downsampling_utils.py
+-rw-r--r--   0        0        0     4398 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/export_wkw_as_nifti.py
+-rw-r--r--   0        0        0     9775 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/export_wkw_as_tiff.py
+-rw-r--r--   0        0        0    32047 2022-02-01 15:06:18.729040 wkcuber-0.9.9/wkcuber/image_readers.py
+-rw-r--r--   0        0        0     4305 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/knossos.py
+-rw-r--r--   0        0        0       96 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/mag.py
+-rw-r--r--   0        0        0    15001 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/metadata.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/py.typed
+-rw-r--r--   0        0        0     5328 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/recubing.py
+-rw-r--r--   0        0        0    15437 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/tile_cubing.py
+-rw-r--r--   0        0        0     2105 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/upload.py
+-rw-r--r--   0        0        0     4524 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/upsampling.py
+-rw-r--r--   0        0        0      108 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/upsampling_utils.py
+-rw-r--r--   0        0        0     8367 2022-03-02 13:46:28.700438 wkcuber-0.9.9/wkcuber/utils.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/vendor/__init__.py
+-rw-r--r--   0        0        0    30205 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/vendor/dm3.py
+-rw-r--r--   0        0        0    11172 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/vendor/dm4.py
+-rw-r--r--   0        0        0       22 2022-03-03 15:42:01.642295 wkcuber-0.9.9/wkcuber/version.py
+-rw-r--r--   0        0        0      711 2022-01-28 15:48:11.867556 wkcuber-0.9.9/wkcuber/versioning.py
+-rw-r--r--   0        0        0     9057 2022-03-03 15:42:03.487709 wkcuber-0.9.9/setup.py
+-rw-r--r--   0        0        0     8930 2022-03-03 15:42:03.503540 wkcuber-0.9.9/PKG-INFO
```

### Comparing `wkcuber-0.9.8/LICENSE` & `wkcuber-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/README.md` & `wkcuber-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/pyproject.toml` & `wkcuber-0.9.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "wkcuber"
-version = "0.9.8"  # filled by dunamai
+version = "0.9.9"  # filled by dunamai
 description = "Python package to create, cube, and work with webKnossos WKW datasets"
 authors = ["scalable minds <hello@scalableminds.com>"]
 readme = "README.md"
 license = "AGPL-3.0"
 include = ["wkcuber/version.py"]
 
 [tool.poetry.dependencies]
 python = "^3.7,>=3.7.1"
 attrs = "^21.1.0"
 cattrs = "1.7.1"
-cluster_tools = "0.9.8"
+cluster_tools = "0.9.9"
 czifile = "^2019.7.2"
 GitPython = "^3.0.5"
 imagecodecs = "^2020.5.30"
 natsort = "^6.2.0"
 nibabel = "^2.5.1"
 numpy = "1.19.5"
 pillow = ">=6.2.1,<9.0.0"
 requests = "^2.22.0"
 scikit-image = "^0.18.3"
 scikit-learn = "^0.24.0"
 scipy = "^1.6.0"
 tifffile = "^2020.11.26"
-webknossos = "0.9.8"
+webknossos = "0.9.9"
 wkw = "1.1.11"
 zarr = "^2.10.3"
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 mypy = "^0.800"
 pylint = "^2.6.0"
```

### Comparing `wkcuber-0.9.8/wkcuber/__main__.py` & `wkcuber-0.9.9/wkcuber/__main__.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/check_equality.py` & `wkcuber-0.9.9/wkcuber/check_equality.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/compress.py` & `wkcuber-0.9.9/wkcuber/compress.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/convert_image_stack_to_wkw.py` & `wkcuber-0.9.9/wkcuber/convert_image_stack_to_wkw.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/convert_knossos.py` & `wkcuber-0.9.9/wkcuber/convert_knossos.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/convert_nifti.py` & `wkcuber-0.9.9/wkcuber/convert_nifti.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/convert_raw.py` & `wkcuber-0.9.9/wkcuber/convert_raw.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/convert_zarr.py` & `wkcuber-0.9.9/wkcuber/convert_zarr.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/converter.py` & `wkcuber-0.9.9/wkcuber/converter.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/cubing.py` & `wkcuber-0.9.9/wkcuber/cubing.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/downsampling.py` & `wkcuber-0.9.9/wkcuber/downsampling.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/export_wkw_as_nifti.py` & `wkcuber-0.9.9/wkcuber/export_wkw_as_nifti.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/export_wkw_as_tiff.py` & `wkcuber-0.9.9/wkcuber/export_wkw_as_tiff.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/image_readers.py` & `wkcuber-0.9.9/wkcuber/image_readers.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/knossos.py` & `wkcuber-0.9.9/wkcuber/knossos.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/metadata.py` & `wkcuber-0.9.9/wkcuber/metadata.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/recubing.py` & `wkcuber-0.9.9/wkcuber/recubing.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/tile_cubing.py` & `wkcuber-0.9.9/wkcuber/tile_cubing.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/upload.py` & `wkcuber-0.9.9/wkcuber/upload.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/upsampling.py` & `wkcuber-0.9.9/wkcuber/upsampling.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/utils.py` & `wkcuber-0.9.9/wkcuber/utils.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/vendor/dm3.py` & `wkcuber-0.9.9/wkcuber/vendor/dm3.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/vendor/dm4.py` & `wkcuber-0.9.9/wkcuber/vendor/dm4.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/wkcuber/versioning.py` & `wkcuber-0.9.9/wkcuber/versioning.py`

 * *Files identical despite different names*

### Comparing `wkcuber-0.9.8/setup.py` & `wkcuber-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['GitPython>=3.0.5,<4.0.0',
  'attrs>=21.1.0,<22.0.0',
  'cattrs==1.7.1',
- 'cluster_tools==0.9.8',
+ 'cluster_tools==0.9.9',
  'czifile>=2019.7.2,<2020.0.0',
  'imagecodecs>=2020.5.30,<2021.0.0',
  'natsort>=6.2.0,<7.0.0',
  'nibabel>=2.5.1,<3.0.0',
  'numpy==1.19.5',
  'pillow>=6.2.1,<9.0.0',
  'requests>=2.22.0,<3.0.0',
  'scikit-image>=0.18.3,<0.19.0',
  'scikit-learn>=0.24.0,<0.25.0',
  'scipy>=1.6.0,<2.0.0',
  'tifffile>=2020.11.26,<2021.0.0',
- 'webknossos==0.9.8',
+ 'webknossos==0.9.9',
  'wkw==1.1.11',
  'zarr>=2.10.3,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wkcuber = wkcuber.__main__:main']}
 
 setup_kwargs = {
     'name': 'wkcuber',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Python package to create, cube, and work with webKnossos WKW datasets',
     'long_description': '# webKnossos cuber (wkcuber)\n[![PyPI version](https://img.shields.io/pypi/v/wkcuber)](https://pypi.python.org/pypi/wkcuber)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/wkcuber.svg)](https://pypi.python.org/pypi/wkcuber)\n[![Build Status](https://img.shields.io/github/workflow/status/scalableminds/webknossos-libs/CI/master)](https://github.com/scalableminds/webknossos-libs/actions?query=workflow%3A%22CI%22)\n[![Documentation](https://img.shields.io/badge/docs-passing-brightgreen.svg)](https://docs.webknossos.org/wkcuber/index.html)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nPython library for creating and working with [webKnossos](https://webknossos.org) [WKW](https://github.com/scalableminds/webknossos-wrap) datasets. WKW is a container format for efficiently storing large, scale 3D image data as found in (electron) microscopy.\n\nThe tools are modular components to allow easy integration into existing pipelines and workflows.\n\n## Features\n\n* `wkcuber`: Convert supported input files to fully ready WKW datasets (includes type detection, downsampling, compressing and metadata generation)\n* `wkcuber.convert_image_stack_to_wkw`: Convert image stacks to fully ready WKW datasets (includes downsampling, compressing and metadata generation)\n* `wkcuber.export_wkw_as_tiff`: Convert WKW datasets to a tiff stack (writing as tiles to a `z/y/x.tiff` folder structure is also supported)\n* `wkcuber.cubing`: Convert image stacks (e.g., `tiff`, `jpg`, `png`, `dm3`, `dm4`) to WKW cubes\n* `wkcuber.tile_cubing`: Convert tiled image stacks (e.g. in `z/y/x.ext` folder structure) to WKW cubes\n* `wkcuber.convert_knossos`: Convert KNOSSOS cubes to WKW cubes\n* `wkcuber.convert_nifti`: Convert NIFTI files to WKW files (Currently without applying transformations).\n* `wkcuber.convert_raw`: Convert RAW binary data (.raw, .vol) files to WKW datasets\n* `wkcuber.downsampling`: Create downsampled magnifications (with `median`, `mode` and linear interpolation modes). Downsampling compresses the new magnifications by default (disable via `--no_compress`).\n* `wkcuber.compress`: Compress WKW cubes for efficient file storage (especially useful for segmentation data)\n* `wkcuber.metadata`: Create (or refresh) metadata (with guessing of most parameters)\n* `wkcuber.recubing`: Read existing WKW cubes in and write them again specifying the WKW file length. Useful when dataset was written e.g. with file length 1.\n* `wkcuber.check_equality`: Compare two WKW datasets to check whether they are equal (e.g., after compressing a dataset, this task can be useful to double-check that the compressed dataset contains the same data).\n* Most modules support multiprocessing\n\n## Supported input formats\n\n* Standard image formats, e.g. `tiff`, `jpg`, `png`, `bmp`\n* Proprietary image formats, e.g. `dm3`\n* Tiled image stacks (used for Catmaid)\n* KNOSSOS cubes\n* NIFTI files\n* Raw binary files\n\n## Installation\n### Python 3 with pip from PyPi\n- `wkcuber` requires at least Python 3.7+\n\n```\n# Make sure to have lz4 installed:\n# Mac: brew install lz4\n# Ubuntu/Debian: apt-get install liblz4-1\n# CentOS/RHEL: yum install lz4\n\npip install wkcuber\n```\n\n### Docker\nUse the CI-built image: [scalableminds/webknossos-cuber](https://hub.docker.com/r/scalableminds/webknossos-cuber/). Example usage `docker run -v <host path>:/data --rm scalableminds/webknossos-cuber wkcuber --layer_name color --scale 11.24,11.24,25 --name great_dataset /data/source/color /data/target`.\n\n\n## Usage\n\n```\n# Convert arbitrary, supported input files into wkw datasets. This sets reasonable defaults, but see other commands for customization.\npython -m wkcuber \\\n  --scale 11.24,11.24,25 \\\n  data/source data/target\n\n# Convert image stacks into wkw datasets\npython -m wkcuber.convert_image_stack_to_wkw \\\n  --layer_name color \\\n  --scale 11.24,11.24,25 \\\n  --name great_dataset \\\n  data/source/color data/target\n\n# Convert image files to wkw cubes\npython -m wkcuber.cubing --layer_name color data/source/color data/target\npython -m wkcuber.cubing --layer_name segmentation data/source/segmentation data/target\n\n# Convert tiled image files to wkw cubes\npython -m wkcuber.tile_cubing --layer_name color data/source data/target\n\n# Convert Knossos cubes to wkw cubes\npython -m wkcuber.convert_knossos --layer_name color data/source/mag1 data/target\n\n# Convert NIFTI file to wkw file\npython -m wkcuber.convert_nifti --layer_name color --scale 10,10,30 data/source/nifti_file data/target\n\n# Convert folder with NIFTI files to wkw files\npython -m wkcuber.convert_nifti --color_file one_nifti_file --segmentation_file --scale 10,10,30 another_nifti data/source/ data/target\n\n# Convert RAW file to wkw file\npython -m wkcuber.convert_raw --layer_name color --scale 10,10,30 --input_dtype uint8 --shape 2048,2048,1024 data/source/raw_file.raw data/target\n\n# Create downsampled magnifications\npython -m wkcuber.downsampling --layer_name color data/target\npython -m wkcuber.downsampling --layer_name segmentation --interpolation_mode mode data/target\n\n# Compress data in-place (mostly useful for segmentation)\npython -m wkcuber.compress --layer_name segmentation data/target\n\n# Compress data copy (mostly useful for segmentation)\npython -m wkcuber.compress --layer_name segmentation data/target data/target_compress\n\n# Create metadata\npython -m wkcuber.metadata --name great_dataset --scale 11.24,11.24,25 data/target\n\n# Refresh metadata so that new layers and/or magnifications are picked up\npython -m wkcuber.metadata --refresh data/target\n\n# Recubing an existing dataset\npython -m wkcuber.recubing --layer_name color --dtype uint8 /data/source/wkw /data/target\n\n# Check two datasets for equality\npython -m wkcuber.check_equality /data/source /data/target\n```\n\n### Parallelization\n\nMost tasks can be configured to be executed in a parallelized manner. Via `--distribution_strategy` you can pass `multiprocessing`, `slurm` or `kubernetes`. The first can be further configured with `--jobs` and the latter via `--job_resources=\'{"mem": "10M"}\'`. Use `--help` to get more information.\n\n## Development\nMake sure to install all the required dependencies using Poetry:\n```\npip install poetry\npoetry install\n```\n\nPlease, format, lint, and unit test your code changes before merging them.\n```\npoetry run black .\npoetry run pylint -j4 wkcuber\npoetry run pytest tests\n```\n\nPlease, run the extended test suite:\n```\ntests/scripts/all_tests.sh\n```\n\nPyPi releases are automatically pushed when creating a new Git tag/Github release. \n\n## API documentation\nCheck out the [latest version of the API documentation](https://docs.webknossos.org/api/wkcuber.html).\n\n### Generate the API documentation\nRun `docs/generate.sh` to open a server displaying the API docs. `docs/generate.sh --persist` persists the html to `docs/api`.\n\n## Test Data Credits\nExcerpts for testing purposes have been sampled from:\n\n* Dow Jacobo Hossain Siletti Hudspeth (2018). **Connectomics of the zebrafish\'s lateral-line neuromast reveals wiring and miswiring in a simple microcircuit.** eLife. [DOI:10.7554/eLife.33988](https://elifesciences.org/articles/33988)\n* Zheng Lauritzen Perlman Robinson Nichols Milkie Torrens Price Fisher Sharifi Calle-Schuler Kmecova Ali Karsh Trautman Bogovic Hanslovsky Jefferis Kazhdan Khairy Saalfeld Fetter Bock (2018). **A Complete Electron Microscopy Volume of the Brain of Adult Drosophila melanogaster.** Cell. [DOI:10.1016/j.cell.2018.06.019](https://www.cell.com/cell/fulltext/S0092-8674(18)30787-6). License: [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)\n\n## License\nAGPLv3\nCopyright scalable minds\n',
     'author': 'scalable minds',
     'author_email': 'hello@scalableminds.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `wkcuber-0.9.8/PKG-INFO` & `wkcuber-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: wkcuber
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python package to create, cube, and work with webKnossos WKW datasets
 License: AGPL-3.0
 Author: scalable minds
 Author-email: hello@scalableminds.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: GitPython (>=3.0.5,<4.0.0)
 Requires-Dist: attrs (>=21.1.0,<22.0.0)
 Requires-Dist: cattrs (==1.7.1)
-Requires-Dist: cluster_tools (==0.9.8)
+Requires-Dist: cluster_tools (==0.9.9)
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
 Requires-Dist: imagecodecs (>=2020.5.30,<2021.0.0)
 Requires-Dist: natsort (>=6.2.0,<7.0.0)
 Requires-Dist: nibabel (>=2.5.1,<3.0.0)
 Requires-Dist: numpy (==1.19.5)
 Requires-Dist: pillow (>=6.2.1,<9.0.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Requires-Dist: scikit-image (>=0.18.3,<0.19.0)
 Requires-Dist: scikit-learn (>=0.24.0,<0.25.0)
 Requires-Dist: scipy (>=1.6.0,<2.0.0)
 Requires-Dist: tifffile (>=2020.11.26,<2021.0.0)
-Requires-Dist: webknossos (==0.9.8)
+Requires-Dist: webknossos (==0.9.9)
 Requires-Dist: wkw (==1.1.11)
 Requires-Dist: zarr (>=2.10.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # webKnossos cuber (wkcuber)
 [![PyPI version](https://img.shields.io/pypi/v/wkcuber)](https://pypi.python.org/pypi/wkcuber)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/wkcuber.svg)](https://pypi.python.org/pypi/wkcuber)
```

