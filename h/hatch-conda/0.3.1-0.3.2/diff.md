# Comparing `tmp/hatch_conda-0.3.1.tar.gz` & `tmp/hatch_conda-0.3.2.tar.gz`

## Comparing `hatch_conda-0.3.1.tar` & `hatch_conda-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/.flake8
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/.gitattributes
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/HISTORY.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/hatch_conda/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/hatch_conda/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/hatch_conda/hooks.py
--rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/hatch_conda/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/tests/test_config.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/tests/utils.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/hatch.toml
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 hatch_conda-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.flake8
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.gitattributes
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/HISTORY.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/hooks.py
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/test_config.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/utils.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch.toml
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/PKG-INFO
```

### Comparing `hatch_conda-0.3.1/.github/workflows/build.yml` & `hatch_conda-0.3.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.1/.github/workflows/test.yml` & `hatch_conda-0.3.2/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
```

### Comparing `hatch_conda-0.3.1/hatch_conda/plugin.py` & `hatch_conda-0.3.2/hatch_conda/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,68 @@
 from __future__ import annotations
 
+import shutil
+import signal
 import sys
 from contextlib import contextmanager
+from types import FrameType
+from typing import Callable
 
+import pexpect
 from hatch.env.plugin.interface import EnvironmentInterface
 
 
+class ShellManager:
+    def __init__(self, environment: EnvironmentInterface):
+        self.environment = environment
+
+    def enter_bash(self, path: str, args: list[str], cmdl: str) -> None:
+        self.spawn_linux_shell(path or 'bash', args or ['-i'], cmdl)
+
+    def enter_zsh(self, path: str, args: list[str], cmdl: str) -> None:
+        self.spawn_linux_shell(path or 'zsh', args or ['-i'], cmdl)
+
+    def spawn_linux_shell(
+        self, path: str, args: list[str] | None = None, cmdl: str = '', callback: Callable | None = None
+    ) -> None:
+        columns, lines = shutil.get_terminal_size()
+        terminal = pexpect.spawn(path, args=args, dimensions=(lines, columns))
+
+        def sigwinch_passthrough(sig: int, data: FrameType | None) -> None:
+            new_columns, new_lines = shutil.get_terminal_size()
+            terminal.setwinsize(new_lines, new_columns)
+
+        signal.signal(signal.SIGWINCH, sigwinch_passthrough)
+
+        terminal.sendline(cmdl)
+
+        if callback is not None:
+            callback(terminal)
+
+        terminal.interact(escape_character=None)
+        terminal.close()
+
+        self.environment.platform.exit_with_code(terminal.exitstatus)
+
+
 class CondaEnvironment(EnvironmentInterface):
     PLUGIN_NAME = 'conda'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._config_command = None
         self._config_conda_forge = None
         self.__python_version = None
 
         self.conda_env_name = f'{self.metadata.core.name}_{self.name}_{self.python_version}'
         self.project_path = '.'
 
+        self.shells = ShellManager(self)
+
     @staticmethod
     def get_option_types():
         return {'command': str, 'conda-forge': bool}
 
     def _config_value(self, field_name, default, valid=None):
         class_name = f'_config_{field_name.replace("-", "_")}'
         if self.__dict__[class_name] is None:
@@ -148,18 +188,21 @@
                         command,
                     ]
                 )
             )
         )
 
     def enter_shell(self, name, path, args):  # no cov
-        with self:
+        cmdl = f'{self.config_command} activate {self.conda_env_name}'
+        shell_executor = getattr(self.shells, f'enter_{name}', None)
+        if shell_executor is None:
+            raise NotImplementedError(f'entering {name} shell in not supported yet')
+        else:
             self.apply_env_vars()
-            process = self.platform.run_command(' '.join([self.config_command, 'activate', self.conda_env_name]))
-            self.platform.exit_with_code(process.returncode)
+            shell_executor(path, args, cmdl)
 
     def apply_env_vars(self):
         env_vars = []
         for env_var, value in dict(self.env_vars).items():
             value_fixed = value
             if sys.platform == 'win32':
                 value_fixed = value_fixed.replace('%', '%%%%%%%%')
