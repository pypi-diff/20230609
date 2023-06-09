# Comparing `tmp/emrecharge-0.0.8.tar.gz` & `tmp/emrecharge-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emrecharge-0.0.8.tar", last modified: Wed Mar 22 10:37:43 2023, max compression
+gzip compressed data, was "emrecharge-0.0.9.tar", last modified: Wed Apr  5 08:26:30 2023, max compression
```

## Comparing `emrecharge-0.0.8.tar` & `emrecharge-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-03-22 10:37:43.862335 emrecharge-0.0.8/
--rw-r--r--   0 stevejpurves   (501) staff       (20)     1059 2023-02-10 11:47:27.000000 emrecharge-0.0.8/LICENSE.md
--rw-r--r--   0 stevejpurves   (501) staff       (20)      592 2023-03-22 10:37:43.862394 emrecharge-0.0.8/PKG-INFO
--rw-r--r--   0 stevejpurves   (501) staff       (20)      154 2023-02-10 12:07:40.000000 emrecharge-0.0.8/README.md
-drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-03-22 10:37:43.861486 emrecharge-0.0.8/emrecharge/
--rw-r--r--   0 stevejpurves   (501) staff       (20)        0 2023-02-10 11:47:27.000000 emrecharge-0.0.8/emrecharge/__init__.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     4751 2023-02-16 16:01:41.000000 emrecharge-0.0.8/emrecharge/app.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     6445 2023-03-22 10:24:17.000000 emrecharge-0.0.8/emrecharge/colocation.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     2469 2023-03-17 10:54:09.000000 emrecharge-0.0.8/emrecharge/datasets.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     1178 2023-02-10 11:47:27.000000 emrecharge-0.0.8/emrecharge/gis.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     4823 2023-03-07 20:46:54.000000 emrecharge-0.0.8/emrecharge/metrics.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     7270 2023-03-07 20:46:54.000000 emrecharge-0.0.8/emrecharge/rockphysics.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)     2404 2023-02-10 11:47:27.000000 emrecharge-0.0.8/emrecharge/utils.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)       22 2023-03-22 10:37:33.000000 emrecharge-0.0.8/emrecharge/version.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)    14490 2023-03-17 10:27:33.000000 emrecharge-0.0.8/emrecharge/viz.py
-drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-03-22 10:37:43.862242 emrecharge-0.0.8/emrecharge.egg-info/
--rw-r--r--   0 stevejpurves   (501) staff       (20)      592 2023-03-22 10:37:43.000000 emrecharge-0.0.8/emrecharge.egg-info/PKG-INFO
--rw-r--r--   0 stevejpurves   (501) staff       (20)      438 2023-03-22 10:37:43.000000 emrecharge-0.0.8/emrecharge.egg-info/SOURCES.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)        1 2023-03-22 10:37:43.000000 emrecharge-0.0.8/emrecharge.egg-info/dependency_links.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)      115 2023-03-22 10:37:43.000000 emrecharge-0.0.8/emrecharge.egg-info/requires.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)       11 2023-03-22 10:37:43.000000 emrecharge-0.0.8/emrecharge.egg-info/top_level.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)      103 2023-02-10 11:47:27.000000 emrecharge-0.0.8/pyproject.toml
--rw-r--r--   0 stevejpurves   (501) staff       (20)      118 2023-03-22 10:37:43.862607 emrecharge-0.0.8/setup.cfg
--rw-r--r--   0 stevejpurves   (501) staff       (20)     1083 2023-02-10 11:47:27.000000 emrecharge-0.0.8/setup.py
+drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-04-05 08:26:30.494850 emrecharge-0.0.9/
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     1059 2023-02-10 11:47:27.000000 emrecharge-0.0.9/LICENSE.md
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      592 2023-04-05 08:26:30.494910 emrecharge-0.0.9/PKG-INFO
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      154 2023-02-10 12:07:40.000000 emrecharge-0.0.9/README.md
+drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-04-05 08:26:30.493980 emrecharge-0.0.9/emrecharge/
+-rw-r--r--   0 stevejpurves   (501) staff       (20)        0 2023-02-10 11:47:27.000000 emrecharge-0.0.9/emrecharge/__init__.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     4751 2023-02-16 16:01:41.000000 emrecharge-0.0.9/emrecharge/app.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     6445 2023-03-22 10:24:17.000000 emrecharge-0.0.9/emrecharge/colocation.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     3316 2023-04-03 20:24:19.000000 emrecharge-0.0.9/emrecharge/datasets.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     1178 2023-02-10 11:47:27.000000 emrecharge-0.0.9/emrecharge/gis.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     4823 2023-03-07 20:46:54.000000 emrecharge-0.0.9/emrecharge/metrics.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     7805 2023-04-03 20:24:19.000000 emrecharge-0.0.9/emrecharge/rockphysics.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     2404 2023-02-10 11:47:27.000000 emrecharge-0.0.9/emrecharge/utils.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)       22 2023-04-05 08:25:56.000000 emrecharge-0.0.9/emrecharge/version.py
+-rw-r--r--   0 stevejpurves   (501) staff       (20)    14492 2023-04-03 20:24:19.000000 emrecharge-0.0.9/emrecharge/viz.py
+drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-04-05 08:26:30.494744 emrecharge-0.0.9/emrecharge.egg-info/
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      592 2023-04-05 08:26:30.000000 emrecharge-0.0.9/emrecharge.egg-info/PKG-INFO
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      438 2023-04-05 08:26:30.000000 emrecharge-0.0.9/emrecharge.egg-info/SOURCES.txt
+-rw-r--r--   0 stevejpurves   (501) staff       (20)        1 2023-04-05 08:26:30.000000 emrecharge-0.0.9/emrecharge.egg-info/dependency_links.txt
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      115 2023-04-05 08:26:30.000000 emrecharge-0.0.9/emrecharge.egg-info/requires.txt
+-rw-r--r--   0 stevejpurves   (501) staff       (20)       11 2023-04-05 08:26:30.000000 emrecharge-0.0.9/emrecharge.egg-info/top_level.txt
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      103 2023-02-10 11:47:27.000000 emrecharge-0.0.9/pyproject.toml
+-rw-r--r--   0 stevejpurves   (501) staff       (20)      118 2023-04-05 08:26:30.495193 emrecharge-0.0.9/setup.cfg
+-rw-r--r--   0 stevejpurves   (501) staff       (20)     1083 2023-02-10 11:47:27.000000 emrecharge-0.0.9/setup.py
```

### Comparing `emrecharge-0.0.8/LICENSE.md` & `emrecharge-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `emrecharge-0.0.8/PKG-INFO` & `emrecharge-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emrecharge
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for EM Groundwater Recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
```

