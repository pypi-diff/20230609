# Comparing `tmp/nbsite-0.8.0rc9.tar.gz` & `tmp/nbsite-0.8.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nbsite-0.8.0rc9.tar", last modified: Thu Mar  9 16:55:32 2023, max compression
+gzip compressed data, was "dist/nbsite-0.8.1a1.tar", last modified: Fri Jun  9 15:26:13 2023, max compression
```

## Comparing `nbsite-0.8.0rc9.tar` & `nbsite-0.8.1a1.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/holoviz-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/nbsite.js
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/require.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18035 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11127 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 15:26:12.000000 nbsite-0.8.1a1/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/holoviz-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/_shared_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-09 15:26:13.000000 nbsite-0.8.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-09 15:25:09.000000 nbsite-0.8.1a1/setup.py
```

### Comparing `nbsite-0.8.0rc9/LICENSE.txt` & `nbsite-0.8.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/PKG-INFO` & `nbsite-0.8.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.0rc9
+Version: 0.8.1a1
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.pyviz.org/
 Author: PyViz developers
 Author-email: developers@pyviz.org
 Maintainer: PyViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD-3
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: refman
 Provides-Extra: gallery
 Provides-Extra: tests
 Provides-Extra: build
 License-File: LICENSE.txt
 
-<img src="doc/_static/nbsite-logo.png" height=150><br>
+<img src="https://github.com/pyviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
 
 # NBSite: Build a tested, sphinx-based website from notebooks
 
 |    |    |
 | --- | --- |
```

### Comparing `nbsite-0.8.0rc9/README.md` & `nbsite-0.8.1a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="doc/_static/nbsite-logo.png" height=150><br>
+<img src="https://github.com/pyviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
 
 # NBSite: Build a tested, sphinx-based website from notebooks
 
 |    |    |
 | --- | --- |
```

### Comparing `nbsite-0.8.0rc9/nbsite/__main__.py` & `nbsite-0.8.1a1/nbsite/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import argparse
 import inspect
 
-from .cmd import init, generate_rst, build
+from .cmd import build, generate_rst, init
+
 
 def _add_common_args(parser,*names):
     common = {
         '--project-root': dict(type=str,help='defaults to current working directory',default=''),
         '--examples': dict(type=str,help='if relative, should be relative to project-root',default='examples'),
-        '--doc': dict(type=str,help='if relative, should be releative to project-root',default='doc'),
+        '--doc': dict(type=str,help='if relative, should be relative to project-root',default='doc'),
         '--overwrite': dict(action='store_true', help='whether to overwrite any files [DANGEROUS]')
         }
     for name in names:
         parser.add_argument(name,**common[name])
 
 def _set_defaults(parser,fn):
     parser.set_defaults(func=lambda args: fn( **{k: getattr(args,k) for k in vars(args) if k!='func'} ))
@@ -33,14 +34,15 @@
     generaterst_parser.add_argument('--repo',type=str,help='name of repo',default='')
     generaterst_parser.add_argument('--branch',type=str,help='branch to point to in notebook links',default='main')
     generaterst_parser.add_argument('--offset',type=int,help='number of cells to delete from top of notebooks',default=0)
     generaterst_parser.add_argument('--nblink',type=str,help='where to place notebook links',choices=['bottom', 'top', 'both', 'none'], default='bottom')
     generaterst_parser.add_argument('--binder',type=str,help='where to place binder link',choices=['bottom', 'top', 'both', 'none'], default='none')
     generaterst_parser.add_argument('--skip',type=str,help='notebooks to skip running; comma separated case insensitive re to match',default='')
     generaterst_parser.add_argument('--keep-numbers',action='store_true',help='whether to keep the leading numbers of notebook URLs and titles')
+    generaterst_parser.add_argument('--disable-interactivity-warning',action='store_true',help='whether to disable interactivity warnings')
     _set_defaults(generaterst_parser,generate_rst)
 
     build_parser = subparsers.add_parser("build", help=inspect.getdoc(build))
     build_parser.add_argument('--what',type=str,help='type of output to generate',default='html')
 
     build_parser.add_argument('--project-name', type=str, help='name of project', default='')
     build_parser.add_argument('--org',type=str,help='github organization',default='')
@@ -48,15 +50,15 @@
     build_parser.add_argument('--repo',type=str,help='name of repo',default='')
     build_parser.add_argument('--branch',type=str,help='branch to point to in notebook links',default='main')
     build_parser.add_argument('--binder',type=str,help='where to place binder link',choices=['bottom', 'top', 'both', 'none'], default='none')
 
     build_parser.add_argument('--output',type=str,help='where to place output',default="builtdocs")
     _add_common_args(build_parser,'--project-root','--doc','--examples', '--overwrite')
     build_parser.add_argument('--examples-assets',type=str,default="assets",
-                              help='dir in which assets for examples are located - if relative, should be releative to project-root')
+                              help='dir in which assets for examples are located - if relative, should be relative to project-root')
     build_parser.add_argument('--clean-dry-run',action='store_true',help='whether to not actually delete files from output (useful for uploading)')
     build_parser.add_argument('--inspect-links',action='store_true',help='whether to not to print all links')
     _set_defaults(build_parser,build)
 
     args = parser.parse_args()
     return args.func(args) if hasattr(args,'func') else parser.error("must supply command to run")
```

### Comparing `nbsite-0.8.0rc9/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.1a1/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.1a1/nbsite/_shared_static/mystnb.css`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 /* Whole cell */
 div.container.cell {
   padding-left: 0;
   margin-bottom: 1em;
 }
 
-.cell_output .output pre, .cell_input pre {
+.cell_output .output pre,
+.cell_input pre {
   margin: 0px;
 }
 
 /* Input cells */
 div.cell div.cell_input {
   padding-left: 0em;
   padding-right: 0em;
   border: 1px #ccc solid;
   background-color: #f7f7f7;
   border-left-color: green;
   border-left-width: medium;
 }
 
-div.cell_input > div, div.cell_output div.output > div.highlight {
+div.cell_input > div,
+div.cell_output div.output > div.highlight {
   margin: 0em !important;
   border: none !important;
 }
 
 /* All cell outputs */
 .cell_output {
   padding-left: 1em;
   padding-right: 0em;
   margin-top: 1em;
 }
 
 /* Outputs from jupyter_sphinx overrides to remove extra CSS */
 div.section div.jupyter_container {
-  padding: .4em;
-  margin: 0 0 .4em 0;
+  padding: 0.4em;
+  margin: 0 0 0.4em 0;
   background-color: none;
   border: none;
   -moz-box-shadow: none;
   -webkit-box-shadow: none;
   box-shadow: none;
 }
 
 /* Text outputs from cells */
 .cell_output .output.text_plain,
 .cell_output .output.traceback,
 .cell_output .output.stream,
-.cell_output .output.stderr
-  {
+.cell_output .output.stderr {
   background: #fcfcfc;
   margin-top: 1em;
   margin-bottom: 0em;
   box-shadow: none;
 }
 
 .cell_output .output.text_plain,
@@ -70,46 +71,45 @@
 /* Math align to the left */
 .cell_output .MathJax_Display {
   text-align: left !important;
 }
 
 /* Pandas tables. Pulled from the Jupyter / nbsphinx CSS */
 div.cell_output table {
-    border: none;
-    border-collapse: collapse;
-    border-spacing: 0;
-    color: black;
-    font-size: 1em;
-    table-layout: fixed;
-  }
-  div.cell_output thead {
-    border-bottom: 1px solid black;
-    vertical-align: bottom;
-  }
-  div.cell_output tr,
-  div.cell_output th,
-  div.cell_output td {
-    text-align: right;
-    vertical-align: middle;
-    padding: 0.5em 0.5em;
-    line-height: normal;
-    white-space: normal;
-    max-width: none;
-    border: none;
-  }
-  div.cell_output th {
-    font-weight: bold;
-  }
-  div.cell_output tbody tr:nth-child(odd) {
-    background: #f5f5f5;
-  }
-  div.cell_output tbody tr:hover {
-    background: rgba(66, 165, 245, 0.2);
-  }
-
+  border: none;
+  border-collapse: collapse;
+  border-spacing: 0;
+  color: black;
+  font-size: 1em;
+  table-layout: fixed;
+}
+div.cell_output thead {
+  border-bottom: 1px solid black;
+  vertical-align: bottom;
+}
+div.cell_output tr,
+div.cell_output th,
+div.cell_output td {
+  text-align: right;
+  vertical-align: middle;
+  padding: 0.5em 0.5em;
+  line-height: normal;
+  white-space: normal;
+  max-width: none;
+  border: none;
+}
+div.cell_output th {
+  font-weight: bold;
+}
+div.cell_output tbody tr:nth-child(odd) {
+  background: #f5f5f5;
+}
+div.cell_output tbody tr:hover {
+  background: rgba(66, 165, 245, 0.2);
+}
 
 /* Inline text from `paste` operation */
 
 span.pasted-text {
   font-weight: bold;
 }
 
@@ -123,55 +123,55 @@
 
 /* Font colors for translated ANSI escape sequences
 Color values are adapted from share/jupyter/nbconvert/templates/classic/static/style.css
 */
 div.highlight .-Color-Bold {
   font-weight: bold;
 }
-div.highlight .-Color[class*=-Black] {
-  color :#3E424D
+div.highlight .-Color[class*="-Black"] {
+  color: #3e424d;
 }
-div.highlight .-Color[class*=-Red] {
-  color: #E75C58
+div.highlight .-Color[class*="-Red"] {
+  color: #e75c58;
 }
-div.highlight .-Color[class*=-Green] {
-  color: #00A250
+div.highlight .-Color[class*="-Green"] {
+  color: #00a250;
 }
-div.highlight .-Color[class*=-Yellow] {
-  color: yellow
+div.highlight .-Color[class*="-Yellow"] {
+  color: yellow;
 }
-div.highlight .-Color[class*=-Blue] {
-  color: #208FFB
+div.highlight .-Color[class*="-Blue"] {
+  color: #208ffb;
 }
-div.highlight .-Color[class*=-Magenta] {
-  color: #D160C4
+div.highlight .-Color[class*="-Magenta"] {
+  color: #d160c4;
 }
-div.highlight .-Color[class*=-Cyan] {
-  color: #60C6C8
+div.highlight .-Color[class*="-Cyan"] {
+  color: #60c6c8;
 }
-div.highlight .-Color[class*=-White] {
-  color: #C5C1B4
+div.highlight .-Color[class*="-White"] {
+  color: #c5c1b4;
 }
-div.highlight .-Color[class*=-BGBlack] {
-  background-color: #3E424D
+div.highlight .-Color[class*="-BGBlack"] {
+  background-color: #3e424d;
 }
-div.highlight .-Color[class*=-BGRed] {
-  background-color: #E75C58
+div.highlight .-Color[class*="-BGRed"] {
+  background-color: #e75c58;
 }
-div.highlight .-Color[class*=-BGGreen] {
-  background-color: #00A250
+div.highlight .-Color[class*="-BGGreen"] {
+  background-color: #00a250;
 }
-div.highlight .-Color[class*=-BGYellow] {
-  background-color: yellow
+div.highlight .-Color[class*="-BGYellow"] {
+  background-color: yellow;
 }
-div.highlight .-Color[class*=-BGBlue] {
-  background-color: #208FFB
+div.highlight .-Color[class*="-BGBlue"] {
+  background-color: #208ffb;
 }
-div.highlight .-Color[class*=-BGMagenta] {
-  background-color: #D160C4
+div.highlight .-Color[class*="-BGMagenta"] {
+  background-color: #d160c4;
 }
-div.highlight .-Color[class*=-BGCyan] {
-  background-color: #60C6C8
+div.highlight .-Color[class*="-BGCyan"] {
+  background-color: #60c6c8;
 }
-div.highlight .-Color[class*=-BGWhite] {
-  background-color: #C5C1B4
+div.highlight .-Color[class*="-BGWhite"] {
+  background-color: #c5c1b4;
 }
```

