# Comparing `tmp/streamlit-d3-network-component-0.0.8.tar.gz` & `tmp/streamlit-d3-network-component-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-d3-network-component-0.0.8.tar", last modified: Mon Jun  5 10:34:30 2023, max compression
+gzip compressed data, was "streamlit-d3-network-component-0.0.9.tar", last modified: Mon Jun  5 11:37:55 2023, max compression
```

## Comparing `streamlit-d3-network-component-0.0.8.tar` & `streamlit-d3-network-component-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.473634 streamlit-d3-network-component-0.0.8/
--rw-r--r--   0 andras     (501) staff       (20)       65 2023-06-05 10:12:17.000000 streamlit-d3-network-component-0.0.8/MANIFEST.in
--rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 10:34:30.473359 streamlit-d3-network-component-0.0.8/PKG-INFO
--rw-r--r--   0 andras     (501) staff       (20)       38 2023-06-05 10:34:30.473694 streamlit-d3-network-component-0.0.8/setup.cfg
--rw-r--r--   0 andras     (501) staff       (20)      798 2023-06-05 10:34:27.000000 streamlit-d3-network-component-0.0.8/setup.py
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.441422 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/
--rw-r--r--   0 andras     (501) staff       (20)     3512 2023-06-05 10:31:56.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/__init__.py
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.438925 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.448314 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/
--rw-r--r--   0 andras     (501) staff       (20)     1307 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/asset-manifest.json
--rw-rw-r--   0 andras     (501) staff       (20)     3150 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/favicon.ico
--rw-r--r--   0 andras     (501) staff       (20)     2302 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/index.html
--rw-rw-r--   0 andras     (501) staff       (20)     5347 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/logo192.png
--rw-rw-r--   0 andras     (501) staff       (20)     9664 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/logo512.png
--rw-rw-r--   0 andras     (501) staff       (20)      492 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/manifest.json
--rw-r--r--   0 andras     (501) staff       (20)     2486 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js
--rw-rw-r--   0 andras     (501) staff       (20)       67 2023-06-05 09:41:06.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/robots.txt
--rw-r--r--   0 andras     (501) staff       (20)     1181 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/service-worker.js
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.439980 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.450089 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/
--rw-r--r--   0 andras     (501) staff       (20)    58890 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css
--rw-r--r--   0 andras     (501) staff       (20)    89084 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map
--rw-r--r--   0 andras     (501) staff       (20)     1007 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css
--rw-r--r--   0 andras     (501) staff       (20)     1899 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.457767 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/
--rw-r--r--   0 andras     (501) staff       (20)  1022852 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js
--rw-r--r--   0 andras     (501) staff       (20)     5927 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt
--rw-r--r--   0 andras     (501) staff       (20)  4266749 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map
--rw-r--r--   0 andras     (501) staff       (20)     5506 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js
--rw-r--r--   0 andras     (501) staff       (20)    21943 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map
--rw-r--r--   0 andras     (501) staff       (20)     1575 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js
--rw-r--r--   0 andras     (501) staff       (20)     8288 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.472324 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/
--rw-r--r--   0 andras     (501) staff       (20)   715890 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg
--rw-r--r--   0 andras     (501) staff       (20)   132728 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf
--rw-r--r--   0 andras     (501) staff       (20)    76612 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2
--rw-r--r--   0 andras     (501) staff       (20)   133034 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot
--rw-r--r--   0 andras     (501) staff       (20)    89824 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff
--rw-r--r--   0 andras     (501) staff       (20)    34390 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot
--rw-r--r--   0 andras     (501) staff       (20)   144322 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg
--rw-r--r--   0 andras     (501) staff       (20)    13584 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2
--rw-r--r--   0 andras     (501) staff       (20)    34092 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf
--rw-r--r--   0 andras     (501) staff       (20)    16800 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff
--rw-r--r--   0 andras     (501) staff       (20)   202616 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf
--rw-r--r--   0 andras     (501) staff       (20)   202902 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot
--rw-r--r--   0 andras     (501) staff       (20)    79444 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2
--rw-r--r--   0 andras     (501) staff       (20)   103300 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff
--rw-r--r--   0 andras     (501) staff       (20)   897426 2023-06-05 09:41:31.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg
-drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 10:34:30.444010 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/
--rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 10:34:30.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/PKG-INFO
--rw-r--r--   0 andras     (501) staff       (20)     3107 2023-06-05 10:34:30.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/SOURCES.txt
--rw-r--r--   0 andras     (501) staff       (20)        1 2023-06-05 10:34:30.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/dependency_links.txt
--rw-r--r--   0 andras     (501) staff       (20)       16 2023-06-05 10:34:30.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/requires.txt
--rw-r--r--   0 andras     (501) staff       (20)       31 2023-06-05 10:34:30.000000 streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/top_level.txt
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.536678 streamlit-d3-network-component-0.0.9/
+-rw-r--r--   0 andras     (501) staff       (20)       65 2023-06-05 10:12:17.000000 streamlit-d3-network-component-0.0.9/MANIFEST.in
+-rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 11:37:55.536418 streamlit-d3-network-component-0.0.9/PKG-INFO
+-rw-r--r--   0 andras     (501) staff       (20)       38 2023-06-05 11:37:55.536743 streamlit-d3-network-component-0.0.9/setup.cfg
+-rw-r--r--   0 andras     (501) staff       (20)      798 2023-06-05 11:37:51.000000 streamlit-d3-network-component-0.0.9/setup.py
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.512424 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/
+-rw-r--r--   0 andras     (501) staff       (20)     3512 2023-06-05 10:31:56.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/__init__.py
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.510434 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.518931 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/
+-rw-r--r--   0 andras     (501) staff       (20)     1307 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/asset-manifest.json
+-rw-rw-r--   0 andras     (501) staff       (20)     3150 2023-06-05 11:34:23.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/favicon.ico
+-rw-r--r--   0 andras     (501) staff       (20)     2302 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/index.html
+-rw-rw-r--   0 andras     (501) staff       (20)     5347 2023-06-05 11:34:23.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/logo192.png
+-rw-rw-r--   0 andras     (501) staff       (20)     9664 2023-06-05 11:34:23.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/logo512.png
+-rw-rw-r--   0 andras     (501) staff       (20)      492 2023-06-05 11:34:23.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/manifest.json
+-rw-r--r--   0 andras     (501) staff       (20)     2486 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js
+-rw-rw-r--   0 andras     (501) staff       (20)       67 2023-06-05 11:34:23.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/robots.txt
+-rw-r--r--   0 andras     (501) staff       (20)     1181 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/service-worker.js
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.511315 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.520613 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/
+-rw-r--r--   0 andras     (501) staff       (20)    58890 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css
+-rw-r--r--   0 andras     (501) staff       (20)    89084 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map
+-rw-r--r--   0 andras     (501) staff       (20)     1007 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css
+-rw-r--r--   0 andras     (501) staff       (20)     1899 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.527820 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/
+-rw-r--r--   0 andras     (501) staff       (20)  1022852 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js
+-rw-r--r--   0 andras     (501) staff       (20)     5927 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js.LICENSE.txt
+-rw-r--r--   0 andras     (501) staff       (20)  4266749 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js.map
+-rw-r--r--   0 andras     (501) staff       (20)     5506 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js
+-rw-r--r--   0 andras     (501) staff       (20)    21943 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map
+-rw-r--r--   0 andras     (501) staff       (20)     1575 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js
+-rw-r--r--   0 andras     (501) staff       (20)     8288 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.535485 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/
+-rw-r--r--   0 andras     (501) staff       (20)   715890 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg
+-rw-r--r--   0 andras     (501) staff       (20)   132728 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf
+-rw-r--r--   0 andras     (501) staff       (20)    76612 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2
+-rw-r--r--   0 andras     (501) staff       (20)   133034 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot
+-rw-r--r--   0 andras     (501) staff       (20)    89824 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff
+-rw-r--r--   0 andras     (501) staff       (20)    34390 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot
+-rw-r--r--   0 andras     (501) staff       (20)   144322 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg
+-rw-r--r--   0 andras     (501) staff       (20)    13584 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2
+-rw-r--r--   0 andras     (501) staff       (20)    34092 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf
+-rw-r--r--   0 andras     (501) staff       (20)    16800 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff
+-rw-r--r--   0 andras     (501) staff       (20)   202616 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf
+-rw-r--r--   0 andras     (501) staff       (20)   202902 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot
+-rw-r--r--   0 andras     (501) staff       (20)    79444 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2
+-rw-r--r--   0 andras     (501) staff       (20)   103300 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff
+-rw-r--r--   0 andras     (501) staff       (20)   897426 2023-06-05 11:34:49.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg
+drwxr-xr-x   0 andras     (501) staff       (20)        0 2023-06-05 11:37:55.514947 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/
+-rw-r--r--   0 andras     (501) staff       (20)      406 2023-06-05 11:37:55.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/PKG-INFO
+-rw-r--r--   0 andras     (501) staff       (20)     3107 2023-06-05 11:37:55.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/SOURCES.txt
+-rw-r--r--   0 andras     (501) staff       (20)        1 2023-06-05 11:37:55.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/dependency_links.txt
+-rw-r--r--   0 andras     (501) staff       (20)       16 2023-06-05 11:37:55.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/requires.txt
+-rw-r--r--   0 andras     (501) staff       (20)       31 2023-06-05 11:37:55.000000 streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/top_level.txt
```

### Comparing `streamlit-d3-network-component-0.0.8/setup.py` & `streamlit-d3-network-component-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-d3-network-component",
-    version="0.0.8",
+    version="0.0.9",
     author="Andras Gyacsok",
     author_email="andras.gyacsok@boehringer-ingelheim.com",
     description="This package is a Streamlit custom component to represent network diagram using D3.js",
     long_description="This package is the custom Streamlit component to visualise network graphs using D3.js",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/__init__.py` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/asset-manifest.json` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/asset-manifest.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8114035087719298%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/2.e9368623.chunk.js')], delete: [2]}",*

 * * "'files'": "{'static/js/2.e9368623.chunk.js': '/static/js/2.e9368623.chunk.js', "*

 * *            "'static/js/2.e9368623.chunk.js.map': '/static/js/2.e9368623.chunk.js.map', "*

 * *            "'precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js': "*

 * *            "'/precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js', "*

 * *            "'static/js/2.e9368623.chunk.js.LICENSE.txt': "*

 * *            "'/static/js/2.e9368623.chunk.js.LICENS […]*

