# Comparing `tmp/snkit-1.7.2.tar.gz` & `tmp/snkit-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snkit-1.7.2.tar", last modified: Fri Oct 14 15:03:21 2022, max compression
+gzip compressed data, was "snkit-1.8.0.tar", last modified: Fri Jun  9 16:23:47 2023, max compression
```

## Comparing `snkit-1.7.2.tar` & `snkit-1.8.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.525318 snkit-1.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.525318 snkit-1.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-10-14 15:03:11.000000 snkit-1.7.2/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-10-14 15:03:11.000000 snkit-1.7.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-14 15:03:11.000000 snkit-1.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-14 15:03:11.000000 snkit-1.7.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-10-14 15:03:11.000000 snkit-1.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-10-14 15:03:11.000000 snkit-1.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-14 15:03:11.000000 snkit-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-10-14 15:03:21.529318 snkit-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3914 2022-10-14 15:03:11.000000 snkit-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-14 15:03:11.000000 snkit-1.7.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.525318 snkit-1.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     7582 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/_static/connected-network.png
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/_static/theme_tweaks.css
--rw-r--r--   0 runner    (1001) docker     (121)     7315 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/_static/unconnected-network.png
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-14 15:03:11.000000 snkit-1.7.2/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-14 15:03:11.000000 snkit-1.7.2/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)     4060 2022-10-14 15:03:11.000000 snkit-1.7.2/notebooks/small-demo.geojson
--rw-r--r--   0 runner    (1001) docker     (121)    65220 2022-10-14 15:03:11.000000 snkit-1.7.2/notebooks/snkit-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-14 15:03:11.000000 snkit-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 15:03:21.529318 snkit-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-10-14 15:03:11.000000 snkit-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.525318 snkit-1.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/src/snkit/
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-14 15:03:11.000000 snkit-1.7.2/src/snkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28484 2022-10-14 15:03:11.000000 snkit-1.7.2/src/snkit/network.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-14 15:03:11.000000 snkit-1.7.2/src/snkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/src/snkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-10-14 15:03:21.000000 snkit-1.7.2/src/snkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-10-14 15:03:21.000000 snkit-1.7.2/src/snkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 15:03:21.000000 snkit-1.7.2/src/snkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 15:03:21.000000 snkit-1.7.2/src/snkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-14 15:03:21.000000 snkit-1.7.2/src/snkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-14 15:03:21.000000 snkit-1.7.2/src/snkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:03:21.529318 snkit-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    20950 2022-10-14 15:03:11.000000 snkit-1.7.2/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.086167 snkit-1.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.074167 snkit-1.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.078167 snkit-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-09 16:23:35.000000 snkit-1.8.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 16:23:35.000000 snkit-1.8.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 16:23:35.000000 snkit-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-09 16:23:35.000000 snkit-1.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-09 16:23:35.000000 snkit-1.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 16:23:35.000000 snkit-1.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 16:23:35.000000 snkit-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-09 16:23:47.086167 snkit-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-09 16:23:35.000000 snkit-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 16:23:35.000000 snkit-1.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.082167 snkit-1.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.082167 snkit-1.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.082167 snkit-1.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/_static/connected-network.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/_static/theme_tweaks.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/_static/unconnected-network.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 16:23:35.000000 snkit-1.8.0/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-09 16:23:35.000000 snkit-1.8.0/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.082167 snkit-1.8.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-09 16:23:35.000000 snkit-1.8.0/notebooks/small-demo.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    65220 2023-06-09 16:23:35.000000 snkit-1.8.0/notebooks/snkit-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 16:23:35.000000 snkit-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:23:47.086167 snkit-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-09 16:23:35.000000 snkit-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.074167 snkit-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.086167 snkit-1.8.0/src/snkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-09 16:23:35.000000 snkit-1.8.0/src/snkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31540 2023-06-09 16:23:35.000000 snkit-1.8.0/src/snkit/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 16:23:35.000000 snkit-1.8.0/src/snkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.086167 snkit-1.8.0/src/snkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-09 16:23:47.000000 snkit-1.8.0/src/snkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-09 16:23:47.000000 snkit-1.8.0/src/snkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:23:47.000000 snkit-1.8.0/src/snkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:23:47.000000 snkit-1.8.0/src/snkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 16:23:47.000000 snkit-1.8.0/src/snkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 16:23:47.000000 snkit-1.8.0/src/snkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:23:47.086167 snkit-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-06-09 16:23:35.000000 snkit-1.8.0/tests/test_init.py
```

### Comparing `snkit-1.7.2/.github/workflows/package.yml` & `snkit-1.8.0/.github/workflows/package.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 name: package
 
 on:
   release:
     types: [published]
 
 jobs:
-  build_sdist:
-    name: Build SDist
+  build:
+    name: Build
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
 