```

### Comparing `hatch_conda-0.3.1/tests/conftest.py` & `hatch_conda-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.1/tests/test_config.py` & `hatch_conda-0.3.2/tests/test_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,41 +10,66 @@
             isolation,
             config={
                 'project': {'name': 'my_app', 'version': '0.0.1'},
                 'tool': {'hatch': {'envs': {'default': env_config}}},
             },
         )
         environment = CondaEnvironment(
-            isolation, project.metadata, 'default', project.config.envs['default'], {}, data_dir, platform, 0
+            root=isolation,
+            metadata=project.metadata,
+            name='default',
+            config=project.config.envs['default'],
+            matrix_variables={},
+            data_directory=data_dir,
+            isolated_data_directory=None,
+            platform=platform,
+            verbosity=0,
         )
 
         assert environment.python_version == default_python_version
 
     def test_long(self, isolation, data_dir, platform):
         env_config = {'python': '3.10'}
         project = Project(
             isolation,
             config={
                 'project': {'name': 'my_app', 'version': '0.0.1'},
                 'tool': {'hatch': {'envs': {'default': env_config}}},
             },
         )
         environment = CondaEnvironment(
-            isolation, project.metadata, 'default', project.config.envs['default'], {}, data_dir, platform, 0
+            root=isolation,
+            metadata=project.metadata,
+            name='default',
+            config=project.config.envs['default'],
+            matrix_variables={},
+            data_directory=data_dir,
+            isolated_data_directory=None,
+            platform=platform,
+            verbosity=0,
         )
 
         assert environment.python_version == '3.10'
 
     def test_short(self, isolation, data_dir, platform):
         env_config = {'python': '310'}
         project = Project(
             isolation,
             config={
                 'project': {'name': 'my_app', 'version': '0.0.1'},
                 'tool': {'hatch': {'envs': {'default': env_config}}},
             },
         )
+
         environment = CondaEnvironment(
-            isolation, project.metadata, 'default', project.config.envs['default'], {}, data_dir, platform, 0
+            root=isolation,
+            metadata=project.metadata,
+            name='default',
+            config=project.config.envs['default'],
+            matrix_variables={},
+            data_directory=data_dir,
+            isolated_data_directory=None,
+            platform=platform,
+            verbosity=0,
         )
 
         assert environment.python_version == '3.10'
```

### Comparing `hatch_conda-0.3.1/tests/utils.py` & `hatch_conda-0.3.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.1/LICENSE.txt` & `hatch_conda-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.1/README.md` & `hatch_conda-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.1/hatch.toml` & `hatch_conda-0.3.2/hatch.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [envs.default]
 dependencies = [
   "coverage[toml]>=6.2",
   "pytest",
   "pytest-cov",
   "pytest-mock",
+  "tomli"
 ]
 
 [envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=hatch_containers --cov=tests"
 no-cov = "cov --no-cov"
 
 [envs.lint]
```

### Comparing `hatch_conda-0.3.1/pyproject.toml` & `hatch_conda-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,22 @@
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Framework :: Hatch",
 ]
 dependencies = [
   "hatch>=1.2.0",
+  "pexpect~=4.8",
 ]
 dynamic = ["version"]
 
 [project.urls]
 History = "https://github.com/OldGrumpyViking/hatch-conda/blob/master/HISTORY.md"
 Issues = "https://github.com/OldGrumpyViking/hatch-conda/issues"
 Source = "https://github.com/OldGrumpyViking/hatch-conda"
```

### Comparing `hatch_conda-0.3.1/PKG-INFO` & `hatch_conda-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: hatch-conda
-Version: 0.3.1
+Version: 0.3.2
 Summary: Hatch plugin for conda environments
 Project-URL: History, https://github.com/OldGrumpyViking/hatch-conda/blob/master/HISTORY.md
 Project-URL: Issues, https://github.com/OldGrumpyViking/hatch-conda/issues
 Project-URL: Source, https://github.com/OldGrumpyViking/hatch-conda
 Author-email: OldGrumpyViking <old.grumpy.viking@hotmail.com>
+License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: conda,environment,hatch,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: hatch>=1.2.0
+Requires-Dist: pexpect~=4.8
 Description-Content-Type: text/markdown
 
 # hatch-conda
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/OldGrumpyViking/hatch-conda/actions/workflows/test.yml/badge.svg)](https://github.com/OldGrumpyViking/hatch-conda/actions/workflows/test.yml) [![CD - Build](https://github.com/OldGrumpyViking/hatch-conda/actions/workflows/build.yml/badge.svg)](https://github.com/OldGrumpyViking/hatch-conda/actions/workflows/build.yml) |
```

