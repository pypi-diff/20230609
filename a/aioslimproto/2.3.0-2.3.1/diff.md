# Comparing `tmp/aioslimproto-2.3.0.tar.gz` & `tmp/aioslimproto-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioslimproto-2.3.0.tar", last modified: Thu Jun  8 22:39:48 2023, max compression
+gzip compressed data, was "aioslimproto-2.3.1.tar", last modified: Fri Jun  9 05:38:05 2023, max compression
```

## Comparing `aioslimproto-2.3.0.tar` & `aioslimproto-2.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.537163 aioslimproto-2.3.0/aioslimproto/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/aioslimproto/font/
--rw-r--r--   0 runner    (1001) docker     (123)   480716 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   540048 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   448868 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   499228 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   438596 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   504492 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   309664 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   201752 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   289124 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   209552 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   303604 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   475244 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   569008 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.537163 aioslimproto-2.3.0/aioslimproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:38:05.822280 aioslimproto-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-09 05:38:05.822280 aioslimproto-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:38:05.814280 aioslimproto-2.3.1/aioslimproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:38:05.818280 aioslimproto-2.3.1/aioslimproto/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   480716 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   540048 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   448868 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   499228 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   438596 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   504492 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   309664 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   201752 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   289124 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   209552 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   303604 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   475244 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   569008 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/aioslimproto/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:38:05.814280 aioslimproto-2.3.1/aioslimproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-09 05:38:05.000000 aioslimproto-2.3.1/aioslimproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-09 05:38:05.000000 aioslimproto-2.3.1/aioslimproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:38:05.000000 aioslimproto-2.3.1/aioslimproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 05:38:05.000000 aioslimproto-2.3.1/aioslimproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 05:38:05.000000 aioslimproto-2.3.1/aioslimproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:38:05.000000 aioslimproto-2.3.1/aioslimproto.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-09 05:38:05.822280 aioslimproto-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-09 05:37:54.000000 aioslimproto-2.3.1/setup.py
```

### Comparing `aioslimproto-2.3.0/LICENSE` & `aioslimproto-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/PKG-INFO` & `aioslimproto-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.3.0/aioslimproto/cli.py` & `aioslimproto-2.3.1/aioslimproto/cli.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/client.py` & `aioslimproto-2.3.1/aioslimproto/client.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/const.py` & `aioslimproto-2.3.1/aioslimproto/const.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/discovery.py` & `aioslimproto-2.3.1/aioslimproto/discovery.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/display.py` & `aioslimproto-2.3.1/aioslimproto/display.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Bold.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Condensed.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Mono.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Oblique.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans.ttf` & `aioslimproto-2.3.1/aioslimproto/font/DejaVu-Sans.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/server.py` & `aioslimproto-2.3.1/aioslimproto/server.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/util.py` & `aioslimproto-2.3.1/aioslimproto/util.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/visualisation.py` & `aioslimproto-2.3.1/aioslimproto/visualisation.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto/volume.py` & `aioslimproto-2.3.1/aioslimproto/volume.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/aioslimproto.egg-info/PKG-INFO` & `aioslimproto-2.3.1/aioslimproto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.3.0/aioslimproto.egg-info/SOURCES.txt` & `aioslimproto-2.3.1/aioslimproto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/setup.cfg` & `aioslimproto-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.0/setup.py` & `aioslimproto-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README_FILE = PROJECT_DIR / "README.md"
 REQUIREMENTS_FILE = PROJECT_DIR / "requirements.txt"
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
 PROJECT_REQ_PYTHON_VERSION = "3.9"
 
 setup(
     name="aioslimproto",
-    version="2.3.0",
+    version="2.3.1",
     license="Apache License 2.0",
     url="https://github.com/music-assistant/aioslimproto",
     author="Marcel van der Veldt",
     author_email="marcelveldt@users.noreply.github.com",
     description="Python module to talk to Logitech Squeezebox players directly (without Logitech server).",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
```

