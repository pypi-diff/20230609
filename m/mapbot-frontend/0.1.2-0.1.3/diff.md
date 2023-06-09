# Comparing `tmp/mapbot_frontend-0.1.2.tar.gz` & `tmp/mapbot_frontend-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapbot_frontend-0.1.2.tar", last modified: Fri Jun  9 14:53:23 2023, max compression
+gzip compressed data, was "mapbot_frontend-0.1.3.tar", last modified: Fri Jun  9 15:04:48 2023, max compression
```

## Comparing `mapbot_frontend-0.1.2.tar` & `mapbot_frontend-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:53:23.286929 mapbot_frontend-0.1.2/
--rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 14:53:23.286664 mapbot_frontend-0.1.2/PKG-INFO
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:53:23.285579 mapbot_frontend-0.1.2/mapbot_frontend/
--rw-r--r--   0 martinweiss   (501) staff       (20)      621 2023-06-09 14:52:15.000000 mapbot_frontend-0.1.2/mapbot_frontend/__init__.py
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:53:23.286450 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/
--rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/PKG-INFO
--rw-r--r--   0 martinweiss   (501) staff       (20)      192 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/top_level.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 14:53:23.286991 mapbot_frontend-0.1.2/setup.cfg
--rw-r--r--   0 martinweiss   (501) staff       (20)      133 2023-06-09 14:53:06.000000 mapbot_frontend-0.1.2/setup.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:04:48.097704 mapbot_frontend-0.1.3/
+-rw-r--r--   0 martinweiss   (501) staff       (20)       66 2023-06-09 15:02:04.000000 mapbot_frontend-0.1.3/MANIFEST.in
+-rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 15:04:48.097475 mapbot_frontend-0.1.3/PKG-INFO
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:04:48.096162 mapbot_frontend-0.1.3/mapbot_frontend/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      621 2023-06-09 14:52:15.000000 mapbot_frontend-0.1.3/mapbot_frontend/__init__.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 15:04:48.097091 mapbot_frontend-0.1.3/mapbot_frontend.egg-info/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 15:04:48.000000 mapbot_frontend-0.1.3/mapbot_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 martinweiss   (501) staff       (20)      204 2023-06-09 15:04:48.000000 mapbot_frontend-0.1.3/mapbot_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 15:04:48.000000 mapbot_frontend-0.1.3/mapbot_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 15:04:48.000000 mapbot_frontend-0.1.3/mapbot_frontend.egg-info/top_level.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 15:04:48.097766 mapbot_frontend-0.1.3/setup.cfg
+-rw-r--r--   0 martinweiss   (501) staff       (20)      133 2023-06-09 15:04:16.000000 mapbot_frontend-0.1.3/setup.py
```

### Comparing `mapbot_frontend-0.1.2/mapbot_frontend/__init__.py` & `mapbot_frontend-0.1.3/mapbot_frontend/__init__.py`

 * *Files identical despite different names*

