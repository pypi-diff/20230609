# Comparing `tmp/pipen_filters-0.7.0.tar.gz` & `tmp/pipen_filters-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_filters-0.7.0.tar", max compression
+gzip compressed data, was "pipen_filters-0.8.0.tar", max compression
```

## Comparing `pipen_filters-0.7.0.tar` & `pipen_filters-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     2853 2023-04-14 06:40:22.644777 pipen_filters-0.7.0/README.md
--rw-r--r--   0        0        0     1831 2023-04-14 06:40:22.644777 pipen_filters-0.7.0/pipen_filters/__init__.py
--rw-r--r--   0        0        0     5720 2023-04-14 06:40:22.644777 pipen_filters-0.7.0/pipen_filters/filters.py
--rwxr-xr-x   0        0        0     1180 2023-04-14 06:40:22.644777 pipen_filters-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 pipen_filters-0.7.0/setup.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pipen_filters-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2853 2023-06-08 23:21:52.632104 pipen_filters-0.8.0/README.md
+-rw-r--r--   0        0        0     1831 2023-06-08 23:21:52.632104 pipen_filters-0.8.0/pipen_filters/__init__.py
+-rw-r--r--   0        0        0     5720 2023-06-08 23:21:52.632104 pipen_filters-0.8.0/pipen_filters/filters.py
+-rwxr-xr-x   0        0        0     1181 2023-06-08 23:21:52.632104 pipen_filters-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 pipen_filters-0.8.0/setup.py
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 pipen_filters-0.8.0/PKG-INFO
```

### Comparing `pipen_filters-0.7.0/README.md` & `pipen_filters-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_filters-0.7.0/pipen_filters/__init__.py` & `pipen_filters-0.8.0/pipen_filters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pipen.utils import logger
 
 from .filters import FILTERS
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Pipen
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 
 class PipenFilters:
     __version__: str = __version__
 
     @plugin.impl
     async def on_init(pipen: "Pipen") -> None:  # type: ignore
```

### Comparing `pipen_filters-0.7.0/pipen_filters/filters.py` & `pipen_filters-0.8.0/pipen_filters/filters.py`

 * *Files identical despite different names*

### Comparing `pipen_filters-0.7.0/pyproject.toml` & `pipen_filters-0.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pipen-filters"
-version = "0.7.0"
+version = "0.8.0"
 description = "Add a set of useful filters for pipen templates"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-filters"
 repository = "https://github.com/pwwang/pipen-filters"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pipen = "^0.9"
+pipen = "^0.10"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
```

### Comparing `pipen_filters-0.7.0/setup.py` & `pipen_filters-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['pipen_filters']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pipen>=0.9,<0.10']
+['pipen>=0.10,<0.11']
 
 entry_points = \
 {'pipen': ['filters = pipen_filters:PipenFilters']}
 
 setup_kwargs = {
     'name': 'pipen-filters',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'Add a set of useful filters for pipen templates',
     'long_description': '# pipen-filters\n\nAdd a set of useful filters for [pipen][1] templates.\n\nThese filters can be used for both liquid and jinja2 templating in pipen.\n\n## Installation\n\n```shell\npip install -U pipen-filters\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:filters"]`, or uninstall this plugin.\n\n## Usage\n\n```python\nfrom pipen import Proc\n\nclass MyProc(Proc):\n    input = "infile:file"\n    output = "outfile:file:{{in.infile | stem}}.txt"\n    ...\n```\n\n## Filters\n\n- Parse the symbolic links\n\n  - `realpath`: `os.path.realpath`\n  - `readlink`: `os.readlink`\n\n- Find common prefix of given paths\n\n  - `commonprefix`:\n\n      ```python\n      >>> commonprefix("/a/b/abc.txt", "/a/b/abc.png")\n      >>> # "abc."\n      >>> commonprefix("/a/b/abc.txt", "/a/b/abc.png", basename_only=False)\n      >>> # "/a/b/abc."\n      ```\n\n- Get parts of the path\n\n  - `dirname`: `path.dirname`\n  - `basename`: `path.basename`\n  - `ext`: get the extension (`/a/b/c.txt -> .txt`)\n  - `ext0`: get the extension without dot (`/a/b/c.txt -> txt`)\n  - `prefix`: get the prefix of a path (`/a/b/c.d.txt -> /a/b/c.d`)\n  - `prefix0`: get the prefix of a path without dot in basename (`/a/b/c.d.txt -> /a/b/c`)\n  - `filename`, `fn`, `stem`: get the stem of a path (`/a/b.c.txt -> b.c`)\n  - `filename0`, `fn0`, `stem0`: get the stem of a path without dot (`/a/b.c.txt -> b`)\n  - `joinpaths`: join path parts (`os.path.join`)\n  - `as_path`: convert a string into a `pathlib.Path` object\n\n- Path stat\n\n  - `isdir`: `os.path.isdir`\n  - `isfile`: `os.path.isfile`\n  - `islink`: `os.path.islink`\n  - `exists`: `os.path.exists`\n  - `getsize`: `os.path.getsize`, return -1 if the path doesn\'t exist\n  - `getmtime`: `os.path.getmtime`, return -1 if the path doesn\'t exist\n  - `getctime`: `os.path.getctime`, return -1 if the path doesn\'t exist\n  - `getatime`: `os.path.getatime`, return -1 if the path doesn\'t exist\n  - `isempty`: check if a file is empty\n\n- Quote data\n\n  - `quote`: put double quotes around data (`1 -> "1"`)\n  - `squote`: put single quotes around data (`1 -> \'1\'`)\n\n- Configurations\n  - `json`: `json.dumps`\n  - `json_dump`: Load json froma  file\n  - `json_dumps`: Alias of `json`\n  - `json_loads`: `json.loads`\n  - `toml`: `toml.dumps`\n  - `toml_dump`: Load toml from a file\n  - `toml_dumps`: Alias of `toml`\n  - `toml_loads`: `toml.loads`\n  - `config`: Load configuration from an object, a string or a file\n\n- Globs\n\n  - `glob`: Like `glob.glob`, but allows passing multiple parts of a path\n  - `glob0`: Like `glob`, but only returns the first matched path\n\n- Read file contents\n\n  - `read`: Read file content. You can also pass arguments to `open`\n  - `readlines`: Read file content as a list of lines. Additional arguments will be passed to `open`\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-filters',
```

### Comparing `pipen_filters-0.7.0/PKG-INFO` & `pipen_filters-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-filters
-Version: 0.7.0
+Version: 0.8.0
 Summary: Add a set of useful filters for pipen templates
 Home-page: https://github.com/pwwang/pipen-filters
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pipen (>=0.9,<0.10)
+Requires-Dist: pipen (>=0.10,<0.11)
 Project-URL: Repository, https://github.com/pwwang/pipen-filters
 Description-Content-Type: text/markdown
 
 # pipen-filters
 
 Add a set of useful filters for [pipen][1] templates.
```

