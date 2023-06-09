# Comparing `tmp/python_manifest-0.1.0.tar.gz` & `tmp/python_manifest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_manifest-0.1.0.tar", max compression
+gzip compressed data, was "python_manifest-1.0.1.tar", max compression
```

## Comparing `python_manifest-0.1.0.tar` & `python_manifest-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     4075 2023-06-08 22:59:50.019318 python_manifest-0.1.0/README.md
--rw-r--r--   0        0        0      221 2023-06-08 22:59:01.534215 python_manifest-0.1.0/manifest/__init__.py
--rw-r--r--   0        0        0     8972 2023-06-06 06:31:26.532393 python_manifest-0.1.0/manifest/base.py
--rw-r--r--   0        0        0      324 2023-06-02 01:52:23.259358 python_manifest-0.1.0/manifest/expressions/__init__.py
--rw-r--r--   0        0        0     3988 2023-06-06 20:22:18.129013 python_manifest-0.1.0/manifest/expressions/operations.py
--rw-r--r--   0        0        0     3232 2023-06-02 05:09:24.543175 python_manifest-0.1.0/manifest/expressions/resolve.py
--rw-r--r--   0        0        0     1169 2023-06-06 05:14:35.315237 python_manifest-0.1.0/manifest/hooks.py
--rw-r--r--   0        0        0     2085 2023-06-02 04:19:32.618288 python_manifest-0.1.0/manifest/instantiable.py
--rw-r--r--   0        0        0     9658 2023-06-06 06:48:03.068229 python_manifest-0.1.0/manifest/parse.py
--rw-r--r--   0        0        0        0 2023-06-08 22:59:10.862430 python_manifest-0.1.0/manifest/py.typed
--rw-r--r--   0        0        0      386 2023-06-06 06:37:53.161724 python_manifest-0.1.0/manifest/serializers/__init__.py
--rw-r--r--   0        0        0      272 2023-06-06 06:46:00.564385 python_manifest-0.1.0/manifest/serializers/base.py
--rw-r--r--   0        0        0      503 2023-06-02 02:57:07.495149 python_manifest-0.1.0/manifest/serializers/jsons.py
--rw-r--r--   0        0        0      353 2023-06-02 05:04:07.052998 python_manifest-0.1.0/manifest/serializers/noop.py
--rw-r--r--   0        0        0      356 2023-06-06 06:37:21.601870 python_manifest-0.1.0/manifest/serializers/tomls.py
--rw-r--r--   0        0        0      350 2023-06-02 05:04:27.465791 python_manifest-0.1.0/manifest/serializers/yamls.py
--rw-r--r--   0        0        0     9635 2023-06-02 05:56:38.075877 python_manifest-0.1.0/manifest/utils.py
--rw-r--r--   0        0        0     1516 2023-06-08 22:54:40.459529 python_manifest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 python_manifest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-08 23:41:21.591796 python_manifest-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4702 2023-06-08 23:30:24.948770 python_manifest-1.0.1/README.md
+-rw-r--r--   0        0        0      221 2023-06-08 22:59:01.534215 python_manifest-1.0.1/manifest/__init__.py
+-rw-r--r--   0        0        0     8972 2023-06-06 06:31:26.532393 python_manifest-1.0.1/manifest/base.py
+-rw-r--r--   0        0        0      324 2023-06-02 01:52:23.259358 python_manifest-1.0.1/manifest/expressions/__init__.py
+-rw-r--r--   0        0        0     3988 2023-06-06 20:22:18.129013 python_manifest-1.0.1/manifest/expressions/operations.py
+-rw-r--r--   0        0        0     3232 2023-06-02 05:09:24.543175 python_manifest-1.0.1/manifest/expressions/resolve.py
+-rw-r--r--   0        0        0     1169 2023-06-06 05:14:35.315237 python_manifest-1.0.1/manifest/hooks.py
+-rw-r--r--   0        0        0     2085 2023-06-02 04:19:32.618288 python_manifest-1.0.1/manifest/instantiable.py
+-rw-r--r--   0        0        0     9658 2023-06-06 06:48:03.068229 python_manifest-1.0.1/manifest/parse.py
+-rw-r--r--   0        0        0        0 2023-06-08 22:59:10.862430 python_manifest-1.0.1/manifest/py.typed
+-rw-r--r--   0        0        0      386 2023-06-06 06:37:53.161724 python_manifest-1.0.1/manifest/serializers/__init__.py
+-rw-r--r--   0        0        0      272 2023-06-06 06:46:00.564385 python_manifest-1.0.1/manifest/serializers/base.py
+-rw-r--r--   0        0        0      503 2023-06-02 02:57:07.495149 python_manifest-1.0.1/manifest/serializers/jsons.py
+-rw-r--r--   0        0        0      353 2023-06-02 05:04:07.052998 python_manifest-1.0.1/manifest/serializers/noop.py
+-rw-r--r--   0        0        0      356 2023-06-06 06:37:21.601870 python_manifest-1.0.1/manifest/serializers/tomls.py
+-rw-r--r--   0        0        0      350 2023-06-02 05:04:27.465791 python_manifest-1.0.1/manifest/serializers/yamls.py
+-rw-r--r--   0        0        0     9635 2023-06-02 05:56:38.075877 python_manifest-1.0.1/manifest/utils.py
+-rw-r--r--   0        0        0     1599 2023-06-09 00:12:07.537069 python_manifest-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 python_manifest-1.0.1/PKG-INFO
```

### Comparing `python_manifest-0.1.0/manifest/base.py` & `python_manifest-1.0.1/manifest/base.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/manifest/expressions/operations.py` & `python_manifest-1.0.1/manifest/expressions/operations.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/manifest/expressions/resolve.py` & `python_manifest-1.0.1/manifest/expressions/resolve.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/manifest/hooks.py` & `python_manifest-1.0.1/manifest/hooks.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/manifest/instantiable.py` & `python_manifest-1.0.1/manifest/instantiable.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/manifest/parse.py` & `python_manifest-1.0.1/manifest/parse.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/manifest/utils.py` & `python_manifest-1.0.1/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `python_manifest-0.1.0/pyproject.toml` & `python_manifest-1.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "python-manifest"
-version = "0.1.0"
+version = "1.0.1"
 description = "A modern toolkit for working with application manifests and configurations."
 authors = ["Timothy Pogue <tim@emergentmethods.ai>"]
 readme = "README.md"
 packages = [
     { include = "manifest" },
 ]
+license = "MIT"
+repository = "https://github.com/emergentmethods/python-manifest"
+
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyyaml = "^6.0"
 python-rapidjson = "^1.10"
 pydantic = "^1.10.8"
 python-dotenv = "^1.0.0"
```