-      - name: Build SDist
-        run: pipx run build --sdist
+      - name: Build SDist and wheel
+        run: pipx run build
 
       - name: Check metadata
         run: pipx run twine check dist/*
 
       - uses: actions/upload-artifact@v2
         with:
-          path: dist/*.tar.gz
+          path: dist/*
 
   upload_all:
     name: Upload if release
-    needs: [build_sdist]
+    needs: [build]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/setup-python@v2
 
       - uses: actions/download-artifact@v2
```

### Comparing `snkit-1.7.2/.github/workflows/test.yml` & `snkit-1.8.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push]
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.8", "3.11"]
 
     runs-on:  ubuntu-latest
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
```

### Comparing `snkit-1.7.2/CODE_OF_CONDUCT.md` & `snkit-1.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/CONTRIBUTING.md` & `snkit-1.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/LICENSE` & `snkit-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/PKG-INFO` & `snkit-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snkit
-Version: 1.7.2
+Version: 1.8.0
 Summary: a spatial networks toolkit
 Home-page: https://github.com/tomalrussell/snkit
 Author: Tom Russell
 Author-email: tomalrussell@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `snkit-1.7.2/README.md` & `snkit-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/docs/Makefile` & `snkit-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/docs/make.bat` & `snkit-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/docs/source/_static/connected-network.png` & `snkit-1.8.0/docs/source/_static/connected-network.png`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/docs/source/_static/unconnected-network.png` & `snkit-1.8.0/docs/source/_static/unconnected-network.png`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/docs/source/conf.py` & `snkit-1.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/docs/source/index.rst` & `snkit-1.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/notebooks/small-demo.geojson` & `snkit-1.8.0/notebooks/small-demo.geojson`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/notebooks/snkit-demo.ipynb` & `snkit-1.8.0/notebooks/snkit-demo.ipynb`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/setup.py` & `snkit-1.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,23 +42,23 @@
     ],
     keywords=[
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
     setup_requires=["setuptools_scm"],
     install_requires=[
         # eg: 'aspectlib==1.1.1', 'six>=1.7',
-        "geopandas>=0.10",
-        "pygeos>=0.12",
+        "geopandas>=0.13",
+        "shapely>=2.0",
     ],
     extras_require={
         "dev": ["black", "nbstripout", "pytest", "pytest-cov"],
         # eg:
         #   'rst': ['docutils>=0.11'],
         #   ':python_version=="2.6"': ['argparse'],
-        "networkx": ["networkx>=1.9"],
+        "networkx": ["networkx>=3.0"],
     },
     entry_points={
         "console_scripts": [
             # eg: 'snkit = snkit.cli:main',
         ]
     },
 )
```

### Comparing `snkit-1.7.2/src/snkit/__init__.py` & `snkit-1.8.0/src/snkit/__init__.py`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/src/snkit/network.py` & `snkit-1.8.0/src/snkit/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Network representation and utilities
 """
 import os
 import warnings
 
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-    import geopandas
-
+import geopandas
 import numpy as np
 import pandas
 import shapely.errors
 
 try:
     import networkx as nx
 
@@ -36,14 +33,21 @@
     try:
         from tqdm import tqdm
     except ImportError:
         from snkit.utils import tqdm_standin as tqdm
 else:
     from snkit.utils import tqdm_standin as tqdm
 
+# optional parallel processing
+if "SNKIT_PARALLEL" in os.environ and os.environ["SNKIT_PARALLEL"] in ("1", "TRUE"):
+    PARALLEL = True
+    import multiprocessing
+else:
+    PARALLEL = False
+
 
 class Network:
     """A Network is composed of nodes (points in space) and edges (lines)
 
     Parameters
     ----------
     nodes : geopandas.geodataframe.GeoDataFrame, optional
@@ -55,60 +59,101 @@
     edges : geopandas.geodataframe.GeoDataFrame
 
     """
 
     def __init__(self, nodes=None, edges=None):
         """ """
         if nodes is None:
-            nodes = GeoDataFrame()
+            nodes = GeoDataFrame(geometry=[])
         self.nodes = nodes
 
         if edges is None:
-            edges = GeoDataFrame()
+            edges = GeoDataFrame(geometry=[])
         self.edges = edges
 
-    def set_crs(self, crs=None, epsg=None):
-        """Set network (node and edge) crs
+    def set_crs(self, crs=None, epsg=None, allow_override=False):
+        """Set the coordinate reference system (CRS) of the network nodes and
+        edges.
 
         Parameters
         ----------
-        crs : dict or str
-            Projection parameters as PROJ4 string or in dictionary form.
-        epsg : int
-            EPSG code specifying output projection
+        crs : pyproj.CRS, optional if epsg is specified
+            The value can be anything accepted by pyproj.CRS.from_user_input(),
+            such as an authority string (eg “EPSG:4326”) or a WKT string.
+        epsg : int, optional if crs is specified
+            EPSG code specifying output projection.
+        allow_override : bool, default False
+            If the nodes or edges GeoDataFrame already has a CRS, allow to
+            replace the existing CRS, even when both are not equal.
 
         """
-        if crs is None and epsg is None:
-            raise ValueError("Either crs or epsg must be provided to Network.set_crs")
-
-        if epsg is not None:
-            crs = {"init": "epsg:{}".format(epsg)}
-
-        self.edges.crs = crs
-        self.nodes.crs = crs
+        inplace = True
+        self.edges.set_crs(crs, epsg, inplace, allow_override)
+        self.nodes.set_crs(crs, epsg, inplace, allow_override)
 
     def to_crs(self, crs=None, epsg=None):
-        """Set network (node and edge) crs
+        """Transform network nodes and edges geometries to a new coordinate
+        reference system (CRS).
 
         Parameters
         ----------
-        crs : dict or str
-            Projection parameters as PROJ4 string or in dictionary form.
-        epsg : int
-            EPSG code specifying output projection
+        crs : pyproj.CRS, optional if epsg is specified
+            The value can be anything accepted by pyproj.CRS.from_user_input(),
+            such as an authority string (eg “EPSG:4326”) or a WKT string.
+        epsg : int, optional if crs is specified
+            EPSG code specifying output projection.
 
         """
-        if crs is None and epsg is None:
-            raise ValueError("Either crs or epsg must be provided to Network.set_crs")
+        inplace = True
+        self.edges.to_crs(crs, epsg, inplace)
+        self.nodes.to_crs(crs, epsg, inplace)
 
-        if epsg is not None:
-            crs = {"init": "epsg:{}".format(epsg)}
+    def to_file(self, filename, nodes_layer="nodes", edges_layer="edges", **kwargs):
+        """Write nodes and edges to a geographic data file with layers.
 
-        self.edges.to_crs(crs, inplace=True)
-        self.nodes.to_crs(crs, inplace=True)
+        Any additional keyword arguments are passed through to `geopandas.GeoDataFrame.to_file`.
+
+        Parameters
+        ----------
+        filename : str
+            Path to geographic data file with layers
+        nodes_layer : str, optional, default 'nodes'
+            Layer name for nodes.
+        edges_layer : str, optional, default 'edges'
+            Layer name for edges.
+        """
+        self.nodes.to_file(filename, layer=nodes_layer, **kwargs)
+        self.edges.to_file(filename, layer=edges_layer, **kwargs)
+
+
+def read_file(filename, nodes_layer="nodes", edges_layer="edges", **kwargs):
+    """Read a geographic data file with layers containing nodes and edges.
+
+    Any additional keyword arguments are passed through to `geopandas.read_file`.
+
+    Parameters
+    ----------
+    filename : str
+        Path to geographic data file with layers
+    nodes_layer : str, optional, default 'nodes'
+        Layer name for nodes, or None if nodes should not be read.
+    edges_layer : str, optional, default 'edges'
+        Layer name for edges, or None if edges should not be read.
+    """
+    if nodes_layer is not None:
+        nodes = geopandas.read_file(filename, layer=nodes_layer, **kwargs)
+    else:
+        nodes = None
+
+    if edges_layer is not None:
+        edges = geopandas.read_file(filename, layer=edges_layer, **kwargs)
+    else:
+        edges = None
+
+    return Network(nodes, edges)
 
 
 def add_ids(network, id_col="id", edge_prefix="edge", node_prefix="node"):
     """Add or replace an id column with ascending ids"""
     nodes = network.nodes.copy()
     if not nodes.empty:
         nodes = nodes.reset_index(drop=True)
@@ -150,15 +195,15 @@
     """Get nodes for each edge endpoint"""
     endpoints = []
     for edge in tqdm(
         network.edges.itertuples(), desc="endpoints", total=len(network.edges)
     ):
         if edge.geometry is None:
             continue
-        if edge.geometry.geometryType() == "MultiLineString":
+        if edge.geometry.geom_type == "MultiLineString":
             for line in edge.geometry.geoms:
                 start, end = line_endpoints(line)
                 endpoints.append(start)
                 endpoints.append(end)
         else:
             start, end = line_endpoints(edge.geometry)
             endpoints.append(start)
@@ -196,15 +241,15 @@
     """
 
     edges = network.edges
     geom_col: str = geometry_column_name(edges)
     split_edges = edges.explode(column=geom_col, ignore_index=True)
 
     geo_types = set(split_edges.geom_type)
-    if geo_types != {'LineString'}:
+    if geo_types != {"LineString"}:
         raise ValueError(
             f"exploded edges are of type(s) {geo_types} but should only be LineString"
         )
 
     return Network(nodes=network.nodes, edges=split_edges)
 
 
@@ -244,33 +289,57 @@
         pandas.concat(
             [
                 network.nodes.drop(geom_col, axis=1),
                 GeoDataFrame(snapped_geoms, columns=[geom_col]),
             ],
             axis=1,
         ),
-        crs=network.nodes.crs
+        crs=network.nodes.crs,
     )
 
     return Network(nodes=nodes, edges=network.edges)
 
 
-def split_edges_at_nodes(network, tolerance=1e-9):
-    """Split network edges where they intersect node geometries"""
+def _split_edges_at_nodes(
+    edges: GeoDataFrame, nodes: GeoDataFrame, tolerance: float
+) -> list:
+    """Split edges at nodes for a network chunk"""
     split_edges = []
-    for edge in tqdm(
-        network.edges.itertuples(index=False), desc="split", total=len(network.edges)
-    ):
-        hits = nodes_intersecting(edge.geometry, network.nodes, tolerance)
+
+    for edge in edges.itertuples(index=False):
+        hits = nodes_intersecting(edge.geometry, nodes, tolerance)
         split_points = MultiPoint([hit.geometry for hit in hits.itertuples()])
 
         # potentially split to multiple edges
         edges = split_edge_at_points(edge, split_points, tolerance)
         split_edges.append(edges)
 
+    return split_edges
+
+
+def split_edges_at_nodes(network, tolerance=1e-9):
+    """Split network edges where they intersect node geometries"""
+    split_edges = []
+
+    n = len(network.edges)
+    if PARALLEL and (n > 10_000):
+        chunk_size = int(n / os.cpu_count())
+        args = [
+            (network.edges.iloc[i : i + chunk_size, :], network.nodes, tolerance)
+            for i in range(0, n, chunk_size)
+        ]
+        with multiprocessing.Pool() as pool:
+            results = pool.starmap(_split_edges_at_nodes, args)
+
+        # flatten return list
+        split_edges: list = [df for chunk in results for df in chunk]
+
+    else:
+        split_edges = _split_edges_at_nodes(network.edges, network.nodes, tolerance)
+
     # combine dfs
     edges = pandas.concat(split_edges, axis=0)
     edges = edges.reset_index().drop("index", axis=1)
 
     return Network(nodes=network.nodes, edges=edges)
 
 
@@ -365,15 +434,19 @@
     all_nodes = concat_dedup([network.nodes, new_nodes])
 
     new_edges = matching_gdf_from_geoms(network.edges, new_edge_geoms)
     all_edges = concat_dedup([network.edges, new_edges])
 
     # split edges as necessary after new node creation
     unsplit = Network(nodes=all_nodes, edges=all_edges)
-    return split_edges_at_nodes(unsplit)
+
+    # this step is typically the majority of processing time
+    split = split_edges_at_nodes(unsplit)
+
+    return split
 
 
 def merge_edges(network, id_col="id", by=None):
     """Merge edges that share a node with a connectivity degree of 2
 
     Parameters
     ----------
@@ -482,27 +555,22 @@
     return geom_col
 
 
 def matching_gdf_from_geoms(gdf, geoms):
     """Create a geometry-only GeoDataFrame with column name to match an existing GeoDataFrame"""
     geom_col = geometry_column_name(gdf)
     geom_arr = geoms_to_array(geoms)
-    return GeoDataFrame(geom_arr, columns=[geom_col])
+    matching_gdf = GeoDataFrame(geometry=geom_arr, crs=gdf.crs)
+    matching_gdf.geometry.name = geom_col
+    return matching_gdf
 
 
 def geoms_to_array(geoms):
     geom_arr = np.empty(len(geoms), dtype="object")
-
-    # Filter warnings until Shapely 2.0
-    # see https://shapely.readthedocs.io/en/stable/migration.html
-    with warnings.catch_warnings():
-        warnings.filterwarnings(
-            "ignore", category=shapely.errors.ShapelyDeprecationWarning
-        )
-        geom_arr[:] = geoms
+    geom_arr[:] = geoms
 
     return geom_arr
 
 
 def concat_dedup(dfs):
     """Concatenate a list of GeoDataFrames, dropping duplicate geometries
     - note: repeatedly drops indexes for deduplication to work
@@ -518,21 +586,17 @@
     return len(
         network.edges[(network.edges.from_id == node) | (network.edges.to_id == node)]
     )
 
 
 def drop_duplicate_geometries(gdf, keep="first"):
     """Drop duplicate geometries from a dataframe"""
-
-    # convert to wkb so drop_duplicates will work
+    # as of geopandas ~0.6 this should work without explicit conversion to wkb
     # discussed in https://github.com/geopandas/geopandas/issues/521
-    mask = gdf.geometry.apply(lambda geom: geom.wkb).drop_duplicates(keep=keep).index
-
-    # use mask to drop from actual dataframe
-    return gdf.loc[mask]
+    return gdf.drop_duplicates([gdf.geometry.name])
 
 
 def nearest_point_on_edges(point, edges):
     """Find nearest point on edges to a point"""
     edge = nearest_edge(point, edges)
     snap = nearest_point_on_line(point, edge.geometry)
     return snap
@@ -546,16 +610,25 @@
 def nearest_edge(point, edges):
     """Find nearest edge to a point"""
     return nearest(point, edges)
 
 
 def nearest(geom, gdf):
     """Find the element of a GeoDataFrame nearest a shapely geometry"""
-    match_idx = gdf.sindex.nearest(geom, return_all=False)[1][0]
-    return gdf.loc[match_idx]
+    try:
+        match_idx = gdf.sindex.nearest(geom, return_all=False)[1][0]
+        return gdf.loc[match_idx]
+    except TypeError:
+        warnings.warn("Falling back to RTree index method for nearest element")
+        matches_idx = gdf.sindex.nearest(geom.bounds)
+        nearest_geom = min(
+            [gdf.iloc[match_idx] for match_idx in matches_idx],
+            key=lambda match: geom.distance(match.geometry),
+        )
+        return nearest_geom
 
 
 def edges_within(point, edges, distance):
     """Find edges within a distance of point"""
     return d_within(point, edges, distance)
 
 
@@ -677,16 +750,18 @@
     return output
 
 
 def split_edge_at_points(edge, points, tolerance=1e-9):
     """Split edge at point/multipoint"""
     try:
         segments = split_line(edge.geometry, points, tolerance)
-    except ValueError:
-        # if splitting fails, e.g. because points is empty GeometryCollection
+    except (ValueError, shapely.errors.GeometryTypeError):
+        # GeometryTypeError derives from ShapelyError and not TypeError or
+        # ValueError since Shapely 2.0. May be raised if splitting fails, e.g.
+        # because points is an empty GeometryCollection
         segments = [edge.geometry]
     edges = GeoDataFrame([edge] * len(segments))
     edges.geometry = segments
     return edges
 
 
 def split_line(line, points, tolerance=1e-9):
@@ -823,27 +898,28 @@
     if not USE_NX:
         raise ImportError("No module named networkx")
     else:
         G = to_networkx(network)
         return sorted(nx.connected_components(G), key=len, reverse=True)
 
 
-def add_component_ids(network, id_col="component_id"):
-    """Add column of component IDs to network data"""
-    # get connected components
-    connected_parts = get_connected_components(network)
-    # add unique id to each graph
-    network.edges[id_col] = 0  # init id_col
-    network.nodes[id_col] = 0  # init id_col
+def add_component_ids(network: Network, id_col: str = "component_id") -> Network:
+    """Add column of connected component IDs to network edges and nodes"""
+
+    # get connected components in descending size order
+    connected_parts: list[set] = get_connected_components(network)
+
+    # init id_col
+    network.edges[id_col] = 0
+    network.nodes[id_col] = 0
+
+    # add unique id for each graph component
     for count, part in enumerate(connected_parts):
         # edges
-        network.edges.loc[
-            (network.edges.from_id.isin(list(part)))
-            | (network.edges.to_id.isin(list(part))),
-            id_col,
-        ] = (
-            count + 1
-        )
+        edge_mask = network.edges.from_id.isin(part).values
+        network.edges.loc[edge_mask, id_col] = count + 1
+
         # nodes
-        network.nodes.loc[(network.nodes.id.isin(list(part))), id_col] = count + 1
-    # return
+        node_mask = network.nodes.id.isin(part).values
+        network.nodes.loc[node_mask, id_col] = count + 1
+
     return network
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snkit-1.7.2/src/snkit.egg-info/PKG-INFO` & `snkit-1.8.0/src/snkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snkit
-Version: 1.7.2
+Version: 1.8.0
 Summary: a spatial networks toolkit
 Home-page: https://github.com/tomalrussell/snkit
 Author: Tom Russell
 Author-email: tomalrussell@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `snkit-1.7.2/src/snkit.egg-info/SOURCES.txt` & `snkit-1.8.0/src/snkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snkit-1.7.2/tests/test_init.py` & `snkit-1.8.0/tests/test_init.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """Test core objects/concepts
 """
-# pylint: disable=C0103
-import warnings
-
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-    from geopandas import GeoDataFrame
+from geopandas import GeoDataFrame
 
 import pandas as pd
 from pandas.testing import assert_frame_equal
 from pytest import fixture, mark
 from shapely.geometry import Point, LineString, MultiPoint, MultiLineString
 
 try:
@@ -28,58 +23,58 @@
 def edge_only():
     """Single edge:
     |
     |
     |
     """
     edge = LineString([(0, 0), (0, 2)])
-    edges = GeoDataFrame([{"geometry": edge}])
+    edges = GeoDataFrame(geometry=[edge])
     return snkit.Network(edges=edges)
 
 
 @fixture
 def nodes_only():
     """Two nodes:
     x
 
     x
     """
     a = Point((0, 0))
     b = Point((0, 2))
-    nodes = GeoDataFrame([{"geometry": a}, {"geometry": b}])
+    nodes = GeoDataFrame(geometry=[a, b])
     return snkit.Network(nodes=nodes)
 
 
 @fixture
 def connected():
     """Edge with nodes:
     b
     |
     a
     """
     a = Point((0, 0))
     b = Point((0, 2))
     edge = LineString([a, b])
-    edges = GeoDataFrame([{"geometry": edge}])
-    nodes = GeoDataFrame([{"geometry": a}, {"geometry": b}])
+    edges = GeoDataFrame(geometry=[edge])
+    nodes = GeoDataFrame(geometry=[a, b])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def misaligned():
     """Edge with nodes offset:
     b |
       |
       | a
     """
     edge = LineString([(0, 0), (0, 2)])
     a = Point((0.5, 0))
     b = Point((-0.5, 2))
-    edges = GeoDataFrame([{"geometry": edge}])
-    nodes = GeoDataFrame([{"geometry": a}, {"geometry": b}])
+    edges = GeoDataFrame(geometry=[edge])
+    nodes = GeoDataFrame(geometry=[a, b])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def unsplit():
     """T-junction with nodes, long edge not split:
     b
@@ -90,16 +85,16 @@
     """
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0, 1))
     d = Point((1, 1))
     ab = LineString([a, b])
     cd = LineString([c, d])
-    edges = GeoDataFrame([ab, cd], columns=["geometry"])
-    nodes = GeoDataFrame([a, b, c, d], columns=["geometry"])
+    edges = GeoDataFrame(geometry=[ab, cd])
+    nodes = GeoDataFrame(geometry=[a, b, c, d])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split():
     """T-junction with nodes, long edge split:
     b
@@ -108,19 +103,19 @@
     |
     a
     """
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0, 1))
     d = Point((1, 1))
-    nodes = GeoDataFrame([a, b, c, d], columns=["geometry"])
+    nodes = GeoDataFrame(geometry=[a, b, c, d])
     ac = LineString([a, c])
     cb = LineString([c, b])
     cd = LineString([c, d])
-    edges = GeoDataFrame([ac, cb, cd], columns=["geometry"])
+    edges = GeoDataFrame(geometry=[ac, cb, cd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split_with_ids():
     """T-junction with nodes, long edge split, and node and edge ids:
      b
@@ -129,19 +124,19 @@
     1|
      a
     """
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0, 1))
     d = Point((1, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d], "id": ["a", "b", "c", "d"]})
+    nodes = GeoDataFrame(data={"id": ["a", "b", "c", "d"]}, geometry=[a, b, c, d])
     ac = LineString([a, c])
     cb = LineString([c, b])
     cd = LineString([c, d])
-    edges = GeoDataFrame(data={"geometry": [ac, cb, cd], "id": [1, 2, 3]})
+    edges = GeoDataFrame(data={"id": [1, 2, 3]}, geometry=[ac, cb, cd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def unsplit_intersection():
     """Edges intersection, both edges not split
        b
@@ -150,18 +145,18 @@
        |
        a
     """
     a = Point((1, 0))
     b = Point((1, 2))
     c = Point((0, 1))
     d = Point((2, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d])
     ab = LineString([a, b])
     cd = LineString([c, d])
-    edges = GeoDataFrame(data={"geometry": [ab, cd]})
+    edges = GeoDataFrame(geometry=[ab, cd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split_intersection():
     """Edges intersection, both edges split
        b
@@ -171,20 +166,20 @@
        a
     """
     a = Point((1, 0))
     b = Point((1, 2))
     c = Point((0, 1))
     d = Point((2, 1))
     x = Point((1, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d, x]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d, x])
     ax = LineString([a, x])
     xb = LineString([x, b])
     cx = LineString([c, x])
     xd = LineString([x, d])
-    edges = GeoDataFrame(data={"geometry": [ax, xb, cx, xd]})
+    edges = GeoDataFrame(geometry=[ax, xb, cx, xd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def unsplit_multiple_intersections():
     """Multiple edges intersections, all edges unsplit
        b   f
@@ -195,19 +190,19 @@
     """
     a = Point((1, 0))
     b = Point((1, 2))
     c = Point((0, 1))
     d = Point((3, 1))
     e = Point((2, 0))
     f = Point((2, 2))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d, e, f]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d, e, f])
     ab = LineString([a, b])
     cd = LineString([c, d])
     ef = LineString([e, f])
-    edges = GeoDataFrame(data={"geometry": [ab, cd, ef]})
+    edges = GeoDataFrame(geometry=[ab, cd, ef])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split_multiple_intersections():
     """Multiple edges intersections, all edges split
        b   f
@@ -220,23 +215,23 @@
     b = Point((1, 2))
     c = Point((0, 1))
     d = Point((3, 1))
     e = Point((2, 0))
     f = Point((2, 2))
     x = Point((1, 1))
     y = Point((2, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d, e, f, x, y]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d, e, f, x, y])
     ax = LineString([a, x])
     xb = LineString([x, b])
     cx = LineString([c, x])
     xy = LineString([x, y])
     yd = LineString([y, d])
     ey = LineString([e, y])
     yf = LineString([y, f])
-    edges = GeoDataFrame(data={"geometry": [ax, xb, cx, xy, yd, ey, yf]})
+    edges = GeoDataFrame(geometry=[ax, xb, cx, xy, yd, ey, yf])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def unsplit_overlapping_lines():
     """Overlapping lines for a section
        c--d
@@ -247,18 +242,18 @@
     """
     a = Point((1, 0))
     b = Point((0, 1))
     c = Point((1, 2))
     d = Point((2, 2))
     # x is just a construction point
     x = Point((1, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d])
     ac = LineString([a, c])
     bd = LineString([b, x, c, d])
-    edges = GeoDataFrame(data={"geometry": [ac, bd]})
+    edges = GeoDataFrame(geometry=[ac, bd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split_overlapping_lines():
     """Split of overlapping lines for a section
        c--d
@@ -268,21 +263,21 @@
        a
     """
     a = Point((1, 0))
     b = Point((0, 1))
     c = Point((1, 2))
     d = Point((2, 2))
     x = Point((1, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d, x]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d, x])
     ax = LineString([a, x])
     bx = LineString([b, x])
     xc = LineString([x, c])
     cd = LineString([c, d])
     # note that there are two edges 'xc'
-    edges = GeoDataFrame(data={"geometry": [ax, xc, bx, xc, cd]})
+    edges = GeoDataFrame(geometry=[ax, xc, bx, xc, cd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def unsplit_heterogeneous_intersection():
     """Crossing point and overlapping line
        b--c
@@ -297,18 +292,18 @@
     b = Point((1, 2))
     c = Point((2, 2))
     # y is just a construction point
     y = Point((2, 1))
     d = Point((3, 1))
     e = Point((0, 1))
     f = Point((4, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d, e, f]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d, e, f])
     ad = LineString([a, b, c, y, d])
     ef = LineString([e, f])
-    edges = GeoDataFrame(data={"geometry": [ad, ef]})
+    edges = GeoDataFrame(geometry=[ad, ef])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split_heterogeneous_intersection():
     """Crossing point and overlapping line, all edges split
        b--c
@@ -322,25 +317,25 @@
     c = Point((2, 2))
     d = Point((3, 1))
     e = Point((0, 1))
     f = Point((4, 1))
     x = Point((1, 1))
     y = Point((2, 1))
     # note: this is order sensitive although it shouldn't matter
-    nodes = GeoDataFrame(data={"geometry": [a, b, c, d, e, f, y, x]})
+    nodes = GeoDataFrame(geometry=[a, b, c, d, e, f, y, x])
     ax = LineString([a, x])
     xb = LineString([x, b])
     bc = LineString([b, c])
     cy = LineString([c, y])
     yd = LineString([y, d])
     ex = LineString([e, x])
     xy = LineString([x, y])
     df = LineString([d, f])
     # note that there are two edges 'yd'
-    edges = GeoDataFrame(data={"geometry": [ax, xb, bc, cy, yd, ex, xy, yd, df]})
+    edges = GeoDataFrame(geometry=[ax, xb, bc, cy, yd, ex, xy, yd, df])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def unsplit_self_intersection():
     """A line crossing with itself
        b--c
@@ -351,17 +346,17 @@
     """
     a = Point((1, 0))
     e = Point((0, 1))
     # 'b', 'c' and 'd' are construction points, not nodes
     b = Point((1, 2))
     c = Point((2, 2))
     d = Point((2, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, e]})
+    nodes = GeoDataFrame(geometry=[a, e])
     ae = LineString([a, b, c, d, e])
-    edges = GeoDataFrame(data={"geometry": [ae]})
+    edges = GeoDataFrame(geometry=[ae])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def split_self_intersection():
     """A line crossing with itself, edge split
        b--c
@@ -373,19 +368,19 @@
     a = Point((1, 0))
     e = Point((0, 1))
     x = Point((1, 1))
     # 'b', 'c' and 'd' are construction points, not nodes
     b = Point((1, 2))
     c = Point((2, 2))
     d = Point((2, 1))
-    nodes = GeoDataFrame(data={"geometry": [a, e, x]})
+    nodes = GeoDataFrame(geometry=[a, e, x])
     ax = LineString([a, x])
     xx = LineString([x, b, c, d, x])
     xe = LineString([x, e])
-    edges = GeoDataFrame(data={"geometry": [ax, xx, xe]})
+    edges = GeoDataFrame(geometry=[ax, xx, xe])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def gap():
     """T-junction with nodes, edges not quite intersecting:
     b
@@ -394,18 +389,18 @@
     |
     a
     """
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0.1, 1))
     d = Point((1, 1))
-    nodes = GeoDataFrame([a, b, c, d], columns=["geometry"])
+    nodes = GeoDataFrame(geometry=[a, b, c, d])
     ab = LineString([a, b])
     cd = LineString([c, d])
-    edges = GeoDataFrame([ab, cd], columns=["geometry"])
+    edges = GeoDataFrame(geometry=[ab, cd])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
 @fixture
 def bridged():
     """T-junction with nodes, bridged by short edge:
     b
@@ -415,30 +410,63 @@
     a
     """
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0.1, 1))
     d = Point((1, 1))
     e = Point((0, 1))
-    nodes = GeoDataFrame([a, b, c, d, e], columns=["geometry"])
+    nodes = GeoDataFrame(geometry=[a, b, c, d, e])
     ae = LineString([a, e])
     eb = LineString([e, b])
     cd = LineString([c, d])
     ce = LineString([c, e])
-    edges = GeoDataFrame([ae, eb, cd, ce], columns=["geometry"])
+    edges = GeoDataFrame(geometry=[ae, eb, cd, ce])
     return snkit.Network(edges=edges, nodes=nodes)
 
 
+@fixture
+def two_components(gap):
+    """Two network components
+    b
+    |
+    |   c--d--e
+    |
+    a
+    """
+    a = Point((0, 0))
+    b = Point((0, 2))
+    c = Point((1, 1))
+    d = Point((2, 1))
+    e = Point((3, 1))
+    nodes = GeoDataFrame(geometry=[a, b, c, d, e])
+    ab = LineString([a, b])
+    cd = LineString([c, d])
+    de = LineString([d, e])
+    edges = GeoDataFrame(geometry=[ab, cd, de])
+    network = snkit.Network(edges=edges, nodes=nodes)
+    network = snkit.network.add_ids(network)
+    network = snkit.network.add_topology(network)
+    return network
+
+
 def test_init():
     """Should create an empty network"""
     net = snkit.Network()
     assert len(net.nodes) == 0
     assert len(net.edges) == 0
 
 
+def test_roundtrip(connected, tmp_path):
+    """Should write and read back a network"""
+    connected.to_file(tmp_path / "connected.gpkg", driver="GPKG")
+    actual = snkit.network.read_file(tmp_path / "connected.gpkg")
+    assert_frame_equal(actual.nodes, connected.nodes)
+    assert_frame_equal(actual.edges, connected.edges)
+
+
 def test_round_geometries(misaligned, connected):
     """Should round coordinates to some tolerance"""
     rounded = snkit.network.round_geometries(misaligned, precision=0)
     assert_frame_equal(rounded.nodes, connected.nodes)
 
 
 def test_add_ids(edge_only, connected):
@@ -699,15 +727,16 @@
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0, 1))
     d = Point((1, 1))
     ac = LineString([a, c])
     cb = LineString([c, b])
     cd = LineString([c, d])
-    edges = GeoDataFrame([ac, cb, cd], columns=["geometry"])
+    edges = GeoDataFrame(geometry=[ac, cb, cd])
+
     network = snkit.Network(edges=edges[1:])
     with_endpoints = snkit.network.add_endpoints(network)
     with_ids = snkit.network.add_ids(with_endpoints)
 
     actual = with_ids.edges
     expected = GeoDataFrame(
         [(cb, "edge_0"), (cd, "edge_1")], columns=["geometry", "id"]
@@ -721,19 +750,15 @@
     a = Point((0, 0))
     b = Point((0, 2))
     c = Point((0, 1))
     ac = LineString([a, c])
     cb = LineString([c, b])
     # use an index that doesn't start from 0 to check our indexing hygiene
     index = pd.Index([2, 3, 5, 7, 11, 13])
-    gdf_with_dupes = GeoDataFrame(
-        index=index,
-        data=[a, a, b, ac, ac, cb],
-        columns=["geometry"]
-    )
+    gdf_with_dupes = GeoDataFrame(index=index, geometry=[a, a, b, ac, ac, cb])
     deduped = snkit.network.drop_duplicate_geometries(gdf_with_dupes)
     # we should have just the first of each duplicate item
     assert (deduped.index == pd.Index([2, 5, 7, 13])).all()
 
 
 @mark.skipif(not USE_NX, reason="networkx not available")
 def test_to_networkx(connected):
@@ -744,7 +769,22 @@
 
     G_true = nx.Graph()
     G_true.add_node("n0", pos=(0, 0))
     G_true.add_node("n1", pos=(0, 2))
     G_true.add_edge("n0", "n1", weight=2)
 
     assert graphs_equal(G, G_true)
+
+
+def test_add_component_ids(two_components):
+    labelled = snkit.network.add_component_ids(two_components)
+    assert all(labelled.edges.component_id == pd.Series([2, 1, 1]))
+
+
+def test_matching_gdf_from_geoms(edge_only):
+    expected = edge_only.edges.copy()
+    gdf = edge_only.edges.copy()
+    geoms = gdf.geometry
+    gdf["a"] = range(len(gdf))
+    gdf["b"] = "abc"
+    actual = snkit.network.matching_gdf_from_geoms(gdf, geoms)
+    assert_frame_equal(actual, expected)
```

