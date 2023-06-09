# Comparing `tmp/smartem-0.1.2.tar.gz` & `tmp/smartem-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartem-0.1.2.tar", last modified: Mon Oct 24 11:49:19 2022, max compression
+gzip compressed data, was "smartem-0.1.3.tar", last modified: Fri Jun  9 09:19:16 2023, max compression
```

## Comparing `smartem-0.1.2.tar` & `smartem-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.445421 smartem-0.1.2/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1486 2022-06-01 11:07:25.000000 smartem-0.1.2/LICENSE
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1248 2022-10-24 11:49:19.445421 smartem-0.1.2/PKG-INFO
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1046 2022-06-01 12:11:08.000000 smartem-0.1.2/README.rst
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      130 2022-06-01 11:44:37.000000 smartem-0.1.2/pyproject.toml
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1163 2022-10-24 11:49:19.446421 smartem-0.1.2/setup.cfg
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      154 2022-06-01 11:07:25.000000 smartem-0.1.2/setup.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.430421 smartem-0.1.2/src/
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.433421 smartem-0.1.2/src/smartem/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      212 2022-10-24 11:48:01.000000 smartem-0.1.2/src/smartem/__init__.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.437421 smartem-0.1.2/src/smartem/cli/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/cli/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      808 2022-06-01 15:51:48.000000 smartem-0.1.2/src/smartem/cli/change_epu_directory.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1143 2022-09-28 11:51:20.000000 smartem-0.1.2/src/smartem/cli/export.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2864 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/cli/initialise.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      158 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/cli/launch.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2105 2022-06-07 15:03:21.000000 smartem-0.1.2/src/smartem/cli/missing.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1253 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/cli/start.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      883 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/cli/stop.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.440421 smartem-0.1.2/src/smartem/data_model/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     7130 2022-10-05 09:04:05.000000 smartem-0.1.2/src/smartem/data_model/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2375 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/data_model/construct.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    35995 2022-07-14 14:09:47.000000 smartem-0.1.2/src/smartem/data_model/extract.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    11757 2022-06-24 14:10:56.000000 smartem-0.1.2/src/smartem/data_model/structure.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    14898 2022-10-24 11:27:26.000000 smartem-0.1.2/src/smartem/data_model/torch.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.440421 smartem-0.1.2/src/smartem/gui/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/gui/__init__.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.443421 smartem-0.1.2/src/smartem/gui/qt/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    10881 2022-08-08 10:49:51.000000 smartem-0.1.2/src/smartem/gui/qt/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2164 2022-06-20 16:22:21.000000 smartem-0.1.2/src/smartem/gui/qt/component_tab.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    38827 2022-10-24 11:47:57.000000 smartem-0.1.2/src/smartem/gui/qt/display.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12229 2022-09-28 11:51:20.000000 smartem-0.1.2/src/smartem/gui/qt/image_utils.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    24920 2022-06-27 16:06:26.000000 smartem-0.1.2/src/smartem/gui/qt/loader.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     5086 2022-06-23 16:20:23.000000 smartem-0.1.2/src/smartem/gui/qt/loader_csv.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1419 2022-06-24 11:19:21.000000 smartem-0.1.2/src/smartem/gui/qt/plotting_utils.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1289 2022-08-08 11:23:01.000000 smartem-0.1.2/src/smartem/gui/qt/qt_style.css
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.445421 smartem-0.1.2/src/smartem/parsing/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.2/src/smartem/parsing/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    19391 2022-10-05 09:03:24.000000 smartem-0.1.2/src/smartem/parsing/epu.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    13637 2022-10-24 11:27:26.000000 smartem-0.1.2/src/smartem/parsing/export.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     5608 2022-08-05 15:49:38.000000 smartem-0.1.2/src/smartem/parsing/relion_default.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12683 2022-06-27 16:06:15.000000 smartem-0.1.2/src/smartem/parsing/star.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2434 2022-08-05 10:46:09.000000 smartem-0.1.2/src/smartem/stage_model.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2022-10-24 11:49:19.435421 smartem-0.1.2/src/smartem.egg-info/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1248 2022-10-24 11:49:19.000000 smartem-0.1.2/src/smartem.egg-info/PKG-INFO
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1193 2022-10-24 11:49:19.000000 smartem-0.1.2/src/smartem.egg-info/SOURCES.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        1 2022-10-24 11:49:19.000000 smartem-0.1.2/src/smartem.egg-info/dependency_links.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      318 2022-10-24 11:49:19.000000 smartem-0.1.2/src/smartem.egg-info/entry_points.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        1 2022-06-01 11:46:31.000000 smartem-0.1.2/src/smartem.egg-info/not-zip-safe
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)       91 2022-10-24 11:49:19.000000 smartem-0.1.2/src/smartem.egg-info/requires.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        8 2022-10-24 11:49:19.000000 smartem-0.1.2/src/smartem.egg-info/top_level.txt
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.288080 smartem-0.1.3/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1486 2022-06-01 11:07:25.000000 smartem-0.1.3/LICENSE
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1248 2023-06-09 09:19:16.288080 smartem-0.1.3/PKG-INFO
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1046 2022-06-01 12:11:08.000000 smartem-0.1.3/README.rst
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      130 2022-06-01 11:44:37.000000 smartem-0.1.3/pyproject.toml
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1218 2023-06-09 09:19:16.289080 smartem-0.1.3/setup.cfg
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      154 2022-06-01 11:07:25.000000 smartem-0.1.3/setup.py
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.266080 smartem-0.1.3/src/
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.269080 smartem-0.1.3/src/smartem/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      212 2023-06-09 09:16:37.000000 smartem-0.1.3/src/smartem/__init__.py
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.276080 smartem-0.1.3/src/smartem/cli/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/__init__.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      808 2022-06-01 15:51:48.000000 smartem-0.1.3/src/smartem/cli/change_epu_directory.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1143 2022-09-28 11:51:20.000000 smartem-0.1.3/src/smartem/cli/export.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2864 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/initialise.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      158 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/launch.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2105 2022-06-07 15:03:21.000000 smartem-0.1.3/src/smartem/cli/missing.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      717 2023-06-09 09:16:23.000000 smartem-0.1.3/src/smartem/cli/quick_epu_viewer.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1253 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/start.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      883 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/stop.py
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.279080 smartem-0.1.3/src/smartem/data_model/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     7130 2022-10-05 09:04:05.000000 smartem-0.1.3/src/smartem/data_model/__init__.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2375 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/data_model/construct.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    35995 2022-07-14 14:09:47.000000 smartem-0.1.3/src/smartem/data_model/extract.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    11757 2022-06-24 14:10:56.000000 smartem-0.1.3/src/smartem/data_model/structure.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    14708 2023-06-09 09:16:14.000000 smartem-0.1.3/src/smartem/data_model/torch.py
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.279080 smartem-0.1.3/src/smartem/gui/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/gui/__init__.py
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.284079 smartem-0.1.3/src/smartem/gui/qt/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    10881 2022-08-08 10:49:51.000000 smartem-0.1.3/src/smartem/gui/qt/__init__.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2164 2022-06-20 16:22:21.000000 smartem-0.1.3/src/smartem/gui/qt/component_tab.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    38827 2022-10-24 11:47:57.000000 smartem-0.1.3/src/smartem/gui/qt/display.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12229 2022-09-28 11:51:20.000000 smartem-0.1.3/src/smartem/gui/qt/image_utils.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    24920 2022-06-27 16:06:26.000000 smartem-0.1.3/src/smartem/gui/qt/loader.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     5086 2022-06-23 16:20:23.000000 smartem-0.1.3/src/smartem/gui/qt/loader_csv.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1419 2022-06-24 11:19:21.000000 smartem-0.1.3/src/smartem/gui/qt/plotting_utils.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1289 2022-08-08 11:23:01.000000 smartem-0.1.3/src/smartem/gui/qt/qt_style.css
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.287079 smartem-0.1.3/src/smartem/parsing/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/parsing/__init__.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    19542 2023-06-09 09:16:23.000000 smartem-0.1.3/src/smartem/parsing/epu.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12274 2023-06-09 09:16:23.000000 smartem-0.1.3/src/smartem/parsing/epu_vis.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    13637 2022-10-24 11:27:26.000000 smartem-0.1.3/src/smartem/parsing/export.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     5608 2022-08-05 15:49:38.000000 smartem-0.1.3/src/smartem/parsing/relion_default.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12683 2022-06-27 16:06:15.000000 smartem-0.1.3/src/smartem/parsing/star.py
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2434 2022-08-05 10:46:09.000000 smartem-0.1.3/src/smartem/stage_model.py
+drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.272080 smartem-0.1.3/src/smartem.egg-info/
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1248 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/PKG-INFO
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1260 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/SOURCES.txt
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        1 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/dependency_links.txt
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      372 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/entry_points.txt
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        1 2022-06-01 11:46:31.000000 smartem-0.1.3/src/smartem.egg-info/not-zip-safe
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)       91 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/requires.txt
+-rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        8 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/top_level.txt
```

### Comparing `smartem-0.1.2/LICENSE` & `smartem-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/PKG-INFO` & `smartem-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
```

### Comparing `smartem-0.1.2/README.rst` & `smartem-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/setup.cfg` & `smartem-0.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartem
-version = 0.1.2
+version = 0.1.3
 description = Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 long_description = file: README.rst
 license_file = LICENSE
 
 [options]
 include_package_data = True
 install_requires = 
