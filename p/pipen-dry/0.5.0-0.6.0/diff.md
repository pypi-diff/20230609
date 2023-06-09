# Comparing `tmp/pipen_dry-0.5.0.tar.gz` & `tmp/pipen_dry-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_dry-0.5.0.tar", max compression
+gzip compressed data, was "pipen_dry-0.6.0.tar", max compression
```

## Comparing `pipen_dry-0.5.0.tar` & `pipen_dry-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      416 2023-04-15 03:45:37.241097 pipen_dry-0.5.0/README.md
--rw-r--r--   0        0        0     2711 2023-04-15 03:45:37.241097 pipen_dry-0.5.0/pipen_dry.py
--rw-r--r--   0        0        0      628 2023-04-15 03:45:37.241097 pipen_dry-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 pipen_dry-0.5.0/setup.py
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pipen_dry-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      416 2023-06-09 06:34:54.108463 pipen_dry-0.6.0/README.md
+-rw-r--r--   0        0        0     2713 2023-06-09 06:34:54.108463 pipen_dry-0.6.0/pipen_dry.py
+-rw-r--r--   0        0        0      629 2023-06-09 06:34:54.108463 pipen_dry-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 pipen_dry-0.6.0/setup.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 pipen_dry-0.6.0/PKG-INFO
```

### Comparing `pipen_dry-0.5.0/pipen_dry.py` & `pipen_dry-0.6.0/pipen_dry.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pipen.defaults import ProcOutputType
 from pipen.utils import get_logger
 
 if TYPE_CHECKING:
     from pipen import Proc
 
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 SCHEDULER_NAME = "dry"
 
 logger = get_logger("dry", "info")
 
 
 class DryJob(Job):
@@ -69,15 +69,15 @@
 
 class PipenDry:
     """Implement some hooks to modify settings and print information"""
 
     version = __version__
 
     @plugin.impl
-    def on_proc_init(self, proc: Proc) -> None:
+    def on_proc_create(self, proc: Proc) -> None:
         """Modify the workdir of the process and set cache/export to False"""
         sched = get_scheduler(
             proc.scheduler or proc.pipeline.config.scheduler
         )
 
         if sched.name != SCHEDULER_NAME:
             return
```

### Comparing `pipen_dry-0.5.0/pyproject.toml` & `pipen_dry-0.6.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pipen-dry"
-version = "0.5.0"
+version = "0.6.0"
 description = "Dry runner for pipen pipelines"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pipen = "^0.9"
+pipen = "^0.10"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.plugins.pipen_sched]
```

### Comparing `pipen_dry-0.5.0/setup.py` & `pipen_dry-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['pipen_dry']
 install_requires = \
-['pipen>=0.9,<0.10']
+['pipen>=0.10,<0.11']
 
 entry_points = \
 {'pipen': ['dry = pipen_dry:PipenDry'],
  'pipen_sched': ['dry = pipen_dry:PipenDryScheduler']}
 
 setup_kwargs = {
     'name': 'pipen-dry',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Dry runner for pipen pipelines',
     'long_description': '# pipen-dry\n\nDry runner for [pipen][1]\n\nIt is useful to quickly check if there are misconfigurations for your pipeline without actually running it.\n\n## Install\n\n```shell\npip install -U pipen-dry\n```\n\n## Usage\n\n- Use it for process\n\n    ```python\n    class P1(Proc):\n        scheduler = "dry"\n    ```\n\n- Use it for pipeline\n\n    ```python\n    Pipen(scheduler="dry", ...)\n    ```\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_dry-0.5.0/PKG-INFO` & `pipen_dry-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pipen-dry
-Version: 0.5.0
+Version: 0.6.0
 Summary: Dry runner for pipen pipelines
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
 Description-Content-Type: text/markdown
 
 # pipen-dry
 
 Dry runner for [pipen][1]
 
 It is useful to quickly check if there are misconfigurations for your pipeline without actually running it.
```

