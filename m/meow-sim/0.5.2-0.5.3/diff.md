# Comparing `tmp/meow-sim-0.5.2.tar.gz` & `tmp/meow-sim-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.2.tar", last modified: Thu Jun  8 00:26:58 2023, max compression
+gzip compressed data, was "meow-sim-0.5.3.tar", last modified: Fri Jun  9 13:49:38 2023, max compression
```

## Comparing `meow-sim-0.5.2.tar` & `meow-sim-0.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-08 00:26:54.000000 meow-sim-0.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-08 00:26:58.972550 meow-sim-0.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-08 00:26:54.000000 meow-sim-0.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5533 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12966 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7469 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-08 00:26:54.000000 meow-sim-0.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:26:58.972550 meow-sim-0.5.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-08 00:26:54.000000 meow-sim-0.5.2/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-08 00:26:54.000000 meow-sim-0.5.2/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-08 00:26:54.000000 meow-sim-0.5.2/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.035423 meow-sim-0.5.3/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-09 13:49:34.000000 meow-sim-0.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 13:49:38.035423 meow-sim-0.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-09 13:49:34.000000 meow-sim-0.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5533 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.031423 meow-sim-0.5.3/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12966 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7905 2023-06-09 13:49:34.000000 meow-sim-0.5.3/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.035423 meow-sim-0.5.3/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 13:49:38.000000 meow-sim-0.5.3/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 13:49:34.000000 meow-sim-0.5.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:49:38.035423 meow-sim-0.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:49:38.035423 meow-sim-0.5.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-09 13:49:34.000000 meow-sim-0.5.3/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-09 13:49:34.000000 meow-sim-0.5.3/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-09 13:49:34.000000 meow-sim-0.5.3/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.2/LICENSE` & `meow-sim-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/PKG-INFO` & `meow-sim-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.2
+Version: 0.5.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.2/README.md` & `meow-sim-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/__init__.py` & `meow-sim-0.5.3/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.2/meow/assets/silicon.csv` & `meow-sim-0.5.3/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.3/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/base_model.py` & `meow-sim-0.5.3/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/cache.py` & `meow-sim-0.5.3/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/cell.py` & `meow-sim-0.5.3/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/cross_section.py` & `meow-sim-0.5.3/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/eme/__init__.py` & `meow-sim-0.5.3/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/eme/common.py` & `meow-sim-0.5.3/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/eme/sax.py` & `meow-sim-0.5.3/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/environment.py` & `meow-sim-0.5.3/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/fde/lumerical.py` & `meow-sim-0.5.3/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/fde/tidy3d.py` & `meow-sim-0.5.3/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/gds_structures.py` & `meow-sim-0.5.3/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/geometries.py` & `meow-sim-0.5.3/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/integrate.py` & `meow-sim-0.5.3/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/materials.py` & `meow-sim-0.5.3/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/mesh.py` & `meow-sim-0.5.3/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/mode.py` & `meow-sim-0.5.3/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/structures.py` & `meow-sim-0.5.3/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/meow/visualize.py` & `meow-sim-0.5.3/meow/visualize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """ Visualizations for common meow-datatypes """
 
-from typing import Any
+from collections.abc import Iterable
+from typing import Any, Callable
 
 import numpy as np
 
+from meow.structures import visualize_structures
+
 try:
     import matplotlib.pyplot as plt  # fmt: skip
 
 
 except ImportError:
     plt = None
 
@@ -164,35 +167,25 @@
 
     if show:
         plt.show()
 
     return p
 
 
-def _visualize_gdsfactory(comp):
+def _visualize_gf_component(comp):
     import gdsfactory as gf  # fmt: skip
 
     gf.plot(comp)  # type: ignore
 
 
-def _is_s_matrix(obj: Any):
-    return (
-        (
-            isinstance(obj, np.ndarray)
-            or (DeviceArray is not None and isinstance(obj, DeviceArray))
-        )
-        and obj.ndim == 2
-        and obj.shape[0] > 1
-        and obj.shape[1] > 1
-    )
-
-
 def _is_two_tuple(obj):
+    if not isinstance(obj, tuple):
+        return False
     try:
-        x, y = obj
+        x, y = obj  # type: ignore
         return True
     except Exception:
         return False
 
 
 def _figsize_visualize_mode(cs, W0):
     x_min, x_max = cs.mesh.x.min(), cs.mesh.x.max()
@@ -213,15 +206,14 @@
     operation=lambda x: np.abs(x) ** 2,
     show=True,
 ):
     import matplotlib.pyplot as plt  # fmt: skip
 
     num_modes = len(modes)
     cs = modes[0].cs
