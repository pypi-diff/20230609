# Comparing `tmp/pipen_verbose-0.6.0.tar.gz` & `tmp/pipen_verbose-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_verbose-0.6.0.tar", max compression
+gzip compressed data, was "pipen_verbose-0.7.0.tar", max compression
```

## Comparing `pipen_verbose-0.6.0.tar` & `pipen_verbose-0.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     5398 2023-04-14 07:09:46.761085 pipen_verbose-0.6.0/README.md
--rwxr-xr-x   0        0        0     6266 2023-04-14 07:09:46.761085 pipen_verbose-0.6.0/pipen_verbose.py
--rwxr-xr-x   0        0        0     1130 2023-04-14 07:09:46.761085 pipen_verbose-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 pipen_verbose-0.6.0/setup.py
--rw-r--r--   0        0        0     6090 1970-01-01 00:00:00.000000 pipen_verbose-0.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0     5395 2023-06-08 23:35:31.978129 pipen_verbose-0.7.0/README.md
+-rwxr-xr-x   0        0        0     6266 2023-06-08 23:35:31.978129 pipen_verbose-0.7.0/pipen_verbose.py
+-rwxr-xr-x   0        0        0     1131 2023-06-08 23:35:31.978129 pipen_verbose-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 pipen_verbose-0.7.0/setup.py
+-rw-r--r--   0        0        0     6088 1970-01-01 00:00:00.000000 pipen_verbose-0.7.0/PKG-INFO
```

### Comparing `pipen_verbose-0.6.0/README.md` & `pipen_verbose-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 [09/12/21 22:57:01] I main
 [09/12/21 22:57:01] I main                                version: 0.1.0
 [09/12/21 22:57:01] I main
 [09/12/21 22:57:01] I main    ╭═════════════════════════════ PIPEN-0 ══════════════════════════════╮
 [09/12/21 22:57:01] I main    ║  # procs          = 1                                              ║
 [09/12/21 22:57:01] I main    ║  plugins          = ['main', 'verbose-0.0.1']                      ║
 [09/12/21 22:57:01] I main    ║  profile          = default                                        ║
-[09/12/21 22:57:01] I main    ║  outdir           = pipen-0_results                                ║
+[09/12/21 22:57:01] I main    ║  outdir           = ./Pipen-output                                 ║
 [09/12/21 22:57:01] I main    ║  cache            = True                                           ║
 [09/12/21 22:57:01] I main    ║  dirsig           = 1                                              ║
 [09/12/21 22:57:01] I main    ║  error_strategy   = ignore                                         ║
 [09/12/21 22:57:01] I main    ║  forks            = 1                                              ║
 [09/12/21 22:57:01] I main    ║  lang             = bash                                           ║
 [09/12/21 22:57:01] I main    ║  loglevel         = info                                           ║
 [09/12/21 22:57:01] I main    ║  num_retries      = 3                                              ║
@@ -77,13 +77,13 @@
 [09/12/21 22:57:02] I main    Process: Workdir: '.pipen/pipen-0/process'
 [09/12/21 22:57:02] I main    Process: <<< [START]
 [09/12/21 22:57:02] I main    Process: >>> [END]
 [09/12/21 22:57:02] I verbose Process: cache: False
 [09/12/21 22:57:02] I verbose Process: size : 10
 [09/12/21 22:57:02] I verbose Process: [0/9] in.a: 0
 [09/12/21 22:57:02] I verbose Process: [0/9] out.b:
-                      /home/pwwang/github/pipen-verbose/pipen-0_results/Process/0/a.txt
+                      /home/pwwang/github/pipen-verbose/Pipen-output/Process/0/a.txt
 [09/12/21 22:57:04] I verbose Process: Time elapsed: 00:00:02.043s
 [09/12/21 22:57:04] I main
 ```
 
 [1]: https://github.com/pwwang/pipen
```

