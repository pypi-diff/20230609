# Comparing `tmp/python_opensky-0.0.8.tar.gz` & `tmp/python_opensky-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.0.8.tar", max compression
+gzip compressed data, was "python_opensky-0.0.9.tar", max compression
```

## Comparing `python_opensky-0.0.8.tar` & `python_opensky-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-06-01 11:43:00.841027 python_opensky-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     5328 2023-06-01 11:43:00.841027 python_opensky-0.0.8/README.md
--rw-r--r--   0        0        0     3659 2023-06-01 11:43:15.744941 python_opensky-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      444 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      849 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/const.py
--rw-r--r--   0        0        0      384 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     3573 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/models.py
--rw-r--r--   0        0        0     9203 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 python_opensky-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-08 08:13:32.549572 python_opensky-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     5328 2023-06-08 08:13:32.549572 python_opensky-0.0.9/README.md
+-rw-r--r--   0        0        0     3661 2023-06-08 08:13:50.987213 python_opensky-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      849 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/const.py
+-rw-r--r--   0        0        0      384 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     3573 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/models.py
+-rw-r--r--   0        0        0     9203 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 python_opensky-0.0.9/PKG-INFO
```

### Comparing `python_opensky-0.0.8/LICENSE.md` & `python_opensky-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.8/README.md` & `python_opensky-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.8/pyproject.toml` & `python_opensky-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.0.8"
+version = "0.0.9"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
@@ -24,15 +24,15 @@
     { include = "python_opensky", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.0.0"
 yarl = ">=1.6.0"
-pydantic = "1.10.8"
+pydantic = ">=1.10.8"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "2.1.6"
 black = "23.3.0"
 blacken-docs = "1.13.0"
 codespell = "2.2.4"
 covdefaults = "2.3.0"
@@ -40,15 +40,15 @@
 mypy = "1.3.0"
 pre-commit = "3.3.2"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.1.0"
-ruff = "0.0.270"
+ruff = "0.0.272"
 safety = "2.4.0b1"
 yamllint = "1.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-opensky/issues"
 Changelog = "https://github.com/joostlek/python-opensky/releases"
```

### Comparing `python_opensky-0.0.8/src/python_opensky/const.py` & `python_opensky-0.0.9/src/python_opensky/const.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.8/src/python_opensky/models.py` & `python_opensky-0.0.9/src/python_opensky/models.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.8/src/python_opensky/opensky.py` & `python_opensky-0.0.9/src/python_opensky/opensky.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.8/PKG-INFO` & `python_opensky-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: pydantic (==1.10.8)
+Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/joostlek/python-opensky/issues
 Project-URL: Changelog, https://github.com/joostlek/python-opensky/releases
 Project-URL: Documentation, https://github.com/joostlek/python-opensky
 Project-URL: Repository, https://github.com/joostlek/python-opensky
 Description-Content-Type: text/markdown
```

