# Comparing `tmp/refaci-0.6.0.tar.gz` & `tmp/refaci-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refaci-0.6.0.tar", max compression
+gzip compressed data, was "refaci-0.6.1.tar", max compression
```

## Comparing `refaci-0.6.0.tar` & `refaci-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-05-27 11:26:39.245469 refaci-0.6.0/LICENSE
--rw-r--r--   0        0        0      961 2023-05-28 23:14:34.768094 refaci-0.6.0/README.md
--rw-r--r--   0        0        0     3854 2023-06-06 05:55:11.364110 refaci-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-28 23:14:34.914760 refaci-0.6.0/refaci/__init__.py
--rw-r--r--   0        0        0      434 2023-05-28 22:39:51.012862 refaci-0.6.0/refaci/__main__.py
--rw-r--r--   0        0        0     2901 2023-06-06 05:54:59.307510 refaci-0.6.0/refaci/gather.py
--rw-r--r--   0        0        0     4958 2023-06-06 05:49:09.949427 refaci-0.6.0/refaci/refactor.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 refaci-0.6.0/setup.py
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 refaci-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-27 11:26:39.245469 refaci-0.6.1/LICENSE
+-rw-r--r--   0        0        0      961 2023-05-28 23:14:34.768094 refaci-0.6.1/README.md
+-rw-r--r--   0        0        0     3854 2023-06-09 06:37:40.083455 refaci-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-28 23:14:34.914760 refaci-0.6.1/refaci/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-28 22:39:51.012862 refaci-0.6.1/refaci/__main__.py
+-rw-r--r--   0        0        0     2901 2023-06-06 05:54:59.307510 refaci-0.6.1/refaci/gather.py
+-rw-r--r--   0        0        0     4987 2023-06-09 06:37:22.630122 refaci-0.6.1/refaci/refactor.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 refaci-0.6.1/setup.py
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 refaci-0.6.1/PKG-INFO
```

### Comparing `refaci-0.6.0/LICENSE` & `refaci-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `refaci-0.6.0/README.md` & `refaci-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `refaci-0.6.0/pyproject.toml` & `refaci-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refaci"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/refaci"
 
 [tool.poetry.dependencies]
```

### Comparing `refaci-0.6.0/refaci/gather.py` & `refaci-0.6.1/refaci/gather.py`

 * *Files identical despite different names*

### Comparing `refaci-0.6.0/refaci/refactor.py` & `refaci-0.6.1/refaci/refactor.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 import json
 import os
 import re
 from collections import defaultdict
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Callable, Collection, TypeVar, cast
+from typing import Any, Callable, Collection, Mapping, TypeVar, cast
 
 T = TypeVar("T", Path, str)
 
 
 def refactor(
     root_dir: Path,
     imports_to_change: dict[str, tuple[str, str]] = {},
@@ -26,15 +26,15 @@
     contents_re = {
         regex: replacements for regex, replacements in replacement_dict.items() if isinstance(regex, ContentsRegex)
     }
 
     for root, dirs, files in os.walk(root_dir):
         root = Path(root)
         dirs = [root / dir for dir in dirs]
-        files = [root / file for file in files]
+        files = [root / file for file in files if file.endswith(".py")]
 
         for file in files:
             print(str(file))
             try:
                 contents = file.read_text()
                 file_replacements = []
                 file_replacements.extend(
@@ -59,32 +59,32 @@
                     for replacement in replacements:
                         assert callable(replacement), "DirRegex must be a callable that accepts a dir path"
                         run_replacement(dir, replacement)
 
 
 def refactor_imports(
     contents: str,
-    imports_to_change: dict[str, tuple[str, str]] = {},
+    imports_to_change: Mapping = {},
     missing_imports_to_add: dict[str, str] = {},
 ):
-    modules = to_modules(imports_to_change)
     tree = ast.parse(contents)
     lines = cast(list[str | list[str]], contents.splitlines())
 
     for node in ast.walk(tree):
         # TODO
         if isinstance(node, ast.Import):
             for alias in node.names:
                 ...
-        elif isinstance(node, ast.ImportFrom) and node.module in modules:
+        elif isinstance(node, ast.ImportFrom) and node.module in imports_to_change:
             replacing_lines = []
             for alias in node.names:
-                if alias.name in modules[node.module]:
+                if alias.name in imports_to_change[node.module]:
                     replacing_lines.append(
-                        " " * node.col_offset + f"from {modules[node.module][alias.name]} import {alias.name}",
+                        " " * node.col_offset
+                        + f"from {imports_to_change[node.module][alias.name]} import {alias.name}",
                     )
                 else:
                     replacing_lines.append(" " * node.col_offset + f"from {node.module} import {alias.name}")
             # this trick allows us to replace without changing the number/order of lines
             lines[node.lineno - 1 : node.end_lineno] = [replacing_lines] + [[]] * (node.end_lineno - node.lineno)
     lines.insert(
         0,
```

### Comparing `refaci-0.6.0/setup.py` & `refaci-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['typer[all]', 'typing-extensions']
 
 entry_points = \
 {'console_scripts': ['refaci = refaci.__main__:app']}
 
 setup_kwargs = {
     'name': 'refaci',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': '',
     'long_description': '# refaci\n\nA toolbox for changing imports in enormous codebases after a large refactoring.\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/refaci/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/refaci/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/refaci" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/refaci?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/refaci/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/refaci?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/refaci/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/refaci?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install refaci\n```\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ovsyanka83/refaci',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['refaci']
 package_data = \ {'': ['*']} install_requires = \ ['typer[all]', 'typing-
 extensions'] entry_points = \ {'console_scripts': ['refaci = refaci.__main__:
-app']} setup_kwargs = { 'name': 'refaci', 'version': '0.6.0', 'description':
+app']} setup_kwargs = { 'name': 'refaci', 'version': '0.6.1', 'description':
 '', 'long_description': '# refaci\n\nA toolbox for changing imports in enormous
 codebases after a large refactoring.\n\n---\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
 \n\n## Installation\n\n```bash\npip install refaci\n```\n', 'author':
 'Stanislav Zmiev', 'author_email': 'szmiev2000@gmail.com', 'maintainer':
 'None', 'maintainer_email': 'None', 'url': 'https://github.com/ovsyanka83/
 refaci', 'packages': packages, 'package_data': package_data,
```

### Comparing `refaci-0.6.0/PKG-INFO` & `refaci-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refaci
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Home-page: https://github.com/ovsyanka83/refaci
 License: MIT
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refaci Version: 0.6.0 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: refaci Version: 0.6.1 Summary: Home-page: https://
 github.com/ovsyanka83/refaci License: MIT Author: Stanislav Zmiev Author-email:
 szmiev2000@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: typer[all] Requires-Dist: typing-
 extensions Project-URL: Repository, https://github.com/ovsyanka83/refaci
 Description-Content-Type: text/markdown # refaci A toolbox for changing imports
```

