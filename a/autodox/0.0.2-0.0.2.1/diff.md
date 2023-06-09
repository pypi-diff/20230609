# Comparing `tmp/autodox-0.0.2.tar.gz` & `tmp/autodox-0.0.2.1.tar.gz`

## Comparing `autodox-0.0.2.tar` & `autodox-0.0.2.1.tar`

### file list

```diff
@@ -1,12 +1,7 @@
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 autodox-0.0.2/autodox/__init__.py
--rw-r--r--   0        0        0    13833 2020-02-02 00:00:00.000000 autodox-0.0.2/autodox/functions.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 autodox-0.0.2/tests/test.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 autodox-0.0.2/tests/tapescript/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 autodox-0.0.2/tests/tapescript/classes.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 autodox-0.0.2/tests/tapescript/errors.py
--rw-r--r--   0        0        0    42770 2020-02-02 00:00:00.000000 autodox-0.0.2/tests/tapescript/functions.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.2/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.2/license
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 autodox-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 autodox-0.0.2/readme.md
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 autodox-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 autodox-0.0.2.1/autodox/__init__.py
+-rw-r--r--   0        0        0    13833 2020-02-02 00:00:00.000000 autodox-0.0.2.1/autodox/functions.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.2.1/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.2.1/license
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 autodox-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 autodox-0.0.2.1/PKG-INFO
```

### Comparing `autodox-0.0.2/autodox/functions.py` & `autodox-0.0.2.1/autodox/functions.py`

 * *Files identical despite different names*

### Comparing `autodox-0.0.2/license` & `autodox-0.0.2.1/license`

 * *Files identical despite different names*

### Comparing `autodox-0.0.2/pyproject.toml` & `autodox-0.0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autodox"
-version = "0.0.2"
+version = "0.0.2.1"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Tool for generating documentation automatically from code annotations, types, and docstrings."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `autodox-0.0.2/readme.md` & `autodox-0.0.2.1/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -91,35 +91,14 @@
 - `exclude_names: list[str]` - names to exclude from docs
 - `header_level: int` - number of additional hashtags to add to headers
 - `include_private: bool` - if True, includes things with names prefaced by '_'
 - `include_dunder: bool` - if True, includes things with names prefaced by '__'
 - `method_format: str` - can be one of 'header', 'paragraph', or 'list'
 
 
-## Testing
-
-First, clone the repo, set up the virtualenv, and install requirements.
-
-```bash
-git clone ...
-python -m venv venv/
-source venv/bin/activate
-pip install -r requirements.txt
-```
-
-For windows, replace `source venv/bin/activate` with `source venv/Scripts/activate`.
-
-Then run the test suite with the following:
-
-```bash
-python test/test_functions.py
-```
-
-There are currently 0 tests.
-
 ## ISC License
 
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
 that the above copyleft notice and this permission notice appear in
```

### Comparing `autodox-0.0.2/PKG-INFO` & `autodox-0.0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodox
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Tool for generating documentation automatically from code annotations, types, and docstrings.
 Project-URL: Homepage, https://github.com/k98kurz/autodox
 Project-URL: Bug Tracker, https://github.com/k98kurz/autodox/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -107,35 +107,14 @@
 - `exclude_names: list[str]` - names to exclude from docs
 - `header_level: int` - number of additional hashtags to add to headers
 - `include_private: bool` - if True, includes things with names prefaced by '_'
 - `include_dunder: bool` - if True, includes things with names prefaced by '__'
 - `method_format: str` - can be one of 'header', 'paragraph', or 'list'
 
 
-## Testing
-
-First, clone the repo, set up the virtualenv, and install requirements.
-
-```bash
-git clone ...
-python -m venv venv/
-source venv/bin/activate
-pip install -r requirements.txt
-```
-
-For windows, replace `source venv/bin/activate` with `source venv/Scripts/activate`.
-
-Then run the test suite with the following:
-
-```bash
-python test/test_functions.py
-```
-
-There are currently 0 tests.
-
 ## ISC License
 
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
 that the above copyleft notice and this permission notice appear in
```