### Comparing `nbsite-0.8.0rc9/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.1a1/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/nbsite/cmd.py` & `nbsite-0.8.1a1/nbsite/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import os
 import glob
+import os
 import re
-import sys
 import subprocess
-from os.path import dirname
+import sys
+
 from collections import ChainMap
+from os.path import dirname
 
 from .util import copy_files
 
 DEFAULT_SITE_ORDERING = [
     "Introduction",
     "Getting Started",
     "User Guide",
@@ -138,14 +139,15 @@
         branch='main',
         offset=0,
         overwrite=False,
         nblink='bottom',
         skip='',
         keep_numbers=False,
         binder='none',
+        disable_interactivity_warning=False
 ):
     """Auto-generates notebook-including rsts from notebooks in examples.
 
     titles
     ======
 
     rst file takes title from notebook filename in general, replacing
@@ -230,32 +232,37 @@
             title = _to_title(title, apply_title_case=True)
 
         if os.path.exists(rst):
             if not overwrite:
                 print("...skipping %s"%rst)
                 continue
 
-        print("...writing %s"%rst)
+        print(f"...writing {rst}")
         with open(rst, 'w') as rst_file:
             import nbsite
-            rst_file.write('..\n   Originally generated by nbsite (%s):\n     %s\n   Will not subsequently be overwritten by nbsite, so can be edited.\n\n'%(nbsite.__version__,' '.join(sys.argv)))
-
+            rst_file.write(
+                f'..\n   Originally generated by nbsite ({nbsite.__version__}):\n'
+                f'   {" ".join(sys.argv)}\n   Will not subsequently be overwritten by '
+                'nbsite, so can be edited.\n\n'
+            )
             if binder in ['top', 'both']:
                 add_binder(rst_file, org, repo, branch, relpath, examples)
 
             rst_file.write('*'*len(title)+'\n')
             rst_file.write(title+'\n')
             rst_file.write('*'*len(title)+'\n\n')
 
             if nblink in ['top', 'both']:
                 add_nblink(rst_file, host, org, repo, branch, examples, relpath)
                 rst_file.write('\n\n-------\n\n')
 
             rst_file.write(".. notebook:: %s %s" % (project_name,os.path.relpath(paths['examples'],start=dirname(rst))+'/'+relpath+"\n"))
             rst_file.write("    :offset: %s\n" % offset)
+            if disable_interactivity_warning:
+                rst_file.write("    :disable_interactivity_warning:\n")
 
             if pretitle=='index':
                 rst_file.write("%s\n"%_toctree(dirname(filename), paths['examples'], keep_numbers))
             if nblink in ['bottom', 'both']:
                 rst_file.write('\n\n-------\n\n')
                 add_nblink(rst_file, host, org, repo, branch, examples, relpath)
             if binder in ['bottom', 'both']:
```

### Comparing `nbsite-0.8.0rc9/nbsite/gallery/gen.py` & `nbsite-0.8.1a1/nbsite/gallery/gen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import os
 import glob
+import json
 import logging
+import os
 
 import requests
 import sphinx.util
 
 from PIL import Image
 
 try:
     import bs4
-except:
+except ImportError:
     bs4 = None
 
-from .thumbnailer import notebook_thumbnail, execute
+from .thumbnailer import execute, notebook_thumbnail
 
 logger = sphinx.util.logging.getLogger('nbsite-gallery')
 logging.getLogger(requests.packages.urllib3.__package__).setLevel(logging.ERROR)
 
 BUTTON_GROUP_TEMPLATE = """
 .. raw:: html
 
