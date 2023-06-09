# Comparing `tmp/napari-live-recording-0.2.1.tar.gz` & `tmp/napari-live-recording-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-live-recording-0.2.1.tar", last modified: Mon May  2 11:27:45 2022, max compression
+gzip compressed data, was "napari-live-recording-0.3.0.tar", last modified: Fri Jun  9 18:49:21 2023, max compression
```

## Comparing `napari-live-recording-0.2.1.tar` & `napari-live-recording-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.306490 napari-live-recording-0.2.1/
--rw-rw-rw-   0        0        0     1076 2022-04-11 12:31:00.000000 napari-live-recording-0.2.1/.gitignore
--rw-rw-rw-   0        0        0     1101 2021-10-22 10:11:44.000000 napari-live-recording-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4094 2022-05-02 11:27:45.306490 napari-live-recording-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2700 2022-05-02 11:21:31.000000 napari-live-recording-0.2.1/README.md
--rwxrwxrwx   0        0        0      213 2022-05-02 11:26:56.000000 napari-live-recording-0.2.1/deploy.bat
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.287540 napari-live-recording-0.2.1/docs/
--rw-rw-rw-   0        0        0      112 2022-05-02 11:19:24.000000 napari-live-recording-0.2.1/docs/README.md
--rw-rw-rw-   0        0        0      959 2022-05-02 11:07:37.000000 napari-live-recording-0.2.1/docs/changelog.md
--rw-rw-rw-   0        0        0    11685 2022-05-02 11:16:43.000000 napari-live-recording-0.2.1/docs/interface.md
--rw-rw-rw-   0        0        0       91 2022-04-11 12:42:20.000000 napari-live-recording-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1709 2022-05-02 11:27:45.308495 napari-live-recording-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       87 2022-04-12 11:43:46.000000 napari-live-recording-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.277567 napari-live-recording-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.289536 napari-live-recording-0.2.1/src/napari_live_recording/
--rw-rw-rw-   0        0        0     2426 2022-04-25 12:55:52.000000 napari-live-recording-0.2.1/src/napari_live_recording/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.301503 napari-live-recording-0.2.1/src/napari_live_recording/common/
--rw-rw-rw-   0        0        0       83 2022-04-07 14:13:33.000000 napari-live-recording-0.2.1/src/napari_live_recording/common/__init__.py
--rw-rw-rw-   0        0        0      292 2022-04-07 09:25:11.000000 napari-live-recording-0.2.1/src/napari_live_recording/common/common.py
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.302501 napari-live-recording-0.2.1/src/napari_live_recording/control/
--rw-rw-rw-   0        0        0       31 2022-04-07 09:25:11.000000 napari-live-recording-0.2.1/src/napari_live_recording/control/__init__.py
--rw-rw-rw-   0        0        0     3642 2022-04-26 08:25:27.000000 napari-live-recording-0.2.1/src/napari_live_recording/control/control.py
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.304495 napari-live-recording-0.2.1/src/napari_live_recording/devices/
--rw-rw-rw-   0        0        0     1609 2022-04-11 09:13:24.000000 napari-live-recording-0.2.1/src/napari_live_recording/devices/__init__.py
--rw-rw-rw-   0        0        0     9197 2022-05-02 11:20:36.000000 napari-live-recording-0.2.1/src/napari_live_recording/devices/interface.py
--rw-rw-rw-   0        0        0     4504 2022-05-02 09:40:16.000000 napari-live-recording-0.2.1/src/napari_live_recording/devices/opencv.py
--rw-rw-rw-   0        0        0     9047 2022-05-02 08:49:48.000000 napari-live-recording-0.2.1/src/napari_live_recording/devices/ximea.py
--rw-rw-rw-   0        0        0      299 2022-04-11 12:39:19.000000 napari-live-recording-0.2.1/src/napari_live_recording/napari.yaml
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.306490 napari-live-recording-0.2.1/src/napari_live_recording/widgets/
--rw-rw-rw-   0        0        0      245 2022-04-11 09:13:24.000000 napari-live-recording-0.2.1/src/napari_live_recording/widgets/__init__.py
--rw-rw-rw-   0        0        0    24842 2022-04-26 08:21:14.000000 napari-live-recording-0.2.1/src/napari_live_recording/widgets/widgets.py
-drwxrwxrwx   0        0        0        0 2022-05-02 11:27:45.300505 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/
--rw-rw-rw-   0        0        0     4094 2022-05-02 11:27:44.000000 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      954 2022-05-02 11:27:45.000000 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-02 11:27:44.000000 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2022-05-02 11:27:44.000000 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2022-05-02 11:27:44.000000 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-05-02 11:27:45.000000 napari-live-recording-0.2.1/src/napari_live_recording.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      896 2022-04-11 09:23:02.000000 napari-live-recording-0.2.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.209030 napari-live-recording-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.139921 napari-live-recording-0.3.0/.github/
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.155111 napari-live-recording-0.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0      590 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/.github/workflows/plugin_preview.yml
+-rw-rw-rw-   0        0        0     1076 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1101 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4527 2023-06-09 18:49:21.209030 napari-live-recording-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3206 2023-06-09 18:21:57.000000 napari-live-recording-0.3.0/README.md
+-rwxrwxrwx   0        0        0      213 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/deploy.bat
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.157112 napari-live-recording-0.3.0/docs/
+-rw-rw-rw-   0        0        0       67 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/docs/README.md
+-rw-rw-rw-   0        0        0     1184 2023-06-09 18:45:26.000000 napari-live-recording-0.3.0/docs/changelog.md
+-rw-rw-rw-   0        0        0       91 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1718 2023-06-09 18:49:21.211091 napari-live-recording-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       87 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.141918 napari-live-recording-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.159113 napari-live-recording-0.3.0/src/napari_live_recording/
+-rw-rw-rw-   0        0        0      676 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.197108 napari-live-recording-0.3.0/src/napari_live_recording/common/
+-rw-rw-rw-   0        0        0     2671 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.198110 napari-live-recording-0.3.0/src/napari_live_recording/control/
+-rw-rw-rw-   0        0        0     9015 2023-06-09 18:24:39.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.205108 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/
+-rw-rw-rw-   0        0        0     1585 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/__init__.py
+-rw-rw-rw-   0        0        0     3916 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/interface.py
+-rw-rw-rw-   0        0        0     2655 2023-06-09 18:17:32.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/micro_manager.py
+-rw-rw-rw-   0        0        0     4061 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/control/devices/opencv.py
+-rw-rw-rw-   0        0        0      299 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/src/napari_live_recording/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.207970 napari-live-recording-0.3.0/src/napari_live_recording/ui/
+-rw-rw-rw-   0        0        0     7754 2023-06-09 17:35:28.000000 napari-live-recording-0.3.0/src/napari_live_recording/ui/__init__.py
+-rw-rw-rw-   0        0        0    24878 2023-06-09 18:25:13.000000 napari-live-recording-0.3.0/src/napari_live_recording/ui/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:49:21.195109 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/
+-rw-rw-rw-   0        0        0     4527 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-06-09 18:49:21.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-09 18:49:20.000000 napari-live-recording-0.3.0/src/napari_live_recording.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      896 2023-01-27 10:07:39.000000 napari-live-recording-0.3.0/tox.ini
```

### Comparing `napari-live-recording-0.2.1/.gitignore` & `napari-live-recording-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.2.1/LICENSE` & `napari-live-recording-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-live-recording-0.2.1/PKG-INFO` & `napari-live-recording-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: napari-live-recording
-Version: 0.2.1
+Version: 0.3.0
 Summary: A napari plugin for live video recording with a generic camera device.
 Home-page: https://github.com/jethro33/napari-live-recording
 Author: Jacopo Abramo
 Author-email: jacopo.abramo@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jacopoabramo/napari-live-recording/issues
 Project-URL: Documentation, https://github.com/jacopoabramo/napari-live-recording#README.md
 Project-URL: Source Code, https://github.com/jacopoabramo/napari-live-recording
 Project-URL: User Support, https://github.com/jacopoabramo/napari-live-recording/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # napari-live-recording
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/jacopoabramo/napari-live-recording/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-live-recording.svg?color=green)](https://pypi.org/project/napari-live-recording)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-live-recording.svg?color=green)](https://python.org)
 [![tests](https://github.com/jethro33/napari-live-recording/workflows/tests/badge.svg)](https://github.com/jacopoabramo/napari-live-recording/actions)
 [![codecov](https://codecov.io/gh/jethro33/napari-live-recording/branch/master/graph/badge.svg)](https://codecov.io/gh/jacopoabramo/napari-live-recording)
 
 A napari plugin for live video recording with a generic camera device and generate a stack of TIFF images from said device.
 
+The plugin provides a common interface for a generic camera device to be directly controlled from the napari GUI. The plugin can
+
+- acquire continously in live view;
+- record a stack of images and store them as ImageJ-compatible TIFF, OME-TIFF or HDF5 files.
+
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
@@ -52,14 +55,20 @@
 
 ## Installation
 
 You can install `napari-live-recording` via [pip]:
 
     pip install napari-live-recording
 
+If you want to install the plugin using the source code, you can do so by cloning the project and installing locally:
+
+    git clone https://github.com/jacopoabramo/napari-live-recording
+    cd napari-live-recording
+    pip install .
+
 ## Documentation
 
 You can review the documentation of this plugin [here](./docs/README.md)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
@@ -87,9 +96,7 @@
 
 [file an issue]: https://github.com/jacopoabramo/napari-live-recording/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-live-recording-0.2.1/README.md` & `napari-live-recording-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 [![PyPI](https://img.shields.io/pypi/v/napari-live-recording.svg?color=green)](https://pypi.org/project/napari-live-recording)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-live-recording.svg?color=green)](https://python.org)
 [![tests](https://github.com/jethro33/napari-live-recording/workflows/tests/badge.svg)](https://github.com/jacopoabramo/napari-live-recording/actions)
 [![codecov](https://codecov.io/gh/jethro33/napari-live-recording/branch/master/graph/badge.svg)](https://codecov.io/gh/jacopoabramo/napari-live-recording)
 
 A napari plugin for live video recording with a generic camera device and generate a stack of TIFF images from said device.
 
+The plugin provides a common interface for a generic camera device to be directly controlled from the napari GUI. The plugin can
+
+- acquire continously in live view;
+- record a stack of images and store them as ImageJ-compatible TIFF, OME-TIFF or HDF5 files.
+
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
@@ -22,14 +27,20 @@
 
 ## Installation
 
 You can install `napari-live-recording` via [pip]:
 
     pip install napari-live-recording
 
+If you want to install the plugin using the source code, you can do so by cloning the project and installing locally:
+
+    git clone https://github.com/jacopoabramo/napari-live-recording
+    cd napari-live-recording
+    pip install .
+
 ## Documentation
 
 You can review the documentation of this plugin [here](./docs/README.md)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
```

### Comparing `napari-live-recording-0.2.1/docs/changelog.md` & `napari-live-recording-0.3.0/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Changelog
 
+## 0.3.0
+
+- Full rework of the plugin architecture ad user interface (hopefully for the last time)
+- Removed old device interface documentation
+- Fixed issues #16, #17
+- Added MicroManager interface (@felixwanitschke)
+
 ## 0.2.1
 
-- Added documentation of new architecture.
+- Added documentation of new architecture
 
 ## 0.2.0
 
 - Full architecture rework
 - Deleted old documentation
 - Adapted plugin to be compatible with `npe2`
```

### Comparing `napari-live-recording-0.2.1/setup.cfg` & `napari-live-recording-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 6c69 7665 2d72   = napari-live-r
 00000020: 6563 6f72 6469 6e67 0d0a 7665 7273 696f  ecording..versio
-00000030: 6e20 3d20 302e 322e 310d 0a61 7574 686f  n = 0.2.1..autho
+00000030: 6e20 3d20 302e 332e 300d 0a61 7574 686f  n = 0.3.0..autho
 00000040: 7220 3d20 4a61 636f 706f 2041 6272 616d  r = Jacopo Abram
 00000050: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000060: 3d20 6a61 636f 706f 2e61 6272 616d 6f40  = jacopo.abramo@
 00000070: 676d 6169 6c2e 636f 6d0d 0a75 726c 203d  gmail.com..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6a65 7468 726f 3333 2f6e 6170  com/jethro33/nap
 000000a0: 6172 692d 6c69 7665 2d72 6563 6f72 6469  ari-live-recordi
@@ -33,75 +33,76 @@
 00000200: 696e 670d 0a09 5072 6f67 7261 6d6d 696e  ing...Programmin
 00000210: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 00000220: 7468 6f6e 0d0a 0950 726f 6772 616d 6d69  thon...Programmi
 00000230: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 00000240: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
 00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 2e36 0d0a 0950 726f 6772 616d 6d69 6e67  .6...Programming
+00000270: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
 00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000290: 686f 6e20 3a3a 2033 2e37 0d0a 0950 726f  hon :: 3.7...Pro
+00000290: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
 000002a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000002b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002c0: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-000002d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002e0: 686f 6e20 3a3a 2033 2e39 0d0a 094f 7065  hon :: 3.9...Ope
-000002f0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000300: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000310: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000320: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000330: 204c 6963 656e 7365 0d0a 0954 6f70 6963   License...Topic
-00000340: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-00000350: 6e67 696e 6565 7269 6e67 203a 3a20 496d  ngineering :: Im
-00000360: 6167 6520 5072 6f63 6573 7369 6e67 0d0a  age Processing..
-00000370: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-00000380: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-00000390: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000003a0: 6f6d 2f6a 6163 6f70 6f61 6272 616d 6f2f  om/jacopoabramo/
-000003b0: 6e61 7061 7269 2d6c 6976 652d 7265 636f  napari-live-reco
-000003c0: 7264 696e 672f 6973 7375 6573 0d0a 0944  rding/issues...D
-000003d0: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
-000003e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003f0: 6d2f 6a61 636f 706f 6162 7261 6d6f 2f6e  m/jacopoabramo/n
-00000400: 6170 6172 692d 6c69 7665 2d72 6563 6f72  apari-live-recor
-00000410: 6469 6e67 2352 4541 444d 452e 6d64 0d0a  ding#README.md..
-00000420: 0953 6f75 7263 6520 436f 6465 203d 2068  .Source Code = h
-00000430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000440: 6d2f 6a61 636f 706f 6162 7261 6d6f 2f6e  m/jacopoabramo/n
-00000450: 6170 6172 692d 6c69 7665 2d72 6563 6f72  apari-live-recor
-00000460: 6469 6e67 0d0a 0955 7365 7220 5375 7070  ding...User Supp
-00000470: 6f72 7420 3d20 6874 7470 733a 2f2f 6769  ort = https://gi
-00000480: 7468 7562 2e63 6f6d 2f6a 6163 6f70 6f61  thub.com/jacopoa
-00000490: 6272 616d 6f2f 6e61 7061 7269 2d6c 6976  bramo/napari-liv
-000004a0: 652d 7265 636f 7264 696e 672f 6973 7375  e-recording/issu
-000004b0: 6573 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  es....[options].
-000004c0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-000004d0: 3a0d 0a69 6e63 6c75 6465 5f70 6163 6b61  :..include_packa
-000004e0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-000004f0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000500: 203d 200d 0a09 7375 7065 7271 740d 0a09   = ...superqt...
-00000510: 6e75 6d70 790d 0a09 6f70 656e 6376 2d70  numpy...opencv-p
-00000520: 7974 686f 6e0d 0a09 6f70 656e 6376 2d63  ython...opencv-c
-00000530: 6f6e 7472 6962 2d70 7974 686f 6e0d 0a09  ontrib-python...
-00000540: 6461 736b 5f69 6d61 6765 0d0a 096e 6170  dask_image...nap
-00000550: 6172 690d 0a09 7174 7079 0d0a 7079 7468  ari...qtpy..pyth
-00000560: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000570: 332e 360d 0a70 6163 6b61 6765 5f64 6972  3.6..package_dir
-00000580: 203d 200d 0a09 3d73 7263 0d0a 7365 7475   = ...=src..setu
-00000590: 705f 7265 7175 6972 6573 203d 200d 0a09  p_requires = ...
-000005a0: 7365 7475 7074 6f6f 6c73 2d73 636d 0d0a  setuptools-scm..
-000005b0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000005c0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-000005d0: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-000005e0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-000005f0: 0d0a 6e61 7061 7269 2e6d 616e 6966 6573  ..napari.manifes
-00000600: 7420 3d20 0d0a 096e 6170 6172 692d 6c69  t = ...napari-li
-00000610: 7665 2d72 6563 6f72 6469 6e67 203d 206e  ve-recording = n
-00000620: 6170 6172 695f 6c69 7665 5f72 6563 6f72  apari_live_recor
-00000630: 6469 6e67 3a6e 6170 6172 692e 7961 6d6c  ding:napari.yaml
-00000640: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000650: 6b61 6765 5f64 6174 615d 0d0a 6e61 7061  kage_data]..napa
-00000660: 7269 2d6c 6976 652d 7265 636f 7264 696e  ri-live-recordin
-00000670: 6720 3d20 6e61 7061 7269 2e79 616d 6c0d  g = napari.yaml.
-00000680: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000690: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000006a0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000002c0: 2e31 300d 0a09 4f70 6572 6174 696e 6720  .10...Operating 
+000002d0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000002e0: 6570 656e 6465 6e74 0d0a 094c 6963 656e  ependent...Licen
+000002f0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000300: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000310: 650d 0a09 546f 7069 6320 3a3a 2053 6369  e...Topic :: Sci
+00000320: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000330: 696e 6720 3a3a 2049 6d61 6765 2050 726f  ing :: Image Pro
+00000340: 6365 7373 696e 670d 0a70 726f 6a65 6374  cessing..project
+00000350: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
+00000360: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+00000370: 2f67 6974 6875 622e 636f 6d2f 6a61 636f  /github.com/jaco
+00000380: 706f 6162 7261 6d6f 2f6e 6170 6172 692d  poabramo/napari-
+00000390: 6c69 7665 2d72 6563 6f72 6469 6e67 2f69  live-recording/i
+000003a0: 7373 7565 730d 0a09 446f 6375 6d65 6e74  ssues...Document
+000003b0: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
+000003c0: 6769 7468 7562 2e63 6f6d 2f6a 6163 6f70  github.com/jacop
+000003d0: 6f61 6272 616d 6f2f 6e61 7061 7269 2d6c  oabramo/napari-l
+000003e0: 6976 652d 7265 636f 7264 696e 6723 5245  ive-recording#RE
+000003f0: 4144 4d45 2e6d 640d 0a09 536f 7572 6365  ADME.md...Source
+00000400: 2043 6f64 6520 3d20 6874 7470 733a 2f2f   Code = https://
+00000410: 6769 7468 7562 2e63 6f6d 2f6a 6163 6f70  github.com/jacop
+00000420: 6f61 6272 616d 6f2f 6e61 7061 7269 2d6c  oabramo/napari-l
+00000430: 6976 652d 7265 636f 7264 696e 670d 0a09  ive-recording...
+00000440: 5573 6572 2053 7570 706f 7274 203d 2068  User Support = h
+00000450: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000460: 6d2f 6a61 636f 706f 6162 7261 6d6f 2f6e  m/jacopoabramo/n
+00000470: 6170 6172 692d 6c69 7665 2d72 6563 6f72  apari-live-recor
+00000480: 6469 6e67 2f69 7373 7565 730d 0a0d 0a5b  ding/issues....[
+00000490: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+000004a0: 6573 203d 2066 696e 643a 0d0a 696e 636c  es = find:..incl
+000004b0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+000004c0: 203d 2054 7275 650d 0a69 6e73 7461 6c6c   = True..install
+000004d0: 5f72 6571 7569 7265 7320 3d20 0d0a 0973  _requires = ...s
+000004e0: 7570 6572 7174 0d0a 096e 756d 7079 0d0a  uperqt...numpy..
+000004f0: 096e 705f 696d 6167 655f 6275 6666 6572  .np_image_buffer
+00000500: 0d0a 096f 7065 6e63 762d 7079 7468 6f6e  ...opencv-python
+00000510: 0d0a 096f 7065 6e63 762d 636f 6e74 7269  ...opencv-contri
+00000520: 622d 7079 7468 6f6e 0d0a 0974 6966 6666  b-python...tifff
+00000530: 696c 650d 0a09 6835 7079 0d0a 096e 6170  ile...h5py...nap
+00000540: 6172 690d 0a09 7174 7079 0d0a 0970 796d  ari...qtpy...pym
+00000550: 6d63 6f72 652d 706c 7573 203e 3d20 302e  mcore-plus >= 0.
+00000560: 362e 370d 0a70 7974 686f 6e5f 7265 7175  6.7..python_requ
+00000570: 6972 6573 203d 203e 3d33 2e38 0d0a 7061  ires = >=3.8..pa
+00000580: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000590: 7372 630d 0a73 6574 7570 5f72 6571 7569  src..setup_requi
+000005a0: 7265 7320 3d20 0d0a 0973 6574 7570 746f  res = ...setupto
+000005b0: 6f6c 732d 7363 6d0d 0a0d 0a5b 6f70 7469  ols-scm....[opti
+000005c0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000005d0: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+000005e0: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
+000005f0: 795f 706f 696e 7473 5d0d 0a6e 6170 6172  y_points]..napar
+00000600: 692e 6d61 6e69 6665 7374 203d 200d 0a09  i.manifest = ...
+00000610: 6e61 7061 7269 2d6c 6976 652d 7265 636f  napari-live-reco
+00000620: 7264 696e 6720 3d20 6e61 7061 7269 5f6c  rding = napari_l
+00000630: 6976 655f 7265 636f 7264 696e 673a 6e61  ive_recording:na
+00000640: 7061 7269 2e79 616d 6c0d 0a0d 0a5b 6f70  pari.yaml....[op
+00000650: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000660: 7461 5d0d 0a6e 6170 6172 692d 6c69 7665  ta]..napari-live
+00000670: 2d72 6563 6f72 6469 6e67 203d 206e 6170  -recording = nap
+00000680: 6172 692e 7961 6d6c 0d0a 0d0a 5b65 6767  ari.yaml....[egg
+00000690: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000006a0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000006b0: 2030 0d0a 0d0a                            0....
```

### Comparing `napari-live-recording-0.2.1/src/napari_live_recording/devices/__init__.py` & `napari-live-recording-0.3.0/src/napari_live_recording/control/devices/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from inspect import isclass, getmembers
 from pkgutil import iter_modules
 from pathlib import Path
 from importlib import import_module
-from napari_live_recording.devices.interface import ICamera
+from .interface import ICamera
 
 package_dir = Path(__file__).resolve().parent
 devicesDict = {}
 
 # iterate through the modules of the devices module
 # in order to find all submodules containing the class definitions
 # of all cameras
-for (_, module_name, _) in iter_modules([package_dir]):
+for (_, module_name, _) in iter_modules([str(package_dir)]):
     # import the modulte and iterate through the attributes
     try:
         # we skip the interface module
         if module_name != "interface":
             module = import_module(f"{__name__}.{module_name}")
             for attr in getmembers(module, isclass):
                 # attr[0]: class name as string
```

### Comparing `napari-live-recording-0.2.1/src/napari_live_recording/widgets/widgets.py` & `napari-live-recording-0.3.0/src/napari_live_recording/ui/widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,552 +1,561 @@
+import os
+import numpy as np
 from typing import Union
 from qtpy.QtCore import Qt, QObject, Signal, QTimer
 from qtpy.QtWidgets import (
-    QWidget, 
-    QLabel, 
-    QComboBox, 
-    QSpinBox, 
-    QDoubleSpinBox, 
-    QLineEdit, 
-    QPushButton
+    QWidget,
+    QLabel,
+    QComboBox,
+    QSpinBox,
+    QLineEdit,
+    QPushButton,
+    QFileDialog,
+    QStackedWidget,
 )
-from superqt import QLabeledSlider
+from superqt import QLabeledSlider, QLabeledDoubleSlider, QEnumComboBox
 from qtpy.QtWidgets import QFormLayout, QGridLayout, QGroupBox
 from abc import ABC, abstractmethod
 from dataclasses import replace
-from napari_live_recording.common import ROI
+from napari_live_recording.common import ROI, FileFormat, RecordType, MMC_DEVICE_MAP
 from enum import Enum
+from typing import Dict, List, Tuple
+
 
 class Timer(QTimer):
     pass
 
+
 class WidgetEnum(Enum):
-    ComboBox = 0,
-    SpinBox = 1,
-    DoubleSpinBox = 2,
-    LabeledSlider = 3,
+    ComboBox = (0,)
+    SpinBox = (1,)
+    DoubleSpinBox = (2,)
+    LabeledSlider = (3,)
     LineEdit = 4
 
+
 class LocalWidget(ABC):
-    def __init__(self, internalWidget : QWidget, name: str, unit: str = "", orientation: str = "left") -> None:
+    def __init__(
+        self,
+        internalWidget: QWidget,
+        name: str,
+        unit: str = "",
+        orientation: str = "left",
+    ) -> None:
         """Common widget constructor.
 
         Args:
             internalWidget (QWidget): widget to construct the form layout.
             name (str): parameter label description.
             unit (str, optional): parameter unit measure. Defaults to "".
             orientation (str, optional): label orientation on the layout. Defaults to "left".
         """
+        super().__init__()
         self.__name = name
         self.__unit = unit
-        labelStr = (self.__name + " (" + self.__unit + ")" if self.__unit != "" else self.__name)
+        labelStr = (
+            self.__name + " (" + self.__unit + ")" if self.__unit != "" else self.__name
+        )
         self.label = QLabel(labelStr)
         self.label.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.widget = internalWidget
-    
+
     @property
     def isEnabled(self) -> bool:
-        """Widget is enabled for editing (True) or not (False).
-        """
+        """Widget is enabled for editing (True) or not (False)."""
         return self.widget.isEnabled()
-    
+
     @isEnabled.setter
-    def isEnabled(self, enable : bool) -> None:
-        """Sets widget enabled for editing (True) or not (False).
-        """
+    def isEnabled(self, enable: bool) -> None:
+        """Sets widget enabled for editing (True) or not (False)."""
         self.widget.setEnabled(enable)
 
     @abstractmethod
     def changeWidgetSettings(self, newParam) -> None:
-        """Common widget update parameter abstract method.
-        """
+        """Common widget update parameter abstract method."""
         pass
 
     @property
     @abstractmethod
     def value(self) -> None:
-        """Widget current value.
-        """
+        """Widget current value."""
         pass
 
     @value.setter
     @abstractmethod
     def value(self, value: Union[str, int, float]) -> None:
-        """Widget value setter.
-        """
+        """Widget value setter."""
         pass
-    
+
     @property
     @abstractmethod
-    def signals(self) -> dict[str, Signal]:
-        """Common widget method to expose signals to the device.
-        """
+    def signals(self) -> Dict[str, Signal]:
+        """Common widget method to expose signals to the device."""
         pass
 
+
 class ComboBox(LocalWidget):
-    def __init__(self, param : list[str], name : str, unit : str = "", orientation: str = "left") -> None:
+    def __init__(
+        self, param: List[str], name: str, unit: str = "", orientation: str = "left"
+    ) -> None:
         """ComboBox widget.
 
         Args:
-            param (list[str]): list of parameters added to the ComboBox.
+            param (List[str]): List of parameters added to the ComboBox.
             name (str): parameter label description.
             unit (str, optional): parameter unit measure. Defaults to "".
             orientation (str, optional): label orientation on the layout. Defaults to "left".
         """
         self.combobox = QComboBox()
         self.combobox.addItems(param)
         super().__init__(self.combobox, name, unit, orientation)
-    
-    def changeWidgetSettings(self, newParam: list[str]) -> None:
-        """ComboBox update widget parameter method. Old list of items is deleted.
+
+    def changeWidgetSettings(self, newParam: List[str]) -> None:
+        """ComboBox update widget parameter method. Old List of items is deleted.
 
         Args:
-            newParam (list[str]): new list of parameters to add to the ComboBox.
+            newParam (List[str]): new List of parameters to add to the ComboBox.
         """
         self.combobox.clear()
         self.combobox.addItems(newParam)
-    
+
     @property
-    def value(self) -> tuple[str, int]:
-        """Returns a tuple containing the ComboBox current text and index.
-        """
+    def value(self) -> Tuple[str, int]:
+        """Returns a Tuple containing the ComboBox current text and index."""
         return (self.combobox.currentText(), self.combobox.currentIndex())
-    
+
     @value.setter
     def value(self, value: int) -> None:
         """Sets the ComboBox current showed value (based on elements indeces).
 
         Args:
             value (int): index of value to show on the ComboBox.
         """
         self.combobox.setCurrentIndex(value)
-    
+
     @property
-    def signals(self) -> dict[str, Signal]:
+    def signals(self) -> Dict[str, Signal]:
         """Returns a dictionary of signals available for the ComboBox widget.
         Exposed signals are:
-        
+
         - currentIndexChanged,
         - currentTextChanged
 
         Returns:
-            dict: dict of signals (key: function name, value: function objects).
+            Dict: Dict of signals (key: function name, value: function objects).
         """
         return {
-            "currentIndexChanged" : self.combobox.currentIndexChanged,
-            "currentTextChanged" : self.combobox.currentTextChanged
+            "currentIndexChanged": self.combobox.currentIndexChanged,
+            "currentTextChanged": self.combobox.currentTextChanged,
         }
-        
-
-class SpinBox(LocalWidget):
-    def __init__(self, param: tuple[int, int, int], name: str, unit: str = "", orientation: str = "left") -> None:
-        """SpinBox widget.
 
-        Args:
-            param (tuple[int, int, int]): parameters for SpinBox settings: (<minimum_value>, <maximum_value>, <starting_value>)
-            name (str): parameter label description.
-            unit (str, optional): parameter unit measure. Defaults to "".
-            orientation (str, optional): label orientation on the layout. Defaults to "left".
-        """
-        self.spinbox = QSpinBox()
-        self.spinbox.lineEdit().setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.spinbox.setRange(param[0], param[1])
-        self.spinbox.setValue(param[2])
-        super().__init__(self.spinbox, name, unit, orientation)
-    
-    def changeWidgetSettings(self, newParam : tuple[int, int, int]) -> None:
-        """SpinBox update widget parameter method.
-
-        Args:
-            newParam (tuple(int, int, int)): new parameters for SpinBox settings: (<minimum_value>, <maximum_value>, <starting_value>)
-        """
-        self.spinbox.setRange(newParam[0], newParam[1])
-        self.spinbox.setValue(newParam[2])
-    
-    @property
-    def value(self) -> int:
-        """Returns the SpinBox current value.
-        """
-        return self.spinbox.value()
-    
-    @value.setter
-    def value(self, value: int) -> None:
-        """Sets the SpinBox current value to show on the widget.
-
-        Args:
-            value (int): value to set.
-        """
-        self.spinbox.setValue(value)
-    
-    @property
-    def signals(self) -> dict[str, Signal]:
-        """Returns a dictionary of signals available for the SpinBox widget.
-        Exposed signals are:
-        
-        - valueChanged,
-        - textChanged
-
-        Returns:
-            dict: dict of signals (key: function name, value: function objects).
-        """
-        return {
-            "valueChanged" : self.spinbox.valueChanged,
-            "textChanged" : self.spinbox.textChanged
-        }
-
-class DoubleSpinBox(LocalWidget):
-    def __init__(self, param: tuple[float, float, float], name: str, unit: str = "", orientation: str = "left") -> None:
-        """DoubleSpinBox widget.
-
-        Args:
-            param (tuple[float, float, float]): parameters for spinbox settings: (<minimum_value>, <maximum_value>, <starting_value>)
-            name (str): parameter label description.
-            unit (str, optional): parameter unit measure. Defaults to "".
-            orientation (str, optional): label orientation on the layout. Defaults to "left".
-        """
-        self.__spinbox = QDoubleSpinBox()
-        self.__spinbox.setRange(param[0], param[1])
-        self.__spinbox.setValue(param[2])
-        super().__init__(self.__spinbox, name, unit, orientation)
-
-    def changeWidgetSettings(self, newParam : tuple[float, float, float]) -> None:
-        """DoubleSpinBox update widget parameter method.
-
-        Args:
-            newParam (tuple[float, float, float]): new parameters for SpinBox settings: (<minimum_value>, <maximum_value>, <starting_value>)
-        """
-        self.__spinbox.setRange(newParam[0], newParam[1])
-        self.__spinbox.setValue(newParam[2])
-    
-    @property
-    def value(self) -> float:
-        """Returns the DoubleSpinBox current value.
-        """
-        return self.__spinbox.value()
-    
-    @value.setter
-    def value(self, value: float) -> None:
-        """Sets the DoubleSpinBox current value to show on the widget.
-
-        Args:
-            value (float): value to set.
-        """
-        self.__spinbox.setValue(value)
-
-    @property
-    def signals(self) -> dict[str, Signal]:
-        """Returns a dictionary of signals available for the SpinBox widget.
-        Exposed signals are:
-        
-        - valueChanged,
-        - textChanged
-
-        Returns:
-            dict: dict of signals (key: function name, value: function objects).
-        """
-        return {
-            "valueChanged" : self.__spinbox.valueChanged,
-            "textChanged" : self.__spinbox.textChanged
-        }
 
 class LabeledSlider(LocalWidget):
-    def __init__(self, param: tuple[int, int, int], name: str, unit: str = "", orientation: str = "left") -> None:
+    def __init__(
+        self,
+        param: Union[Tuple[int, int, int], Tuple[float, float, float]],
+        name: str,
+        unit: str = "",
+        orientation: str = "left",
+    ) -> None:
         """Slider widget.
 
         Args:
-            param (tuple[int, int, int])): parameters for spinbox settings: (<minimum_value>, <maximum_value>, <starting_value>)
+            param (Tuple[int, int, int])): parameters for spinbox settings: (<minimum_value>, <maximum_value>, <starting_value>)
             name (str): parameter label description.
             unit (str, optional): parameter unit measure. Defaults to "".
             orientation (str, optional): label orientation on the layout. Defaults to "left".
         """
-        self.__slider = QLabeledSlider(Qt.Horizontal)
+        if any(isinstance(parameter, float) for parameter in param):
+            self.__slider = QLabeledDoubleSlider(Qt.Horizontal)
+        else:
+            self.__slider = QLabeledSlider(Qt.Horizontal)
         self.__slider.setRange(param[0], param[1])
         self.__slider.setValue(param[2])
         super().__init__(self.__slider, name, unit, orientation)
-    
-    def changeWidgetSettings(self, newParam : tuple[int, int, int]) -> None:
+
+    def changeWidgetSettings(self, newParam: Tuple[int, int, int]) -> None:
         """Slider update widget parameter method.
 
         Args:
-            newParam (tuple[int, int, int]): new parameters for SpinBox settings: (<minimum_value>, <maximum_value>, <starting_value>)
+            newParam (Tuple[int, int, int]): new parameters for SpinBox settings: (<minimum_value>, <maximum_value>, <starting_value>)
         """
         self.__slider.setRange(newParam[0], newParam[1])
         self.__slider.setValue(newParam[2])
-    
+
     @property
     def value(self) -> int:
-        """Returns the Slider current value.
-        """
+        """Returns the Slider current value."""
         return self.__slider.value()
-    
+
     @value.setter
     def value(self, value: int) -> None:
         """Sets the DoubleSpinBox current value to show on the widget.
 
         Args:
             value (float): value to set.
         """
         self.__slider.setValue(value)
 
     @property
-    def signals(self) -> dict[str, Signal]:
+    def signals(self) -> Dict[str, Signal]:
         """Returns a dictionary of signals available for the SpinBox widget.
         Exposed signals are:
-        
+
         - valueChanged
 
         Returns:
-            dict: dict of signals (key: function name, value: function objects).
+            Dict: Dict of signals (key: function name, value: function objects).
         """
-        return {
-            "valueChanged" : self.__slider.valueChanged
-        }
+        return {"valueChanged": self.__slider.valueChanged}
+
 
 class LineEdit(LocalWidget):
-    
-    def __init__(self, param: str, name: str, unit: str = "", orientation: str = "left") -> None:
+    def __init__(
+        self, param: str, name: str, unit: str = "", orientation: str = "left"
+    ) -> None:
         """LineEdit widget.
 
         Args:
             param (str): line edit contents
             name (str): parameter label description.
             unit (str, optional): parameter unit measure. Defaults to "".
             orientation (str, optional): label orientation on the layout. Defaults to "left".
             editable (bool, optional): sets the LineEdit to be editable. Defaults to False.
         """
         self.__lineEdit = QLineEdit(param)
         super().__init__(self.__lineEdit, name, unit, orientation)
-    
-    def changeWidgetSettings(self, newParam : str) -> None:
+
+    def changeWidgetSettings(self, newParam: str) -> None:
         """Updates LineEdit text contents.
 
         Args:
             newParam (str): new string for LineEdit.
         """
         self.__lineEdit.setText(newParam)
 
     @property
     def value(self) -> str:
-        """Returns the LineEdit current text.
-        """
+        """Returns the LineEdit current text."""
         return self.__lineEdit.text()
-    
+
     @value.setter
     def value(self, value: str) -> None:
         """Sets the LineEdit current text to show on the widget.
 
         Args:
             value (str): string to set.
         """
         self.__lineEdit.setText(value)
-    
+
     @property
-    def signals(self) -> dict[str, Signal]:
+    def signals(self) -> Dict[str, Signal]:
         """Returns a dictionary of signals available for the LineEdit widget.
         Exposed signals are:
-        
+
         - textChanged,
         - textEdited
 
         Returns:
-            dict: dict of signals (key: function name, value: function objects).
+            Dict: Dict of signals (key: function name, value: function objects).
         """
         return {
-            "textChanged" : self.__lineEdit.textChanged,
-            "textEdited" : self.__lineEdit.textEdited
+            "textChanged": self.__lineEdit.textChanged,
+            "textEdited": self.__lineEdit.textEdited,
         }
 
+
 class CameraSelection(QObject):
     newCameraRequested = Signal(str, str, str)
 
     def __init__(self) -> None:
         """Camera selection widget. It includes the following widgets:
 
         - a ComboBox for camera selection based on strings to identify each camera type;
         - a LineEdit for camera ID or serial number input
         - a QPushButton to add the camera
 
         Widget grid layout:
         |(0,0-1) ComboBox                |(0,2) QPushButton|
         |(1,0) LineEdit|Line Edit(1,1)   |(1,2)            |
 
-        The QPushButton remains disabled as long as no camera is selected (first index is highlited). 
+        The QPushButton remains disabled as long as no camera is selected (first index is highlited).
         """
-        super(CameraSelection, self).__init__()        
+        super(CameraSelection, self).__init__()
         self.group = QGroupBox()
+        self.layout = QFormLayout()
+        self.stackedWidget = QStackedWidget()
         self.camerasComboBox = ComboBox([], "Interface")
         self.nameLineEdit = LineEdit(param="MyCamera", name="Camera name")
         self.idLineEdit = LineEdit(param="0", name="Camera ID/SN", orientation="right")
+        self.adapterComboBox = ComboBox(
+            list(MMC_DEVICE_MAP.keys()), name="Adapter", orientation="right"
+        )
+        self.deviceComboBox = ComboBox([], name="Device", orientation="right")
         self.addButton = QPushButton("Add camera")
-        self.addButton.setEnabled(False)
 
-        # create widget layout
+        self.camerasComboBox.signals["currentIndexChanged"].connect(self.changeWidget)
+        self.adapterComboBox.signals["currentIndexChanged"].connect(
+            self.updateDeviceSelectionUI
+        )
         self.camerasComboBox.signals["currentIndexChanged"].connect(self._setAddEnabled)
-        self.addButton.clicked.connect(lambda: self.newCameraRequested.emit(self.camerasComboBox.value[0], self.nameLineEdit.value, self.idLineEdit.value))
-
-        self.formLayout = QFormLayout()
-        self.formLayout.addRow(self.camerasComboBox.label, self.camerasComboBox.widget)
-        self.formLayout.addRow(self.nameLineEdit.label, self.nameLineEdit.widget)
-        self.formLayout.addRow(self.idLineEdit.label, self.idLineEdit.widget)
-        self.formLayout.addRow(self.addButton)
-        self.group.setLayout(self.formLayout)
-        self.group.setFlat(True)
+        self.addButton.clicked.connect(
+            lambda: self.newCameraRequested.emit(
+                self.camerasComboBox.value[0],
+                self.nameLineEdit.value,
+                (self.adapterComboBox.value[0] + " " + self.deviceComboBox.value[0])
+                if self.camerasComboBox.value[0] == "MicroManager"
+                else self.idLineEdit.value,
+            )
+        )
 
-    def setAvailableCameras(self, cameras: list[str]) -> None:
-        """Sets the ComboBox with the list of available camera devices.
+    def setAvailableCameras(self, cameras: List[str]) -> None:
+        """Sets the ComboBox with the List of available camera devices.
 
         Args:
-            cameras (list[str]): list of available camera devices.
+            cameras (List[str]): List of available camera devices.
         """
-        # we need to extend the list of available cameras with a selection text
+        # we need to extend the List of available cameras with a selection text
         cameras.insert(0, "Select device")
         self.camerasComboBox.changeWidgetSettings(cameras)
         self.camerasComboBox.isEnabled = True
-    
+
+    def setDeviceSelectionWidget(self, cameras: List[str]) -> None:
+        cameras.insert(0, "Select device")
+        self.stackWidgets = {}
+        self.stackLayouts = {}
+        for camera in cameras:
+            self.stackWidgets[camera] = QWidget()
+            self.stackLayouts[camera] = QFormLayout()
+            if camera == "MicroManager":
+                self.stackLayouts[camera].addRow(
+                    self.adapterComboBox.label, self.adapterComboBox.widget
+                )
+                self.stackLayouts[camera].addRow(
+                    self.deviceComboBox.label, self.deviceComboBox.widget
+                )
+            else:
+                self.stackLayouts[camera].addRow(
+                    self.idLineEdit.label, self.idLineEdit.widget
+                )
+
+            self.stackWidgets[camera].setLayout(self.stackLayouts[camera])
+            self.stackedWidget.addWidget(self.stackWidgets[camera])
+
+        self.layout.addRow(self.camerasComboBox.label, self.camerasComboBox.widget)
+        self.layout.addRow(self.nameLineEdit.label, self.nameLineEdit.widget)
+        self.layout.addRow(self.stackedWidget)
+        self.layout.addRow(self.addButton)
+
+        self.group.setLayout(self.layout)
+        self.group.setFlat(True)
+
+    def changeWidget(self, idx):
+        self.stackedWidget.setCurrentIndex(idx)
+
+    def updateDeviceSelectionUI(self, idx):
+        self.deviceComboBox.changeWidgetSettings(
+            MMC_DEVICE_MAP[list(MMC_DEVICE_MAP.keys())[idx]]
+        )
+
     def _setAddEnabled(self, idx: int):
         """Private method serving as an enable/disable mechanism for the Add button widget.
         This is done to avoid the first index, the "Select device" string, to be considered
         as a valid camera device (which is not).
         """
         if idx > 0:
             self.addButton.setEnabled(True)
         else:
             self.addButton.setEnabled(False)
 
 
 class RecordHandling(QObject):
     recordRequested = Signal(int)
+
     def __init__(self) -> None:
         """Recording Handling widget. Includes QPushButtons which allow to handle the following operations:
 
         - live viewing;
         - recording to output file;
         - single frame snap;
-        - album stacking snap.
 
         Widget layout:
-        |(0,0) QPushButton (Snap)|(0,1) QPushButton (Album)|(0,2) QPushButton  (Live) |
-        |(1,0-1)          QSpinBox (Record size)           |(0,2) QPushButton (Record)| 
+        |(0,1-2)   QComboBox (File Format)               |(0,2)   QLabel   |
+        |(1,0-1)   QLineEdit (Folder selection)          |(1,2) QPushButton|
+        |(2,0-2)   QLineEdit (Record filename)           |(2,2)   QLabel   |
+        |(3,0-2)   QSpinBox (Record size)                |(3,2)   QLabel   |
+        |(4,0-2)                  QPushButton (Snap)                       |
+        |(5,0-2)                  QPushButton (Live)                       |
+        |(6,0-2)                  QPushButton (Record)                     |
 
         """
         QObject.__init__(self)
 
         self.group = QGroupBox()
         self.layout = QGridLayout()
 
+        self.formatLabel = QLabel("File format")
+        self.formatComboBox = QEnumComboBox(enum_class=FileFormat)
+        self.formatLabel.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.folderTextEdit = QLineEdit(
+            os.path.join(os.path.expanduser("~"), "Documents")
+        )
+        self.folderTextEdit.setReadOnly(True)
+        self.folderButton = QPushButton("Select record folder")
+
+        self.filenameTextEdit = QLineEdit("Filename")
+        self.filenameLabel = QLabel("Record filename")
+        self.filenameLabel.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.recordComboBox = QEnumComboBox(enum_class=RecordType)
+
+        self.recordSpinBox = QSpinBox()
+        self.recordSpinBox.lineEdit().setAlignment(Qt.AlignmentFlag.AlignCenter)
+        self.recordSpinBox.setRange(1, np.iinfo(np.uint16).max)
+        self.recordSpinBox.setValue(100)
+
         self.snap = QPushButton("Snap")
-        self.album = QPushButton("Album")
         self.live = QPushButton("Live")
+        self.record = QPushButton("Record")
 
-        # the live button is implemented as a toggle button
         self.live.setCheckable(True)
+        self.record.setCheckable(True)
 
         self.recordSpinBox = QSpinBox()
         self.recordSpinBox.lineEdit().setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         # todo: this is currently hardcoded
         # maybe should find a way to initialize
         # from outside the instance?
         self.recordSpinBox.setRange(1, 5000)
         self.recordSpinBox.setValue(100)
+        self.record.setCheckable(True)
 
-        self.record = QPushButton("Record")
-        
-        self.layout.addWidget(self.snap, 0, 0)
-        self.layout.addWidget(self.album, 0, 1)
-        self.layout.addWidget(self.live, 0, 2)
-        self.layout.addWidget(self.recordSpinBox, 1, 0, 1, 2)
-        self.layout.addWidget(self.record, 1, 2)
+        self.layout.addWidget(self.formatComboBox, 0, 0, 1, 2)
+        self.layout.addWidget(self.formatLabel, 0, 2)
+        self.layout.addWidget(self.folderTextEdit, 1, 0, 1, 2)
+        self.layout.addWidget(self.folderButton, 1, 2)
+        self.layout.addWidget(self.filenameTextEdit, 2, 0, 1, 2)
+        self.layout.addWidget(self.filenameLabel, 2, 2)
+        self.layout.addWidget(self.recordSpinBox, 3, 0, 1, 2)
+        self.layout.addWidget(self.recordComboBox, 3, 2)
+        self.layout.addWidget(self.snap, 4, 0, 1, 3)
+        self.layout.addWidget(self.live, 5, 0, 1, 3)
+        self.layout.addWidget(self.record, 6, 0, 1, 3)
         self.group.setLayout(self.layout)
+        self.group.setFlat(True)
+
+        self.live.toggled.connect(self.handleLiveToggled)
+        self.record.toggled.connect(self.handleRecordToggled)
+
+        self.folderButton.clicked.connect(self.handleFolderSelection)
+        self.recordComboBox.currentEnumChanged.connect(self.handleRecordTypeChanged)
+
+    def handleFolderSelection(self) -> None:
+        """Handles the selection of the output folder for the recording."""
+        folder = QFileDialog.getExistingDirectory(
+            self.group, "Select output folder", self.folderTextEdit.text()
+        )
+        if folder:
+            self.folderTextEdit.setText(folder)
+
+    def handleRecordTypeChanged(self, recordType: RecordType) -> None:
+        """Handles the change of the record type.
 
-        # whenever the live button is toggled,
-        # the other pushbutton must be enabled/disabled
-        # in order to avoid undefined behaviors
-        # when grabbing frames from the device
-        self.live.toggled.connect(self._handleLiveToggled)
-    
-    def setWidgetsEnabling(self, isEnabled : bool) -> None:
-        """ Enables/Disables all record handling widgets. """
+        Args:
+            recordType (RecordType): new record type.
+        """
+        if recordType == RecordType["Toggled"]:
+            self.recordSpinBox.setEnabled(False)
+            self.recordSpinBox.hide()
+        else:
+            self.recordSpinBox.show()
+            self.recordSpinBox.setEnabled(True)
+            if recordType == RecordType["Number of frames"]:
+                newVal = 100
+            elif recordType == RecordType["Time (seconds)"]:
+                newVal = 1
+            self.recordSpinBox.setValue(newVal)
+
+    def setWidgetsEnabling(self, isEnabled: bool) -> None:
+        """Enables/Disables all record handling widgets."""
         self.snap.setEnabled(isEnabled)
-        self.album.setEnabled(isEnabled)
         self.live.setEnabled(isEnabled)
         self.record.setEnabled(isEnabled)
         self.recordSpinBox.setEnabled(isEnabled)
 
-    def _handleLiveToggled(self, status: bool) -> None:
+    def handleLiveToggled(self, status: bool) -> None:
         """Enables/Disables pushbuttons when the live button is toggled.
 
         Args:
             status (bool): new live button status.
         """
         self.snap.setEnabled(not status)
-        self.album.setEnabled(not status)
         self.record.setEnabled(not status)
-    
+
+    def handleRecordToggled(self, status: bool) -> None:
+        """Enables/Disables pushbuttons when the record button is toggled.
+
+        Args:
+            status (bool): new live button status.
+        """
+        self.snap.setEnabled(not status)
+        self.live.setEnabled(not status)
+        self.recordSpinBox.setEnabled(not status)
+
     @property
     def recordSize(self) -> int:
-        """Returns the record size currently indicated in the QSpinBox widget.
-        """
+        """Returns the record size currently indicated in the QSpinBox widget."""
         return self.recordSpinBox.value()
 
     @property
-    def signals(self) -> dict[str, Signal]:
+    def signals(self) -> Dict[str, Signal]:
         """Returns a dictionary of signals available for the RecordHandling widget.
         Exposed signals are:
-        
+
         - snapRequested,
         - albumRequested,
         - liveRequested,
         - recordRequested
 
         Returns:
-            dict: dict of signals (key: function name, value: function objects).
+            Dict: Dict of signals (key: function name, value: function objects).
         """
         return {
-            "snapRequested" : self.snap.clicked,
-            "albumRequested" : self.album.clicked,
-            "liveRequested" : self.live.toggled,
-            "recordRequested" : self.record.clicked,
+            "snapRequested": self.snap.clicked,
+            "liveRequested": self.live.toggled,
+            "recordRequested": self.record.toggled,
         }
 
-class ROIHandling(QObject):
+
+class ROIHandling(QWidget):
     changeROIRequested = Signal(ROI)
     fullROIRequested = Signal(ROI)
-    def __init__(self, sensorShape : ROI) -> None:
+
+    def __init__(self, sensorShape: ROI) -> None:
         """ROI Handling widget. Defines a set of non-custom widgets to set the Region Of Interest of the device.
         This widget is common for all devices.
-
-        Args:
-            cameraROI (ROI): data describing the device sensor shape and step value to increment/decrement each parameter.
         """
-        QObject.__init__(self)
-        # todo: maybe this is inefficient...
-        # in previous implementation
-        # copying the reference would cause
-        # issues when changing the ROI
-        # so we'll create a local copy
-        # and discard the input
+        QWidget.__init__(self)
+
         self.sensorFullROI = replace(sensorShape)
 
-        # todo: these widgets are not
-        # our custom LocalWidgets
-        # but since they are common
-        # for all types of cameras
-        # it is not worth to customize them...
-        # ... right?
         self.offsetXLabel = QLabel("Offset X (px)")
         self.offsetXLabel.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.offsetXSpinBox = QSpinBox()
         self.offsetXSpinBox.lineEdit().setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.offsetXSpinBox.setRange(0, self.sensorFullROI.width)
         self.offsetXSpinBox.setSingleStep(self.sensorFullROI.ofs_x_step)
         self.offsetXSpinBox.setValue(0)
 
-        self.offsetYLabel = QLabel("Offset Y (px)", )
+        self.offsetYLabel = QLabel(
+            "Offset Y (px)",
+        )
         self.offsetYLabel.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.offsetYSpinBox = QSpinBox()
         self.offsetYSpinBox.lineEdit().setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.offsetYSpinBox.setRange(0, self.sensorFullROI.height)
         self.offsetYSpinBox.setSingleStep(self.sensorFullROI.ofs_y_step)
         self.offsetYSpinBox.setValue(0)
@@ -568,37 +577,36 @@
         self.heightSpinBox.setRange(0, self.sensorFullROI.height)
         self.heightSpinBox.setSingleStep(self.sensorFullROI.height_step)
         self.heightSpinBox.setValue(self.sensorFullROI.height)
 
         self.changeROIButton = QPushButton("Set ROI")
         self.fullROIButton = QPushButton("Full frame")
 
-        self.layout = QGridLayout()
-        self.layout.addWidget(self.offsetXLabel, 0, 0)
-        self.layout.addWidget(self.offsetXSpinBox, 0, 1)
-        self.layout.addWidget(self.offsetYSpinBox, 0, 2)
-        self.layout.addWidget(self.offsetYLabel, 0, 3)
-        
-        self.layout.addWidget(self.widthLabel, 1, 0)
-        self.layout.addWidget(self.widthSpinBox, 1, 1)
-        self.layout.addWidget(self.heightSpinBox, 1, 2)
-        self.layout.addWidget(self.heightLabel, 1, 3)
-        self.layout.addWidget(self.changeROIButton, 2, 0, 1, 2)
-        self.layout.addWidget(self.fullROIButton, 2, 2, 1, 2)
+        layout = QGridLayout()
+        layout.addWidget(self.offsetXLabel, 0, 0)
+        layout.addWidget(self.offsetXSpinBox, 0, 1)
+        layout.addWidget(self.offsetYSpinBox, 0, 2)
+        layout.addWidget(self.offsetYLabel, 0, 3)
+
+        layout.addWidget(self.widthLabel, 1, 0)
+        layout.addWidget(self.widthSpinBox, 1, 1)
+        layout.addWidget(self.heightSpinBox, 1, 2)
+        layout.addWidget(self.heightLabel, 1, 3)
+        layout.addWidget(self.changeROIButton, 2, 0, 1, 2)
+        layout.addWidget(self.fullROIButton, 2, 2, 1, 2)
 
         # "clicked" signals are connected to private slots.
         # These slots expose the signals available to the user
         # to process the new ROI information if necessary.
         self.changeROIButton.clicked.connect(self._onROIChanged)
         self.fullROIButton.clicked.connect(self._onFullROI)
 
-        self.group = QGroupBox()
-        self.group.setLayout(self.layout)
-    
-    def changeWidgetSettings(self, settings : ROI):
+        self.setLayout(layout)
+
+    def changeWidgetSettings(self, settings: ROI):
         """ROI handling update widget settings method.
         This method is useful whenever the ROI values are changed based
         on some device requirements and adapted.
 
         Args:
             settings (ROI): new ROI settings to change the widget values and steps.
         """
@@ -606,50 +614,48 @@
         self.offsetXSpinBox.setValue(settings.offset_x)
 
         self.offsetYSpinBox.setSingleStep(settings.ofs_y_step)
         self.offsetYSpinBox.setValue(settings.offset_y)
 
         self.widthSpinBox.setSingleStep(settings.width_step)
         self.widthSpinBox.setValue(settings.width)
-        
+
         self.heightSpinBox.setSingleStep(settings.height_step)
         self.heightSpinBox.setValue(settings.height)
-        
-    
+
     def _onROIChanged(self) -> None:
-        """Private slot for ROI changed button pressed. Exposes a signal with the updated ROI settings.
-        """
+        """Private slot for ROI changed button pressed. Exposes a signal with the updated ROI settings."""
         # read the current SpinBoxes status
         newRoi = ROI(
             offset_x=self.offsetXSpinBox.value(),
             ofs_x_step=self.offsetXSpinBox.singleStep(),
             offset_y=self.offsetYSpinBox.value(),
-            ofs_y_step=self.offsetXSpinBox.singleStep(),            
+            ofs_y_step=self.offsetXSpinBox.singleStep(),
             width=self.widthSpinBox.value(),
             width_step=self.widthSpinBox.singleStep(),
             height=self.heightSpinBox.value(),
-            height_step=self.heightSpinBox.singleStep()
+            height_step=self.heightSpinBox.singleStep(),
         )
         self.changeROIRequested.emit(newRoi)
 
     def _onFullROI(self) -> None:
         """Private slot for full ROI button pressed. Exposes a signal with the full ROI settings.
         It also returns the widget settings to their original value.
         """
         self.changeWidgetSettings(self.sensorFullROI)
         self.fullROIRequested.emit(replace(self.sensorFullROI))
-    
+
     @property
-    def signals(self) -> dict[str, Signal]:
+    def signals(self) -> Dict[str, Signal]:
         """Returns a dictionary of signals available for the ROIHandling widget.
         Exposed signals are:
-        
+
         - changeROIRequested,
         - fullROIRequested,
 
         Returns:
-            dict: dict of signals (key: function name, value: function objects).
+            Dict: Dict of signals (key: function name, value: function objects).
         """
         return {
-            "changeROIRequested" : self.changeROIRequested,
-            "fullROIRequested" : self.fullROIRequested,
-        }
+            "changeROIRequested": self.changeROIRequested,
+            "fullROIRequested": self.fullROIRequested,
+        }
```

### Comparing `napari-live-recording-0.2.1/src/napari_live_recording.egg-info/PKG-INFO` & `napari-live-recording-0.3.0/src/napari_live_recording.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: napari-live-recording
-Version: 0.2.1
+Version: 0.3.0
 Summary: A napari plugin for live video recording with a generic camera device.
 Home-page: https://github.com/jethro33/napari-live-recording
 Author: Jacopo Abramo
 Author-email: jacopo.abramo@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jacopoabramo/napari-live-recording/issues
 Project-URL: Documentation, https://github.com/jacopoabramo/napari-live-recording#README.md
 Project-URL: Source Code, https://github.com/jacopoabramo/napari-live-recording
 Project-URL: User Support, https://github.com/jacopoabramo/napari-live-recording/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # napari-live-recording
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/jacopoabramo/napari-live-recording/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-live-recording.svg?color=green)](https://pypi.org/project/napari-live-recording)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-live-recording.svg?color=green)](https://python.org)
 [![tests](https://github.com/jethro33/napari-live-recording/workflows/tests/badge.svg)](https://github.com/jacopoabramo/napari-live-recording/actions)
 [![codecov](https://codecov.io/gh/jethro33/napari-live-recording/branch/master/graph/badge.svg)](https://codecov.io/gh/jacopoabramo/napari-live-recording)
 
 A napari plugin for live video recording with a generic camera device and generate a stack of TIFF images from said device.
 
+The plugin provides a common interface for a generic camera device to be directly controlled from the napari GUI. The plugin can
+
+- acquire continously in live view;
+- record a stack of images and store them as ImageJ-compatible TIFF, OME-TIFF or HDF5 files.
+
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
@@ -52,14 +55,20 @@
 
 ## Installation
 
 You can install `napari-live-recording` via [pip]:
 
     pip install napari-live-recording
 
+If you want to install the plugin using the source code, you can do so by cloning the project and installing locally:
+
+    git clone https://github.com/jacopoabramo/napari-live-recording
+    cd napari-live-recording
+    pip install .
+
 ## Documentation
 
 You can review the documentation of this plugin [here](./docs/README.md)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
@@ -87,9 +96,7 @@
 
 [file an issue]: https://github.com/jacopoabramo/napari-live-recording/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-live-recording-0.2.1/src/napari_live_recording.egg-info/SOURCES.txt` & `napari-live-recording-0.3.0/src/napari_live_recording.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 LICENSE
 README.md
 deploy.bat
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/plugin_preview.yml
 docs/README.md
 docs/changelog.md
-docs/interface.md
 src/napari_live_recording/__init__.py
 src/napari_live_recording/napari.yaml
 src/napari_live_recording.egg-info/PKG-INFO
 src/napari_live_recording.egg-info/SOURCES.txt
 src/napari_live_recording.egg-info/dependency_links.txt
 src/napari_live_recording.egg-info/entry_points.txt
 src/napari_live_recording.egg-info/requires.txt
 src/napari_live_recording.egg-info/top_level.txt
 src/napari_live_recording/common/__init__.py
-src/napari_live_recording/common/common.py
 src/napari_live_recording/control/__init__.py
-src/napari_live_recording/control/control.py
-src/napari_live_recording/devices/__init__.py
-src/napari_live_recording/devices/interface.py
-src/napari_live_recording/devices/opencv.py
-src/napari_live_recording/devices/ximea.py
-src/napari_live_recording/widgets/__init__.py
-src/napari_live_recording/widgets/widgets.py
+src/napari_live_recording/control/devices/__init__.py
+src/napari_live_recording/control/devices/interface.py
+src/napari_live_recording/control/devices/micro_manager.py
+src/napari_live_recording/control/devices/opencv.py
+src/napari_live_recording/ui/__init__.py
+src/napari_live_recording/ui/widgets.py
```

### Comparing `napari-live-recording-0.2.1/tox.ini` & `napari-live-recording-0.3.0/tox.ini`

 * *Files identical despite different names*

