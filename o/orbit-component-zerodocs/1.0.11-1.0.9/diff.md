# Comparing `tmp/orbit_component_zerodocs-1.0.11.tar.gz` & `tmp/orbit_component_zerodocs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_zerodocs-1.0.11.tar", max compression
+gzip compressed data, was "orbit_component_zerodocs-1.0.9.tar", max compression
```

## Comparing `orbit_component_zerodocs-1.0.11.tar` & `orbit_component_zerodocs-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.11/LICENSE.md
--rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-1.0.11/README.md
--rw-r--r--   0        0        0       71 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/__init__.py
--rwxr-xr-x   0        0        0    19748 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/doc_python.py
--rw-r--r--   0        0        0     1599 2023-06-08 11:28:29.403019 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/plugin.py
--rw-r--r--   0        0        0     2934 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/APIs.py
--rw-r--r--   0        0        0    11017 2023-06-02 18:29:55.867494 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/Cache.py
--rw-r--r--   0        0        0     1814 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/Project.py
--rw-r--r--   0        0        0      270 2023-06-08 11:36:09.568981 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/Versions.py
--rw-r--r--   0        0        0        0 2023-06-09 10:45:12.264104 orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/version.py
--rw-r--r--   0        0        0     1398 2023-06-09 10:45:12.264104 orbit_component_zerodocs-1.0.11/pyproject.toml
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 orbit_component_zerodocs-1.0.11/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-1.0.9/README.md
+-rw-r--r--   0        0        0       71 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/__init__.py
+-rwxr-xr-x   0        0        0    19748 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/doc_python.py
+-rw-r--r--   0        0        0     1599 2023-06-08 11:28:29.403019 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/plugin.py
+-rw-r--r--   0        0        0     2934 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/APIs.py
+-rw-r--r--   0        0        0    11017 2023-06-02 18:29:55.867494 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Cache.py
+-rw-r--r--   0        0        0     1814 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Project.py
+-rw-r--r--   0        0        0      270 2023-06-08 11:36:09.568981 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Versions.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:29:59.004776 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/version.py
+-rw-r--r--   0        0        0     1404 2023-06-08 17:29:59.004776 orbit_component_zerodocs-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 orbit_component_zerodocs-1.0.9/PKG-INFO
```

### Comparing `orbit_component_zerodocs-1.0.11/LICENSE.md` & `orbit_component_zerodocs-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/doc_python.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/doc_python.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/plugin.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/APIs.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/APIs.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/Cache.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Cache.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.11/orbit_component_zerodocs/schema/Project.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Project.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.11/pyproject.toml` & `orbit_component_zerodocs-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-zerodocs"
-version = "1.0.11"
+version = "1.0.9"
 description = "Orbit Component for inline documentation"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_zerodocs"}]
 classifiers = [
@@ -22,21 +22,21 @@
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-zerodocs"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-zerodocs/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-orbit-database = "^1.0"
-orbit-component-base = "^1.0"
+orbit-database = "^0.99.91"
 loguru = "^0.7.0"
 pygments = "^2.15.1"
 bs4 = "^0.0.1"
 cmarkgfm = "^2022.10.27"
 python-gitlab = "^3.14.0"
+orbit-component-base = "^0.99.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `orbit_component_zerodocs-1.0.11/PKG-INFO` & `orbit_component_zerodocs-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-zerodocs
-Version: 1.0.11
+Version: 1.0.9
 Summary: Orbit Component for inline documentation
 Home-page: https://gitlab.com/madpenguin/orbit-component-zerodocs
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: cmarkgfm (>=2022.10.27,<2023.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: orbit-component-base (>=1.0,<2.0)
-Requires-Dist: orbit-database (>=1.0,<2.0)
+Requires-Dist: orbit-component-base (>=0.99.9,<0.100.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-zerodocs
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-zerodocs
 Description-Content-Type: text/markdown
 
 # Orbit Component :: ZeroDocs
```