-    X, Y, n = cs.mesh.Xz, cs.mesh.Yz, cs.nz
     W, H = _figsize_visualize_mode(cs, 6.4)
 
     fig, ax = plt.subplots(
         num_modes,
         2,
         figsize=(2 * W, num_modes * H),
         sharex=True,
@@ -241,51 +233,83 @@
             show=False,
         )
     fig.subplots_adjust(hspace=0, wspace=2 / (2 * W))
     if show:
         plt.show()
 
 
+def _visualize_base_model(obj, **kwargs):
+    return obj._visualize(**kwargs)
+
+
+def _is_mode_list(obj: Any) -> bool:
+    from .mode import Mode  # fmt: skip
+    return isinstance(obj, Iterable) and all(isinstance(o, Mode) for o in obj)
+
+
+def _is_structure_list(obj: Any) -> bool:
+    from .structures import Structure  # fmt: skip
+    return isinstance(obj, Iterable) and all(isinstance(o, Structure) for o in obj)
+
+
+def _is_base_model(obj: Any) -> bool:
+    from .base_model import BaseModel  # fmt: skip
+    return isinstance(obj, BaseModel)
+
+
+def _is_mode_overlap(obj: Any) -> bool:
+    from .mode import Mode  # fmt: skip
+    return _is_two_tuple(obj) and all(isinstance(o, Mode) for o in obj)
+
+
+def _is_s_matrix(obj: Any):
+    return (
+        (
+            isinstance(obj, np.ndarray)
+            or (DeviceArray is not None and isinstance(obj, DeviceArray))
+        )
+        and obj.ndim == 2
+        and obj.shape[0] > 1
+        and obj.shape[1] > 1
+    )
+
+
+def _is_s_pm_matrix(obj):
+    return _is_two_tuple(obj) and _is_s_matrix(obj[0]) and isinstance(obj[1], dict)
+
+
+def _is_gf_component(obj):
+    return gf is not None and isinstance(obj, gf.Component)
+
+
+VISUALIZATION_MAPPING: dict[Callable, Callable] = {
+    _is_base_model: _visualize_base_model,
+    _is_mode_list: _visualize_modes,
+    _is_structure_list: visualize_structures,
+    _is_mode_overlap: _visualize_overlap_density,
+    _is_s_matrix: _visualize_s_matrix,
+    _is_s_pm_matrix: _visualize_s_pm_matrix,
+    _is_gf_component: _visualize_gf_component,
+}
+
+
 def visualize(obj: Any, **kwargs: Any):
     """visualize any meow object
 
     Args:
         obj: the meow object to visualize
         **kwargs: extra configuration to visualize the object
 
     Note:
         Most meow objects have a `._visualize` method.
         Check out its help to see which kwargs are accepted.
     """
-    from .base_model import BaseModel  # fmt: skip
-    from .mode import Mode  # fmt: skip
-    from .structures import Structure, visualize_structures  # fmt: skip
-
-    # if isinstance(obj, Mode):
-    #    return _visualize_mode(obj)
     if plt is None:
-        return obj
+        print(obj)
+        return
 
-    if isinstance(obj, list) and all(isinstance(o, Mode) for o in obj):
-        return _visualize_modes(obj)
-    elif isinstance(obj, BaseModel):
-        return obj._visualize(**kwargs)
-    elif _is_two_tuple(obj) and all(isinstance(o, Mode) for o in obj):
-        return _visualize_overlap_density(obj, **kwargs)
-    elif _is_s_matrix(obj):
-        _visualize_s_matrix(obj, **kwargs)
-    elif _is_two_tuple(obj) and _is_s_matrix(obj[0]) and isinstance(obj[1], dict):
-        _visualize_s_pm_matrix(obj, **kwargs)
-    elif gf is not None and isinstance(obj, gf.Component):
-        _visualize_gdsfactory(obj, **kwargs)
-    else:
-        try:
-            (*objs,) = obj  # type: ignore
-        except TypeError:
-            return obj
-
-        if all(isinstance(obj, Structure) for obj in objs):
-            return visualize_structures(objs, **kwargs)
-        return objs
+    for check_func, vis_func in VISUALIZATION_MAPPING.items():
+        if check_func(obj):
+            return vis_func(obj, **kwargs)
 
 
 vis = visualize  # shorthand for visualize
```

### Comparing `meow-sim-0.5.2/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.3/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.2
+Version: 0.5.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.2/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.3/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/pyproject.toml` & `meow-sim-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.2/tests/test_deserialization.py` & `meow-sim-0.5.3/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/tests/test_mode_operators.py` & `meow-sim-0.5.3/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.2/tests/test_nbs.py` & `meow-sim-0.5.3/tests/test_nbs.py`

 * *Files identical despite different names*

