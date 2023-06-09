# Comparing `tmp/here-search-demo-0.8.5.tar.gz` & `tmp/here-search-demo-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "here-search-demo-0.8.5.tar", last modified: Thu Apr 27 15:17:25 2023, max compression
+gzip compressed data, was "here-search-demo-0.8.6.tar", last modified: Fri Jun  9 05:29:26 2023, max compression
```

## Comparing `here-search-demo-0.8.5.tar` & `here-search-demo-0.8.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/docs/developers.md
--rw-r--r--   0 runner    (1001) docker     (123)   678996 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/docs/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/lite_run.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/util.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:24.997240 here-search-demo-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:24.997240 here-search-demo-0.8.5/src/here_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/src/here_search/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/api_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/src/here_search/demo/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/lite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search/demo/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_1_api.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_2_api.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_3_widget.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search/demo/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/scripts/here-search-notebooks
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/scripts/lite-run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search/demo/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.529662 here-search-demo-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-09 05:29:26.529662 here-search-demo-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.521662 here-search-demo-0.8.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/docs/developers.md
+-rw-r--r--   0 runner    (1001) docker     (123)   678996 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/docs/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.525662 here-search-demo-0.8.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/requirements/lite_run.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/requirements/util.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-09 05:29:26.529662 here-search-demo-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.521662 here-search-demo-0.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.521662 here-search-demo-0.8.6/src/here_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.525662 here-search-demo-0.8.6/src/here_search/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/api_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.525662 here-search-demo-0.8.6/src/here_search/demo/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/entity/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/entity/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/entity/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/entity/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/entity/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/lite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.525662 here-search-demo-0.8.6/src/here_search/demo/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/notebooks/obm_1_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/notebooks/obm_2_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/notebooks/obm_3_widget.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.525662 here-search-demo-0.8.6/src/here_search/demo/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/scripts/here-search-notebooks
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/scripts/lite-run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.525662 here-search-demo-0.8.6/src/here_search/demo/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/widgets/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/widgets/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/widgets/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/src/here_search/demo/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.529662 here-search-demo-0.8.6/src/here_search_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-09 05:29:26.000000 here-search-demo-0.8.6/src/here_search_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-09 05:29:26.000000 here-search-demo-0.8.6/src/here_search_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:29:26.000000 here-search-demo-0.8.6/src/here_search_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:29:26.000000 here-search-demo-0.8.6/src/here_search_demo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-09 05:29:26.000000 here-search-demo-0.8.6/src/here_search_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 05:29:26.000000 here-search-demo-0.8.6/src/here_search_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:29:26.529662 here-search-demo-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 05:29:09.000000 here-search-demo-0.8.6/tests/test_util.py
```

### Comparing `here-search-demo-0.8.5/LICENSE` & `here-search-demo-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/PKG-INFO` & `here-search-demo-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here-search-demo
-Version: 0.8.5
+Version: 0.8.6
 Summary: HERE Geocoding and Search demo and widgets
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
 Project-URL: Bug Tracker, https://github.com/heremaps/here-search-demo/issues
 Project-URL: Source, https://github.com/heremaps/here-search-demo