@@ -151,14 +152,15 @@
 
 
 DEFAULT_GALLERY_CONF = {
     'backends': None,
     'default_extensions': ['*.ipynb', '*.py'],
     'enable_download': True,
     'only_use_existing': False,
+    'as_pyodide': False,
     'examples_dir': os.path.join('..', 'examples'),
     'labels_dir': 'labels',
     'galleries': {
         'gallery': {
             'backends': [],
             'extensions': ['*.ipynb', '*.py'],
             'intro': 'Sample intro',
@@ -173,20 +175,20 @@
     'deployment_url': None,
     'iframe_spinner': "https://assets.holoviews.org/static/spinner.gif",
     'inline': False,
     'script_prefix': PREFIX,
     'skip_execute': [],
     'thumbnail_url': THUMBNAIL_URL,
     'thumbnail_size': (400, 280),
-    'within_subsection_order': lambda key: key,
+    'within_subsection_order': None,
     'nblink': 'both',  # use this to control the position of the nblink
     'github_ref': 'main',  # branch or tag
+    'jupyterlite_url': None
 }
 
-
 def get_deployed_url(deployment_urls, basename):
     for deployment_url in deployment_urls:
         # Test the deployment_url/basename, then deployment_url/notebooks/basename.ipynb
         candidates = [os.path.join(deployment_url,
                                    basename[:-6] if basename.endswith('.ipynb') else basename),
                       os.path.join(deployment_url, 'notebooks',
                                    basename if basename.endswith('ipynb')
@@ -196,121 +198,317 @@
             if r.status_code == 200:
                 return candidate
 
     # Check deployment_urls directly
     for deployment_url in deployment_urls:
         r = requests.get(deployment_url, verify=False)
         if r.status_code == 200:
-                return deployment_url
+            return deployment_url
     return None
 
-def generate_file_rst(app, src_dir, dest_dir, page, section, backend,
-                      img_extension, skip, deployment_urls):
+def get_nblink_md(
+    host, deployed_file, jupyterlite_url, download_as,
+    org, proj, ref, components, basename, ftype, section
+):
+    text = ''
+    if deployed_file:
+        text += f'[View a running version of this notebook]({deployed_file}) | '
+    if jupyterlite_url:
+        text += f'[Open this notebook in Jupyterlite]({jupyterlite_url}) | '
+    path = '/'.join(components)
+    if host == 'GitHub' and org and proj:
+        text += (
+            f'[Download this {ftype} from GitHub (right-click to download).]'
+            f'(https://raw.githubusercontent.com/{org}/{proj}/{ref}/{path}/{basename})'
+        )
+    elif host == 'assets':
+        if download_as == 'project':
+            text += f'[Download this project.](</assets/{section}.zip>)'
+        else:
+            text += f'[Download this {ftype}](</assets/{path}/{basename})'
+    return text
+
+def get_nblink_rst(
+    host, deployed_file, jupyterlite_url, download_as,
+    org, proj, ref, components, basename, ftype, section
+):
+    text = ''
+    if deployed_file:
+        text += f'`View a running version of this notebook <{deployed_file}>`_ | '
+    if jupyterlite_url:
+        text += f'`Open this notebook in Jupyterlite <{jupyterlite_url}>`_ | '
+    path = '/'.join(components)
+    if host == 'GitHub' and org and proj:
+        text += (
+            f'`Download this {ftype} from GitHub (right-click to download).'
+            f' <https://raw.githubusercontent.com/{org}/{proj}/{ref}/{path}/{basename}>`_'
+        )
+    elif host == 'assets':
+        if download_as == 'project':
+            text += f'`Download this project. </assets/{section}.zip>`_'
+        else:
+            text += f'`Download this {ftype}. </assets/{path}/{basename}>`_'
+    return text
+
+def convert_notebook_to_md(filename, directive='{pyodide}'):
+    with open(filename, encoding='utf-8') as nb:
+        nb_json = json.loads(nb.read())
+
+    md = ''
+    for cell in nb_json['cells']:
+        ctype = cell['cell_type']
+        if ctype == 'raw':
+            continue
+        if md:
+            md += '\n\n'
+        source = cell['source']
+        if ctype == 'code':
+            nticks = 4 if any('```' in src for src in source) else 3
+            backticks = '`'*nticks
+            md += f'{backticks}{directive}\n'
+        for src in source:
+            md += src
+        if ctype == 'code':
+            md += f'\n{backticks}'
+    return md
+
+def generate_pyodide_markdown(
+    app, page, section, backend, filename, src_dir, dest_dir,
+    img_extension, deployed_file, deployed, skip
+):
+    """
+    Generates a Markdown file that renders the notebook cells using
+    the pyodide directive.
+    """
+    # Set up paths
+    extension = filename.split('.')[-1]
+    basename = os.path.basename(filename)
+    md_path = os.path.join(dest_dir, basename[:-len(extension)].replace(' ', '_') + 'md')
+    name = basename[:-(len(extension)+1)]
+    title = ' '.join([n[0].capitalize()+n[1:] for n in name.replace('_', ' ').split(' ')])
+    ftype = 'notebook' if extension == 'ipynb' else 'script'
+
+    # Unpack config
     gallery_conf = app.config.nbsite_gallery_conf
+    examples_dir = gallery_conf['examples_dir']
     content = gallery_conf['galleries'][page]
+
+    # Download link options
     host = gallery_conf['host']
     download_as = gallery_conf['download_as']
-    ref = gallery_conf['github_ref']
+    host = gallery_conf['host']
     nblink = gallery_conf['nblink']
+    ref = gallery_conf['github_ref']
     org = gallery_conf['github_org']
     proj = gallery_conf['github_project']
+    jupyterlite_url = gallery_conf['jupyterlite_url']
+
+    # Deployed app options
+    endpoint = content.get('deployment_url', gallery_conf['deployment_url'])
+    iframe_spinner = gallery_conf['iframe_spinner']
+
+    skip_execute = gallery_conf['skip_execute']
+    directive = 'python' if skip_execute else '{pyodide}'
+
+    if nblink:
+        components = [examples_dir.split(os.path.sep)[-1], page]
+        if section:
+            components.append(section)
+        if backend:
+            components.append(backend)
+        if jupyterlite_url:
+            backend_slug = '/{backend}' if backend else ''
+            lite_path = f'{jupyterlite_url}?path=/{page}/{section}{backend_slug}/{basename}'
+        else:
+            lite_path = None
+        nblink_text = get_nblink_md(
+            host, deployed_file, lite_path, download_as,
+            org, proj, ref, components, basename, ftype, section
+        )
+
+    # Generate RST
+    with open(md_path, 'w') as md_file:
+        md_file.write(f'# {title}\n\n')
+
+        if nblink in ['top', 'both']:
+            md_file.write(f'{nblink_text}\n\n---\n')
+
+        if ftype == 'notebook':
+            nb_md = convert_notebook_to_md(filename, directive)
+            md_file.write(nb_md)
+        else:
+            with open(filename, encoding='utf-8') as script:
+                md_file.write(f'```{directive}\n{script.read()}```')
+        if deployed:
+            md_file.write(
+                IFRAME_TEMPLATE.format(
+                    background=iframe_spinner, url=endpoint+name
+                )
+            )
+
+        if nblink in ['bottom', 'both']:
+            md_file.write(f'\n\n---\n{nblink_text}')
+
+def generate_item_rst(
+    app, page, section, backend, filename, src_dir, dest_dir,
+    img_extension, deployed_file, deployed, skip
+):
+    """
+    Generates an RST file that includes a notebook directive to run
+    the example.
+    """
+    # Set up paths
+    extension = filename.split('.')[-1]
+    basename = os.path.basename(filename)
+    name = basename[:-(len(extension)+1)]
+    rel_path = os.path.relpath(os.path.join(src_dir, basename), dest_dir)
+    rst_path = os.path.join(dest_dir, basename[:-len(extension)].replace(' ', '_') + 'rst')
+    title = ' '.join([n[0].capitalize()+n[1:] for n in name.replace('_', ' ').split(' ')])
+    ftype = 'notebook' if extension == 'ipynb' else 'script'
+
+    # Unpack config
+    gallery_conf = app.config.nbsite_gallery_conf
     examples_dir = gallery_conf['examples_dir']
+    content = gallery_conf['galleries'][page]
     skip_execute = gallery_conf['skip_execute']
-    endpoint = gallery_conf['deployment_url']
+
+    # Download link options
+    download_as = gallery_conf['download_as']
+    host = gallery_conf['host']
+    nblink = gallery_conf['nblink']
+    ref = gallery_conf['github_ref']
+    org = gallery_conf['github_org']
+    proj = gallery_conf['github_project']
+    jupyterlite_url = gallery_conf['jupyterlite_url']
+
+    # Deployed app options
+    endpoint = content.get('deployment_url', gallery_conf['deployment_url'])
     iframe_spinner = gallery_conf['iframe_spinner']
+
+    # Do not write existing (unless auto-generated)
+    if os.path.isfile(rst_path):
+        with open(rst_path) as existing:
+            if 'Originally generated by nbsite' not in existing.read():
+                return
+
+    if nblink:
+        components = [examples_dir.split(os.path.sep)[-1], page]
+        if section:
+            components.append(section)
+        if backend:
+            components.append(backend)
+        nblink_text = get_nblink_rst(
+            host, deployed_file, jupyterlite_url, download_as,
+            org, proj, ref, components, basename, ftype, section
+        )
+
+    # Generate RST
+    with open(rst_path, 'w') as rst_file:
+        rst_file.write(title+'\n')
+        rst_file.write('='*len(title)+'\n\n')
+
+        if nblink in ['top', 'both']:
+            rst_file.write(f'{nblink_text}\n\n-------\n\n')
+
+        if ftype == 'notebook':
+            rst_file.write(".. notebook:: %s %s" % (proj, rel_path))
+            if deployed or (isinstance(skip, bool) and skip) or any(
+                basename.strip().endswith(skipped) for skipped in skip_execute
+            ):
+                rst_file.write('\n    :skip_execute: True\n')
+            if deployed:
+                rst_file.write(IFRAME_TEMPLATE.format(
+                    background=iframe_spinner, url=endpoint+name))
+        else:
+            rst_file.write(f'.. literalinclude:: {rel_path}\n\n')
+            url = os.path.join('thumbnails', f'{name}.{img_extension}')
+            rst_file.write(f'.. figure:: {url}\n\n')
+
+        if nblink in ['bottom', 'both']:
+            rst_file.write(f'\n\n-------\n\n{nblink_text}')
+
+def get_deployed_examples(endpoint):
+    # Try to fetch all deployed examples
+    if not bs4 or endpoint is None:
+        return []
+    r = requests.get(endpoint, verify=False)
+    if r.status_code != 200:
+        return []
+
+    soup = bs4.BeautifulSoup(r.content, features='lxml')
+    try:
+        deployed_examples = [
+            l.text for l in soup.find('div', {"class": "list-group"}).find_all('h4')
+        ]
+    except Exception:
+        deployed_examples = [
+            l.get('id')[1:] for l in soup.find('ul', {"class": "cards-grid"}).find_all('a', {"class": "card-link"})
+        ]
+        if not deployed_examples:
+            deployed_examples = [l.text for l in soup.find('ul').find_all('a')]
+    return deployed_examples
+
+def generate_file_rst(
+    app, src_dir, dest_dir, page, section, backend, img_extension, skip, deployment_urls
+):
+    gallery_conf = app.config.nbsite_gallery_conf
+    content = gallery_conf['galleries'][page]
+    endpoint = content.get('deployment_url', gallery_conf.get('deployment_url', None))
     extensions = content.get('extensions', gallery_conf['default_extensions'])
+    as_pyodide = content.get('as_pyodide', gallery_conf.get('as_pyodide', False))
 
-    components = [examples_dir.split(os.path.sep)[-1], page]
-    if section:
-        components.append(section)
-    if backend:
-        components.append(backend)
+    deployed_examples = get_deployed_examples(endpoint)
 
     files = []
     for extension in extensions:
         files += glob.glob(os.path.join(src_dir, extension))
 
-    # Try to fetch all deployed examples
-    deployed_examples = []
-    if bs4 and endpoint is not None:
-        r = requests.get(endpoint, verify=False)
-        if r.status_code == 200:
-            soup = bs4.BeautifulSoup(r.content, features='lxml')
-            try:
-                deployed_examples = [l.text for l in soup.find('div', {"class": "list-group"}).find_all('h4')]
-            except:
-                deployed_examples = [l.get('id')[1:] for l in soup.find('ul', {"class": "cards-grid"}).find_all('a', {"class": "card-link"})]
-            if not deployed_examples:
-                deployed_examples = [l.text for l in soup.find('ul').find_all('a')]
-
-    for f in files:
-        if isinstance(skip, list) and os.path.basename(f) in skip:
+    for filename in files:
+        if isinstance(skip, list) and os.path.basename(filename) in skip:
             continue
-        extension = f.split('.')[-1]
-        basename = os.path.basename(f)
-        rel_path = os.path.relpath(os.path.join(src_dir, basename), dest_dir)
-        rst_path = os.path.join(dest_dir, basename[:-len(extension)].replace(' ', '_') + 'rst')
+        extension = filename.split('.')[-1]
+        basename = os.path.basename(filename)
         name = basename[:-(len(extension)+1)]
-        title = ' '.join([n[0].capitalize()+n[1:] for n in name.replace('_', ' ').split(' ')])
         deployed = name in deployed_examples
-        ftype = 'notebook' if extension == 'ipynb' else 'script'
+        try:
+            deployed_file = get_deployed_url(deployment_urls, basename)
+        except Exception:
+            deployed_file = None
 
-        if os.path.isfile(rst_path):
-            with open(rst_path) as existing:
-                if not 'Originally generated by nbsite' in existing.read():
-                    continue
-
-        with open(rst_path, 'w') as rst_file:
-            rst_file.write(title+'\n')
-            rst_file.write('='*len(title)+'\n\n')
+        # Generate document
+        gen = generate_pyodide_markdown if as_pyodide else generate_item_rst
+        gen(app, page, section, backend, filename, src_dir, dest_dir,
+            img_extension, deployed_file, deployed, skip)
 
-            deployed_file = get_deployed_url(deployment_urls, basename)
-            if nblink in ['top', 'both']:
-                add_nblink(rst_file, host, deployed_file, download_as,
-                           org, proj, ref, components, basename, ftype, section)
-                rst_file.write('\n\n-------\n\n')
-
-            if ftype == 'notebook':
-                rst_file.write(".. notebook:: %s %s" % (proj, rel_path))
-                if deployed or (isinstance(skip, bool) and skip) or any(basename.strip().endswith(skipped) for skipped in skip_execute):
-                    rst_file.write('\n    :skip_execute: True\n')
-                if deployed:
-                    rst_file.write(IFRAME_TEMPLATE.format(
-                        background=iframe_spinner, url=endpoint+name))
-            else:
-                rst_file.write('.. literalinclude:: %s\n\n' % rel_path)
-                url = os.path.join('thumbnails', '%s.%s' % (name, img_extension))
-                rst_file.write('.. figure:: %s\n\n' % url)
-
-            if nblink in ['bottom', 'both']:
-                rst_file.write('\n\n-------\n\n')
-                add_nblink(rst_file, host, deployed_file, download_as,
-                           org, proj, ref, components, basename, ftype, section)
 
-def add_nblink(rst_file, host, deployed_file, download_as,
-               org, proj, ref, components, basename, ftype, section):
-    if deployed_file:
-        rst_file.write(f'`View a running version of this notebook. <{deployed_file}>`_ | ')
-    if host == 'GitHub' and org and proj:
-        rst_file.write('`Download this {ftype} from GitHub (right-click to download).'
-                        ' <https://raw.githubusercontent.com/{org}/{proj}/{ref}/{path}/{basename}>`_'.format(
-                            org=org, proj=proj, ref=ref, path='/'.join(components),
-                            basename=basename, ftype=ftype))
-    elif host == 'assets':
-        if download_as == 'project':
-            rst_file.write(f'`Download this project. </assets/{section}.zip>`_')
-        else:
-            rst_file.write('`Download this {ftype}. </assets/{path}/{basename}>`_'.format(
-                                path='/'.join(components), basename=basename, ftype=ftype))
+REDIRECT = """.. raw:: html
 
+    <head>
+        <meta http-equiv='refresh' content='0; URL={rel}/index.html#{section}'>
+    </head>
+"""
+
+def generate_section_index(section, items, dest_dir, rel='..', title=None):
+    """
+    Builds index pages for each section which redirect to the main
+    gallery index.
+    """
+    # Reference to section header
+    section_ref = section.lower().replace(' ', '-')
+    index_page = REDIRECT.format(rel=rel, section=section_ref)
+    title = title or section
+    index_page += '\n' + title + '\n' + '_'*len(title) + '\n'
+    index_page += '\n\n.. toctree::\n   :glob:\n   :hidden:\n\n   '
+    index_page += '\n   '.join(items)
+    with open(os.path.join(dest_dir, 'index.rst'), 'w') as f:
+        f.write(index_page)
 
 def _normalize_label(string):
     return ' '.join([s[0].upper()+s[1:] for s in string.split('_')])
 
-
 def _thumbnail_div(thumb_path, section, backend, fname, normalize=True, title=None):
     """Generates RST to place a thumbnail in a gallery"""
     if title is not None:
         label = title
     elif normalize:
         label = _normalize_label(fname)
     else:
@@ -371,14 +569,16 @@
     gallery_dir = os.path.join(examples_dir, page)
     static_dir = app.config.html_static_path[-1]
     static_path = os.path.join(
         os.path.split(gallery_conf['examples_dir'])[-2], static_dir)
     labels_dir = gallery_conf['labels_dir']
     labels_path = os.path.join(static_path, labels_dir)
     logo = app.config.html_theme_options.get('logo', 'images/logo.png')
+    if isinstance(logo, dict):
+        logo = logo['image_light']
     logo_path = os.path.join(static_path, logo)
 
     if 'sections' in content:
         sections = content['sections']
     else:
         sections = [s for s in glob.glob(os.path.join(gallery_dir, '*'))
                     if os.path.isdir(os.path.join(gallery_dir, s)) and
@@ -390,27 +590,31 @@
     sort_fn = gallery_conf['within_subsection_order']
     thumbnail_url = gallery_conf['thumbnail_url']
     download = gallery_conf['enable_download']
     script_prefix = gallery_conf['script_prefix']
     only_use_existing = gallery_conf['only_use_existing']
     inline = gallery_conf['inline']
 
+    if sort_fn is None:
+        sort_fn = lambda key: titles.get(key, key)
+
     # Write gallery index
     title = content['title']
     gallery_rst = title + '\n' + '_'*len(title) + '\n'
     if 'intro' in content:
         gallery_rst += '\n' + content['intro'] + '\n'
 
     if backends:
         buttons = []
         for n, backend in enumerate(backends):
             buttons.append(BUTTON_TEMPLATE.format(N=n+1, checked='' if n else 'checked="checked"',
                                                   label=backend.capitalize()))
         gallery_rst += BUTTON_GROUP_TEMPLATE.format(buttons=''.join(buttons), backends=backends)
 
+    toc = '\n\n.. toctree::\n   :glob:\n   :hidden:\n\n'
     for section in sections:
         if isinstance(section, dict):
             section_backends = section.get('backends', backends)
             skip = section.get('skip', content.get('skip', False))
             orphans = section.get('orphans', content.get('orphans', []))
             heading = section.get('title', section['path'])
             description = section.get('description', None)
@@ -424,27 +628,24 @@
             orphans = content.get('orphans', [])
             section_backends = backends
             subsection_order = sort_fn
             description = None
             labels = []
             deployment_urls = []
 
-        if not heading:
-            pass
-        elif inline:
-            gallery_rst += f'\n\n.. toctree::\n   :glob:\n   :hidden:\n   :maxdepth: 2\n\n   {section}/*'
-        else:
-            underline = '-'*len(heading)
-            gallery_rst += f'\n\n{heading}\n{underline}\n\n'
-
+        # Add section toctree
         if section:
-            gallery_rst += f'.. toctree::\n   :glob:\n   :hidden:\n\n   {heading}\n   {section}/*\n\n'
+            toc += f'   {section}/index\n'
         else:
             gallery_rst += f'.. toctree::\n   :glob:\n   :hidden:\n\n   {heading}\n   *\n\n'
 
+        if heading:
+            underline = '-'*len(heading)
+            gallery_rst += f'\n\n{heading}\n{underline}\n\n'
+
         if labels:
             gallery_rst += '\n\n.. raw:: html\n\n'
             for label in sorted(labels):
                 label_svg = os.path.join(labels_path, f'{label}.svg')
                 if not os.path.exists(os.path.join(doc_dir, label_svg)):
                     logger.info(
                         f'Control the look of the {label} label by adding '
@@ -457,26 +658,38 @@
 
         if description:
             gallery_rst += description + '\n\n'
 
         gallery_rst += '.. grid:: 2 2 4 5\n    :gutter: 3\n    :margin: 0\n'
 
         thumb_extension = 'png'
+
+        path_components = [page]
+        if section:
+            path_components.append(section)
+        dest_path = os.path.join(doc_dir, *path_components)
+        section_path = os.path.join(examples_dir, *path_components)
+
+        try:
+            os.makedirs(dest_path)
+        except Exception:
+            pass
+        if section and section_backends:
+            backend_items = [f'{item}/index' for item in section_backends]
+            generate_section_index(heading, backend_items, dest_path)
         for backend in (section_backends or ('',)):
-            path_components = [page]
-            if section:
-                path_components.append(section)
+            path = section_path
+            dest_dir = dest_path
             if backend:
-                path_components.append(backend)
+                path = os.path.join(path, backend)
+                dest_dir = os.path.join(dest_path, backend)
 
-            path = os.path.join(examples_dir, *path_components)
-            dest_dir = os.path.join(doc_dir, *path_components)
             try:
                 os.makedirs(dest_dir)
-            except:
+            except Exception:
                 pass
 
             # Collect examples
             files = []
             for extension in extensions:
                 files += glob.glob(os.path.join(path, extension))
 
@@ -491,14 +704,23 @@
                 if backend:
                     backend_str = ' for %s backend' % backend
                 else:
                     backend_str = ''
                 logger.info("\n\nGenerating %d %s %s examples%s\n"
                             "__________________________________________________"
                             % (len(files), heading, title, backend_str))
+                if section:
+                    section_items = [
+                        os.path.basename(f).split('.')[0] for f in sorted(files)
+                    ]
+                    generate_section_index(
+                        heading, section_items, dest_dir,
+                        rel='../..' if backend else '..',
+                        title=backend.title() if backend else None
+                    )
 
             for f in sorted(files, key=subsection_order):
                 extension = f.split('.')[-1]
                 basename = os.path.basename(f)[:-(len(extension)+1)]
 
                 # Try to fetch thumbnail otherwise regenerate it
                 url_components = [thumbnail_url, page]
@@ -523,21 +745,28 @@
 
                 if os.path.isfile(thumb_path):
                     verb = 'Used existing'
                     retcode = 0
 
                 # Try download
                 if download and retcode:
-                    thumb_req = requests.get(thumb_url, verify=False)
+                    try:
+                        thumb_req = requests.get(thumb_url)
+                    except Exception:
+                        thumb_req = requests.get(thumb_url, verify=False)
+
                     verb = 'Successfully downloaded'
                     if thumb_req.status_code == 200:
                         verb = 'Successfully downloaded'
                         retcode = 0
                     else:
-                        thumb_req = requests.get(thumb_url[:-4]+'.gif', verify=False)
+                        try:
+                            thumb_req = requests.get(thumb_url[:-4]+'.gif')
+                        except Exception:
+                            thumb_req = requests.get(thumb_url[:-4]+'.gif', verify=False)
                         if thumb_req.status_code == 200:
                             thumb_extension = 'gif'
                             thumb_path = thumb_path[:-4]+'.gif'
                             retcode = 0
                     if not retcode:
                         with open(thumb_path, 'wb') as thumb_f:
                             thumb_f.write(thumb_req.content)
@@ -585,25 +814,28 @@
                         link = basename
                     this_entry = THUMBNAIL_TEMPLATE.format(
                         backend_prefix=backend+'-', thumbnail=logo_path,
                         label=label, link=link,
                     )
                 else:
                     logger.info('%s %s thumbnail' % (verb, basename))
-                    thumb_path = os.path.join(*path_components+['thumbnails', '%s.%s' % (basename, thumb_extension)])
+                    thumb_path = os.path.join(
+                        dest_dir, 'thumbnails', f'{basename}.{thumb_extension}'
+                    )
                     if thumb_extension not in ('svg', 'gif'):
                         resize_pad(os.path.join(doc_dir, thumb_path))
                     this_entry = _thumbnail_div(
                         thumb_path, section, backend, basename,
                         normalize, titles.get(basename)
                     )
 
                 gallery_rst += this_entry
             generate_file_rst(app, path, dest_dir, page, section,
                               backend, thumb_extension, skip, deployment_urls)
+    gallery_rst += toc
 
     if backends or section_backends:
         gallery_rst += HIDE_JS.format(backends=repr(backends[1:]))
     with open(os.path.join(doc_dir, page, 'index.rst'), 'w') as f:
         f.write(gallery_rst)
```

### Comparing `nbsite-0.8.0rc9/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.1a1/nbsite/gallery/thumbnailer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import unicode_literals
-import os, sys, subprocess, ast
-from nbconvert.preprocessors import Preprocessor
+
+import ast
+import os
+import subprocess
+import sys
+import tempfile
+
+import matplotlib.pyplot as plt
 
 from holoviews.core import Dimensioned, Store
-from holoviews.ipython.preprocessors import OptsMagicProcessor, OutputMagicProcessor
-from holoviews.ipython.preprocessors import StripMagicsProcessor
+from holoviews.ipython.preprocessors import (
+    OptsMagicProcessor, OutputMagicProcessor, StripMagicsProcessor,
+)
 from holoviews.util.command import export_to_python
+from nbconvert.preprocessors import Preprocessor
 
-import tempfile
-import matplotlib.pyplot as plt
 plt.switch_backend('agg')
 
 def comment_out_magics(source):
     """
     Utility used to make sure AST parser does not choke on unrecognized
     magics.
     """
```

### Comparing `nbsite-0.8.0rc9/nbsite/nbbuild.py` & `nbsite-0.8.1a1/nbsite/nbbuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 """
 Copyright (c) 2017-2021 HoloViz developers.
 
 Copyright (c) 2013 Nathan Goldbaum. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
@@ -23,48 +24,55 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-import io, json, os, string, glob, copy, re, sys, shutil
+import copy
+import glob
+import io
+import json
+import os
+import re
+import shutil
+import string
+import sys
 
 from collections import OrderedDict
 from contextlib import contextmanager
 
 import nbformat
 
-from docutils.parsers.rst import directives, Directive
+from docutils.parsers.rst import Directive, directives
 from docutils.statemachine import string2lines
 from docutils.utils import new_document
 from myst_nb.sphinx_ import Parser
-
 from nbconvert import NotebookExporter, PythonExporter
 from nbconvert.preprocessors import (
-    ExecutePreprocessor, CellExecutionError, Preprocessor
+    CellExecutionError, ExecutePreprocessor, Preprocessor,
 )
-from .cmd import hosts, _prepare_paths
+
+from .cmd import _prepare_paths, hosts
 
 NOTEBOOK_VERSION = 4
 
-interactivity_warning_binder = """
-This web page was generated from a Jupyter notebook and not all 
-interactivity will work on this website. <a
-href="{download_link}">Right-click to download and run</a> or <a 
-href="{binder_link}">Launch on Binder</a> for full Python-backed 
-interactivity.
-"""
+interactivity_warning_binder = (
+    'This web page was generated from a Jupyter notebook and not all '
+    'interactivity will work on this website. <a href="{download_link}">'
+    'Right-click to download and run</a> or <a href="{binder_link}">'
+    'Launch on Binder</a> for full Python-backed interactivity.'
+)
 
-interactivity_warning = """
-This web page was generated from a Jupyter notebook and not all 
-interactivity will work on this website. <a 
-href="{download_link}">Right click to download and run locally</a> for full 
-Python-backed interactivity.
-"""
+interactivity_warning = (
+    'This web page was generated from a Jupyter notebook and not all '
+    'interactivity will work on this website. <a href="{download_link}">'
+    'Right click to download and run locally</a> for full Python-backed '
+    'interactivity.'
+)
 
 #from nbformat.v4 import output_from_msg
 class ExecutePreprocessor1000(ExecutePreprocessor):
     """Sigh"""
     _ipython_startup = None
 
     @property
@@ -120,15 +128,15 @@
 
     def _find_slice(self, nbc, substring, endstr):
         start = 0 if substring is None else None
         end = None
         try:
             end = int(endstr)
             count = 0
-        except:
+        except Exception:
             count = None
 
         for ind, cell in enumerate(nbc.cells):
             source = cell['source']
             if start is None and substring in source:
                 start = ind
             if None not in [start, count]:
@@ -309,15 +317,15 @@
         # Restore execution mode
         if hasattr(env, 'mystnb_config'):
             env.mystnb_config.execution_mode = old_exec_mode
 
 @contextmanager
 def patch_project_source_suffix(env):
     # Ugly patch required as myst-nb obtains a reader that
-    # is infered by sphinx from the document, sphinx literally
+    # is inferred by sphinx from the document, sphinx literally
     # loops through a glob() result looking for files in a particular
     # order, starting from .rst. As the NotebookDirective is embedded
     # in a .rst, it finds that file instead of the Notebook to be parsed.
     # Overriding this dict temporarily seems to do the trick.
     old_source_suffix = env.project.source_suffix
     env.project.source_suffix = OrderedDict([('.ipynb', 'myst-nb')])
     try:
@@ -406,15 +414,15 @@
                     self.options.get('offset')
                 )
             )
         if self.options.get('skip_output'):
             preprocessors.append(SkipOutput(self.options['skip_output']))
         return preprocessors
 
-    def interactivity_warning(self, nb_abs_path):        
+    def interactivity_warning(self, nb_abs_path):
         project_name = os.environ.get('PROJECT_NAME','')
         project_root = os.environ.get('PROJECT_ROOT','')
         host = os.environ.get('HOST','GitHub')
         branch = os.environ.get('BRANCH','main')
         repo = os.environ.get('REPO','')
         org = os.environ.get('ORG','')
         doc = os.environ.get('DOC','doc')
@@ -428,15 +436,15 @@
             org = repo
 
         paths = _prepare_paths(project_root, examples=examples,
                                doc=doc, examples_assets=examples_assets)
         relpath = os.path.relpath(nb_abs_path, paths['examples'])
         dl_link = get_download_link(relpath, org, branch, repo, examples, host)
         binder_link = get_binder_link(relpath, org, repo, branch, examples)
-        
+
         if binder == 'none':
             inner_msg = interactivity_warning.format(download_link=dl_link)
         else:
             inner_msg = interactivity_warning_binder.format(download_link=dl_link,
                                                             binder_link=binder_link)
         inner_msg = inner_msg.replace('\n', '')
         scroller = f'<div id="scroller-right">{inner_msg}</div>'
@@ -465,28 +473,28 @@
             patterns_to_take_with_me=setup.config.nbbuild_patterns_to_take_along
         )
 
         preprocessors = self.preprocessors(dest_dir)
         rendered_nodes = render_notebook(
             dest_path, self.state.document, preprocessors
         )
-        
+
         link_rst = self.link_rst(nb_basename, nb_abs_path, dest_path)
-        if not ('disable_interactivity_warning' in self.options):
+        if 'disable_interactivity_warning' not in self.options:
             link_rst += self.interactivity_warning(nb_abs_path)
 
         # Insert evaluated notebook HTML into Sphinx
         if link_rst:
             include_lines = string2lines(link_rst, convert_whitespace=True)
             self.state_machine.insert_input(include_lines, rst_file)
 
         # add dependency
         self.state.document.settings.record_dependencies.add(nb_abs_path)
 
-        # TODO: doubt this isdoing anyting
+        # TODO: doubt this is doing anything
         # clean up png files left behind by notebooks.
         png_files = glob.glob("*.png")
         for file in png_files:
             os.remove(file)
 
         return rendered_nodes
```

### Comparing `nbsite-0.8.0rc9/nbsite/paramdoc.py` & `nbsite-0.8.1a1/nbsite/paramdoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+
 from functools import partial
 
 import param
 
 from param.parameterized import label_formatter
 
 param.parameterized.docstring_signature = False
```

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.1a1/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.1a1/nbsite/pyodide/WebWorker.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,17 @@
 importScripts("{{ PYODIDE_URL }}");
 
 const QUEUE = [];
 
+const REQUIRES = {
+    {
+        requires
+    }
+}
+
 function sendPatch(patch, buffers, cell_id) {
     self.postMessage({
         type: 'patch',
         patch: patch,
         buffers: buffers,
         id: cell_id
     })
@@ -23,82 +29,84 @@
     self.postMessage({
         type: 'stderr',
         content: stderr,
         id: cell_id
     })
 }
 
-async function loadApplication(cell_id) {
+async function loadApplication(cell_id, path) {
     console.log("Loading pyodide!");
     self.pyodide = await loadPyodide();
     self.pyodide.globals.set("sendPatch", sendPatch);
     self.pyodide.globals.set("sendStdout", sendStdout);
     self.pyodide.globals.set("sendStderr", sendStderr);
     console.log("Loaded!");
     await self.pyodide.loadPackage("micropip");
     const packages = [{
         {
             env_spec
         }
     }];
+    if (path != null) {
+        for (const key of Object.keys(REQUIRES)) {
+            if (path.replace('.html', '').endsWith(key.replace('.md', ''))) {
+                for (const req of REQUIRES[key]) {
+                    packages.push(req)
+                }
+            }
+        }
+    }
+
     await self.pyodide.runPythonAsync("{{ setup_code }}")
     self.pyodide.runPython("import micropip")
     for (const pkg of packages) {
         self.postMessage({
             type: 'loading',
             msg: `Loading ${pkg}`,
             id: cell_id
         });
         await self.pyodide.runPythonAsync(`
-      await micropip.install('${pkg}');
+      await micropip.install('${pkg}', keep_going=True);
     `);
     }
     console.log("Packages loaded!");
 }
 
-function autodetect_deps_code(msg) {
-    const escaped = msg.code.replace(/"""/g, '\\"\\"\\"');
-    return `
+const autodetect_deps_code = `
 import json
 from panel.io.mime_render import find_imports
-code = r"""\n${escaped}""".replace(r'\\"\\"\\"', '"""')
-json.dumps(find_imports(code))`
-}
+json.dumps(find_imports(msg.to_py()['code']))`
 
-function exec_code(msg) {
-    const escaped = msg.code.replace(/"""/g, '\\"\\"\\"');
-    return `
+const exec_code = `
 from functools import partial
 from panel.io.pyodide import pyrender
 from js import console
 
-code = r"""\n${escaped}""".replace(r'\\"\\"\\"', '"""')
-stdout_cb = partial(sendStdout, '${msg.id}')
-stderr_cb = partial(sendStderr, '${msg.id}')
-target = 'output-${msg.id}'
+msg = msg.to_py()
+code = msg['code']
+stdout_cb = partial(sendStdout, msg['id'])
+stderr_cb = partial(sendStderr, msg['id'])
+target = f"output-{msg['id']}"
 pyrender(code, stdout_cb, stderr_cb, target)`
-}
 
-function onload_code(msg) {
-    return `
-if '${msg.mime}' == 'application/bokeh':
+const onload_code = `
+msg = msg.to_py()
+if msg['mime'] == 'application/bokeh':
     from panel.io.pyodide import _link_docs_worker
     from panel.io.state import state
-    doc = state.cache['output-${msg.id}']
-    _link_docs_worker(doc, sendPatch, '${msg.id}', 'js')
-`
-}
+    doc = state.cache[f"output-{msg['id']}"]
+    _link_docs_worker(doc, sendPatch, msg['id'], 'js')`
 
-function patch_code(msg) {
-    return `
+const patch_code = `
 import json
 from panel import state
-doc = state.cache['output-${msg.id}']
-doc.apply_json_patch(json.loads('${msg.patch}'), setter='js')`
-}
+
+msg = msg.to_py()
+doc = state.cache[f"output-{msg['id']}"]
+doc.apply_json_patch(msg['patch'], setter='js')`
 
 const MESSAGES = {
     patch: patch_code,
     execute: exec_code,
     rendered: onload_code
 }
 
@@ -128,15 +136,15 @@
     // Init pyodide
     if (self.pyodide == null) {
         self.postMessage({
             type: 'loading',
             msg: 'Loading pyodide',
             id: msg.id
         });
-        await loadApplication(msg.id)
+        await loadApplication(msg.id, msg.path)
         self.postMessage({
             type: 'loaded',
             id: msg.id
         });
     }
 
     // Handle message
@@ -153,37 +161,39 @@
     {
         %
         if autodetect_deps %
     }
     if (msg.type === 'execute') {
         let deps
         try {
-            deps = self.pyodide.runPython(autodetect_deps_code(msg))
+            self.pyodide.globals.set('msg', msg)
+            deps = self.pyodide.runPython(autodetect_deps_code)
         } catch (e) {
             deps = '[]'
             console.warn(`Auto-detection of dependencies failed with error: ${e}`)
         }
         for (const pkg of JSON.parse(deps)) {
             self.postMessage({
                 type: 'loading',
                 msg: `Loading ${pkg}`,
                 id: msg.id
             });
             try {
-                await self.pyodide.runPythonAsync(`await micropip.install('${pkg}')`)
+                await self.pyodide.runPythonAsync(`await micropip.install('${pkg}', keep_going=True)`)
             } catch (e) {
                 console.log(`Auto-detected dependency ${pkg} could not be installed.`)
             }
         }
     } {
         % endif %
     }
 
     try {
-        let out = await self.pyodide.runPythonAsync(MESSAGES[msg.type](msg))
+        self.pyodide.globals.set('msg', msg)
+        let out = await self.pyodide.runPythonAsync(MESSAGES[msg.type])
         resolveExecution()
         if (out == null) {
             out = new Map()
         }
         if (out.has('content')) {
             self.postMessage({
                 type: 'render',
```

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.1a1/nbsite/pyodide/WorkerHandler.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -23,15 +23,15 @@
                 }
             }
         }
         events.push(event)
         pyodideWorker.queues.set(doc_id, events)
         return
     }
-    const patch = jsdoc.create_json_patch_string([event])
+    const patch = jsdoc.create_json_patch([event])
     const uuid = uid()
     pyodideWorker.busy = uuid
     pyodideWorker.postMessage({
         type: 'patch',
         patch: patch,
         id: doc_id,
         uuid
@@ -44,15 +44,15 @@
     const stdout = document.getElementById(`stdout-${event.data.id}`)
     const stderr = document.getElementById(`stderr-${event.data.id}`)
     const msg = event.data;
 
     if (msg.uuid == pyodideWorker.busy) {
         if (pyodideWorker.queues.size) {
             const [msg_id, events] = pyodideWorker.queues.entries().next().value
-            const patch = pyodideWorker.documents[msg_id].create_json_patch_string(events)
+            const patch = pyodideWorker.documents[msg_id].create_json_patch(events)
             const uuid = uid()
             pyodideWorker.busy = uuid
             pyodideWorker.postMessage({
                 type: 'patch',
                 patch: patch,
                 id: msg_id,
                 uuid
@@ -98,12 +98,12 @@
         }
         pyodideWorker.postMessage({
             type: 'rendered',
             id: msg.id,
             mime: msg.mime
         })
     } else if (msg.type === 'patch') {
-        pyodideWorker.documents[msg.id].apply_json_patch(JSON.parse(msg.patch), msg.buffers, setter_id = 'py')
+        pyodideWorker.documents[msg.id].apply_json_patch(msg.patch, msg.buffers, setter_id = 'py')
     }
 };
 
 window.pyodideWorker = pyodideWorker;
```

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/__init__.py` & `nbsite-0.8.1a1/nbsite/pyodide/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-import importlib
 import io
 import json
-import re
+import sys
+import warnings
 
 from collections import defaultdict
 from html import escape
 from multiprocessing import Pipe, Process
 from pathlib import Path
-from typing import Any, Dict, List, Tuple
+from typing import (
+    Any, Dict, List, Tuple,
+)
 
-from docutils import nodes
-from docutils.parsers.rst import Directive, roles
-from jinja2.environment import Environment
-from jinja2.loaders import FileSystemLoader
-from sphinx.application import Sphinx
+import param
 
 from bokeh.document import Document
+from bokeh.embed.bundle import _bundle_extensions
 from bokeh.embed.util import standalone_docs_json_and_render_items
 from bokeh.model import Model
-from panel.config import panel_extension
+from docutils import nodes
+from docutils.parsers.rst import Directive, roles
+from jinja2.environment import Environment
+from jinja2.loaders import FileSystemLoader
+from packaging.version import Version
+from panel.config import config, panel_extension as extension
 from panel.io.convert import BOKEH_VERSION
 from panel.io.mime_render import exec_with_return, format_mime
-from panel.io.resources import CDN_DIST, set_resource_mode
-from panel.pane import panel as as_panel
-from panel.util import is_holoviews
+from panel.io.resources import CDN_DIST, Resources, set_resource_mode
+from panel.pane import HoloViews, Interactive, panel as as_panel
+from panel.reactive import ReactiveHTML
 from panel.viewable import Viewable, Viewer
+from sphinx.application import Sphinx
 
 HERE = Path(__file__).parent
 
 def get_env() -> Environment:
     ''' Get the correct Jinja2 Environment, also for frozen scripts.
     '''
     return Environment(loader=FileSystemLoader(HERE))
@@ -39,22 +44,31 @@
 
 WEB_WORKER_TEMPLATE = _env.get_template('WebWorker.js')
 WORKER_HANDLER_TEMPLATE = _env.get_template('WorkerHandler.js')
 SERVICE_WORKER_TEMPLATE = _env.get_template('ServiceWorker.js')
 SERVICE_HANDLER_TEMPLATE = _env.get_template('ServiceHandler.js')
 WEB_MANIFEST_TEMPLATE = _env.get_template('site.webmanifest')
 
+JS_MODULE_TAG = """
+<script type="module" src="{file}"></script>"""
+JS_MODULE_EXPORT = """
+<script type="module">
+  import {name} from "{file}";
+  window.{name} = {name}
+</script>
+"""
+
 bokeh_version = Version(BOKEH_VERSION)
 if bokeh_version.is_devrelease or bokeh_version.is_prerelease:
     bk_prefix = 'dev'
 else:
     bk_prefix = 'release'
 
 DEFAULT_PYODIDE_CONF = {
-    'PYODIDE_URL': 'https://cdn.jsdelivr.net/pyodide/v0.21.3/full/pyodide.js',
+    'PYODIDE_URL': 'https://cdn.jsdelivr.net/pyodide/v0.23.1/full/pyodide.js',
     'autodetect_deps': True,
     'enable_pwa': True,
     'requirements': ['panel', 'pandas'],
     'precache': [],
     'scripts': [
         f'https://cdn.bokeh.org/bokeh/{bk_prefix}/bokeh-{BOKEH_VERSION}.min.js',
         f'https://cdn.bokeh.org/bokeh/{bk_prefix}/bokeh-widgets-{BOKEH_VERSION}.min.js',
@@ -66,42 +80,58 @@
         CDN_DIST,
         'https://cdn.bokeh.org/bokeh/',
         'https://cdn.jsdelivr.net/pyodide/',
         'https://files.pythonhosted.org/packages/',
         'https://pypi.org/pypi/'
     ],
     'setup_code': "",
-    'warn_message': "Executing this cell will download Python runtime (typically 40+ MB)."
+    'warn_message': "Executing this cell will download Python runtime (typically 40+ MB).",
+    'requires': {}
 }
 
-EXTRA_RESOURCES = defaultdict(lambda: {'js': [], 'css': []})
+EXTRA_RESOURCES = defaultdict(lambda: {'js': [], 'css': [], 'js_modules': {}, 'js_exports': {}})
 
 def extract_extensions(code: str) -> List[str]:
     """
     Extracts JS and CSS dependencies of Panel extensions from code snippets
     containing pn.extension calls.
     """
-    ext_args = re.findall(r'pn.extension\((.*)\)', code)
-    if not ext_args:
-        return [], []
-    extensions = re.findall(r"(?<!=)\s*['\"](.*?)['\"]", ext_args[0])
-    prev_models = dict(Model.model_class_reverse_map)
-    for ext in extensions:
-        if ext not in panel_extension._imports:
-            continue
-        importlib.import_module(panel_extension._imports[ext])
-    js, css = [], []
+    js, js_exports, js_modules, css = [], {}, {}, []
     with set_resource_mode('cdn'):
         for name, model in Model.model_class_reverse_map.items():
-            if name not in prev_models:
-                if hasattr(model, '__javascript__'):
-                    js += model.__javascript__
-                if hasattr(model, '__css__'):
-                    css += model.__css__
-    return js, css
+            if hasattr(model, '__javascript__'):
+                js += model.__javascript__
+            if hasattr(model, '__css__'):
+                css += model.__css__
+            if hasattr(model, '__javascript_module_exports__'):
+                js_exports.update(
+                    dict(zip(model.__javascript_module_exports__,
+                             model.__javascript_modules__))
+                )
+        for model in param.concrete_descendents(ReactiveHTML).values():
+            if not model._loaded():
+                continue
+            js += getattr(model, '__javascript__', []) or []
+            css += getattr(model, '__css__', []) or []
+    if config.design and hasattr(config.design, 'resolve_resources'):
+        design_resources = config.design().resolve_resources(
+            cdn=True, include_theme=True
+        )
+        js += list(design_resources['js'].values())
+        css += list(design_resources['css'].values())
+        js_modules.update(design_resources['js_modules'])
+    resources = Resources(mode='cdn')
+    extensions = _bundle_extensions(None, resources)
+    js += [bundle.cdn_url for bundle in extensions if bundle.cdn_url and
+           '@holoviz/panel@' not in bundle.cdn_url]
+    global_exports = [
+        extension._globals[ext][0] for ext, imp in extension._imports.items()
+        if imp in sys.modules and ext in extension._globals
+    ]
+    return js, js_exports, js_modules, css, global_exports
 
 def _model_json(model: Model, target: str) -> Tuple[Document, str]:
     """
     Renders a Bokeh Model to JSON representation given a particular
     DOM target and returns the Document and the serialized JSON string.
 
     Arguments
@@ -153,20 +183,15 @@
         'skip-embed': _option_boolean
     }
 
     _current_source = None
     _current_context = {}
     _current_count = 0
     _current_process = None
-    _client = None
-    _listener = None
     _conn = None
-    _send_address = ('localhost', 33355)
-    _rcv_address = ('localhost', 33356)
-    _password = b'pyodide'
 
     @classmethod
     def _execution_process(cls, pipe):
         """
         Process execution loop to run in separate process that is used
         to evaluate code.
         """
@@ -175,54 +200,66 @@
             if msg['type'] == 'close':
                 break
             elif msg['type'] != 'execute':
                 continue
             stdout = io.StringIO()
             stderr = io.StringIO()
             code = msg['code']
-            js, css = extract_extensions(code)
             with set_resource_mode('cdn'):
                 try:
                     out = exec_with_return(code, stdout=stdout, stderr=stderr)
                 except Exception:
                     out = None
-                if isinstance(out, (Model, Viewable, Viewer)) or is_holoviews(out):
+                if isinstance(out, (Model, Viewable, Viewer)) or HoloViews.applies(out) or Interactive.applies(out):
                     _, content = _model_json(as_panel(out), msg['target'])
                     mime_type = 'application/bokeh'
                 elif out is not None:
-                    content, mime_type = format_mime(out)
+                    try:
+                        content, mime_type = format_mime(out)
+                    except Exception:
+                        warnings.warn(f'Could not render {out!r} generated from executed code directive: {code}')
                 else:
                     content, mime_type = None, None
-            pipe.send((content, mime_type, stdout.getvalue(), stderr.getvalue(), js, css))
+            js, js_exports, js_modules, css, global_exports = extract_extensions(code)
+            pipe.send((content, mime_type, stdout.getvalue(), stderr.getvalue(), js, js_exports, js_modules, css, global_exports))
         pipe.close()
 
     @classmethod
     def terminate(cls, *args):
         """
         Terminates a running process.
         """
         if not cls._current_process:
             return
-        cls._conn.send({'type': 'close'})
-        cls._current_process.join()
-        cls._current_process = None
+        try:
+            cls._conn.send({'type': 'close'})
+            cls._current_process.join()
+        except Exception:
+            cls._current_process.terminate()
+        finally:
+            cls._current_process = None
 
     @classmethod
     def _launch_process(cls, timeout=5):
         """
         Launches a process to execute code in.
         """
         cls.terminate()
         cls._conn, child_conn = Pipe()
         cls._current_process = Process(target=cls._execution_process, args=(child_conn,))
         cls._current_process.start()
 
+    @classmethod
+    def _kill(cls):
+        cls._current_process.terminate()
+        cls._current_process = None
+
     def run(self):
         current_source = self.state_machine.get_source()
-        if self._current_source != current_source:
+        if self._current_source != current_source or self._current_process is None:
             PyodideDirective._current_count = 0
             PyodideDirective._current_source = current_source
             self._launch_process()
 
         classes = 'pyodide'
         if 'class' in self.options:
             classes += f" {self.options['class']}"
@@ -235,38 +272,55 @@
 
         PyodideDirective._current_count += 1
         if self.options.get('skip-embed'):
             return [doctree_node]
 
         # Send execution request to client and wait for result
         self._conn.send({'type': 'execute', 'target': f'output-{cellid}', 'code': code})
-        output, mime_type, stdout, stderr, js, css = self._conn.recv()
+        if self._conn.poll(60):
+            try:
+                output, mime_type, stdout, stderr, js, js_exports, js_modules, css, global_exports = (
+                    self._conn.recv()
+                )
+            except Exception:
+                self._kill()
+                return [doctree_node]
+        else:
+            self._kill()
+            return [doctree_node]
         EXTRA_RESOURCES[current_source]['js'] += js
+        EXTRA_RESOURCES[current_source]['js_exports'].update(js_exports)
+        EXTRA_RESOURCES[current_source]['js_modules'].update(js_modules)
         EXTRA_RESOURCES[current_source]['css'] += css
 
         stdout_style = 'style="display: block;"' if stdout else ''
         stdout_html = f'<pre id="stdout-{cellid}" class="pyodide-stdout" {stdout_style}>{escape(stdout)}</pre>'
         stdout_node = nodes.raw(stdout, stdout_html, format='html')
 
         stderr_style = 'style="display: block;"' if stderr else ''
         stderr_html = f'<pre id="stderr-{cellid}" class="pyodide-stderr" {stderr_style}>{escape(stderr)}</pre>'
         stderr_node = nodes.raw(stderr, stderr_html, format='html')
 
         rendered_nodes = [doctree_node, stdout_node, stderr_node]
         if output is None:
             return rendered_nodes
 
+        # Ensure we wait for all JS module exports to be initialized
+        exports = ' && '.join(f'window.{export}' for export in global_exports)
+        if exports:
+            exports = f' && {exports}'
+
         script = ""
         if mime_type == 'text/plain':
             output = f'<pre>{output}</pre>'
         elif mime_type == 'application/bokeh':
             script = f"""
             <script>
               async function embed_bokeh_{self._current_count} () {{
-                if (window.Bokeh && window.Bokeh.Panel) {{
+                if (window.Bokeh && window.Bokeh.Panel{exports}) {{
                   await Bokeh.embed.embed_item({output})
                 }} else {{
                    setTimeout(embed_bokeh_{self._current_count}, 200)
                 }}
               }};
               embed_bokeh_{self._current_count}()
             </script>
@@ -286,15 +340,16 @@
     staticdir = builddir / '_static'
 
     # Render Web Worker
     web_worker = WEB_WORKER_TEMPLATE.render({
         'PYODIDE_URL': pyodide_conf['PYODIDE_URL'],
         'env_spec': ', '.join([repr(req) for req in pyodide_conf['requirements']]),
         'setup_code': pyodide_conf['setup_code'],
-        'autodetect_deps': pyodide_conf['autodetect_deps']
+        'autodetect_deps': pyodide_conf['autodetect_deps'],
+        'requires': json.dumps(pyodide_conf['requires'])
     })
     with open(staticdir/ 'PyodideWebWorker.js', 'w') as f:
         f.write(web_worker)
     worker_setup = WORKER_HANDLER_TEMPLATE.render(
         scripts=pyodide_conf['scripts']
     )
     with open(staticdir/ 'WorkerHandler.js', 'w') as f:
@@ -354,25 +409,33 @@
         ] += f"""
             <link rel="manifest" href="{relpath}site.webmanifest"/>
             """
 
     # Add additional resources extracted from pn.extension calls
     sourcename = context['sourcename'].replace('.txt', '')
     extra_resources = [
-        (r['js'], r['css']) for filename, r in EXTRA_RESOURCES.items()
+        (r['js'], r['js_exports'], r['js_modules'], r['css']) for filename, r in EXTRA_RESOURCES.items()
         if filename.endswith(sourcename)
     ]
     if extra_resources:
-        extra_js, extra_css = extra_resources[0]
+        extra_js, js_exports, js_modules, extra_css = extra_resources[0]
     else:
-        extra_js, extra_css = [], []
+        extra_js, js_exports, js_modules, extra_css = [], {}, {}, []
     extra_css += app.config.nbsite_pyodide_conf.get('extra_css', [])
     context["script_files"] += extra_js
     context["css_files"] += extra_css
 
+    module_tags = ""
+    for export, module in js_modules.items():
+        module_tags += JS_MODULE_TAG.format(file=module)
+    for export, module in js_exports.items():
+        module_tags += JS_MODULE_EXPORT.format(name=export, file=module)
+    if module_tags:
+        context["body"] = f'{module_tags}{context["body"]}'
+
     # Remove Scripts and CSS from page if no pyodide cells are found.
     if any(
         'pyodide' in cb.attributes.get('classes', [])
         for cb in doctree.traverse(nodes.literal_block)
     ):
         return
```

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.1a1/nbsite/pyodide/_static/run_cell.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,29 @@
 /**
  * SVG files for our copy buttons
  */
 let iconRun = `
-<svg class="pyodide-run-icon" style="width:24px;height:24px" viewBox="0 0 24 24">
+<svg class="pyodide-run-icon" style="width:32px;height:25px" viewBox="0 0 24 24">
     <path stroke="none" fill="#28a745" d="M8,5.14V19.14L19,12.14L8,5.14Z" />
 </svg>`
 
 let iconLoading = `
-<svg class="pyodide-loading-icon" style="width:24px;height:24px" viewBox="0 0 24 24">
+<svg class="pyodide-loading-icon" style="width:32px;height:25px" viewBox="0 0 24 24">
     <path fill="currentColor" d="M12,15.5A3.5,3.5 0 0,1 8.5,12A3.5,3.5 0 0,1 12,8.5A3.5,3.5 0 0,1 15.5,12A3.5,3.5 0 0,1 12,15.5M19.43,12.97C19.47,12.65 19.5,12.33 19.5,12C19.5,11.67 19.47,11.34 19.43,11L21.54,9.37C21.73,9.22 21.78,8.95 21.66,8.73L19.66,5.27C19.54,5.05 19.27,4.96 19.05,5.05L16.56,6.05C16.04,5.66 15.5,5.32 14.87,5.07L14.5,2.42C14.46,2.18 14.25,2 14,2H10C9.75,2 9.54,2.18 9.5,2.42L9.13,5.07C8.5,5.32 7.96,5.66 7.44,6.05L4.95,5.05C4.73,4.96 4.46,5.05 4.34,5.27L2.34,8.73C2.21,8.95 2.27,9.22 2.46,9.37L4.57,11C4.53,11.34 4.5,11.67 4.5,12C4.5,12.33 4.53,12.65 4.57,12.97L2.46,14.63C2.27,14.78 2.21,15.05 2.34,15.27L4.34,18.73C4.46,18.95 4.73,19.03 4.95,18.95L7.44,17.94C7.96,18.34 8.5,18.68 9.13,18.93L9.5,21.58C9.54,21.82 9.75,22 10,22H14C14.25,22 14.46,21.82 14.5,21.58L14.87,18.93C15.5,18.67 16.04,18.34 16.56,17.94L19.05,18.95C19.27,19.03 19.54,18.95 19.66,18.73L21.66,15.27C21.78,15.05 21.73,14.78 21.54,14.63L19.43,12.97Z" />
 </svg>`
 
-let iconLoaded = `<svg class="pyodide-loaded-icon" style="width:24px;height:24px" viewBox="0 0 24 24">
+let iconLoaded = `<svg class="pyodide-loaded-icon" style="width:32px;height:25px" viewBox="0 0 24 24">
     <path fill="#28a745" d="M9,20.42L2.79,14.21L5.62,11.38L9,14.77L18.88,4.88L21.71,7.71L9,20.42Z" />
 </svg>`
 
-let iconError = `<svg class="pyodide-error-icon" style="width:24px;height:24px" viewBox="0 0 24 24">
+let iconError = `<svg class="pyodide-error-icon" style="width:32px;height:25px" viewBox="0 0 24 24">
     <path fill="#ff0000" d="M12,2C17.53,2 22,6.47 22,12C22,17.53 17.53,22 12,22C6.47,22 2,17.53 2,12C2,6.47 6.47,2 12,2M15.59,7L12,10.59L8.41,7L7,8.41L10.59,12L7,15.59L8.41,17L12,13.41L15.59,17L17,15.59L13.41,12L17,8.41L15.59,7Z" />
 </svg>`
 
-let iconAlert = `<svg class="pyodide-alert-icon" style="width:24px;height:24px" viewBox="0 0 24 24">
+let iconAlert = `<svg class="pyodide-alert-icon" style="width:32px;height:25px" viewBox="0 0 24 24">
     <path fill="#f6be00" d="M13 13H11V7H13M11 15H13V17H11M15.73 3H8.27L3 8.27V15.73L8.27 21H15.73L21 15.73V8.27L15.73 3Z" />
 </svg>`
 
 /**
  * Set up run for code blocks
  */
 
@@ -74,14 +74,15 @@
         output.setAttribute('id', `output-${id}`)
         output.setAttribute('class', 'pyodide-output')
         cell.parentElement.parentElement.appendChild(output)
     }
     window.pyodideWorker.postMessage({
         type: 'execute',
         id: id,
+        path: document.location.pathname,
         code: cell.textContent
     })
     cell.setAttribute('executed', true)
 }
 
 const _query_params = new Proxy(new URLSearchParams(window.location.search), {
     get: (searchParams, prop) => searchParams.get(prop),
```

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.1a1/nbsite/pyodide/_static/runbutton.css`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 /* Copy buttons */
 button.runbtn {
-    position: absolute;
-    display: flex;
-    bottom: .3em;
-    right: .3em;
-    width: 1.7em;
-    height: 1.7em;
-    user-select: none;
-    padding: 0;
-    border: none;
-    outline: none;
-    border-radius: 0.4em;
-    /* The colors that GitHub uses */
-    border: #1b1f2426 1px solid;
-    background-color: #f6f8fa;
-    color: #57606a;
+  position: absolute;
+  display: flex;
+  bottom: 0.3em;
+  right: 0.3em;
+  width: 1.7em;
+  height: 1.7em;
+  user-select: none;
+  padding: 0;
+  border: none;
+  outline: none;
+  border-radius: 0.4em;
+  /* The colors that GitHub uses */
+  border: #1b1f2426 1px solid;
+  background-color: #f6f8fa;
+  color: #57606a;
 }
 
-div.highlight  {
-    position: relative;
+div.highlight {
+  position: relative;
 }
 
 .highlight button.runbtn:hover {
-    background-color: rgb(235, 235, 235);
+  background-color: rgb(235, 235, 235);
 }
 
 .highlight button.runbtn:active {
-    background-color: rgb(187, 187, 187);
+  background-color: rgb(187, 187, 187);
 }
 
 /**
  * A minimal CSS-only tooltip copied from:
  *   https://codepen.io/mildrenben/pen/rVBrpK
  *
  * To use, write HTML like the following:
  *
  * <p class="o-tooltip--left" data-tooltip="Hey">Short</p>
  */
- .o-tooltip--left {
+.o-tooltip--left {
   position: relative;
- }
+}
 
- .o-tooltip--left:after {
-    opacity: 0;
-    visibility: hidden;
-    position: absolute;
-    content: attr(data-tooltip);
-    padding: .2em;
-    font-size: .8em;
-    left: -.2em;
-    background: grey;
-    color: white;
-    white-space: nowrap;
-    z-index: 2;
-    border-radius: 2px;
-    transform: translateX(-102%) translateY(0);
-    transition: opacity 0.2s cubic-bezier(0.64, 0.09, 0.08, 1), transform 0.2s cubic-bezier(0.64, 0.09, 0.08, 1);
- }
-
- .o-tooltip--left:has(.pyodide-alert-icon):after {
-     opacity: 1;
-     visibility: visible;
- }
+.o-tooltip--left:after {
+  opacity: 0;
+  visibility: hidden;
+  position: absolute;
+  content: attr(data-tooltip);
+  padding: 0.2em;
+  font-size: 0.8em;
+  left: -0.2em;
+  background: grey;
+  color: white;
+  white-space: nowrap;
+  z-index: 2;
+  border-radius: 2px;
+  transform: translateX(-102%) translateY(0);
+  transition: opacity 0.2s cubic-bezier(0.64, 0.09, 0.08, 1),
+    transform 0.2s cubic-bezier(0.64, 0.09, 0.08, 1);
+}
+
+.o-tooltip--left:has(.pyodide-alert-icon):after {
+  opacity: 1;
+  visibility: visible;
+}
 
 .o-tooltip--left:hover:after {
-    display: block;
-    opacity: 1;
-    visibility: visible;
-    transform: translateX(-100%) translateY(0);
-    transition: opacity 0.2s cubic-bezier(0.64, 0.09, 0.08, 1), transform 0.2s cubic-bezier(0.64, 0.09, 0.08, 1);
-    transition-delay: .5s;
+  display: block;
+  opacity: 1;
+  visibility: visible;
+  transform: translateX(-100%) translateY(0);
+  transition: opacity 0.2s cubic-bezier(0.64, 0.09, 0.08, 1),
+    transform 0.2s cubic-bezier(0.64, 0.09, 0.08, 1);
+  transition-delay: 0.5s;
 }
 
 /* By default the copy button shouldn't show up when printing a page */
 @media print {
-    button.runbtn {
-        display: none;
-    }
+  button.runbtn {
+    display: none;
+  }
 }
 
 button.runbtn svg.pyodide-loading-icon {
   transform-box: fill-box;
   transform-origin: 50% 50%;
   animation-duration: 3s;
   animation-name: rotate;
@@ -93,34 +95,34 @@
   }
   to {
     transform: rotate(360deg);
   }
 }
 
 .pyodide-output {
-    margin: 1em 0;
-    overflow-x: auto;
+  margin: 1em 0;
+  overflow-x: auto;
 }
 
 .pyodide-output-wrapper {
-    margin-left: 0.5em;
+  margin-left: 0.5em;
 }
 
 .pyodide-stderr {
-    background-color: rgba(194, 103, 103, 0.35);
-    border: indianred solid 1px;
-    display: none;
+  background-color: rgba(194, 103, 103, 0.35);
+  border: indianred solid 1px;
+  display: none;
 }
 
 .pyodide-stdout {
-    display: none
+  display: none;
 }
 
 .pyodide-output.embedded {
-    border-left: 0.5em solid darkgoldenrod;
-    border-radius: 0.4em;
+  border-left: 0.5em solid darkgoldenrod;
+  border-radius: 0.4em;
 }
 
 .pyodide-output.live {
-    border-left: 0.5em solid green;
-    border-radius: 0.5em;
+  border-left: 0.5em solid green;
+  border-radius: 0.5em;
 }
```

### Comparing `nbsite-0.8.0rc9/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.1a1/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/nbsite/shared_conf.py` & `nbsite-0.8.1a1/nbsite/shared_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import datetime
 import os
+import pathlib as _pathlib
 
 import nbsite as _nbsite
-import pathlib as _pathlib
 
 from nbsite import nbbuild
 from nbsite.util import base_version  # noqa
 
 NBSITE_DIR = _pathlib.Path(_nbsite.__file__).parent
 
 
@@ -45,14 +45,15 @@
     'sphinx.ext.doctest',
     'sphinx.ext.intersphinx',
     'sphinx.ext.coverage',
     'sphinx.ext.mathjax',
     'sphinx.ext.ifconfig',
     'sphinx.ext.viewcode',
     'sphinx.ext.inheritance_diagram',
+    'sphinx_copybutton',
 ]
 
 # Default theme is the PyData Sphinx Theme
 html_theme = "pydata_sphinx_theme"
 
 inheritance_graph_attrs = dict(
     rankdir="LR",
@@ -87,18 +88,24 @@
         os.path.join(
             os.path.dirname(__file__),
             '_shared_templates'
         )
     )
 ]
 
-html_context = {
-    'js_includes': ['nbsite.js', 'require.js'],
-    'css_includes': ['nbsite.css'] 
-}
+html_context = {}
+
+html_css_files = [
+    'nbsite.css',
+    'notebook.css',
+    'gallery.css',
+    'alert.css',
+    'dataframe.css',
+    'scroller.css'
+]
 
 # A single line footer that includes the copyright and the last updated date.
 html_theme_options = {
     "footer_items": [
         "copyright-last-updated",
     ],
 }
@@ -108,7 +115,15 @@
 # copyright_years['start_year'] = '2000'
 # copyright = copyright_fmt.format(**copyright_years)
 copyright_years = {'current_year': str(datetime.date.today().year)}
 copyright_fmt = "{start_year}-{current_year} Holoviz contributors"
 
 # Format of the last updated date in the footer.
 html_last_updated_fmt = '%Y-%m-%d'
+
+
+suppress_warnings = [
+    # Ignore: (WARNING/2) Document headings start at H2, not H1
+    "myst.header",
+    # Ignores: skipping unknown output mime type: application/vnd.holoviews_exec.v0+json
+    "mystnb.unknown_mime_type"
+]
```

### Comparing `nbsite-0.8.0rc9/nbsite/templates/basic/conf.py` & `nbsite-0.8.1a1/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.1a1/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/nbsite/tests/test_cmd.py` & `nbsite-0.8.1a1/nbsite/tests/test_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import shutil
 
 import pytest
 
-from nbsite.cmd import generate_rst, build
+from nbsite.cmd import build, generate_rst
 
 # Note: a lot of this setup is copied from the new (2018-11-01) test in
 # pyct. Potentially this could be consolidated at some point. The fixture
 # setup could also move to conftest.py
 
 # Use `pytest  --pdb -m "not slow"` to run just the faster rst generating tests
```

### Comparing `nbsite-0.8.0rc9/nbsite/tests/test_util.py` & `nbsite-0.8.1a1/nbsite/tests/test_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pytest
 
 from nbsite.util import base_version
 
+
 @pytest.mark.parametrize(
     "version,expected",
     [
         ("0.3.0", "0.3.0"),
         ("0.13.0a19", "0.13.0a19"),
         ("0.13.0rc1", "0.13.0rc1"),
         ("0.13.0b1", "0.13.0b1"),
         ("no.match", "no.match"),
         ("0.13.0a19.post4+g0695e214", "0.13.0a19"),
         ("1.14.4", "1.14.4"),
         ("1.14.4.post82+g46ba8bbf2", "1.14.4"),
-        # Only 3 compontents version are matched.
+        # Only 3 component versions are matched.
         ("0.13.post4+g0695e214", "0.13.post4+g0695e214"),
         ("v0.3.0", "v0.3.0"),
     ]
 )
 def test_base_version(version, expected):
     assert base_version(version) == expected
```

### Comparing `nbsite-0.8.0rc9/nbsite/util.py` & `nbsite-0.8.1a1/nbsite/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import os
 import glob
+import os
 import re
 import shutil
 
+
 def copy_files(src, dest, pattern='**'):
     """Copy every file matching pattern from src to dest
     """
     for path in glob.glob(os.path.join(src, pattern), recursive=True):
         if not os.path.isfile(path):
             continue
         d = os.path.join(dest, os.path.dirname(path.split(src)[1][1:]))
@@ -19,15 +20,15 @@
             shutil.copy(path, f)
 
 
 def base_version(version):
     """Extract the final release and if available pre-release (alpha, beta,
     release candidate) segments of a PEP440 version, defined with three
     components (major.minor.micro).
-    
+
     Useful to avoid nbsite/sphinx to display the documentation HTML title
     with a not so informative and rather ugly long version (e.g.
     ``0.13.0a19.post4+g0695e214``). Use it in ``conf.py``::
 
         version = release = base_version(package.__version__)
 
     Return the version passed as input if no match is found with the pattern.
```

### Comparing `nbsite-0.8.0rc9/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.1a1/nbsite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.0rc9
+Version: 0.8.1a1
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.pyviz.org/
 Author: PyViz developers
 Author-email: developers@pyviz.org
 Maintainer: PyViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD-3
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: refman
 Provides-Extra: gallery
 Provides-Extra: tests
 Provides-Extra: build
 License-File: LICENSE.txt
 
-<img src="doc/_static/nbsite-logo.png" height=150><br>
+<img src="https://github.com/pyviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
 
 # NBSite: Build a tested, sphinx-based website from notebooks
 
 |    |    |
 | --- | --- |
```

### Comparing `nbsite-0.8.0rc9/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.1a1/nbsite.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,25 @@
 nbsite/util.py
 nbsite.egg-info/PKG-INFO
 nbsite.egg-info/SOURCES.txt
 nbsite.egg-info/dependency_links.txt
 nbsite.egg-info/entry_points.txt
 nbsite.egg-info/requires.txt
 nbsite.egg-info/top_level.txt
+nbsite/_shared_static/alert.css
+nbsite/_shared_static/dataframe.css
+nbsite/_shared_static/gallery.css
 nbsite/_shared_static/holoviz-icon-white.svg
 nbsite/_shared_static/mystnb.css
 nbsite/_shared_static/nbsite.css
-nbsite/_shared_static/nbsite.js
-nbsite/_shared_static/require.js
+nbsite/_shared_static/notebook.css
+nbsite/_shared_static/scroller.css
 nbsite/_shared_templates/copyright-last-updated.html
+nbsite/_shared_templates/layout.html
+nbsite/_shared_templates/sidebar-nav-bs.html
 nbsite/gallery/__init__.py
 nbsite/gallery/gen.py
 nbsite/gallery/thumbnailer.py
 nbsite/pyodide/ServiceHandler.js
 nbsite/pyodide/ServiceWorker.js
 nbsite/pyodide/WebWorker.js
 nbsite/pyodide/WorkerHandler.js
```

### Comparing `nbsite-0.8.0rc9/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.1a1/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc9/scripts/nbsite_fix_links.py` & `nbsite-0.8.1a1/scripts/nbsite_fix_links.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 """
 Cleans up relative cross-notebook links by replacing them with .html
 extension.
 """
 import os
 import re
-from bs4 import BeautifulSoup
 import warnings
 
+from bs4 import BeautifulSoup
 
 # TODO: holoviews specific links e.g. to reference manual...doc & generalize
 
 #BOKEH_REPLACEMENTS = {'cell.output_area.append_execute_result': '//cell.output_area.append_execute_result',
 #                      '}(window));\n</div>': '}(window));\n</script></div>',
 #                      '\n(function(root) {': '<script>\n(function(root) {'}
```

### Comparing `nbsite-0.8.0rc9/scripts/nbsite_generate_modules.py` & `nbsite-0.8.1a1/scripts/nbsite_generate_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
-import os
 import optparse
-
+import os
 
 # automodule options
 OPTIONS = ['members',
            #'undoc-members',
            'inherited-members', # disabled because there's a bug in sphinx
            'show-inheritance',
           ]
@@ -115,15 +114,15 @@
         text += format_inheritance_diagram(is_package and subroot or py_path, master_package)
         text += '\n\n'
         text += format_directive(is_package and subroot or py_path, master_package)
         text += '\n-------\n\n'
 
     # build a list of directories that are packages (they contain an INIT file)
     subs = [sub for sub in subs if os.path.isfile(os.path.join(root, sub, INIT))]
-    # if there are some package directories, add a TOC for theses subpackages
+    # if there are some package directories, add a TOC for these subpackages
     if subs:
         text += format_heading(2, 'Subpackages')
         text += '.. toctree::\n\n'
         for sub in subs:
             text += '    %s.%s\n' % (makename(master_package, subroot), sub)
         text += '\n'
 
@@ -232,15 +231,15 @@
     return f_excludes
 
 def is_excluded(root, excludes):
     """
     Check if the directory is in the exclude list.
 
     Note: by having trailing slashes, we avoid common prefix issues, like
-          e.g. an exlude "foo" also accidentally excluding "foobar".
+          e.g. an exclude "foo" also accidentally excluding "foobar".
     """
     sep = os.path.sep
     if not root.endswith(sep):
         root += sep
     for exclude in excludes:
         if root.startswith(exclude):
             return True
```

### Comparing `nbsite-0.8.0rc9/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.1a1/scripts/nbsite_nbpagebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 
-import sys
 import os
+import sys
 
 from nbsite.cmd import generate_rst
 
 # if only someone had made a way to handle parameters
 org = sys.argv[1]
 project = sys.argv[2]
 examples_path = os.path.abspath(sys.argv[3])
 doc_path = os.path.abspath(sys.argv[4])
 offset = 0
 overwrite = bool(1)
 if len(sys.argv) > 5:
     offset = int(sys.argv[5])
 if len(sys.argv) > 6:
     overwrite = int(sys.argv[6])
-    
+
 generate_rst(
     project,
     examples=examples_path,
     doc=doc_path,
     org = org,
     repo=project,
     offset=offset,
```

### Comparing `nbsite-0.8.0rc9/setup.py` & `nbsite-0.8.1a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import glob
-from setuptools import setup, find_packages
 
+from setuptools import find_packages, setup
 
 NAME = 'nbsite'
 DESCRIPTION = 'Build a tested, sphinx-based website from notebooks.'
 
 # duplicated from pyct.build.get_setup_version until pyct[build] >0.4.6 lands
 def get_setup_version(root, reponame):
     """
     Helper to get the current version from either git describe or the
     .version file (if available) - allows for param to not be available.
     Normally used in setup.py as follows:
     >>> from pyct.build import get_setup_version
     >>> version = get_setup_version(__file__, reponame)  # noqa
     """
-    import os
     import json
+    import os
 
     filepath = os.path.abspath(os.path.dirname(root))
     version_file_path = os.path.join(filepath, reponame, '.version')
     try:
         from param import version
-    except:
+    except Exception:
         version = None
     if version is not None:
         return version.Version.setup_version(filepath, reponame, archive_commit="$Format:%h$")
-    else:
-        print("WARNING: param>=1.6.0 unavailable. If you are installing a package, this warning can safely be ignored. If you are creating a package or otherwise operating in a git repository, you should install param>=1.6.0.")
-        return json.load(open(version_file_path, 'r'))['version_string']
+    print(
+        "WARNING: param>=1.6.0 unavailable. If you are installing a package, "
+        "this warning can safely be ignored. If you are creating a package or "
+        "otherwise operating in a git repository, you should install param>=1.6.0."
+    )
+    return json.load(open(version_file_path, 'r'))['version_string']
 
 setup_args = dict(
     name=NAME,
     version=get_setup_version(__file__, NAME),
     description=DESCRIPTION,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
@@ -60,16 +63,18 @@
         'myst-nb >=0.17',
         'sphinx-design',
         'notebook',
         'sphinx',
         'beautifulsoup4',
         'jinja2',
         'pillow',
-        'pydata-sphinx-theme',
+        'pydata-sphinx-theme >=0.13.3,<0.14',
         'myst-parser',
+        'sphinx-copybutton',
+        'sphinx-design',
     ],
     extras_require= {
         'refman':[
             'graphviz',
         ],
         'gallery':[
             'selenium',
```