### Comparing `pipen_verbose-0.6.0/pipen_verbose.py` & `pipen_verbose-0.7.0/pipen_verbose.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pipen import plugin
 from pipen.utils import get_logger, brief_list
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Proc
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 logger = get_logger("verbose", "info")
 
 VERBOSAL_CONFIGS = {
     # name: getter
     "scheduler": lambda proc: proc.scheduler.name,
     "lang": None,
```

### Comparing `pipen_verbose-0.6.0/pyproject.toml` & `pipen_verbose-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pipen-verbose"
-version = "0.6.0"
+version = "0.7.0"
 description = "Add verbosal information in logs for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-verbose"
 repository = "https://github.com/pwwang/pipen-verbose"
 
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

### Comparing `pipen_verbose-0.6.0/setup.py` & `pipen_verbose-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['pipen_verbose']
 install_requires = \
-['pipen>=0.9,<0.10']
+['pipen>=0.10,<0.11']
 
 entry_points = \
 {'pipen': ['verbose = pipen_verbose:PipenVerbose']}
 
 setup_kwargs = {
     'name': 'pipen-verbose',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Add verbosal information in logs for pipen.',
-    'long_description': '# pipen-verbose\n\nAdd verbosal information in logs for [pipen][1].\n\n## Additional information\n\n- Following process properties if not `None` and different from pipeline-level configurations: `scheduler`, `lang`, `forks`, `cache`, `dirsig`, `size`, `template`\n- Ellapsed time for a process. Note that this is time ellapsed from process initialization to completion, no matter the jobs are cached or not, so this is not the real running time for the jobs.\n- Process `envs` if set.\n- Computed input data for processes.\n- The indices of failed jobs if any.\n- The stderr, paths to script, stdout file, stderr file, of the first failed jobs if any.\n- The input/output data of the first job.\n\n## Installation\n\n```\npip install -U pipen-verbose\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:verbose"]`, or uninstall this plugin.\n\n## Usage\n\n`example.py`\n```python\nfrom pipen import Proc, Pipen\n\nclass Process(Proc):\n    input = \'a\'\n    input_data = range(10)\n    output = \'b:file:a.txt\'\n    cache = False\n    script = \'echo {{in.a}} > {{out.b}}\'\n\nPipen().run(Process)\n```\n\n```\n> python example.py\n[09/12/21 22:57:01] I main                   _____________________________________   __\n[09/12/21 22:57:01] I main                   ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/12/21 22:57:01] I main                   __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/12/21 22:57:01] I main                   _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/12/21 22:57:01] I main                   /_/     /___/  /_/     /_____/  /_/ |_/\n[09/12/21 22:57:01] I main\n[09/12/21 22:57:01] I main                                version: 0.1.0\n[09/12/21 22:57:01] I main\n[09/12/21 22:57:01] I main    ╭═════════════════════════════ PIPEN-0 ══════════════════════════════╮\n[09/12/21 22:57:01] I main    ║  # procs          = 1                                              ║\n[09/12/21 22:57:01] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                      ║\n[09/12/21 22:57:01] I main    ║  profile          = default                                        ║\n[09/12/21 22:57:01] I main    ║  outdir           = pipen-0_results                                ║\n[09/12/21 22:57:01] I main    ║  cache            = True                                           ║\n[09/12/21 22:57:01] I main    ║  dirsig           = 1                                              ║\n[09/12/21 22:57:01] I main    ║  error_strategy   = ignore                                         ║\n[09/12/21 22:57:01] I main    ║  forks            = 1                                              ║\n[09/12/21 22:57:01] I main    ║  lang             = bash                                           ║\n[09/12/21 22:57:01] I main    ║  loglevel         = info                                           ║\n[09/12/21 22:57:01] I main    ║  num_retries      = 3                                              ║\n[09/12/21 22:57:01] I main    ║  plugin_opts      = {}                                             ║\n[09/12/21 22:57:01] I main    ║  plugins          = None                                           ║\n[09/12/21 22:57:01] I main    ║  scheduler        = local                                          ║\n[09/12/21 22:57:01] I main    ║  scheduler_opts   = {}                                             ║\n[09/12/21 22:57:01] I main    ║  submission_batch = 8                                              ║\n[09/12/21 22:57:01] I main    ║  template         = liquid                                         ║\n[09/12/21 22:57:01] I main    ║  template_opts    = {}                                             ║\n[09/12/21 22:57:01] I main    ║  workdir          = ./.pipen                                       ║\n[09/12/21 22:57:01] I main    ╰════════════════════════════════════════════════════════════════════╯\n[09/12/21 22:57:02] I main\n[09/12/21 22:57:02] I main    ╭═════════════════════════════ Process ══════════════════════════════╮\n[09/12/21 22:57:02] I main    ║ Undescribed                                                        ║\n[09/12/21 22:57:02] I main    ╰════════════════════════════════════════════════════════════════════╯\n[09/12/21 22:57:02] I main    Process: Workdir: \'.pipen/pipen-0/process\'\n[09/12/21 22:57:02] I main    Process: <<< [START]\n[09/12/21 22:57:02] I main    Process: >>> [END]\n[09/12/21 22:57:02] I verbose Process: cache: False\n[09/12/21 22:57:02] I verbose Process: size : 10\n[09/12/21 22:57:02] I verbose Process: [0/9] in.a: 0\n[09/12/21 22:57:02] I verbose Process: [0/9] out.b:\n                      /home/pwwang/github/pipen-verbose/pipen-0_results/Process/0/a.txt\n[09/12/21 22:57:04] I verbose Process: Time elapsed: 00:00:02.043s\n[09/12/21 22:57:04] I main\n```\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-verbose\n\nAdd verbosal information in logs for [pipen][1].\n\n## Additional information\n\n- Following process properties if not `None` and different from pipeline-level configurations: `scheduler`, `lang`, `forks`, `cache`, `dirsig`, `size`, `template`\n- Ellapsed time for a process. Note that this is time ellapsed from process initialization to completion, no matter the jobs are cached or not, so this is not the real running time for the jobs.\n- Process `envs` if set.\n- Computed input data for processes.\n- The indices of failed jobs if any.\n- The stderr, paths to script, stdout file, stderr file, of the first failed jobs if any.\n- The input/output data of the first job.\n\n## Installation\n\n```\npip install -U pipen-verbose\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:verbose"]`, or uninstall this plugin.\n\n## Usage\n\n`example.py`\n```python\nfrom pipen import Proc, Pipen\n\nclass Process(Proc):\n    input = \'a\'\n    input_data = range(10)\n    output = \'b:file:a.txt\'\n    cache = False\n    script = \'echo {{in.a}} > {{out.b}}\'\n\nPipen().run(Process)\n```\n\n```\n> python example.py\n[09/12/21 22:57:01] I main                   _____________________________________   __\n[09/12/21 22:57:01] I main                   ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/12/21 22:57:01] I main                   __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/12/21 22:57:01] I main                   _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/12/21 22:57:01] I main                   /_/     /___/  /_/     /_____/  /_/ |_/\n[09/12/21 22:57:01] I main\n[09/12/21 22:57:01] I main                                version: 0.1.0\n[09/12/21 22:57:01] I main\n[09/12/21 22:57:01] I main    ╭═════════════════════════════ PIPEN-0 ══════════════════════════════╮\n[09/12/21 22:57:01] I main    ║  # procs          = 1                                              ║\n[09/12/21 22:57:01] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                      ║\n[09/12/21 22:57:01] I main    ║  profile          = default                                        ║\n[09/12/21 22:57:01] I main    ║  outdir           = ./Pipen-output                                 ║\n[09/12/21 22:57:01] I main    ║  cache            = True                                           ║\n[09/12/21 22:57:01] I main    ║  dirsig           = 1                                              ║\n[09/12/21 22:57:01] I main    ║  error_strategy   = ignore                                         ║\n[09/12/21 22:57:01] I main    ║  forks            = 1                                              ║\n[09/12/21 22:57:01] I main    ║  lang             = bash                                           ║\n[09/12/21 22:57:01] I main    ║  loglevel         = info                                           ║\n[09/12/21 22:57:01] I main    ║  num_retries      = 3                                              ║\n[09/12/21 22:57:01] I main    ║  plugin_opts      = {}                                             ║\n[09/12/21 22:57:01] I main    ║  plugins          = None                                           ║\n[09/12/21 22:57:01] I main    ║  scheduler        = local                                          ║\n[09/12/21 22:57:01] I main    ║  scheduler_opts   = {}                                             ║\n[09/12/21 22:57:01] I main    ║  submission_batch = 8                                              ║\n[09/12/21 22:57:01] I main    ║  template         = liquid                                         ║\n[09/12/21 22:57:01] I main    ║  template_opts    = {}                                             ║\n[09/12/21 22:57:01] I main    ║  workdir          = ./.pipen                                       ║\n[09/12/21 22:57:01] I main    ╰════════════════════════════════════════════════════════════════════╯\n[09/12/21 22:57:02] I main\n[09/12/21 22:57:02] I main    ╭═════════════════════════════ Process ══════════════════════════════╮\n[09/12/21 22:57:02] I main    ║ Undescribed                                                        ║\n[09/12/21 22:57:02] I main    ╰════════════════════════════════════════════════════════════════════╯\n[09/12/21 22:57:02] I main    Process: Workdir: \'.pipen/pipen-0/process\'\n[09/12/21 22:57:02] I main    Process: <<< [START]\n[09/12/21 22:57:02] I main    Process: >>> [END]\n[09/12/21 22:57:02] I verbose Process: cache: False\n[09/12/21 22:57:02] I verbose Process: size : 10\n[09/12/21 22:57:02] I verbose Process: [0/9] in.a: 0\n[09/12/21 22:57:02] I verbose Process: [0/9] out.b:\n                      /home/pwwang/github/pipen-verbose/Pipen-output/Process/0/a.txt\n[09/12/21 22:57:04] I verbose Process: Time elapsed: 00:00:02.043s\n[09/12/21 22:57:04] I main\n```\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-verbose',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `pipen_verbose-0.6.0/PKG-INFO` & `pipen_verbose-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-verbose
-Version: 0.6.0
+Version: 0.7.0
 Summary: Add verbosal information in logs for pipen.
 Home-page: https://github.com/pwwang/pipen-verbose
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
 Project-URL: Repository, https://github.com/pwwang/pipen-verbose
 Description-Content-Type: text/markdown
 
 # pipen-verbose
 
 Add verbosal information in logs for [pipen][1].
 
@@ -68,15 +68,15 @@
 [09/12/21 22:57:01] I main
 [09/12/21 22:57:01] I main                                version: 0.1.0
 [09/12/21 22:57:01] I main
 [09/12/21 22:57:01] I main    ╭═════════════════════════════ PIPEN-0 ══════════════════════════════╮
 [09/12/21 22:57:01] I main    ║  # procs          = 1                                              ║
 [09/12/21 22:57:01] I main    ║  plugins          = ['main', 'verbose-0.0.1']                      ║
 [09/12/21 22:57:01] I main    ║  profile          = default                                        ║
-[09/12/21 22:57:01] I main    ║  outdir           = pipen-0_results                                ║
+[09/12/21 22:57:01] I main    ║  outdir           = ./Pipen-output                                 ║
 [09/12/21 22:57:01] I main    ║  cache            = True                                           ║
 [09/12/21 22:57:01] I main    ║  dirsig           = 1                                              ║
 [09/12/21 22:57:01] I main    ║  error_strategy   = ignore                                         ║
 [09/12/21 22:57:01] I main    ║  forks            = 1                                              ║
 [09/12/21 22:57:01] I main    ║  lang             = bash                                           ║
 [09/12/21 22:57:01] I main    ║  loglevel         = info                                           ║
 [09/12/21 22:57:01] I main    ║  num_retries      = 3                                              ║
@@ -96,14 +96,14 @@
 [09/12/21 22:57:02] I main    Process: Workdir: '.pipen/pipen-0/process'
 [09/12/21 22:57:02] I main    Process: <<< [START]
 [09/12/21 22:57:02] I main    Process: >>> [END]
 [09/12/21 22:57:02] I verbose Process: cache: False
 [09/12/21 22:57:02] I verbose Process: size : 10
 [09/12/21 22:57:02] I verbose Process: [0/9] in.a: 0
 [09/12/21 22:57:02] I verbose Process: [0/9] out.b:
-                      /home/pwwang/github/pipen-verbose/pipen-0_results/Process/0/a.txt
+                      /home/pwwang/github/pipen-verbose/Pipen-output/Process/0/a.txt
 [09/12/21 22:57:04] I verbose Process: Time elapsed: 00:00:02.043s
 [09/12/21 22:57:04] I main
 ```
 
 [1]: https://github.com/pwwang/pipen
```

