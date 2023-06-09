# Comparing `tmp/stac-fastapi.pgstac-2.4.7.tar.gz` & `tmp/stac-fastapi.pgstac-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.pgstac-2.4.7.tar", last modified: Thu May 18 12:48:46 2023, max compression
+gzip compressed data, was "stac-fastapi.pgstac-2.4.8.tar", last modified: Fri Jun  9 18:28:38 2023, max compression
```

## Comparing `stac-fastapi.pgstac-2.4.7.tar` & `stac-fastapi.pgstac-2.4.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.773734 stac-fastapi.pgstac-2.4.8/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.777734 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 18:28:38.000000 stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.773734 stac-fastapi.pgstac-2.4.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:38.781734 stac-fastapi.pgstac-2.4.8/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 18:28:28.000000 stac-fastapi.pgstac-2.4.8/tests/resources/test_mgmt.py
```

### Comparing `stac-fastapi.pgstac-2.4.7/LICENSE` & `stac-fastapi.pgstac-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/PKG-INFO` & `stac-fastapi.pgstac-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.7
+Version: 2.4.8
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.pgstac-2.4.7/README.md` & `stac-fastapi.pgstac-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/setup.py` & `stac-fastapi.pgstac-2.4.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
     "attrs",
     "orjson",
-    "pydantic[dotenv]",
+    "pydantic[dotenv]>=1.10.8",  # https://github.com/pydantic/pydantic/issues/5821
     "stac_pydantic==2.0.*",
-    "stac-fastapi.types~=2.4.7",
-    "stac-fastapi.api~=2.4.7",
-    "stac-fastapi.extensions~=2.4.7",
+    "stac-fastapi.types~=2.4.8",
+    "stac-fastapi.api~=2.4.8",
+    "stac-fastapi.extensions~=2.4.8",
     "asyncpg",
     "buildpg",
     "brotli_asgi",
     "pygeofilter>=0.2",
     "pypgstac==0.7.*",
 ]
```

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/app.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/config.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/core.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/core.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/db.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/filter.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/query.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/links.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/models/links.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/transactions.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/transactions.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/base_item_cache.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/search.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/types/search.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/utils.py` & `stac-fastapi.pgstac-2.4.8/stac_fastapi/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.7
+Version: 2.4.8
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac-fastapi.pgstac-2.4.8/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/tests/api/test_api.py` & `stac-fastapi.pgstac-2.4.8/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/tests/clients/test_postgres.py` & `stac-fastapi.pgstac-2.4.8/tests/clients/test_postgres.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/tests/resources/test_collection.py` & `stac-fastapi.pgstac-2.4.8/tests/resources/test_collection.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/tests/resources/test_conformance.py` & `stac-fastapi.pgstac-2.4.8/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.7/tests/resources/test_item.py` & `stac-fastapi.pgstac-2.4.8/tests/resources/test_item.py`

 * *Files identical despite different names*