@@ -33,14 +33,15 @@
 	smartem.launch = smartem.cli.launch:run
 	smartem.init = smartem.cli.initialise:run
 	smartem.start = smartem.cli.start:run
 	smartem.stop = smartem.cli.stop:run
 	smartem.missing = smartem.cli.missing:run
 	smartem.export = smartem.cli.export:run
 	smartem.change_epu_dir = smartem.cli.change_epu_directory:run
+	smartem.quick_view = smartem.cli.quick_epu_viewer:run
 
 [options.packages.find]
 where = src
 
 [flake8]
 ignore = E203, E266, E501, W503
 max-line-length = 88
```

### Comparing `smartem-0.1.2/src/smartem/cli/change_epu_directory.py` & `smartem-0.1.3/src/smartem/cli/change_epu_directory.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/cli/export.py` & `smartem-0.1.3/src/smartem/cli/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/cli/initialise.py` & `smartem-0.1.3/src/smartem/cli/initialise.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/cli/missing.py` & `smartem-0.1.3/src/smartem/cli/missing.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/cli/start.py` & `smartem-0.1.3/src/smartem/cli/start.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/cli/stop.py` & `smartem-0.1.3/src/smartem/cli/stop.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/data_model/__init__.py` & `smartem-0.1.3/src/smartem/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/data_model/construct.py` & `smartem-0.1.3/src/smartem/data_model/construct.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/data_model/extract.py` & `smartem-0.1.3/src/smartem/data_model/extract.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/data_model/structure.py` & `smartem-0.1.3/src/smartem/data_model/structure.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/data_model/torch.py` & `smartem-0.1.3/src/smartem/data_model/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,35 +335,23 @@
 
 class SmartEMMaskDataLoader(DataLoader):
     def __init__(self, data_dir: Path, labels_csv: str = "labels.csv"):
         self._data_dir = data_dir
         self._df = (
             pd.read_csv(self._data_dir / labels_csv).groupby("grid_square").mean()
         )
