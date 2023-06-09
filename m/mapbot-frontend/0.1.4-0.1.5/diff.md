# Comparing `tmp/mapbot_frontend-0.1.4.tar.gz` & `tmp/mapbot_frontend-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapbot_frontend-0.1.4.tar", last modified: Fri Jun  9 15:43:22 2023, max compression
+gzip compressed data, was "mapbot_frontend-0.1.5.tar", last modified: Fri Jun  9 15:57:56 2023, max compression
```

## Comparing `mapbot_frontend-0.1.4.tar` & `mapbot_frontend-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.246986 mapbot_frontend-0.1.4/
--rw-r--r--   0 martinweiss   (501) staff       (20)       34 2023-06-09 15:43:19.000000 mapbot_frontend-0.1.4/MANIFEST.in
--rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 15:43:22.246681 mapbot_frontend-0.1.4/PKG-INFO
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.229990 mapbot_frontend-0.1.4/frontend/
--rw-r--r--   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:18:47.000000 mapbot_frontend-0.1.4/frontend/__init__.py
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.231382 mapbot_frontend-0.1.4/frontend/build/
--rw-r--r--   0 martinweiss   (501) staff       (20)      890 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/asset-manifest.json
--rw-r--r--   0 martinweiss   (501) staff       (20)   197459 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/bootstrap.min.css
--rw-r--r--   0 martinweiss   (501) staff       (20)     3066 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/index.html
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.235315 mapbot_frontend-0.1.4/frontend/build/mapillary/
--rw-r--r--   0 martinweiss   (501) staff       (20)     2437 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/construction--flat--driveway.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     2729 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/marking--discrete--other-marking.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1305 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--banner.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     3209 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--banner.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1793 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--bench.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)      931 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--catch-basin.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1760 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--junction-box.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1002 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--mailbox.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1366 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--advertisement.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     2711 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--advertisement.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1371 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--store.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     3318 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--store.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1075 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--street-light.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     1436 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--street-light.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1227 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--support--utility-pole.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     1638 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--support--utility-pole.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1384 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--traffic-cone.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     1155 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--traffic-cone.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     2429 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.4/frontend/build/mapillary/object--trash-can.svg
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.229414 mapbot_frontend-0.1.4/frontend/build/static/
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.235922 mapbot_frontend-0.1.4/frontend/build/static/css/
--rw-r--r--   0 martinweiss   (501) staff       (20)    34837 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/css/2.45e7f682.chunk.css
--rw-r--r--   0 martinweiss   (501) staff       (20)    40852 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/css/2.45e7f682.chunk.css.map
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.245773 mapbot_frontend-0.1.4/frontend/build/static/js/
--rw-r--r--   0 martinweiss   (501) staff       (20)  1515566 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/2.c035aebc.chunk.js
--rw-r--r--   0 martinweiss   (501) staff       (20)     1399 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/2.c035aebc.chunk.js.LICENSE.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)  6332675 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/2.c035aebc.chunk.js.map
--rw-r--r--   0 martinweiss   (501) staff       (20)    14337 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/main.2bcb2eaa.chunk.js
--rw-r--r--   0 martinweiss   (501) staff       (20)    41945 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/main.2bcb2eaa.chunk.js.map
--rw-r--r--   0 martinweiss   (501) staff       (20)     1566 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/runtime-main.48f3c07e.js
--rw-r--r--   0 martinweiss   (501) staff       (20)     8351 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.4/frontend/build/static/js/runtime-main.48f3c07e.js.map
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:43:22.246430 mapbot_frontend-0.1.4/mapbot_frontend.egg-info/
--rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 15:43:22.000000 mapbot_frontend-0.1.4/mapbot_frontend.egg-info/PKG-INFO
--rw-r--r--   0 martinweiss   (501) staff       (20)     1716 2023-06-09 15:43:22.000000 mapbot_frontend-0.1.4/mapbot_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 15:43:22.000000 mapbot_frontend-0.1.4/mapbot_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)        9 2023-06-09 15:43:22.000000 mapbot_frontend-0.1.4/mapbot_frontend.egg-info/top_level.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 15:43:22.247044 mapbot_frontend-0.1.4/setup.cfg
--rw-r--r--   0 martinweiss   (501) staff       (20)      377 2023-06-09 15:15:31.000000 mapbot_frontend-0.1.4/setup.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.566936 mapbot_frontend-0.1.5/
+-rw-r--r--   0 martinweiss   (501) staff       (20)       50 2023-06-09 15:57:28.000000 mapbot_frontend-0.1.5/MANIFEST.in
+-rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 15:57:56.566597 mapbot_frontend-0.1.5/PKG-INFO
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.550557 mapbot_frontend-0.1.5/mapbot_frontend/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      621 2023-06-09 14:52:15.000000 mapbot_frontend-0.1.5/mapbot_frontend/__init__.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.549589 mapbot_frontend-0.1.5/mapbot_frontend/frontend/
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.552797 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      890 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/asset-manifest.json
+-rw-r--r--   0 martinweiss   (501) staff       (20)   197459 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/bootstrap.min.css
+-rw-r--r--   0 martinweiss   (501) staff       (20)     3066 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/index.html
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.556064 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2437 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2729 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1305 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--banner.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     3209 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--banner.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1793 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--bench.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)      931 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1760 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--junction-box.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1002 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--mailbox.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1366 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2711 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1371 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--store.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     3318 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--store.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1075 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--street-light.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1436 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--street-light.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1227 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1638 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1384 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1155 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2429 2023-06-09 15:02:51.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--trash-can.svg
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.550036 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.556695 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/css/
+-rw-r--r--   0 martinweiss   (501) staff       (20)    34837 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css
+-rw-r--r--   0 martinweiss   (501) staff       (20)    40852 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.566290 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/
+-rw-r--r--   0 martinweiss   (501) staff       (20)  1515566 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1399 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js.LICENSE.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)  6332675 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js.map
+-rw-r--r--   0 martinweiss   (501) staff       (20)    14337 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/main.2bcb2eaa.chunk.js
+-rw-r--r--   0 martinweiss   (501) staff       (20)    41945 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/main.2bcb2eaa.chunk.js.map
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1566 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js
+-rw-r--r--   0 martinweiss   (501) staff       (20)     8351 2023-06-09 15:03:00.000000 mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:57:56.551550 mapbot_frontend-0.1.5/mapbot_frontend.egg-info/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 15:57:56.000000 mapbot_frontend-0.1.5/mapbot_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2219 2023-06-09 15:57:56.000000 mapbot_frontend-0.1.5/mapbot_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 15:57:56.000000 mapbot_frontend-0.1.5/mapbot_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 15:57:56.000000 mapbot_frontend-0.1.5/mapbot_frontend.egg-info/top_level.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 15:57:56.567004 mapbot_frontend-0.1.5/setup.cfg
+-rw-r--r--   0 martinweiss   (501) staff       (20)      377 2023-06-09 15:57:43.000000 mapbot_frontend-0.1.5/setup.py
```

### Comparing `mapbot_frontend-0.1.4/frontend/build/asset-manifest.json` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/bootstrap.min.css` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/index.html` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/construction--flat--driveway.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/marking--discrete--other-marking.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--banner.png` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--banner.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--banner.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--banner.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--bench.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--bench.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--catch-basin.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--junction-box.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--junction-box.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--mailbox.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--mailbox.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--advertisement.png` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--advertisement.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--store.png` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--store.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--sign--store.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--sign--store.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--street-light.png` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--street-light.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--street-light.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--street-light.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--support--utility-pole.png` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--support--utility-pole.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--traffic-cone.png` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--traffic-cone.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/mapillary/object--trash-can.svg` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/mapillary/object--trash-can.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/css/2.45e7f682.chunk.css` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/css/2.45e7f682.chunk.css.map` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/2.c035aebc.chunk.js` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/2.c035aebc.chunk.js.LICENSE.txt` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/2.c035aebc.chunk.js.map` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/main.2bcb2eaa.chunk.js` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/main.2bcb2eaa.chunk.js`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/main.2bcb2eaa.chunk.js.map` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/main.2bcb2eaa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/runtime-main.48f3c07e.js` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/frontend/build/static/js/runtime-main.48f3c07e.js.map` & `mapbot_frontend-0.1.5/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.4/mapbot_frontend.egg-info/SOURCES.txt` & `mapbot_frontend-0.1.5/mapbot_frontend.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 MANIFEST.in
 setup.py
-frontend/__init__.py
-frontend/build/asset-manifest.json
-frontend/build/bootstrap.min.css
-frontend/build/index.html
-frontend/build/mapillary/construction--flat--driveway.svg
-frontend/build/mapillary/marking--discrete--other-marking.svg
-frontend/build/mapillary/object--banner.png
-frontend/build/mapillary/object--banner.svg
-frontend/build/mapillary/object--bench.svg
-frontend/build/mapillary/object--catch-basin.svg
-frontend/build/mapillary/object--junction-box.svg
-frontend/build/mapillary/object--mailbox.svg
-frontend/build/mapillary/object--sign--advertisement.png
-frontend/build/mapillary/object--sign--advertisement.svg
-frontend/build/mapillary/object--sign--store.png
-frontend/build/mapillary/object--sign--store.svg
-frontend/build/mapillary/object--street-light.png
-frontend/build/mapillary/object--street-light.svg
-frontend/build/mapillary/object--support--utility-pole.png
-frontend/build/mapillary/object--support--utility-pole.svg
-frontend/build/mapillary/object--traffic-cone.png
-frontend/build/mapillary/object--traffic-cone.svg
-frontend/build/mapillary/object--trash-can.svg
-frontend/build/static/css/2.45e7f682.chunk.css
-frontend/build/static/css/2.45e7f682.chunk.css.map
-frontend/build/static/js/2.c035aebc.chunk.js
-frontend/build/static/js/2.c035aebc.chunk.js.LICENSE.txt
-frontend/build/static/js/2.c035aebc.chunk.js.map
-frontend/build/static/js/main.2bcb2eaa.chunk.js
-frontend/build/static/js/main.2bcb2eaa.chunk.js.map
-frontend/build/static/js/runtime-main.48f3c07e.js
-frontend/build/static/js/runtime-main.48f3c07e.js.map
+mapbot_frontend/__init__.py
 mapbot_frontend.egg-info/PKG-INFO
 mapbot_frontend.egg-info/SOURCES.txt
 mapbot_frontend.egg-info/dependency_links.txt
-mapbot_frontend.egg-info/top_level.txt
+mapbot_frontend.egg-info/top_level.txt
+mapbot_frontend/frontend/build/asset-manifest.json
+mapbot_frontend/frontend/build/bootstrap.min.css
+mapbot_frontend/frontend/build/index.html
+mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg
+mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg
+mapbot_frontend/frontend/build/mapillary/object--banner.png
+mapbot_frontend/frontend/build/mapillary/object--banner.svg
+mapbot_frontend/frontend/build/mapillary/object--bench.svg
+mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg
+mapbot_frontend/frontend/build/mapillary/object--junction-box.svg
+mapbot_frontend/frontend/build/mapillary/object--mailbox.svg
+mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png
+mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg
+mapbot_frontend/frontend/build/mapillary/object--sign--store.png
+mapbot_frontend/frontend/build/mapillary/object--sign--store.svg
+mapbot_frontend/frontend/build/mapillary/object--street-light.png
+mapbot_frontend/frontend/build/mapillary/object--street-light.svg
+mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png
+mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg
+mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png
+mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg
+mapbot_frontend/frontend/build/mapillary/object--trash-can.svg
+mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css
+mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map
+mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js
+mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js.LICENSE.txt
+mapbot_frontend/frontend/build/static/js/2.c035aebc.chunk.js.map
+mapbot_frontend/frontend/build/static/js/main.2bcb2eaa.chunk.js
+mapbot_frontend/frontend/build/static/js/main.2bcb2eaa.chunk.js.map
+mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js
+mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map
```

