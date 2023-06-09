# Comparing `tmp/markpickle-1.6.0.tar.gz` & `tmp/markpickle-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markpickle-1.6.0.tar", max compression
+gzip compressed data, was "markpickle-1.6.1.tar", max compression
```

## Comparing `markpickle-1.6.0.tar` & `markpickle-1.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-06-09 02:32:42.419553 markpickle-1.6.0/LICENSE
--rw-r--r--   0        0        0     7355 2023-06-09 02:32:42.423553 markpickle-1.6.0/README.md
--rw-r--r--   0        0        0      723 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/__init__.py
--rw-r--r--   0        0        0     1437 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/__main__.py
--rw-r--r--   0        0        0     2804 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/atx_as_dictionary.py
--rw-r--r--   0        0        0     1614 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/binary_streams.py
--rw-r--r--   0        0        0       57 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/cli.py
--rw-r--r--   0        0        0     2539 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/config_class.py
--rw-r--r--   0        0        0    14645 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/deserialize.py
--rw-r--r--   0        0        0      412 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/meta.py
--rw-r--r--   0        0        0     1406 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/mypy_types.py
--rw-r--r--   0        0        0       80 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/py.typed
--rw-r--r--   0        0        0     5581 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/python_to_tables.py
--rw-r--r--   0        0        0    15443 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/serialize.py
--rw-r--r--   0        0        0      737 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/simplify_types.py
--rw-r--r--   0        0        0     1043 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/split_file_code.py
--rw-r--r--   0        0        0      538 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/sugar.py
--rw-r--r--   0        0        0     1216 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/third_party_tables.py
--rw-r--r--   0        0        0     1760 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/tool.py
--rw-r--r--   0        0        0      813 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/unicode_formatting.py
--rw-r--r--   0        0        0     3886 2023-06-09 02:32:42.423553 markpickle-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     8879 1970-01-01 00:00:00.000000 markpickle-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-09 02:38:33.606409 markpickle-1.6.1/LICENSE
+-rw-r--r--   0        0        0     7355 2023-06-09 02:38:33.606409 markpickle-1.6.1/README.md
+-rw-r--r--   0        0        0      723 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/__init__.py
+-rw-r--r--   0        0        0     1437 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/__main__.py
+-rw-r--r--   0        0        0     2804 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/atx_as_dictionary.py
+-rw-r--r--   0        0        0     1614 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/binary_streams.py
+-rw-r--r--   0        0        0       57 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/cli.py
+-rw-r--r--   0        0        0     2539 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/config_class.py
+-rw-r--r--   0        0        0    14645 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/deserialize.py
+-rw-r--r--   0        0        0      412 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/meta.py
+-rw-r--r--   0        0        0     1486 2023-06-09 02:39:11.482366 markpickle-1.6.1/markpickle/mypy_types.py
+-rw-r--r--   0        0        0       80 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/py.typed
+-rw-r--r--   0        0        0     5581 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/python_to_tables.py
+-rw-r--r--   0        0        0    15443 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/serialize.py
+-rw-r--r--   0        0        0      737 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/simplify_types.py
+-rw-r--r--   0        0        0     1043 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/split_file_code.py
+-rw-r--r--   0        0        0      538 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/sugar.py
+-rw-r--r--   0        0        0     1216 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/third_party_tables.py
+-rw-r--r--   0        0        0     1760 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/tool.py
+-rw-r--r--   0        0        0      813 2023-06-09 02:38:33.610409 markpickle-1.6.1/markpickle/unicode_formatting.py
+-rw-r--r--   0        0        0     3886 2023-06-09 02:38:33.610409 markpickle-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8879 1970-01-01 00:00:00.000000 markpickle-1.6.1/PKG-INFO
```

### Comparing `markpickle-1.6.0/LICENSE` & `markpickle-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/README.md` & `markpickle-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/__init__.py` & `markpickle-1.6.1/markpickle/__init__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/__main__.py` & `markpickle-1.6.1/markpickle/__main__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/atx_as_dictionary.py` & `markpickle-1.6.1/markpickle/atx_as_dictionary.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/binary_streams.py` & `markpickle-1.6.1/markpickle/binary_streams.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/config_class.py` & `markpickle-1.6.1/markpickle/config_class.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/deserialize.py` & `markpickle-1.6.1/markpickle/deserialize.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/mypy_types.py` & `markpickle-1.6.1/markpickle/mypy_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Subset of python types that markpickle will attempt to roundtrip
 """
 from __future__ import annotations
 
 import datetime
-from typing import Any, Optional, Union
+from typing import Any, Optional, TypeAlias, Union
 
-try:
-    from typing_extensions import TypeAlias
-except ModuleNotFoundError:
-    from typing import TypeAlias  # type: ignore[no-redef,attr-defined]
-except ImportError:
-    from typing import TypeAlias  # type: ignore[no-redef,attr-defined]
+# this isn't 3.9 compatible. Can't catch ModuleNotFound!
+# try:
+#     from typing_extensions import TypeAlias
+# except ModuleNotFoundError:
+#     from typing import TypeAlias  # type: ignore[no-redef,attr-defined]
+# except ImportError:
+#    from typing import TypeAlias  # type: ignore[no-redef,attr-defined]
 
 
 # https://github.com/python/mypy/issues/14219#issuecomment-1528993478
 ScalarTypes = Union[
     None,
     str,
     int,
```

### Comparing `markpickle-1.6.0/markpickle/python_to_tables.py` & `markpickle-1.6.1/markpickle/python_to_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/serialize.py` & `markpickle-1.6.1/markpickle/serialize.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/simplify_types.py` & `markpickle-1.6.1/markpickle/simplify_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/split_file_code.py` & `markpickle-1.6.1/markpickle/split_file_code.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/sugar.py` & `markpickle-1.6.1/markpickle/sugar.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/third_party_tables.py` & `markpickle-1.6.1/markpickle/third_party_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/tool.py` & `markpickle-1.6.1/markpickle/tool.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/markpickle/unicode_formatting.py` & `markpickle-1.6.1/markpickle/unicode_formatting.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.6.0/pyproject.toml` & `markpickle-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markpickle"
-version = "1.6.0"
+version = "1.6.1"
 description = "Lossy python to markdown serializer"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `markpickle-1.6.0/PKG-INFO` & `markpickle-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markpickle
-Version: 1.6.0
+Version: 1.6.1
 Summary: Lossy python to markdown serializer
 Home-page: https://github.com/matthewdeanmartin/markpickle
 License: MIT
 Keywords: serializer,deserializer,markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
```

