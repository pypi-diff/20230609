# Comparing `tmp/multireg-0.0.2.tar.gz` & `tmp/multireg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multireg-0.0.2.tar", last modified: Fri Jun  9 08:48:50 2023, max compression
+gzip compressed data, was "multireg-0.0.3.tar", last modified: Fri Jun  9 08:59:32 2023, max compression
```

## Comparing `multireg-0.0.2.tar` & `multireg-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:48:50.880880 multireg-0.0.2/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.2/LICENSE
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.2/MANIFEST.in
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4796 2023-06-09 08:48:50.880880 multireg-0.0.2/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3565 2023-06-09 08:48:03.000000 multireg-0.0.2/README.md
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.2/pyproject.toml
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1448 2023-06-09 08:48:50.880880 multireg-0.0.2/setup.cfg
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.2/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:48:50.880880 multireg-0.0.2/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:48:50.880880 multireg-0.0.2/src/multireg/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    25236 2023-06-07 16:12:13.000000 multireg-0.0.2/src/multireg/MultiReg.py
--rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.2/src/multireg/Utils.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.2/src/multireg/__init__.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.2/src/multireg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:48:50.880880 multireg-0.0.2/src/multireg.egg-info/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4796 2023-06-09 08:48:50.000000 multireg-0.0.2/src/multireg.egg-info/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 08:48:50.000000 multireg-0.0.2/src/multireg.egg-info/SOURCES.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 08:48:50.000000 multireg-0.0.2/src/multireg.egg-info/dependency_links.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 08:48:50.000000 multireg-0.0.2/src/multireg.egg-info/entry_points.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       36 2023-06-09 08:48:50.000000 multireg-0.0.2/src/multireg.egg-info/requires.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 08:48:50.000000 multireg-0.0.2/src/multireg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:59:32.301865 multireg-0.0.3/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.3/LICENSE
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.3/MANIFEST.in
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 08:59:32.301865 multireg-0.0.3/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3566 2023-06-09 08:56:32.000000 multireg-0.0.3/README.md
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.3/pyproject.toml
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1466 2023-06-09 08:59:32.301865 multireg-0.0.3/setup.cfg
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.3/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:59:32.301865 multireg-0.0.3/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:59:32.301865 multireg-0.0.3/src/multireg/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    25236 2023-06-07 16:12:13.000000 multireg-0.0.3/src/multireg/MultiReg.py
+-rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.3/src/multireg/Utils.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.3/src/multireg/__init__.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.3/src/multireg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 08:59:32.301865 multireg-0.0.3/src/multireg.egg-info/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 08:59:32.000000 multireg-0.0.3/src/multireg.egg-info/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 08:59:32.000000 multireg-0.0.3/src/multireg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 08:59:32.000000 multireg-0.0.3/src/multireg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 08:59:32.000000 multireg-0.0.3/src/multireg.egg-info/entry_points.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       53 2023-06-09 08:59:32.000000 multireg-0.0.3/src/multireg.egg-info/requires.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 08:59:32.000000 multireg-0.0.3/src/multireg.egg-info/top_level.txt
```

### Comparing `multireg-0.0.2/LICENSE` & `multireg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multireg-0.0.2/PKG-INFO` & `multireg-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multireg
 
-[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/raw/main/LICENSE)
+[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/multireg.svg?color=green)](https://pypi.org/project/multireg)
 [![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
 [![codecov](https://codecov.io/gh/gletort/multireg/branch/main/graph/badge.svg)](https://codecov.io/gh/gletort/multireg)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/multireg)
 
 Registration of 3D multiplex images with one common chanel
```

### Comparing `multireg-0.0.2/README.md` & `multireg-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # multireg
 
-[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/raw/main/LICENSE)
+[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/multireg.svg?color=green)](https://pypi.org/project/multireg)
 [![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
 [![codecov](https://codecov.io/gh/gletort/multireg/branch/main/graph/badge.svg)](https://codecov.io/gh/gletort/multireg)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/multireg)
 
 Registration of 3D multiplex images with one common chanel
```

### Comparing `multireg-0.0.2/pyproject.toml` & `multireg-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multireg-0.0.2/setup.cfg` & `multireg-0.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multireg
-version = 0.0.2
+version = 0.0.3
 description = Registration of 3D multiplex images with one common chanel
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/multireg
 project_urls = 
@@ -32,14 +32,15 @@
 packages = find:
 install_requires = 
 	numpy
 	napari
 	magicgui
 	qtpy
 	tifffile
+	itk-registration
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `multireg-0.0.2/src/multireg/MultiReg.py` & `multireg-0.0.3/src/multireg/MultiReg.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.2/src/multireg/Utils.py` & `multireg-0.0.3/src/multireg/Utils.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.2/src/multireg.egg-info/PKG-INFO` & `multireg-0.0.3/src/multireg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multireg
 
-[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/raw/main/LICENSE)
+[![License BSD-3](https://img.shields.io/pypi/l/multireg.svg?color=green)](https://gitlab.pasteur.fr/gletort/multireg/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/multireg.svg?color=green)](https://pypi.org/project/multireg)
 [![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
 [![codecov](https://codecov.io/gh/gletort/multireg/branch/main/graph/badge.svg)](https://codecov.io/gh/gletort/multireg)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/multireg)
 
 Registration of 3D multiplex images with one common chanel
```