### Comparing `emrecharge-0.0.8/emrecharge/app.py` & `emrecharge-0.0.9/emrecharge/app.py`

 * *Files identical despite different names*

### Comparing `emrecharge-0.0.8/emrecharge/colocation.py` & `emrecharge-0.0.9/emrecharge/colocation.py`

 * *Files identical despite different names*

### Comparing `emrecharge-0.0.8/emrecharge/datasets.py` & `emrecharge-0.0.9/emrecharge/datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import json
 from collections import namedtuple
-
 import numpy as np
 import pandas as pd
 
 
 class EMDataset:
     filename: str
     df: pd.DataFrame
 
     def __init__(self, csv_filename: str, csv_filename_thickness: str):
         self.filename = csv_filename
         self.filename_thickness = csv_filename_thickness
         self.df = pd.read_csv(
-            self.filename, dtype={"LINE_NO": "Int32", "RECORD": "Int32"}
+            self.filename, dtype={"LINE_NO": "O", "RECORD": "Int32"}
         ).sort_values("RECORD")
         self.df_thickness = pd.read_csv(self.filename_thickness)
 
     @property
     def header(self):
         return list(self.df.columns)
 
     @property
     def line(self):
-        return self.df["LINE_NO"].values.to_numpy(dtype=int)
+        return self.df["LINE_NO"].values
 
     @property
     def timestamps(self):
         return self.df["RECORD"].values.to_numpy(dtype=int)
 
     @property
     def topography(self):
@@ -35,14 +34,18 @@
 
     @property
     def hz(self):
         hz = np.array(json.loads(self.df_thickness.THICKNESS[0]))
         return np.r_[hz, hz[-1]]
 
     @property
+    def depth(self):
+        return np.cumsum(np.r_[0, self.hz])
+
+    @property
     def resistivity(self):
         if getattr(self, "_resistivity", None) is None:
             resistivity = []
             for string in self.df["MEASUREMENTS"]:
                 resistivity.append(json.loads(string)["RHO"])
             self._resistivity = np.vstack(resistivity)
         return self._resistivity
@@ -73,14 +76,31 @@
 
     @property
     def num_layers(self):
         return self.hz.size
 
     def get_resistivity_by_line(self, line_number: int):
         records = self.df[self.df["LINE_NO"] == line_number][["UTMX", "UTMY"]]