### Comparing `python_manifest-0.1.0/PKG-INFO` & `python_manifest-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: python-manifest
-Version: 0.1.0
+Version: 1.0.1
 Summary: A modern toolkit for working with application manifests and configurations.
+Home-page: https://github.com/emergentmethods/python-manifest
+License: MIT
 Author: Timothy Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-rapidjson (>=1.10,<2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/emergentmethods/python-manifest
 Description-Content-Type: text/markdown
 
 # python-manifest
 
+![Gitlab code coverage (self-managed, specific job)](https://img.shields.io/gitlab/pipeline-coverage/wizrds/manifest?branch=main&gitlab_url=https%3A%2F%2Fgit.freqai.cloud&job_name=unit-tests&style=flat-square)
+![GitLab Release (self-managed)](https://img.shields.io/gitlab/v/release/wizrds/manifest?gitlab_url=https%3A%2F%2Fgit.freqai.cloud&include_prereleases&style=flat-square)
+![GitLab (self-managed)](https://img.shields.io/gitlab/license/wizrds/manifest?gitlab_url=https%3A%2F%2Fgit.freqai.cloud&style=flat-square)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-manifest?style=flat-square)
+
 Manifest is a flexible and dynamic Python library designed for managing application manifests including configurations in Python projects. By using the `pydantic` library for data validation, it allows you to define your own models, support dynamic configurations via expressions, and even instantiate Python objects directly from the configuration.
 
 ## Features
 
 - Load manifests and configurations from various sources including files and environment variables.
 - Define manifests as Pydantic models.
 - Supports dynamic configurations through the use of expressions.
@@ -31,15 +40,15 @@
 - Support for multiple file systems using `fsspec`.
 
 ## Getting Started
 
 Install the library using pip:
 
 ```bash
-pip install manifest
+pip install python-manifest
 ```
 
 ## Usage
 
 ### Manifest Object
 
 The Manifest class allows you to load and process manifests and configurations from various sources. It is designed to be subclassed, allowing you to define your own configuration models.
```

