# Comparing `tmp/multireg-0.0.5.tar.gz` & `tmp/multireg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multireg-0.0.5.tar", last modified: Fri Jun  9 09:07:46 2023, max compression
+gzip compressed data, was "multireg-0.0.6.tar", last modified: Fri Jun  9 09:13:06 2023, max compression
```

## Comparing `multireg-0.0.5.tar` & `multireg-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.5/LICENSE
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.5/MANIFEST.in
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:07:46.334839 multireg-0.0.5/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3566 2023-06-09 08:56:32.000000 multireg-0.0.5/README.md
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.5/pyproject.toml
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1499 2023-06-09 09:07:46.334839 multireg-0.0.5/setup.cfg
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.5/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/src/multireg/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    25211 2023-06-09 09:06:24.000000 multireg-0.0.5/src/multireg/MultiReg.py
--rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.5/src/multireg/Utils.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.5/src/multireg/__init__.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.5/src/multireg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:07:46.334839 multireg-0.0.5/src/multireg.egg-info/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/SOURCES.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/dependency_links.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/entry_points.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       84 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/requires.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 09:07:46.000000 multireg-0.0.5/src/multireg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:13:06.031406 multireg-0.0.6/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.6/LICENSE
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.6/MANIFEST.in
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:13:06.031406 multireg-0.0.6/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3566 2023-06-09 08:56:32.000000 multireg-0.0.6/README.md
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.6/pyproject.toml
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1499 2023-06-09 09:13:06.031406 multireg-0.0.6/setup.cfg
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.6/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:13:06.031406 multireg-0.0.6/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:13:06.031406 multireg-0.0.6/src/multireg/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    24872 2023-06-09 09:12:46.000000 multireg-0.0.6/src/multireg/MultiReg.py
+-rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.6/src/multireg/Utils.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.6/src/multireg/__init__.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.6/src/multireg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:13:06.031406 multireg-0.0.6/src/multireg.egg-info/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:13:06.000000 multireg-0.0.6/src/multireg.egg-info/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 09:13:06.000000 multireg-0.0.6/src/multireg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 09:13:06.000000 multireg-0.0.6/src/multireg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 09:13:06.000000 multireg-0.0.6/src/multireg.egg-info/entry_points.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       84 2023-06-09 09:13:06.000000 multireg-0.0.6/src/multireg.egg-info/requires.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 09:13:06.000000 multireg-0.0.6/src/multireg.egg-info/top_level.txt
```

### Comparing `multireg-0.0.5/LICENSE` & `multireg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multireg-0.0.5/PKG-INFO` & `multireg-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
```

### Comparing `multireg-0.0.5/README.md` & `multireg-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `multireg-0.0.5/pyproject.toml` & `multireg-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multireg-0.0.5/setup.cfg` & `multireg-0.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multireg
-version = 0.0.5
+version = 0.0.6
 description = Registration of 3D multiplex images with one common chanel
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/multireg
 project_urls =
```

### Comparing `multireg-0.0.5/src/multireg/MultiReg.py` & `multireg-0.0.6/src/multireg/MultiReg.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,18 +212,15 @@
             side_by_side_view=False, 
             To_edit="Select a point ('3') \n Press 'u' or 'd' to move it up or down \n Change its label below:",
             selected_point_label=0,
             set_label = False,
             save_points = False,
             ):
         if "Moving points" in viewer.window._dock_widgets:
-            wid = viewer.window._dock_widgets["Moving points"]
-            wid.disconnect()
-            del viewer.window._dock_widgets["Moving points"]
-            wid.destroyOnClose()
+            remove_widget("Moving points")
             viewer.grid.enabled = False
         calc_alignement()
         return
 
     def save_points():
         save_points_file(movname, "movingPoints")
 
@@ -546,19 +543,15 @@
     remove_widget("Calculate alignement")
     remove_layer("movingPoints")
     remove_layer("movingImg"+"_C"+str(refchanel))
     #for chan in range(movimg.shape[0]):
     #    remove_layer("imageAligned"+str(chan))
     remove_layer("alignedMovingImg")
     del movimg
-    if "Apply alignement" in viewer.window._dock_widgets:
-        wid = viewer.window._dock_widgets["Apply alignement"]
-        wid.disconnect()
-        del viewer.window._dock_widgets["Apply alignement"]
-        wid.destroyOnClose()
+    remove_widget("Apply alignement")
 
 def remove_layer(layname):
     if layname in viewer.layers:
         viewer.layers.remove(layname)
 
 def save_points_file(imname, layname):
     points_fixed = viewer.layers[layname]
```

### Comparing `multireg-0.0.5/src/multireg/Utils.py` & `multireg-0.0.6/src/multireg/Utils.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.5/src/multireg.egg-info/PKG-INFO` & `multireg-0.0.6/src/multireg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
```