-        inds_line = self.df["LINE_NO"].values.to_numpy(dtype=int) == line_number
-        xy = records.values[:, :]
+        inds_line = self.line == line_number
+        xy = self.xy[inds_line,:]
         rho = self.resistivity[inds_line, :]
         delta = np.concatenate(
             [[0], (np.diff(xy[:, 0]) ** 2 + np.diff(xy[:, 1]) ** 2) ** 0.5]
         )
         return rho, delta, xy
+
+    def get_binned_resistivity_by_line(self, line_number: int, n_bins: int, maximum_depth: float):
+        rho, delta, xy = self.get_resistivity_by_line(line_number)
+        distance = np.cumsum(delta)
+        d_max = distance.max()
+        distance_bins = np.linspace(0, d_max, n_bins+1)
+        inds = np.digitize(distance, distance_bins)
+        depth_all = np.cumsum(np.r_[0., self.hz[:-1]])
+        inds_above = depth_all<maximum_depth
+        n_layer = inds_above.sum()
+        rho_bins = np.zeros((n_bins, n_layer), dtype=float) * np.nan
+        for ii in range(n_bins):
+            inds_tmp = inds == ii
+            if inds_tmp.sum() > 0:
+                rho_bins[ii,:] = rho[inds_tmp,:n_layer].mean(axis=0)
+        depth = np.cumsum(np.r_[0., self.hz[:n_layer]])
+        return distance, distance_bins, depth, rho_bins
```

### Comparing `emrecharge-0.0.8/emrecharge/gis.py` & `emrecharge-0.0.9/emrecharge/gis.py`

 * *Files identical despite different names*

### Comparing `emrecharge-0.0.8/emrecharge/metrics.py` & `emrecharge-0.0.9/emrecharge/metrics.py`

 * *Files identical despite different names*

### Comparing `emrecharge-0.0.8/emrecharge/rockphysics.py` & `emrecharge-0.0.9/emrecharge/rockphysics.py`

 * *Files 7% similar despite different names*

```diff
@@ -190,7 +190,24 @@
         func_cf_aboves.append(func_cf_above)
         # func_cf_belows.append(func_cf_below)
 
     # return dict(
     #     func_cf_aboves=func_cf_aboves, func_cf_belows=func_cf_belows, rho=rho_tmp
     # )
     return dict(func_cf_aboves=func_cf_aboves, rho=rho_tmp)
+
+
+def compute_rho_to_cf_mappings_with_rho(
+    rho_fine_above, rho_coarse_above, rho_min, rho_max
+):
+    func_cf_aboves = []
+
+    rho_tmp = np.logspace(np.log10(rho_min), np.log10(rho_max), 500)
+    sigma_above_fine, sigma_above_coarse = (
+        1.0 / rho_fine_above,
+        1.0 / rho_coarse_above,
+    )
+    f_tmp_above = from_sigma_to_fraction(
+        1.0 / rho_tmp, sigma_above_fine, sigma_above_coarse
+    )
+    func_cf_above = interp1d(np.log10(rho_tmp), f_tmp_above)
+    return dict(func_cf_above=func_cf_above, rho=rho_tmp)
```

### Comparing `emrecharge-0.0.8/emrecharge/utils.py` & `emrecharge-0.0.9/emrecharge/utils.py`

 * *Files identical despite different names*

### Comparing `emrecharge-0.0.8/emrecharge/viz.py` & `emrecharge-0.0.9/emrecharge/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class Stitched1DModel(properties.HasProperties):
     topography = properties.Array("topography (x, y, z)", dtype=float, shape=("*", "*"))
 
     physical_property = properties.Array("Physical property", dtype=float)
 
-    line = properties.Array("Line", dtype=float, default=None)
+    # line = properties.Array("Line", dtype=float, default=None)
 
     time_stamp = properties.Array("Time stamp", dtype=float, default=None)
 
     hz = properties.Array("Vertical thickeness of 1D mesh", dtype=float)
 
     def __init__(self, **kwargs):
         super(Stitched1DModel, self).__init__(**kwargs)
```

### Comparing `emrecharge-0.0.8/emrecharge.egg-info/PKG-INFO` & `emrecharge-0.0.9/emrecharge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emrecharge
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for EM Groundwater Recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
```

### Comparing `emrecharge-0.0.8/setup.py` & `emrecharge-0.0.9/setup.py`

 * *Files identical despite different names*

