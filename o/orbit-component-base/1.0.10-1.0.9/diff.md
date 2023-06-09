# Comparing `tmp/orbit_component_base-1.0.10.tar.gz` & `tmp/orbit_component_base-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-1.0.10.tar", max compression
+gzip compressed data, was "orbit_component_base-1.0.9.tar", max compression
```

## Comparing `orbit_component_base-1.0.10.tar` & `orbit_component_base-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/README.md
--rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      832 2023-06-07 22:18:42.405891 orbit_component_base-1.0.10/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1290 2023-06-08 11:30:57.895776 orbit_component_base-1.0.10/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/schema/OrbitUsers.py
--rw-r--r--   0        0        0     1787 2023-06-08 11:31:11.007490 orbit_component_base-1.0.10/orbit_component_base/schema/OrbitVersions.py
--rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.10/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6551 2023-06-08 12:34:02.238300 orbit_component_base-1.0.10/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     6878 2023-06-05 13:02:31.115557 orbit_component_base-1.0.10/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.10/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.10/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2983 2023-06-08 12:54:23.664990 orbit_component_base-1.0.10/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.10/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.10/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.10/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.10/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0       23 2023-06-09 10:37:57.397617 orbit_component_base-1.0.10/orbit_component_base/version.py
--rw-r--r--   0        0        0     1393 2023-06-09 10:37:57.393617 orbit_component_base-1.0.10/pyproject.toml
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 orbit_component_base-1.0.10/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-07 22:18:42.405891 orbit_component_base-1.0.9/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1290 2023-06-08 11:30:57.895776 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitUsers.py
+-rw-r--r--   0        0        0     1787 2023-06-08 11:31:11.007490 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitVersions.py
+-rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6551 2023-06-08 12:34:02.238300 orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6878 2023-06-05 13:02:31.115557 orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2983 2023-06-08 12:54:23.664990 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0       22 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/orbit_component_base/version.py
+-rw-r--r--   0        0        0     1394 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 orbit_component_base-1.0.9/PKG-INFO
```

### Comparing `orbit_component_base-1.0.10/LICENSE.md` & `orbit_component_base-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/plugin.py` & `orbit_component_base-1.0.9/orbit_component_base/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/schema/OrbitVersions.py` & `orbit_component_base-1.0.9/orbit_component_base/schema/OrbitVersions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_app.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_config.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_database.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_router.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.10/pyproject.toml` & `orbit_component_base-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "1.0.10"
+version = "1.0.9"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
@@ -24,15 +24,15 @@
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-base"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-base/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-socketio = "^5.8.0"
-orbit-database = "^1.0.0"
+orbit-database = "^0.99.91"
 loguru = "^0.7.0"
 ujson = "^5.7.0"
 pycryptodome = "^3.18.0"
 tqdm = "^4.65.0"
 aiohttp = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `orbit_component_base-1.0.10/PKG-INFO` & `orbit_component_base-1.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 1.0.10
+Version: 1.0.9
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: orbit-database (>=1.0.0,<2.0.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: python-socketio (>=5.8.0,<6.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-base
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-base
 Description-Content-Type: text/markdown
```