-        if (
-            (self._data_dir / self._df.iloc[0]["grid_square"])
-            .with_suffix(".mrc")
-            .exists()
-        ):
+        if (self._data_dir / self._df.iloc[0].name).with_suffix(".mrc").exists():
             self._full_res_extension = ".mrc"
-        elif (
-            (self._data_dir / self._df.iloc[0]["grid_square"])
-            .with_suffix(".tiff")
-            .exists()
-        ):
+        elif (self._data_dir / self._df.iloc[0].name).with_suffix(".tiff").exists():
             self._full_res_extension = ".tiff"
-        elif (
-            (self._data_dir / self._df.iloc[0]["grid_square"])
-            .with_suffix(".tif")
-            .exists()
-        ):
+        elif (self._data_dir / self._df.iloc[0].name).with_suffix(".tif").exists():
             self._full_res_extension = ".tif"
         else:
             raise FileNotFoundError(
-                f"{self._data_dir / self._df.iloc[0]['grid_square']} was not found with any of the following suffixes: .mrc, .tiff, .tif"
+                f"{self._data_dir / self._df.iloc[0].name} was not found with any of the following suffixes: .mrc, .tiff, .tif"
             )
 
     def __len__(self) -> int:
         return len(self._df.index)
 
     def __getitem__(self, idx: int) -> Tuple[Tensor, Tensor]:
         image_path = (self._data_dir / self._df.iloc[idx].name).with_suffix(
```

### Comparing `smartem-0.1.2/src/smartem/gui/qt/__init__.py` & `smartem-0.1.3/src/smartem/gui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/component_tab.py` & `smartem-0.1.3/src/smartem/gui/qt/component_tab.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/display.py` & `smartem-0.1.3/src/smartem/gui/qt/display.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/image_utils.py` & `smartem-0.1.3/src/smartem/gui/qt/image_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/loader.py` & `smartem-0.1.3/src/smartem/gui/qt/loader.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/loader_csv.py` & `smartem-0.1.3/src/smartem/gui/qt/loader_csv.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/plotting_utils.py` & `smartem-0.1.3/src/smartem/gui/qt/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/gui/qt/qt_style.css` & `smartem-0.1.3/src/smartem/gui/qt/qt_style.css`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/parsing/epu.py` & `smartem-0.1.3/src/smartem/parsing/epu.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,39 +38,14 @@
     version = data["microscopeData"]["core"]["ApplicationSoftwareVersion"]
     return {
         "software": software,
         "version": version,
     }
 
 
-def metadata_foil_hole_positions(xml_path: Path) -> Dict[str, Tuple[int, int]]:
-    with open(xml_path, "r") as xml:
-        for_parsing = xml.read()
-        data = xmltodict.parse(for_parsing)
-    data = data["GridSquareXml"]
-    serialization_array = data["TargetLocations"]["TargetLocationsEfficient"][
-        "a:m_serializationArray"
-    ]
-    required_key = ""
-    for key in serialization_array.keys():
-        if key.startswith("b:KeyValuePairOfintTargetLocation"):
-            required_key = key
-            break
-    if not required_key:
-        return {}
-    fh_pix_positions = {}
-    for fh_block in serialization_array[required_key]:
-        pix_center = fh_block["b:value"]["PixelCenter"]
-        fh_pix_positions[fh_block["b:key"]] = (
-            int(float(pix_center["c:x"])),
-            int(float(pix_center["c:y"])),
-        )
-    return fh_pix_positions
-
-
 def metadata_grid_square_positions(xml_path: Path) -> Dict[str, Tuple[int, int]]:
     with open(xml_path, "r") as xml:
         for_parsing = xml.read()
         data = xmltodict.parse(for_parsing)
     tile_info = data["AtlasSessionXml"]["Atlas"]["TilesEfficient"]["_items"]["TileXml"]
     gs_pix_positions = {}
     for ti in tile_info:
@@ -163,14 +138,40 @@
                     mask[fh[0] - xshift][yidx] = True
                 except IndexError:
                     pass
                 xidx += 1
     return mask.transpose()
 
 
+def metadata_foil_hole_positions(xml_path: Path) -> Dict[str, Tuple[int, int]]:
+    with open(xml_path, "r") as xml:
+        for_parsing = xml.read()
+        data = xmltodict.parse(for_parsing)
+    data = data["GridSquareXml"]
+    serialization_array = data["TargetLocations"]["TargetLocationsEfficient"][
+        "a:m_serializationArray"
+    ]
+    required_key = ""
+    for key in serialization_array.keys():
+        if key.startswith("b:KeyValuePairOfintTargetLocation"):
+            required_key = key
+            break
+    if not required_key:
+        return {}
+    fh_stage_positions = {}
+    for fh_block in serialization_array[required_key]:
+        if fh_block["b:value"]["IsNearGridBar"] == "false":
+            stage = fh_block["b:value"]["PixelCenter"]
+            fh_stage_positions[fh_block["b:key"]] = (
+                int(float(stage["c:x"])),
+                int(float(stage["c:y"])),
+            )
+    return fh_stage_positions
+
+
 def metadata_foil_hole_stage(xml_path: Path) -> Dict[str, Tuple[float, float]]:
     with open(xml_path, "r") as xml:
         for_parsing = xml.read()
         data = xmltodict.parse(for_parsing)
     data = data["GridSquareXml"]
     serialization_array = data["TargetLocations"]["TargetLocationsEfficient"][
         "a:m_serializationArray"
@@ -180,19 +181,20 @@
         if key.startswith("b:KeyValuePairOfintTargetLocation"):
             required_key = key
             break
     if not required_key:
         return {}
     fh_stage_positions = {}
     for fh_block in serialization_array[required_key]:
-        stage = fh_block["b:value"]["StagePosition"]
-        fh_stage_positions[fh_block["b:key"]] = (
-            float(stage["c:X"]) * 1e9,
-            float(stage["c:Y"]) * 1e9,
-        )
+        if fh_block["b:value"]["IsNearGridBar"] == "false":
+            stage = fh_block["b:value"]["StagePosition"]
+            fh_stage_positions[fh_block["b:key"]] = (
+                float(stage["c:X"]) * 1e9,
+                float(stage["c:Y"]) * 1e9,
+            )
     return fh_stage_positions
 
 
 def metadata_foil_hole_corrected_stage(
     xml_path: Path,
 ) -> Dict[str, tuple]:
     with open(xml_path, "r") as xml:
```

### Comparing `smartem-0.1.2/src/smartem/parsing/export.py` & `smartem-0.1.3/src/smartem/parsing/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/parsing/relion_default.py` & `smartem-0.1.3/src/smartem/parsing/relion_default.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/parsing/star.py` & `smartem-0.1.3/src/smartem/parsing/star.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem/stage_model.py` & `smartem-0.1.3/src/smartem/stage_model.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.2/src/smartem.egg-info/PKG-INFO` & `smartem-0.1.3/src/smartem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
```

### Comparing `smartem-0.1.2/src/smartem.egg-info/SOURCES.txt` & `smartem-0.1.3/src/smartem.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/smartem.egg-info/top_level.txt
 src/smartem/cli/__init__.py
 src/smartem/cli/change_epu_directory.py
 src/smartem/cli/export.py
 src/smartem/cli/initialise.py
 src/smartem/cli/launch.py
 src/smartem/cli/missing.py
+src/smartem/cli/quick_epu_viewer.py
 src/smartem/cli/start.py
 src/smartem/cli/stop.py
 src/smartem/data_model/__init__.py
 src/smartem/data_model/construct.py
 src/smartem/data_model/extract.py
 src/smartem/data_model/structure.py
 src/smartem/data_model/torch.py
@@ -32,10 +33,11 @@
 src/smartem/gui/qt/image_utils.py
 src/smartem/gui/qt/loader.py
 src/smartem/gui/qt/loader_csv.py
 src/smartem/gui/qt/plotting_utils.py
 src/smartem/gui/qt/qt_style.css
 src/smartem/parsing/__init__.py
 src/smartem/parsing/epu.py
+src/smartem/parsing/epu_vis.py
 src/smartem/parsing/export.py
 src/smartem/parsing/relion_default.py
 src/smartem/parsing/star.py
```

