# Comparing `tmp/meow-sim-0.5.4.tar.gz` & `tmp/meow-sim-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.4.tar", last modified: Fri Jun  9 14:33:26 2023, max compression
+gzip compressed data, was "meow-sim-0.5.5.tar", last modified: Fri Jun  9 19:08:23 2023, max compression
```

## Comparing `meow-sim-0.5.4.tar` & `meow-sim-0.5.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-09 14:33:21.000000 meow-sim-0.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 14:33:26.446741 meow-sim-0.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-09 14:33:21.000000 meow-sim-0.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.442741 meow-sim-0.5.4/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.442741 meow-sim-0.5.4/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.442741 meow-sim-0.5.4/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5533 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    13437 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7905 2023-06-09 14:33:21.000000 meow-sim-0.5.4/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 14:33:26.000000 meow-sim-0.5.4/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 14:33:21.000000 meow-sim-0.5.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 14:33:26.446741 meow-sim-0.5.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:33:26.446741 meow-sim-0.5.4/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-09 14:33:21.000000 meow-sim-0.5.4/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-09 14:33:21.000000 meow-sim-0.5.4/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-09 14:33:21.000000 meow-sim-0.5.4/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-09 19:08:19.000000 meow-sim-0.5.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 19:08:23.546071 meow-sim-0.5.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-09 19:08:19.000000 meow-sim-0.5.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.542071 meow-sim-0.5.5/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.542071 meow-sim-0.5.5/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6170 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    13437 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7920 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 19:08:19.000000 meow-sim-0.5.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 19:08:23.546071 meow-sim-0.5.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-09 19:08:19.000000 meow-sim-0.5.5/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-09 19:08:19.000000 meow-sim-0.5.5/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-09 19:08:19.000000 meow-sim-0.5.5/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.4/LICENSE` & `meow-sim-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/PKG-INFO` & `meow-sim-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.4
+Version: 0.5.5
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.4/README.md` & `meow-sim-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/__init__.py` & `meow-sim-0.5.5/meow/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.4/meow/assets/silicon.csv` & `meow-sim-0.5.5/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.5/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/base_model.py` & `meow-sim-0.5.5/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/cache.py` & `meow-sim-0.5.5/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/cell.py` & `meow-sim-0.5.5/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/cross_section.py` & `meow-sim-0.5.5/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/eme/__init__.py` & `meow-sim-0.5.5/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/eme/common.py` & `meow-sim-0.5.5/meow/eme/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -121,30 +121,47 @@
             enforce_reciprocity=enforce_reciprocity,
             enforce_lossy_unitarity=enforce_lossy_unitarity,
         )
         for i, (modes1, modes2) in enumerate(zip(modes[:-1], modes[1:]))
     }
 
 
-def compute_propagation_s_matrix(modes: List[Mode]):
+def compute_propagation_s_matrix(
+    modes: List[Mode], override_cell_length: float | None = None
+):
     """get the propagation S-matrix of each `Mode` belonging to a `CrossSection` in a `Cell` with a certain length."""
+    cell_length = modes[0].cell.length
+    if override_cell_length is not None:
+        cell_length = override_cell_length
+
     s_dict = {
         (f"left@{i}", f"right@{i}"): np.exp(
-            2j * np.pi * mode.neff / mode.env.wl * mode.cell.length
+            2j * np.pi * mode.neff / mode.env.wl * cell_length
         )
         for i, mode in enumerate(modes)
     }
     s_dict = {**s_dict, **{(p2, p1): v for (p1, p2), v in s_dict.items()}}
     return s_dict
 
 
-def compute_propagation_s_matrices(modes: List[List[Mode]]):
+def compute_propagation_s_matrices(
+    modes: List[List[Mode]], override_cell_lengths: list[float] | None = None
+):
     """get all the propagation S-matrices of all the `Modes` belonging to each `CrossSection`"""
