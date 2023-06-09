# Comparing `tmp/pipen_cli_require-0.6.0.tar.gz` & `tmp/pipen_cli_require-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_cli_require-0.6.0.tar", max compression
+gzip compressed data, was "pipen_cli_require-0.7.0.tar", max compression
```

## Comparing `pipen_cli_require-0.6.0.tar` & `pipen_cli_require-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2682 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/README.md
--rw-r--r--   0        0        0      132 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/__init__.py
--rw-r--r--   0        0        0     2277 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/entry.py
--rw-r--r--   0        0        0    10514 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/require.py
--rw-r--r--   0        0        0       46 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pipen_cli_require/version.py
--rw-r--r--   0        0        0     1026 2023-04-14 22:20:14.829520 pipen_cli_require-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 pipen_cli_require-0.6.0/setup.py
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 pipen_cli_require-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2682 2023-06-09 06:58:01.543026 pipen_cli_require-0.7.0/README.md
+-rw-r--r--   0        0        0      132 2023-06-09 06:58:01.543026 pipen_cli_require-0.7.0/pipen_cli_require/__init__.py
+-rw-r--r--   0        0        0     2277 2023-06-09 06:58:01.543026 pipen_cli_require-0.7.0/pipen_cli_require/entry.py
+-rw-r--r--   0        0        0    10514 2023-06-09 06:58:01.543026 pipen_cli_require-0.7.0/pipen_cli_require/require.py
+-rw-r--r--   0        0        0       46 2023-06-09 06:58:01.543026 pipen_cli_require-0.7.0/pipen_cli_require/version.py
+-rw-r--r--   0        0        0     1027 2023-06-09 06:58:01.543026 pipen_cli_require-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 pipen_cli_require-0.7.0/setup.py
+-rw-r--r--   0        0        0     3296 1970-01-01 00:00:00.000000 pipen_cli_require-0.7.0/PKG-INFO
```

### Comparing `pipen_cli_require-0.6.0/README.md` & `pipen_cli_require-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_cli_require-0.6.0/pipen_cli_require/entry.py` & `pipen_cli_require-0.7.0/pipen_cli_require/entry.py`

 * *Files identical despite different names*

### Comparing `pipen_cli_require-0.6.0/pipen_cli_require/require.py` & `pipen_cli_require-0.7.0/pipen_cli_require/require.py`

 * *Files identical despite different names*

### Comparing `pipen_cli_require-0.6.0/pyproject.toml` & `pipen_cli_require-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "pipen-cli-require"
-version = "0.6.0"
+version = "0.7.0"
 description = "A pipen cli plugin to check requirements for processes of a pipeline"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pipen-annotate = "^0.7"
+pipen-annotate = "^0.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-asyncio = "^0.20"
 pytest-cov = "^4"
 pytest-xdist = "^3"
 cmdy = "^0.5"
-pipen-args = "^0.9"
+pipen-args = "^0.10"
 
 [tool.poetry.plugins.pipen_cli]
 cli-require = "pipen_cli_require:PipenCliRequirePlugin"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pipen_cli_require-0.6.0/setup.py` & `pipen_cli_require-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['pipen_cli_require']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pipen-annotate>=0.7,<0.8']
+['pipen-annotate>=0.9,<0.10']
 
 entry_points = \
 {'pipen_cli': ['cli-require = pipen_cli_require:PipenCliRequirePlugin']}
 
 setup_kwargs = {
     'name': 'pipen-cli-require',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'A pipen cli plugin to check requirements for processes of a pipeline',
     'long_description': '# pipen-cli-require\n\nChecking the requirements for processes of a [pipen][1] pipeline\n\n## Install\n\n```shell\npip install -U pipen-cli-require\n```\n\n## Usage\n\n### Defining requirements of a process\n\n```python\n# example_pipeline.py\nfrom pipen import Pipen, Proc\n\nclass P1(Proc):\n    """Process 1\n\n    Requires:\n        pipen: Run `pip install -U pipen` to install\n          - check: |\n            {{proc.lang}} -c "import pipen"\n        liquidpy: Run `pip install -U liquidpy` to install\n          - check: |\n            {{proc.lang}} -c "import liquid"\n        nonexist: Run `pip install -U nonexist` to install\n          - check: |\n            {{proc.lang}} -c "import nonexist"\n        conditional:\n          - if: {{envs.require_conditional}}\n          - check:\n            {{proc.lang}} -c "import optional"\n\n    """\n    input = "a"\n    output = "outfile:file:out.txt"\n    envs = {"require_conditional": False}\n    lang = "python"\n\n# Setup the pipeline\n# Must be outside __main__\n# Or define a function to return the pipeline\nclass Pipeline(Pipen):\n    starts = P1\n\n\nif __name__ == \'__main__\':\n    # Pipeline must run with __main__\n    Pipeline().run()\n```\n\n### Parsing process requirements using API\n\n```python\nfrom pipen_cli_require import parse_proc_requirements\n\n\ndef parse_proc_requirements(\n    proc: Type[Proc]\n) -> Tuple[OrderedDiot, OrderedDiot]:\n    """Parse the requirements of a process\n\n    Args:\n        proc: The process class\n\n    Returns:\n        A tuple of two OrderedDiot\'s.\n        The first one is the annotated sections by pipen_annotate\n        The second one is the requirements. The key is the name of the\n            requirement, the value is a dict with message, check and if_ keys.\n    """\n```\n\n## Checking the requirements via the CLI\n\n```shell\n> pipen require --verbose --ncores 2 example_pipeline.py:pipeline\n\nChecking requirements for pipeline: PIPEN-0\n│\n└── P1: Process 1\n    ├── ✅ pipen\n    ├── ✅ liquidpy\n    ├── ❎ nonexist: Run `pip install -U nonexist` to install\n    │   └── Traceback (most recent call last):\n    │         File "<string>", line 1, in <module>\n    │       ModuleNotFoundError: No module named \'nonexist\'\n    │\n    └── ⏩ conditional (skipped by if-statement)\n```\n\n## Checking requirements with runtime arguments\n\nFor example, when I use a different python to run the pipeline:\n\nAdd this to the head of `example_pipeline.py`:\n\n```python\nimport pipen_args\n```\n\nSee also `tests/pipen_args_pipeline.py`\n\nThen specify the path of the python to use:\n\n```shell\npipen require example_pipeline.py:pipeline --P1.lang /path/to/another/python\n```\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_cli_require-0.6.0/PKG-INFO` & `pipen_cli_require-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pipen-cli-require
-Version: 0.6.0
+Version: 0.7.0
 Summary: A pipen cli plugin to check requirements for processes of a pipeline
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
-Requires-Dist: pipen-annotate (>=0.7,<0.8)
+Requires-Dist: pipen-annotate (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # pipen-cli-require
 
 Checking the requirements for processes of a [pipen][1] pipeline
 
 ## Install
```