@@ -26,15 +26,15 @@
 
 # HERE Search notebooks
 
 A set of jupyter notebooks demonstrating the use of [HERE Geocoding & Search][4] endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
 
 ![searching for restaurants](https://github.com/heremaps/here-search-demo/raw/main/docs/screenshot.png)
 
-Requirements: a [HERE API key][1] and a Python environment.
+Requirements: a [HERE API key][1] and a Python environment. Note that HERE Base Plan [Pricing][5] allows you to get started for free.
 
 The notebooks can be [used in your browser][3] without further installation.
 
 ## Installation
 
 If you need to install the notebooks or the underlying library on your workstation, run preferably in a virtual environment:
 
@@ -65,7 +65,8 @@
 
 This project is licensed under the MIT license - see the [LICENSE](./LICENSE) file in the root of this project for license details.
 
 [1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start.html#get-an-api-key
 [2]: https://github.com/heremaps/here-search-demo/blob/main/docs/developers.md
 [3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
 [4]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
+[5]: https://www.here.com/get-started/pricing
```

### Comparing `here-search-demo-0.8.5/README.md` & `here-search-demo-0.8.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # HERE Search notebooks
 
 A set of jupyter notebooks demonstrating the use of [HERE Geocoding & Search][4] endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
 
 ![searching for restaurants](https://github.com/heremaps/here-search-demo/raw/main/docs/screenshot.png)
 
-Requirements: a [HERE API key][1] and a Python environment.
+Requirements: a [HERE API key][1] and a Python environment. Note that HERE Base Plan [Pricing][5] allows you to get started for free.
 
 The notebooks can be [used in your browser][3] without further installation.
 
 ## Installation
 
 If you need to install the notebooks or the underlying library on your workstation, run preferably in a virtual environment:
 
@@ -42,7 +42,8 @@
 
 This project is licensed under the MIT license - see the [LICENSE](./LICENSE) file in the root of this project for license details.
 
 [1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start.html#get-an-api-key
 [2]: https://github.com/heremaps/here-search-demo/blob/main/docs/developers.md
 [3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
 [4]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
+[5]: https://www.here.com/get-started/pricing
```

### Comparing `here-search-demo-0.8.5/docs/developers.md` & `here-search-demo-0.8.6/docs/developers.md`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/docs/screenshot.png` & `here-search-demo-0.8.6/docs/screenshot.png`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/setup.cfg` & `here-search-demo-0.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/api.py` & `here-search-demo-0.8.6/src/here_search/demo/api.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/api_options.py` & `here-search-demo-0.8.6/src/here_search/demo/api_options.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/base.py` & `here-search-demo-0.8.6/src/here_search/demo/base.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/entity/endpoint.py` & `here-search-demo-0.8.6/src/here_search/demo/entity/endpoint.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/entity/intent.py` & `here-search-demo-0.8.6/src/here_search/demo/entity/intent.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/entity/place.py` & `here-search-demo-0.8.6/src/here_search/demo/entity/place.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/entity/request.py` & `here-search-demo-0.8.6/src/here_search/demo/entity/request.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/event.py` & `here-search-demo-0.8.6/src/here_search/demo/event.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/lite.py` & `here-search-demo-0.8.6/src/here_search/demo/lite.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/notebooks/demo.ipynb` & `here-search-demo-0.8.6/src/here_search/demo/notebooks/demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333334%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.6-py3-none-any.whl"], '*

 * *            'keep_going=True)\\n\'), (3, \'    api_key = "<YOUR HERE API KEY>"\\n\')], delete: [3, '*

 * *            '2]}}}'}*

```diff
@@ -5,16 +5,16 @@
             "execution_count": null,
             "id": "717d9c13-684f-4ef9-8045-09624217caeb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
-                "    api_key = \"<YOUR API KEY>\"\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.6-py3-none-any.whl\"], keep_going=True)\n",
+                "    api_key = \"<YOUR HERE API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "712c9ba7-62a7-4795-9a5e-7cdfb320bb1c",
```

### Comparing `here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_1_api.ipynb` & `here-search-demo-0.8.6/src/here_search/demo/notebooks/obm_1_api.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996936274509804%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.6-py3-none-any.whl"], '*

 * *            'keep_going=True)\\n\'), (3, \'    api_key = "<YOUR HERE API KEY>"\\n\')], delete: [3, '*

 * *            '2]}}}'}*

```diff
@@ -5,16 +5,16 @@
             "execution_count": 1,
             "id": "e5c95683-6b47-40aa-8dba-1c815e1549c3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
-                "    api_key = \"<YOUR API KEY>\"\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.6-py3-none-any.whl\"], keep_going=True)\n",
+                "    api_key = \"<YOUR HERE API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a312886c-007e-40e8-90a7-a215e1708ff5",
```

### Comparing `here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_2_api.ipynb` & `here-search-demo-0.8.6/src/here_search/demo/notebooks/obm_2_api.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.6-py3-none-any.whl"], '*

 * *            'keep_going=True)\\n\'), (3, \'    api_key = "<YOUR HERE API KEY>"\\n\')], delete: [3, '*

 * *            '2]}}}'}*

```diff
@@ -5,16 +5,16 @@
             "execution_count": 1,
             "id": "77ac7de0-8ebc-4686-87bf-a9e720cc79e4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
-                "    api_key = \"<YOUR API KEY>\"\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.6-py3-none-any.whl\"], keep_going=True)\n",
+                "    api_key = \"<YOUR HERE API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a312886c-007e-40e8-90a7-a215e1708ff5",
```

### Comparing `here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_3_widget.ipynb` & `here-search-demo-0.8.6/src/here_search/demo/notebooks/obm_3_widget.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222222%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.6-py3-none-any.whl"], '*

 * *            'keep_going=True)\\n\'), (3, \'    api_key = "<YOUR HERE API KEY>"\\n\')], delete: [3, '*

 * *            '2]}}}'}*

```diff
@@ -5,16 +5,16 @@
             "execution_count": null,
             "id": "f4878c23-f9ec-4756-b085-bdccf7d726d8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
-                "    api_key = \"<YOUR API KEY>\"\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.6-py3-none-any.whl\"], keep_going=True)\n",
+                "    api_key = \"<YOUR HERE API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6a2488bf-1023-4b46-aed6-64abae28fd8b",
```

### Comparing `here-search-demo-0.8.5/src/here_search/demo/scripts/lite-run.sh` & `here-search-demo-0.8.6/src/here_search/demo/scripts/lite-run.sh`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/user.py` & `here-search-demo-0.8.6/src/here_search/demo/user.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/util.py` & `here-search-demo-0.8.6/src/here_search/demo/util.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/widgets/app.py` & `here-search-demo-0.8.6/src/here_search/demo/widgets/app.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/widgets/input.py` & `here-search-demo-0.8.6/src/here_search/demo/widgets/input.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/widgets/output.py` & `here-search-demo-0.8.6/src/here_search/demo/widgets/output.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search/demo/widgets/util.py` & `here-search-demo-0.8.6/src/here_search/demo/widgets/util.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/src/here_search_demo.egg-info/PKG-INFO` & `here-search-demo-0.8.6/src/here_search_demo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here-search-demo
-Version: 0.8.5
+Version: 0.8.6
 Summary: HERE Geocoding and Search demo and widgets
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
 Project-URL: Bug Tracker, https://github.com/heremaps/here-search-demo/issues
 Project-URL: Source, https://github.com/heremaps/here-search-demo
@@ -26,15 +26,15 @@
 
 # HERE Search notebooks
 
 A set of jupyter notebooks demonstrating the use of [HERE Geocoding & Search][4] endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
 
 ![searching for restaurants](https://github.com/heremaps/here-search-demo/raw/main/docs/screenshot.png)
 
-Requirements: a [HERE API key][1] and a Python environment.
+Requirements: a [HERE API key][1] and a Python environment. Note that HERE Base Plan [Pricing][5] allows you to get started for free.
 
 The notebooks can be [used in your browser][3] without further installation.
 
 ## Installation
 
 If you need to install the notebooks or the underlying library on your workstation, run preferably in a virtual environment:
 
@@ -65,7 +65,8 @@
 
 This project is licensed under the MIT license - see the [LICENSE](./LICENSE) file in the root of this project for license details.
 
 [1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start.html#get-an-api-key
 [2]: https://github.com/heremaps/here-search-demo/blob/main/docs/developers.md
 [3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
 [4]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
+[5]: https://www.here.com/get-started/pricing
```

### Comparing `here-search-demo-0.8.5/src/here_search_demo.egg-info/SOURCES.txt` & `here-search-demo-0.8.6/src/here_search_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/tests/test_api.py` & `here-search-demo-0.8.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/tests/test_base.py` & `here-search-demo-0.8.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/tests/test_entities.py` & `here-search-demo-0.8.6/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.5/tests/test_util.py` & `here-search-demo-0.8.6/tests/test_util.py`

 * *Files identical despite different names*

