# Comparing `tmp/meow-sim-0.5.3.tar.gz` & `tmp/meow-sim-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.3.tar", last modified: Fri Jun  9 13:49:38 2023, max compression
+gzip compressed data, was "meow-sim-0.5.4.tar", last modified: Fri Jun  9 14:33:26 2023, max compression
```

## Comparing `meow-sim-0.5.3.tar` & `meow-sim-0.5.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.035423 meow-sim-0.5.3/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-09 13:49:34.000000 meow-sim-0.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 13:49:38.035423 meow-sim-0.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-09 13:49:34.000000 meow-sim-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5533 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12966 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7905 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.035423 meow-sim-0.5.3/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 13:49:34.000000 meow-sim-0.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:49:38.035423 meow-sim-0.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.035423 meow-sim-0.5.3/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-09 13:49:34.000000 meow-sim-0.5.3/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-09 13:49:34.000000 meow-sim-0.5.3/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-09 13:49:34.000000 meow-sim-0.5.3/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-09 14:33:21.000000 meow-sim-0.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 14:33:26.446741 meow-sim-0.5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-09 14:33:21.000000 meow-sim-0.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.442741 meow-sim-0.5.4/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.442741 meow-sim-0.5.4/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.442741 meow-sim-0.5.4/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5533 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    13437 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7905 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 14:33:21.000000 meow-sim-0.5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 14:33:26.446741 meow-sim-0.5.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-09 14:33:21.000000 meow-sim-0.5.4/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-09 14:33:21.000000 meow-sim-0.5.4/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-09 14:33:21.000000 meow-sim-0.5.4/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.3/LICENSE` & `meow-sim-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/PKG-INFO` & `meow-sim-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.3
+Version: 0.5.4
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.3/README.md` & `meow-sim-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/__init__.py` & `meow-sim-0.5.4/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.3/meow/assets/silicon.csv` & `meow-sim-0.5.4/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.4/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/base_model.py` & `meow-sim-0.5.4/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/cache.py` & `meow-sim-0.5.4/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/cell.py` & `meow-sim-0.5.4/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/cross_section.py` & `meow-sim-0.5.4/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/eme/__init__.py` & `meow-sim-0.5.4/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/eme/common.py` & `meow-sim-0.5.4/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/eme/sax.py` & `meow-sim-0.5.4/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/environment.py` & `meow-sim-0.5.4/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/fde/lumerical.py` & `meow-sim-0.5.4/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/fde/tidy3d.py` & `meow-sim-0.5.4/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/gds_structures.py` & `meow-sim-0.5.4/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/geometries.py` & `meow-sim-0.5.4/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/integrate.py` & `meow-sim-0.5.4/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/materials.py` & `meow-sim-0.5.4/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/mesh.py` & `meow-sim-0.5.4/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/mode.py` & `meow-sim-0.5.4/meow/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -408,13 +408,28 @@
         Ez=mode.Ez / e,
         Hx=mode.Hx / h,
         Hy=mode.Hy / h,
         Hz=mode.Hz / h,
     )
 
 
+def is_pml_mode(mode, threshold_factor=0.2):
+    numx, numy = mode.cell.mesh.num_pml
+    ed = energy_density(mode)
+    m, n = ed.shape
+    lft = ed[:numx, :]
+    rgt = ed[m - numx :, :]
+    top = ed[numx : m - numx, n:numy]
+    btm = ed[numx : m - numx, n - numy :]
+    rest = ed[numx : m - numx, numy : n - numy]
+    pml_sum = lft.sum() + rgt.sum() + top.sum() + btm.sum()
+    rest_sum = rest.sum()
+    is_pml = pml_sum > threshold_factor * rest_sum
+    return is_pml
+
+
 def te_fraction(mode: Mode) -> float:
     """the TE polarization fraction of the `Mode`"""
     epsx = mode.cs.nx**2
     e = np.sum(0.5 * eps0 * epsx * np.abs(mode.Ex) ** 2)
     h = np.sum(0.5 * mu0 * np.abs(mode.Hx) ** 2)
     return float(e / (e + h))
```

### Comparing `meow-sim-0.5.3/meow/structures.py` & `meow-sim-0.5.4/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow/visualize.py` & `meow-sim-0.5.4/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.4/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.3
+Version: 0.5.4
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.3/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.4/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/pyproject.toml` & `meow-sim-0.5.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.3/tests/test_deserialization.py` & `meow-sim-0.5.4/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/tests/test_mode_operators.py` & `meow-sim-0.5.4/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.3/tests/test_nbs.py` & `meow-sim-0.5.4/tests/test_nbs.py`

 * *Files identical despite different names*

