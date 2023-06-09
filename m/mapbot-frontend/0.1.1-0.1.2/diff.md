# Comparing `tmp/mapbot_frontend-0.1.1.tar.gz` & `tmp/mapbot_frontend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapbot_frontend-0.1.1.tar", last modified: Fri Jun  9 14:43:02 2023, max compression
+gzip compressed data, was "mapbot_frontend-0.1.2.tar", last modified: Fri Jun  9 14:53:23 2023, max compression
```

## Comparing `mapbot_frontend-0.1.1.tar` & `mapbot_frontend-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:43:02.216563 mapbot_frontend-0.1.1/
--rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 14:43:02.216296 mapbot_frontend-0.1.1/PKG-INFO
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:43:02.215265 mapbot_frontend-0.1.1/mapbot_frontend/
--rw-r--r--   0 martinweiss   (501) staff       (20)      637 2023-06-09 14:39:09.000000 mapbot_frontend-0.1.1/mapbot_frontend/__init__.py
-drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:43:02.216079 mapbot_frontend-0.1.1/mapbot_frontend.egg-info/
--rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 14:43:02.000000 mapbot_frontend-0.1.1/mapbot_frontend.egg-info/PKG-INFO
--rw-r--r--   0 martinweiss   (501) staff       (20)      192 2023-06-09 14:43:02.000000 mapbot_frontend-0.1.1/mapbot_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 14:43:02.000000 mapbot_frontend-0.1.1/mapbot_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 14:43:02.000000 mapbot_frontend-0.1.1/mapbot_frontend.egg-info/top_level.txt
--rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 14:43:02.216630 mapbot_frontend-0.1.1/setup.cfg
--rw-r--r--   0 martinweiss   (501) staff       (20)      133 2023-06-09 14:42:03.000000 mapbot_frontend-0.1.1/setup.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:53:23.286929 mapbot_frontend-0.1.2/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 14:53:23.286664 mapbot_frontend-0.1.2/PKG-INFO
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:53:23.285579 mapbot_frontend-0.1.2/mapbot_frontend/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      621 2023-06-09 14:52:15.000000 mapbot_frontend-0.1.2/mapbot_frontend/__init__.py
+drwxr-xr-x   0 martinweiss   (501) staff       (20)        0 2023-06-09 14:53:23.286450 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/
+-rw-r--r--   0 martinweiss   (501) staff       (20)      140 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 martinweiss   (501) staff       (20)      192 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)        1 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       16 2023-06-09 14:53:23.000000 mapbot_frontend-0.1.2/mapbot_frontend.egg-info/top_level.txt
+-rw-r--r--   0 martinweiss   (501) staff       (20)       38 2023-06-09 14:53:23.286991 mapbot_frontend-0.1.2/setup.cfg
+-rw-r--r--   0 martinweiss   (501) staff       (20)      133 2023-06-09 14:53:06.000000 mapbot_frontend-0.1.2/setup.py
```

### Comparing `mapbot_frontend-0.1.1/mapbot_frontend/__init__.py` & `mapbot_frontend-0.1.2/mapbot_frontend/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if not _RELEASE:
     _cartographer = components.declare_component(
         "mapbot_frontend", url=os.environ["FRONTEND_URL"]
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "mapbot_frontend/frontend/build")
+    build_dir = os.path.join(parent_dir, "frontend/build")
     _cartographer = components.declare_component("mapbot_frontend", path=build_dir)
 
 
 def cartographer(cartographer_state, key: Optional[str] = None):
     component_value = _cartographer(cartographer_state=cartographer_state, key=key)
     return component_value
```

