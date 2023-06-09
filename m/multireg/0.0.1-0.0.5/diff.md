# Comparing `tmp/multireg-0.0.1.tar.gz` & `tmp/multireg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multireg-0.0.1.tar", last modified: Fri Jun  9 08:18:11 2023, max compression
+gzip compressed data, was "multireg-0.0.5.tar", last modified: Fri Jun  9 09:07:46 2023, max compression
```

## Comparing `multireg-0.0.1.tar` & `multireg-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:18:11.414060 multireg-0.0.1/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.1/LICENSE
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.1/MANIFEST.in
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4464 2023-06-09 08:18:11.414060 multireg-0.0.1/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3558 2023-06-09 07:58:41.000000 multireg-0.0.1/README.md
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.1/pyproject.toml
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1216 2023-06-09 08:18:11.414060 multireg-0.0.1/setup.cfg
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.1/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:18:11.414060 multireg-0.0.1/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:18:11.414060 multireg-0.0.1/src/multireg/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    25236 2023-06-07 16:12:13.000000 multireg-0.0.1/src/multireg/MultiReg.py
--rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.1/src/multireg/Utils.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.1/src/multireg/__init__.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.1/src/multireg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:18:11.414060 multireg-0.0.1/src/multireg.egg-info/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4464 2023-06-09 08:18:11.000000 multireg-0.0.1/src/multireg.egg-info/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 08:18:11.000000 multireg-0.0.1/src/multireg.egg-info/SOURCES.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 08:18:11.000000 multireg-0.0.1/src/multireg.egg-info/dependency_links.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 08:18:11.000000 multireg-0.0.1/src/multireg.egg-info/entry_points.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       36 2023-06-09 08:18:11.000000 multireg-0.0.1/src/multireg.egg-info/requires.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 08:18:11.000000 multireg-0.0.1/src/multireg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.5/LICENSE
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.5/MANIFEST.in
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:07:46.334839 multireg-0.0.5/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3566 2023-06-09 08:56:32.000000 multireg-0.0.5/README.md
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.5/pyproject.toml
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1499 2023-06-09 09:07:46.334839 multireg-0.0.5/setup.cfg
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.5/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/src/multireg/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    25211 2023-06-09 09:06:24.000000 multireg-0.0.5/src/multireg/MultiReg.py
+-rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.5/src/multireg/Utils.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.5/src/multireg/__init__.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.5/src/multireg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/src/multireg.egg-info/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/entry_points.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       84 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/requires.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/top_level.txt
```

### Comparing `multireg-0.0.1/LICENSE` & `multireg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multireg-0.0.1/PKG-INFO` & `multireg-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.1
+Version: 0.0.5
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
+Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
+Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
+Project-URL: Source Code, https://gitlab.pasteur.fr/gletort/multireg
+Project-URL: User Support, https://gitlab.pasteur.fr/gletort/multireg/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # multireg
 
-[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://github.com/gletort/multireg/raw/main/LICENSE)
+[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/multireg.svg?color=green)](https://pypi.org/project/multireg)
 [![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
 [![codecov](https://codecov.io/gh/gletort/multireg/branch/main/graph/badge.svg)](https://codecov.io/gh/gletort/multireg)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/multireg)
 
 Registration of 3D multiplex images with one common chanel
```

### Comparing `multireg-0.0.1/README.md` & `multireg-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # multireg
 
-[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://github.com/gletort/multireg/raw/main/LICENSE)
+[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/multireg.svg?color=green)](https://pypi.org/project/multireg)
 [![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
 [![codecov](https://codecov.io/gh/gletort/multireg/branch/main/graph/badge.svg)](https://codecov.io/gh/gletort/multireg)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/multireg)
 
 Registration of 3D multiplex images with one common chanel
```

### Comparing `multireg-0.0.1/pyproject.toml` & `multireg-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multireg-0.0.1/setup.cfg` & `multireg-0.0.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 [metadata]
 name = multireg
-version = 0.0.1
+version = 0.0.5
 description = Registration of 3D multiplex images with one common chanel
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/multireg
+project_urls = 
+	Bug Tracker = https://gitlab.pasteur.fr/gletort/multireg/issues
+	Documentation = https://gitlab.pasteur.fr/gletort/mutlireg#README.md
+	Source Code = https://gitlab.pasteur.fr/gletort/multireg
+	User Support = https://gitlab.pasteur.fr/gletort/multireg/issues
 license = BSD-3-Clause
-license_files = https://gitlab.pasteur.fr/gletort/multireg/LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
@@ -27,14 +32,17 @@
 packages = find:
 install_requires = 
 	numpy
 	napari
 	magicgui
 	qtpy
 	tifffile
+	imaris_ims_file_reader
+	czifile
+	itk-registration
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `multireg-0.0.1/src/multireg/MultiReg.py` & `multireg-0.0.5/src/multireg/MultiReg.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,14 @@
         add_points(pts, labels, color, ptlayname)
         show_info("Loaded "+str(len(pts))+" points")
 
 def remove_widget(widname):
     if widname in viewer.window._dock_widgets:
         wid = viewer.window._dock_widgets[widname]
         wid.setDisabled(True)
-        wid.disconnect()
         del viewer.window._dock_widgets[widname]
         wid.destroyOnClose()
 
 def create_result_image():
     allist = glob.glob(os.path.join(aligndir, "*_C*.tif"))
     allist = [os.path.basename(ref) for ref in allist]
     reflist = glob.glob(os.path.join(aligndir, "*_C"+str(refchanel)+".tif"))
```

### Comparing `multireg-0.0.1/src/multireg/Utils.py` & `multireg-0.0.5/src/multireg/Utils.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.1/src/multireg.egg-info/PKG-INFO` & `multireg-0.0.5/src/multireg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.1
+Version: 0.0.5
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
+Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
+Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
+Project-URL: Source Code, https://gitlab.pasteur.fr/gletort/multireg
+Project-URL: User Support, https://gitlab.pasteur.fr/gletort/multireg/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # multireg
 
-[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://github.com/gletort/multireg/raw/main/LICENSE)
+[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/multireg.svg?color=green)](https://pypi.org/project/multireg)
 [![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
 [![codecov](https://codecov.io/gh/gletort/multireg/branch/main/graph/badge.svg)](https://codecov.io/gh/gletort/multireg)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/multireg)
 
 Registration of 3D multiplex images with one common chanel
```