```diff
@@ -1,26 +1,26 @@
 {
     "entrypoints": [
         "static/js/runtime-main.18a1b64b.js",
         "static/css/2.0d21f304.chunk.css",
-        "static/js/2.13e4d720.chunk.js",
+        "static/js/2.e9368623.chunk.js",
         "static/css/main.c3e5bb93.chunk.css",
         "static/js/main.e1d1cd7b.chunk.js"
     ],
     "files": {
         "index.html": "/index.html",
         "main.css": "/static/css/main.c3e5bb93.chunk.css",
         "main.js": "/static/js/main.e1d1cd7b.chunk.js",
         "main.js.map": "/static/js/main.e1d1cd7b.chunk.js.map",
-        "precache-manifest.9a6cee5862e83e747d32a923936a576d.js": "/precache-manifest.9a6cee5862e83e747d32a923936a576d.js",
+        "precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js": "/precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js",
         "runtime-main.js": "/static/js/runtime-main.18a1b64b.js",
         "runtime-main.js.map": "/static/js/runtime-main.18a1b64b.js.map",
         "service-worker.js": "/service-worker.js",
         "static/css/2.0d21f304.chunk.css": "/static/css/2.0d21f304.chunk.css",
         "static/css/2.0d21f304.chunk.css.map": "/static/css/2.0d21f304.chunk.css.map",
         "static/css/main.c3e5bb93.chunk.css.map": "/static/css/main.c3e5bb93.chunk.css.map",
-        "static/js/2.13e4d720.chunk.js": "/static/js/2.13e4d720.chunk.js",
-        "static/js/2.13e4d720.chunk.js.LICENSE.txt": "/static/js/2.13e4d720.chunk.js.LICENSE.txt",
-        "static/js/2.13e4d720.chunk.js.map": "/static/js/2.13e4d720.chunk.js.map",
+        "static/js/2.e9368623.chunk.js": "/static/js/2.e9368623.chunk.js",
+        "static/js/2.e9368623.chunk.js.LICENSE.txt": "/static/js/2.e9368623.chunk.js.LICENSE.txt",
+        "static/js/2.e9368623.chunk.js.map": "/static/js/2.e9368623.chunk.js.map",
         "static/media/all.min.css": "/static/media/fa-solid-900.ec763292.svg"
     }
 }
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/favicon.ico` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/index.html` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>React App</title><link href="/static/css/2.0d21f304.chunk.css" rel="stylesheet"><link href="/static/css/main.c3e5bb93.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="net-root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],a=r[1],c=r[2],p=0,s=[];p<l.length;p++)f=l[p],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(i&&i(r);s.length;)s.shift()();return u.push.apply(u,c||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var a=t[l];0!==o[a]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this["webpackJsonpreact-d3-force"]=this["webpackJsonpreact-d3-force"]||[],a=l.push.bind(l);l.push=r,l=l.slice();for(var c=0;c<l.length;c++)r(l[c]);var i=a;t()}([])</script><script src="/static/js/2.13e4d720.chunk.js"></script><script src="/static/js/main.e1d1cd7b.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>React App</title><link href="/static/css/2.0d21f304.chunk.css" rel="stylesheet"><link href="/static/css/main.c3e5bb93.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="net-root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],a=r[1],c=r[2],p=0,s=[];p<l.length;p++)f=l[p],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(i&&i(r);s.length;)s.shift()();return u.push.apply(u,c||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var a=t[l];0!==o[a]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this["webpackJsonpreact-d3-force"]=this["webpackJsonpreact-d3-force"]||[],a=l.push.bind(l);l.push=r,l=l.slice();for(var c=0;c<l.length;c++)r(l[c]);var i=a;t()}([])</script><script src="/static/js/2.e9368623.chunk.js"></script><script src="/static/js/main.e1d1cd7b.chunk.js"></script></body></html>
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/logo192.png` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/logo192.png`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/logo512.png` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/logo512.png`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "0e2eeec3cb827c0c30a31e2703f0df54",
+    "revision": "967a5f574a01d352dc5d1a5b9a4f1125",
     "url": "/index.html"
 }, {
-    "revision": "15c3b74beea41c69ccb2",
+    "revision": "32f741b76b319b51eb98",
     "url": "/static/css/2.0d21f304.chunk.css"
 }, {
     "revision": "63d08580bc5df8cc4277",
     "url": "/static/css/main.c3e5bb93.chunk.css"
 }, {
-    "revision": "15c3b74beea41c69ccb2",
-    "url": "/static/js/2.13e4d720.chunk.js"
+    "revision": "32f741b76b319b51eb98",
+    "url": "/static/js/2.e9368623.chunk.js"
 }, {
     "revision": "2910be745dad237df0fe0c529bcc3bc3",
-    "url": "/static/js/2.13e4d720.chunk.js.LICENSE.txt"
+    "url": "/static/js/2.e9368623.chunk.js.LICENSE.txt"
 }, {
     "revision": "63d08580bc5df8cc4277",
     "url": "/static/js/main.e1d1cd7b.chunk.js"
 }, {
     "revision": "0e6aac023c37b7e52d31",
     "url": "/static/js/runtime-main.18a1b64b.js"
 }, {
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/service-worker.js` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/service-worker.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "/precache-manifest.9a6cee5862e83e747d32a923936a576d.js"
+    "/precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.13e4d720.chunk.js.LICENSE.txt */
+/*! For license information please see 2.e9368623.chunk.js.LICENSE.txt */
 (this["webpackJsonpreact-d3-force"] = this["webpackJsonpreact-d3-force"] || []).push([
     [2],
     [function(t, e, n) {
         "use strict";
 
         function r(t, e) {
             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
@@ -40890,8 +40890,8 @@
         try {
             regeneratorRuntime = r
         } catch (i) {
             Function("r", "regeneratorRuntime = r")(r)
         }
     }]
 ]);
-//# sourceMappingURL=2.13e4d720.chunk.js.map
+//# sourceMappingURL=2.e9368623.chunk.js.map
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'static/js/2.e9368623.chunk.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "static/js/2.13e4d720.chunk.js",
+    "file": "static/js/2.e9368623.chunk.js",
     "names": [
         "_classCallCheck",
         "instance",
         "Constructor",
         "TypeError",
         "_inherits",
```

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.c1868c95.eot`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.ec3cfdde.woff`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.261d666b.eot`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.89ffa3ab.svg`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.c20b5b73.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.db78b935.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-regular-400.f89ea91e.woff`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.1ab236ed.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.a0369ea5.eot`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.b15db15f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.bea989e8.woff`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component/frontend/build/static/media/fa-solid-900.ec763292.svg`

 * *Files identical despite different names*

### Comparing `streamlit-d3-network-component-0.0.8/streamlit_d3_network_component.egg-info/SOURCES.txt` & `streamlit-d3-network-component-0.0.9/streamlit_d3_network_component.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 streamlit_d3_network_component.egg-info/top_level.txt
 streamlit_d3_network_component/frontend/build/asset-manifest.json
 streamlit_d3_network_component/frontend/build/favicon.ico
 streamlit_d3_network_component/frontend/build/index.html
 streamlit_d3_network_component/frontend/build/logo192.png
 streamlit_d3_network_component/frontend/build/logo512.png
 streamlit_d3_network_component/frontend/build/manifest.json
-streamlit_d3_network_component/frontend/build/precache-manifest.9a6cee5862e83e747d32a923936a576d.js
+streamlit_d3_network_component/frontend/build/precache-manifest.4746b0266f22c1d7ff3f6ae6ca9e9f8b.js
 streamlit_d3_network_component/frontend/build/robots.txt
 streamlit_d3_network_component/frontend/build/service-worker.js
 streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css
 streamlit_d3_network_component/frontend/build/static/css/2.0d21f304.chunk.css.map
 streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css
 streamlit_d3_network_component/frontend/build/static/css/main.c3e5bb93.chunk.css.map
-streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js
-streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.LICENSE.txt
-streamlit_d3_network_component/frontend/build/static/js/2.13e4d720.chunk.js.map
+streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js
+streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js.LICENSE.txt
+streamlit_d3_network_component/frontend/build/static/js/2.e9368623.chunk.js.map
 streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js
 streamlit_d3_network_component/frontend/build/static/js/main.e1d1cd7b.chunk.js.map
 streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js
 streamlit_d3_network_component/frontend/build/static/js/runtime-main.18a1b64b.js.map
 streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.0cb5a5c0.svg
 streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.13685372.ttf
 streamlit_d3_network_component/frontend/build/static/media/fa-brands-400.a06da7f0.woff2
```
