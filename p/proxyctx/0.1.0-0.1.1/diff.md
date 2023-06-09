# Comparing `tmp/proxyctx-0.1.0.tar.gz` & `tmp/proxyctx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyctx-0.1.0.tar", last modified: Fri Jun  9 10:01:05 2023, max compression
+gzip compressed data, was "proxyctx-0.1.1.tar", last modified: Fri Jun  9 14:00:26 2023, max compression
```

## Comparing `proxyctx-0.1.0.tar` & `proxyctx-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.225626 proxyctx-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 10:00:49.000000 proxyctx-0.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 10:00:49.000000 proxyctx-0.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 10:00:49.000000 proxyctx-0.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.221626 proxyctx-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.221626 proxyctx-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 10:00:49.000000 proxyctx-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 10:00:49.000000 proxyctx-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-09 10:00:49.000000 proxyctx-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 10:00:49.000000 proxyctx-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 10:01:05.225626 proxyctx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-09 10:00:49.000000 proxyctx-0.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-06-09 10:00:49.000000 proxyctx-0.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 10:00:49.000000 proxyctx-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-09 10:00:49.000000 proxyctx-0.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-09 10:00:49.000000 proxyctx-0.1.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.225626 proxyctx-0.1.0/proxyctx/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 10:00:49.000000 proxyctx-0.1.0/proxyctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 10:01:05.225626 proxyctx-0.1.0/proxyctx/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 10:00:49.000000 proxyctx-0.1.0/proxyctx/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-09 10:00:49.000000 proxyctx-0.1.0/proxyctx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.221626 proxyctx-0.1.0/proxyctx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 10:01:05.000000 proxyctx-0.1.0/proxyctx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-09 10:01:05.000000 proxyctx-0.1.0/proxyctx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:01:05.000000 proxyctx-0.1.0/proxyctx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 10:01:05.000000 proxyctx-0.1.0/proxyctx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-09 10:00:49.000000 proxyctx-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.225626 proxyctx-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 10:00:49.000000 proxyctx-0.1.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 10:00:49.000000 proxyctx-0.1.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 10:00:49.000000 proxyctx-0.1.0/requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:01:05.225626 proxyctx-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 10:00:49.000000 proxyctx-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:01:05.225626 proxyctx-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:00:49.000000 proxyctx-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 10:00:49.000000 proxyctx-0.1.0/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.402646 proxyctx-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.398645 proxyctx-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.398645 proxyctx-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-09 14:00:09.000000 proxyctx-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 14:00:09.000000 proxyctx-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-09 14:00:26.402646 proxyctx-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-09 14:00:09.000000 proxyctx-0.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-06-09 14:00:09.000000 proxyctx-0.1.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-09 14:00:09.000000 proxyctx-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.398645 proxyctx-0.1.1/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 14:00:09.000000 proxyctx-0.1.1/changes/1.misc
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-09 14:00:09.000000 proxyctx-0.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 14:00:09.000000 proxyctx-0.1.1/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.402646 proxyctx-0.1.1/proxyctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 14:00:09.000000 proxyctx-0.1.1/proxyctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 14:00:26.402646 proxyctx-0.1.1/proxyctx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 14:00:09.000000 proxyctx-0.1.1/proxyctx/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-09 14:00:09.000000 proxyctx-0.1.1/proxyctx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.398645 proxyctx-0.1.1/proxyctx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-09 14:00:26.000000 proxyctx-0.1.1/proxyctx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-09 14:00:26.000000 proxyctx-0.1.1/proxyctx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:00:26.000000 proxyctx-0.1.1/proxyctx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 14:00:26.000000 proxyctx-0.1.1/proxyctx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-09 14:00:09.000000 proxyctx-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.398645 proxyctx-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 14:00:09.000000 proxyctx-0.1.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:00:09.000000 proxyctx-0.1.1/requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:00:26.402646 proxyctx-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 14:00:09.000000 proxyctx-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:26.402646 proxyctx-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:00:09.000000 proxyctx-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 14:00:09.000000 proxyctx-0.1.1/tests/test_context.py
```

### Comparing `proxyctx-0.1.0/.github/workflows/ci.yml` & `proxyctx-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/.gitignore` & `proxyctx-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/.pre-commit-config.yaml` & `proxyctx-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/LICENSE` & `proxyctx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/Pipfile.lock` & `proxyctx-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/proxyctx/context.py` & `proxyctx-0.1.1/proxyctx/context.py`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/proxyctx/proxy.py` & `proxyctx-0.1.1/proxyctx/proxy.py`

 * *Files identical despite different names*

### Comparing `proxyctx-0.1.0/proxyctx.egg-info/SOURCES.txt` & `proxyctx-0.1.1/proxyctx.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 Pipfile
 Pipfile.lock
 README.md
 mypy.ini
 noxfile.py
 pyproject.toml
 setup.py
+.github/pull_request_template.md
 .github/workflows/ci.yml
+changes/1.misc
 proxyctx/__init__.py
 proxyctx/_version.py
 proxyctx/context.py
 proxyctx/proxy.py
 proxyctx.egg-info/PKG-INFO
 proxyctx.egg-info/SOURCES.txt
 proxyctx.egg-info/dependency_links.txt
 proxyctx.egg-info/top_level.txt
 requirements/requirements-dev.txt
-requirements/requirements-docs.txt
 requirements/requirements-tests.txt
 tests/__init__.py
 tests/test_context.py
```

### Comparing `proxyctx-0.1.0/pyproject.toml` & `proxyctx-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -5,19 +5,30 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxyctx"
 authors = [
     {name = "Lucino772", email = "lucapalmi772@gmail.com"},
 ]
-description = "A Object proxy library inspired from Werkzeug's LocalProxy "
+description = "ProxyCTX is a utility library for global context inspired by Flask, leveraging contextvars"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 dynamic = ["version"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9"
+]
+
+[project.urls]
+Homepage = "https://github.com/Lucino772/proxyctx"
+Changelog = "https://github.com/Lucino772/proxyctx/blob/main/CHANGELOG.rst"
 
 [tool.setuptools]
 packages = ["proxyctx"]
 
 [tool.setuptools.dynamic]
 version = {attr = "proxyctx.__version__"}
 
@@ -41,11 +52,12 @@
 '''
 
 [tool.towncrier]
 name = "proxyctx"
 directory = "changes"
 package = "proxyctx"
 filename = "CHANGELOG.rst"
+title_format = "{name} v{version} ({project_date})"
 issue_format = "`#{issue} <https://github.com/Lucino772/proxyctx/issues/{issue}>`_"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --cov=./ --cov-report=xml ./tests"
```

### Comparing `proxyctx-0.1.0/tests/test_context.py` & `proxyctx-0.1.1/tests/test_context.py`

 * *Files identical despite different names*