+    if override_cell_lengths:
+        if not len(override_cell_lengths) == len(modes):
+            raise ValueError(
+                f"len(override_cell_lengths) != len(modes): {len(override_cell_lengths)} != {len(modes)}"
+            )
+        cell_lengths = override_cell_lengths
+    else:
+        cell_lengths = [None for _ in modes]
     return {
-        f"p_{i}": compute_propagation_s_matrix(modes_) for i, modes_ in enumerate(modes)
+        f"p_{i}": compute_propagation_s_matrix(modes_, override_cell_length=cell_length)
+        for i, (modes_, cell_length) in enumerate(zip(modes, cell_lengths))
     }
 
 
 def select_ports(
     S: np.ndarray[Any, np.dtype[np.float_]], port_map: Dict[str, int], ports: List[str]
 ):
     """Keep subset of an S-matrix
```

### Comparing `meow-sim-0.5.4/meow/eme/sax.py` & `meow-sim-0.5.5/meow/eme/sax.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 def compute_s_matrix_sax(
     modes: List[List[Mode]],
     sax_backend: str | None = None,
     conjugate_transpose: bool = DEFAULT_CONJUGATE_TRANSPOSE,
     enforce_reciprocity: bool = DEFAULT_ENFORCE_RECIPROCITY,
     enforce_lossy_unitarity: bool = DEFAULT_ENFORCE_LOSSY_UNITARITY,
+    override_cell_lengths: list[float] | None = None,
     **kwargs,
 ):
     """Calculate the S-matrix for given sets of modes, each set belonging to a `Cell`
 
     Args:
         modes: Each collection of modes for each of the `Cell` objects
         backend: which SAX backend to use to calculate the final S-matrix.
@@ -95,15 +96,17 @@
     sax_backend = _validate_sax_backend(sax_backend)
     _compute_propagation_s_matrices = kwargs.pop(
         "compute_propagation_s_matrices", compute_propagation_s_matrices
     )
     _compute_interface_s_matrices = kwargs.pop(
         "compute_interface_s_matrices", compute_interface_s_matrices
     )
-    propagations = _compute_propagation_s_matrices(modes)
+    propagations = _compute_propagation_s_matrices(
+        modes, override_cell_lengths=override_cell_lengths
+    )
     interfaces = _compute_interface_s_matrices(
         modes,
         conjugate_transpose=conjugate_transpose,
         enforce_reciprocity=enforce_reciprocity,
         enforce_lossy_unitarity=enforce_lossy_unitarity,
         **kwargs,
     )
```

### Comparing `meow-sim-0.5.4/meow/environment.py` & `meow-sim-0.5.5/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/fde/lumerical.py` & `meow-sim-0.5.5/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/fde/tidy3d.py` & `meow-sim-0.5.5/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/gds_structures.py` & `meow-sim-0.5.5/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/geometries.py` & `meow-sim-0.5.5/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/integrate.py` & `meow-sim-0.5.5/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/materials.py` & `meow-sim-0.5.5/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/mesh.py` & `meow-sim-0.5.5/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/mode.py` & `meow-sim-0.5.5/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/structures.py` & `meow-sim-0.5.5/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/meow/visualize.py` & `meow-sim-0.5.5/meow/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,10 +306,11 @@
     if plt is None:
         print(obj)
         return
 
     for check_func, vis_func in VISUALIZATION_MAPPING.items():
         if check_func(obj):
             return vis_func(obj, **kwargs)
+    print(obj)
 
 
 vis = visualize  # shorthand for visualize
```

### Comparing `meow-sim-0.5.4/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.5/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.4
+Version: 0.5.5
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.4/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.5/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/pyproject.toml` & `meow-sim-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.4/tests/test_deserialization.py` & `meow-sim-0.5.5/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/tests/test_mode_operators.py` & `meow-sim-0.5.5/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.4/tests/test_nbs.py` & `meow-sim-0.5.5/tests/test_nbs.py`

 * *Files identical despite different names*

