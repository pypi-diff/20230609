# Comparing `tmp/mapbot_frontend-0.1.6.tar.gz` & `tmp/mapbot_frontend-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapbot_frontend-0.1.6.tar", last modified: Fri Jun  9 16:06:10 2023, max compression
+gzip compressed data, was "mapbot_frontend-0.1.7.tar", last modified: Fri Jun  9 16:13:55 2023, max compression
```

## Comparing `mapbot_frontend-0.1.6.tar` & `mapbot_frontend-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.922535 mapbot_frontend-0.1.6/
--rw-r--r--   0 martinweiss   (501) staff       (20)       50 2023-06-09 15:57:28.000000 mapbot_frontend-0.1.6/MANIFEST.in
--rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 16:06:10.922283 mapbot_frontend-0.1.6/PKG-INFO
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.901352 mapbot_frontend-0.1.6/mapbot_frontend/
--rw-r--r--   0 martinweiss   (501) staff       (20)      621 2023-06-09 14:52:15.000000 mapbot_frontend-0.1.6/mapbot_frontend/__init__.py
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.900565 mapbot_frontend-0.1.6/mapbot_frontend/frontend/
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.903565 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/
--rw-r--r--   0 martinweiss   (501) staff       (20)      890 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/asset-manifest.json
--rw-r--r--   0 martinweiss   (501) staff       (20)   197459 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/bootstrap.min.css
--rw-r--r--   0 martinweiss   (501) staff       (20)     3066 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/index.html
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.907108 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/
--rw-r--r--   0 martinweiss   (501) staff       (20)     2437 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     2729 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1305 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--banner.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     3209 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--banner.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1793 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--bench.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)      931 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1760 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--junction-box.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1002 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--mailbox.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1366 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     2711 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1371 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--store.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     3318 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--store.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1075 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--street-light.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     1436 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--street-light.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1227 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     1638 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     1384 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png
--rw-r--r--   0 martinweiss   (501) staff       (20)     1155 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg
--rw-r--r--   0 martinweiss   (501) staff       (20)     2429 2023-06-09 16:02:24.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--trash-can.svg
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.900885 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.907960 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/css/
--rw-r--r--   0 martinweiss   (501) staff       (20)    34837 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css
--rw-r--r--   0 martinweiss   (501) staff       (20)    40852 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.921585 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/
--rw-r--r--   0 martinweiss   (501) staff       (20)  1515566 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js
--rw-r--r--   0 martinweiss   (501) staff       (20)     1399 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.LICENSE.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)  6332675 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.map
--rw-r--r--   0 martinweiss   (501) staff       (20)    14337 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js
--rw-r--r--   0 martinweiss   (501) staff       (20)    41945 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js.map
--rw-r--r--   0 martinweiss   (501) staff       (20)     1566 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js
--rw-r--r--   0 martinweiss   (501) staff       (20)     8351 2023-06-09 16:02:59.000000 mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:06:10.902094 mapbot_frontend-0.1.6/mapbot_frontend.egg-info/
--rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 16:06:10.000000 mapbot_frontend-0.1.6/mapbot_frontend.egg-info/PKG-INFO
--rw-r--r--   0 martinweiss   (501) staff       (20)     2219 2023-06-09 16:06:10.000000 mapbot_frontend-0.1.6/mapbot_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 16:06:10.000000 mapbot_frontend-0.1.6/mapbot_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 16:06:10.000000 mapbot_frontend-0.1.6/mapbot_frontend.egg-info/top_level.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 16:06:10.922598 mapbot_frontend-0.1.6/setup.cfg
--rw-r--r--   0 martinweiss   (501) staff       (20)      461 2023-06-09 16:06:06.000000 mapbot_frontend-0.1.6/setup.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.878452 mapbot_frontend-0.1.7/
+-rw-r--r--   0 martinweiss   (501) staff       (20)       50 2023-06-09 15:57:28.000000 mapbot_frontend-0.1.7/MANIFEST.in
+-rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 16:13:55.878250 mapbot_frontend-0.1.7/PKG-INFO
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.866929 mapbot_frontend-0.1.7/mapbot_frontend/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      621 2023-06-09 14:52:15.000000 mapbot_frontend-0.1.7/mapbot_frontend/__init__.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.865998 mapbot_frontend-0.1.7/mapbot_frontend/frontend/
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.868447 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      890 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/asset-manifest.json
+-rw-r--r--   0 martinweiss   (501) staff       (20)   197459 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/bootstrap.min.css
+-rw-r--r--   0 martinweiss   (501) staff       (20)     3066 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/index.html
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.872032 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2437 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2729 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1305 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--banner.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     3209 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--banner.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1793 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--bench.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)      931 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1760 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--junction-box.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1002 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--mailbox.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1366 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2711 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1371 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--store.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     3318 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--store.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1075 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--street-light.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1436 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--street-light.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1227 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1638 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1384 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1155 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2429 2023-06-09 16:13:25.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--trash-can.svg
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.866445 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.872373 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/css/
+-rw-r--r--   0 martinweiss   (501) staff       (20)    34837 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css
+-rw-r--r--   0 martinweiss   (501) staff       (20)    40852 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.877860 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/
+-rw-r--r--   0 martinweiss   (501) staff       (20)  1515566 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1399 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.LICENSE.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)  6332675 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.map
+-rw-r--r--   0 martinweiss   (501) staff       (20)    14337 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js
+-rw-r--r--   0 martinweiss   (501) staff       (20)    41945 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js.map
+-rw-r--r--   0 martinweiss   (501) staff       (20)     1566 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js
+-rw-r--r--   0 martinweiss   (501) staff       (20)     8351 2023-06-09 16:13:35.000000 mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 16:13:55.867851 mapbot_frontend-0.1.7/mapbot_frontend.egg-info/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      329 2023-06-09 16:13:55.000000 mapbot_frontend-0.1.7/mapbot_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 martinweiss   (501) staff       (20)     2219 2023-06-09 16:13:55.000000 mapbot_frontend-0.1.7/mapbot_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 16:13:55.000000 mapbot_frontend-0.1.7/mapbot_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 16:13:55.000000 mapbot_frontend-0.1.7/mapbot_frontend.egg-info/top_level.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 16:13:55.878509 mapbot_frontend-0.1.7/setup.cfg
+-rw-r--r--   0 martinweiss   (501) staff       (20)      461 2023-06-09 16:11:49.000000 mapbot_frontend-0.1.7/setup.py
```

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/__init__.py` & `mapbot_frontend-0.1.7/mapbot_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/asset-manifest.json` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/bootstrap.min.css` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/index.html` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/construction--flat--driveway.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/marking--discrete--other-marking.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--banner.png` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--banner.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--banner.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--banner.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--bench.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--bench.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--catch-basin.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--junction-box.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--junction-box.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--mailbox.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--mailbox.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--advertisement.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--store.png` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--store.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--sign--store.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--sign--store.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--street-light.png` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--street-light.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--street-light.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--street-light.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--support--utility-pole.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.png`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--traffic-cone.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/mapillary/object--trash-can.svg` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/mapillary/object--trash-can.svg`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/css/2.45e7f682.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.LICENSE.txt` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.map` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/2.c35007af.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js.map` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/main.380fae73.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map` & `mapbot_frontend-0.1.7/mapbot_frontend/frontend/build/static/js/runtime-main.48f3c07e.js.map`

 * *Files identical despite different names*

### Comparing `mapbot_frontend-0.1.6/mapbot_frontend.egg-info/SOURCES.txt` & `mapbot_frontend-0.1.7/mapbot_frontend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

