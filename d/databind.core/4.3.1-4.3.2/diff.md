# Comparing `tmp/databind.core-4.3.1.tar.gz` & `tmp/databind.core-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.3.1.tar", max compression
+gzip compressed data, was "databind.core-4.3.2.tar", max compression
```

## Comparing `databind.core-4.3.1.tar` & `databind.core-4.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      337 2023-06-07 22:10:11.705365 databind.core-4.3.1/README.md
--rw-r--r--   0        0        0     1687 2023-06-09 13:14:16.060716 databind.core-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     1601 2023-06-09 13:14:16.060716 databind.core-4.3.1/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2023-06-07 22:10:11.705365 databind.core-4.3.1/src/databind/core/context.py
--rw-r--r--   0        0        0     6059 2023-06-09 13:06:50.872189 databind.core-4.3.1/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-06-07 22:10:11.705365 databind.core-4.3.1/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-06-07 22:10:11.705365 databind.core-4.3.1/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-06-07 22:10:11.705365 databind.core-4.3.1/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-06-07 22:10:11.705365 databind.core-4.3.1/src/databind/core/py.typed
--rw-r--r--   0        0        0    15494 2023-06-07 22:10:11.705365 databind.core-4.3.1/src/databind/core/schema.py
--rw-r--r--   0        0        0    27732 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/settings.py
--rw-r--r--   0        0        0     1044 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/tests/context_test.py
--rw-r--r--   0        0        0     1275 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/tests/schema_docspec_example_test.py
--rw-r--r--   0        0        0    11386 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/tests/schema_test.py
--rw-r--r--   0        0        0      733 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/tests/schema_with_nested_dataclasses_test.py
--rw-r--r--   0        0        0     8709 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-06-07 22:10:11.709365 databind.core-4.3.1/src/databind/core/utils.py
--rw-r--r--   0        0        0     1261 2023-06-09 13:14:29.370377 databind.core-4.3.1/setup.py
--rw-r--r--   0        0        0     1435 2023-06-09 13:14:29.370795 databind.core-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0      337 2023-06-07 22:10:11.705365 databind.core-4.3.2/README.md
+-rw-r--r--   0        0        0     1687 2023-06-09 13:43:37.674709 databind.core-4.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1601 2023-06-09 13:43:37.674709 databind.core-4.3.2/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/context.py
+-rw-r--r--   0        0        0     6059 2023-06-09 13:06:50.872189 databind.core-4.3.2/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15494 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/schema.py
+-rw-r--r--   0        0        0    27732 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/settings.py
+-rw-r--r--   0        0        0     1044 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/context_test.py
+-rw-r--r--   0        0        0     1275 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/schema_docspec_example_test.py
+-rw-r--r--   0        0        0    11386 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/schema_test.py
+-rw-r--r--   0        0        0      733 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/schema_with_nested_dataclasses_test.py
+-rw-r--r--   0        0        0     8709 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/utils.py
+-rw-r--r--   0        0        0     1261 2023-06-09 13:43:49.375274 databind.core-4.3.2/setup.py
+-rw-r--r--   0        0        0     1435 2023-06-09 13:43:49.375778 databind.core-4.3.2/PKG-INFO
```

### Comparing `databind.core-4.3.1/pyproject.toml` & `databind.core-4.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.3.1"
+version = "4.3.2"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
```

### Comparing `databind.core-4.3.1/src/databind/core/__init__.py` & `databind.core-4.3.2/src/databind/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.3.1"
+__version__ = "4.3.2"
 
 from .context import Context, Direction, Location, format_context_trace
 from .converter import ConversionError, Converter, DelegateToClassmethodConverter, Module, NoMatchingConverter
 from .mapper import ObjectMapper
 from .schema import (
     Field,
     Schema,
```

### Comparing `databind.core-4.3.1/src/databind/core/context.py` & `databind.core-4.3.2/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/converter.py` & `databind.core-4.3.2/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/dataclasses.py` & `databind.core-4.3.2/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/dataclasses.pyi` & `databind.core-4.3.2/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/mapper.py` & `databind.core-4.3.2/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/schema.py` & `databind.core-4.3.2/src/databind/core/schema.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/settings.py` & `databind.core-4.3.2/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/tests/context_test.py` & `databind.core-4.3.2/src/databind/core/tests/context_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/tests/schema_docspec_example_test.py` & `databind.core-4.3.2/src/databind/core/tests/schema_docspec_example_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/tests/schema_test.py` & `databind.core-4.3.2/src/databind/core/tests/schema_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/tests/schema_with_nested_dataclasses_test.py` & `databind.core-4.3.2/src/databind/core/tests/schema_with_nested_dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/union.py` & `databind.core-4.3.2/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/src/databind/core/utils.py` & `databind.core-4.3.2/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.1/setup.py` & `databind.core-4.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.3.1',
+    'version': '4.3.2',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# `databind.core`\n\nThis library provides the core functionality to implement serialization functions to and from Python objects, with\na great support for many features of the Python type system. A JSON implementation is provided by the `databind.json`\npackage.\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.3.1/PKG-INFO` & `databind.core-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.3.1
+Version: 4.3.2
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

