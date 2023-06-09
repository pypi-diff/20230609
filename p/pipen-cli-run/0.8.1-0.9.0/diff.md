# Comparing `tmp/pipen_cli_run-0.8.1.tar.gz` & `tmp/pipen_cli_run-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_cli_run-0.8.1.tar", max compression
+gzip compressed data, was "pipen_cli_run-0.9.0.tar", max compression
```

## Comparing `pipen_cli_run-0.8.1.tar` & `pipen_cli_run-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      312 2023-06-07 18:55:13.397328 pipen_cli_run-0.8.1/README.md
--rw-r--r--   0        0        0       83 2023-06-07 18:55:13.397328 pipen_cli_run-0.8.1/pipen_cli_run/__init__.py
--rw-r--r--   0        0        0     5714 2023-06-07 18:55:13.397328 pipen_cli_run-0.8.1/pipen_cli_run/entry.py
--rw-r--r--   0        0        0       46 2023-06-07 18:55:13.397328 pipen_cli_run-0.8.1/pipen_cli_run/version.py
--rw-r--r--   0        0        0     1336 2023-06-07 18:55:13.397328 pipen_cli_run-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 pipen_cli_run-0.8.1/setup.py
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 pipen_cli_run-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      312 2023-06-09 06:31:49.443677 pipen_cli_run-0.9.0/README.md
+-rw-r--r--   0        0        0       83 2023-06-09 06:31:49.443677 pipen_cli_run-0.9.0/pipen_cli_run/__init__.py
+-rw-r--r--   0        0        0     5714 2023-06-09 06:31:49.443677 pipen_cli_run-0.9.0/pipen_cli_run/entry.py
+-rw-r--r--   0        0        0       46 2023-06-09 06:31:49.443677 pipen_cli_run-0.9.0/pipen_cli_run/version.py
+-rw-r--r--   0        0        0     1336 2023-06-09 06:31:49.443677 pipen_cli_run-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 pipen_cli_run-0.9.0/setup.py
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 pipen_cli_run-0.9.0/PKG-INFO
```

### Comparing `pipen_cli_run-0.8.1/pipen_cli_run/entry.py` & `pipen_cli_run-0.9.0/pipen_cli_run/entry.py`

 * *Files identical despite different names*

### Comparing `pipen_cli_run-0.8.1/pyproject.toml` & `pipen_cli_run-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pipen-cli-run"
-version = "0.8.1"
+version = "0.9.0"
 description = "A pipen cli plugin to run a process or a pipeline"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-cli-run"
 repository = "https://github.com/pwwang/pipen-cli-run"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pipen-args = "^0.9.11"
+pipen-args = "^0.10.0"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
```

### Comparing `pipen_cli_run-0.8.1/setup.py` & `pipen_cli_run-0.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['pipen_cli_run']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pipen-args>=0.9.11,<0.10.0']
+['pipen-args>=0.10.0,<0.11.0']
 
 entry_points = \
 {'pipen_cli': ['cli-run = pipen_cli_run:PipenCliRunPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-cli-run',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'A pipen cli plugin to run a process or a pipeline',
     'long_description': '# pipen-cli-run\n\nA pipen cli plugin to run a process or a pipeline\n\n## Install\n\n```shell\npip install -U pipen-cli-run\n```\n\n## Usage\n\n### Register a namespace\n\n`pyproject.toml`\n```toml\n[tool.poetry.plugins.pipen_cli_run]\nns = "yourpackage.ns"\n```\n\n`ns` should be a module where you define you processes/pipelines\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-cli-run',
```

### Comparing `pipen_cli_run-0.8.1/PKG-INFO` & `pipen_cli_run-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-cli-run
-Version: 0.8.1
+Version: 0.9.0
 Summary: A pipen cli plugin to run a process or a pipeline
 Home-page: https://github.com/pwwang/pipen-cli-run
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
-Requires-Dist: pipen-args (>=0.9.11,<0.10.0)
+Requires-Dist: pipen-args (>=0.10.0,<0.11.0)
 Project-URL: Repository, https://github.com/pwwang/pipen-cli-run
 Description-Content-Type: text/markdown
 
 # pipen-cli-run
 
 A pipen cli plugin to run a process or a pipeline
```

