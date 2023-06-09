# Comparing `tmp/databind-4.3.0.tar.gz` & `tmp/databind-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind-4.3.0.tar", max compression
+gzip compressed data, was "databind-4.3.1.tar", max compression
```

## Comparing `databind-4.3.0.tar` & `databind-4.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3097 2023-05-28 15:44:00.007979 databind-4.3.0/README.md
--rw-r--r--   0        0        0      612 2023-05-28 18:45:00.557567 databind-4.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-28 18:45:00.561567 databind-4.3.0/src/databind/_version/__init__.py
--rw-r--r--   0        0        0     4056 2023-05-28 18:45:08.057884 databind-4.3.0/setup.py
--rw-r--r--   0        0        0     3903 2023-05-28 18:45:08.058052 databind-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3097 2023-06-07 22:10:11.709365 databind-4.3.1/README.md
+-rw-r--r--   0        0        0      612 2023-06-09 13:14:16.060716 databind-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-09 13:14:16.060716 databind-4.3.1/src/databind/_version/__init__.py
+-rw-r--r--   0        0        0     4056 2023-06-09 13:14:28.018945 databind-4.3.1/setup.py
+-rw-r--r--   0        0        0     3903 2023-06-09 13:14:28.019248 databind-4.3.1/PKG-INFO
```

### Comparing `databind-4.3.0/README.md` & `databind-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `databind-4.3.0/pyproject.toml` & `databind-4.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "databind"
-version = "4.3.0"
+version = "4.3.1"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include="databind/_version", from="src" }]
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
-"databind.core" = "^4.3.0"
-"databind.json" = "^4.3.0"
+"databind.core" = "^4.3.1"
+"databind.json" = "^4.3.1"
 
 [build-system]
 requires = ["poetry-core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `databind-4.3.0/setup.py` & `databind-4.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['_version']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['databind.core>=4.3.0,<5.0.0', 'databind.json>=4.3.0,<5.0.0']
+['databind.core>=4.3.1,<5.0.0', 'databind.json>=4.3.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'databind',
-    'version': '4.3.0',
+    'version': '4.3.1',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.7 and newer.',
     'long_description': '<h1 align="center">databind</h1>\n\n<p align="center">\n  <img src="https://img.shields.io/pypi/pyversions/databind?style=for-the-badge" alt="Python versions">\n  <a href="https://pypi.org/project/databind/"><img src="https://img.shields.io/pypi/v/databind?style=for-the-badge"></a>\n</p>\n<p align="center"><i>\nDatabind is a Python serialization library on top of dataclasses, inspired by similar libraries from other languages\nlike <a href="https://github.com/FasterXML/jackson-databind">jackson-databind</a> and <a href="https://serde.rs/">serde-rs</a>.</i>\n</p>\n<p align="center">\n  <a href="https://niklasrosenstein.github.io/python-databind/core/basic-usage/">CORE Guide</a> |\n  <a href="https://niklasrosenstein.github.io/python-databind/json/examples/">JSON Examples</a>\n</p>\n\n## Overview 📖\n\nThe `databind.core` package provides the core framework for databind. It is then used by `databind.json` to provide\ncomprehensive serializatio support between Python and JSON-like data structure. The serialization can easily be\nextended to YAML or TOML by combining it with respective libraries (e.g. `pyaaml` and `tomli`).\n\n```python\n@dataclass\nclass Server:\n    host: str\n    port: int\n\n@dataclass\nclass Config:\n    server: Server\n\nfrom databind.json import dump, load\nassert load({"server": {"host": "localhost", "port": 8080}}, Config) == Config(server=Server(host=\'localhost\', port=8080))\nassert dump(Config(server=Server(host=\'localhost\', port=8080)), Config) == {"server": {"host": "localhost", "port": 8080}}\n```\n\nIf you install the `databind` proxy package, you get matching versions of `databind.core` and `databind.json`.\n\n## Features ✨\n\n  [typeapi]: https://github.com/NiklasRosenstein/python-typeapi\n\n* Support for a plethora of builtin types, including `Enum`, `Decimal`, `UUID`, `Path`, `datetime`, `date`, `time`, `timedelta`\n* Support for multiple union serialization modes (nested, flat, keyed, `typing.Literal`)\n* Support for generic types, e.g. `load([{"name": "Jane Doe"}], list[Person])`\n* Support for new-style type hints in older Python versions when using forward refererences (strings or `__future__.annotations`) thanks to [typeapi][]\n    * [PEP 604 - Allow writing union types as X | Y](https://www.python.org/dev/peps/pep-0604/)\n    * [PEP585 - Type Hinting Generics in Standard Collections](https://www.python.org/dev/peps/pep-0585/))\n* Support for customized serialization and deserialization of types\n* Support for flattening fields of a nested dataclass or collecting remaining fields in a `dict`\n* Full runtime type checking during serialization\n* Use "settings" to customize serialization behaviour\n    * As global settings per `load()`/`dump()` call: `load(..., settings=[ExtraKeys(True)])`\n    * As class-level settings using a decorator: `@Union(style=Union.FLAT)` or `@ExtraKeys(True)`\n    * As type-hint level settings using `typing.Annotated` (or `typing_extensions.Annotated`): `full_name: Annotated[str, Alias("fullName")]` or `FullNameField = Annotated[str, Alias("fullName")]`\n\n---\n\n<p align="center">Copyright &copy; 2022 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['_version'] package_data = \ {'': ['*']} install_requires
-= \ ['databind.core>=4.3.0,<5.0.0', 'databind.json>=4.3.0,<5.0.0'] setup_kwargs
-= { 'name': 'databind', 'version': '4.3.0', 'description': 'Databind is a
+= \ ['databind.core>=4.3.1,<5.0.0', 'databind.json>=4.3.1,<5.0.0'] setup_kwargs
+= { 'name': 'databind', 'version': '4.3.1', 'description': 'Databind is a
 library inspired by jackson-databind to de-/serialize Python dataclasses. The
 `databind` package will install the full suite of databind packages. Compatible
 with Python 3.7 and newer.', 'long_description': '
                             ****** databind ******
 \n\n
  \n [Python versions]\n [https://img.shields.io/pypi/v/databind?style=for-the-
                                    badge]\n
```

### Comparing `databind-4.3.0/PKG-INFO` & `databind-4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: databind
-Version: 4.3.0
+Version: 4.3.1
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: databind.core (>=4.3.0,<5.0.0)
-Requires-Dist: databind.json (>=4.3.0,<5.0.0)
+Requires-Dist: databind.core (>=4.3.1,<5.0.0)
+Requires-Dist: databind.json (>=4.3.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">databind</h1>
 
 <p align="center">
   <img src="https://img.shields.io/pypi/pyversions/databind?style=for-the-badge" alt="Python versions">
   <a href="https://pypi.org/project/databind/"><img src="https://img.shields.io/pypi/v/databind?style=for-the-badge"></a>
```

