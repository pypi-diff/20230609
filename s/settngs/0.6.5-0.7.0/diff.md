# Comparing `tmp/settngs-0.6.5.tar.gz` & `tmp/settngs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settngs-0.6.5.tar", last modified: Wed Apr 26 22:34:48 2023, max compression
+gzip compressed data, was "settngs-0.7.0.tar", last modified: Fri Jun  9 06:04:07 2023, max compression
```

## Comparing `settngs-0.6.5.tar` & `settngs-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.051508 settngs-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-26 22:34:34.000000 settngs-0.6.5/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-26 22:34:34.000000 settngs-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 22:34:34.000000 settngs-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-26 22:34:34.000000 settngs-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-26 22:34:48.055508 settngs-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-26 22:34:34.000000 settngs-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 22:34:34.000000 settngs-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:34:34.000000 settngs-0.6.5/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/settngs/
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-04-26 22:34:34.000000 settngs-0.6.5/settngs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 22:34:34.000000 settngs-0.6.5/settngs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:34.000000 settngs-0.6.5/settngs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/settngs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-26 22:34:48.055508 settngs-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 22:34:34.000000 settngs-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:34.000000 settngs-0.6.5/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-26 22:34:34.000000 settngs-0.6.5/testing/settngs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:34.000000 settngs-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-04-26 22:34:34.000000 settngs-0.6.5/tests/settngs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-26 22:34:34.000000 settngs-0.6.5/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-26 22:34:34.000000 settngs-0.6.5/workflows/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.426365 settngs-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.418365 settngs-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-09 06:03:46.000000 settngs-0.7.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 06:03:46.000000 settngs-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-09 06:03:46.000000 settngs-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-09 06:03:46.000000 settngs-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 06:04:07.426365 settngs-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-09 06:03:46.000000 settngs-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-09 06:03:46.000000 settngs-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:03:46.000000 settngs-0.7.0/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/settngs/
+-rw-r--r--   0 runner    (1001) docker     (123)    33397 2023-06-09 06:03:46.000000 settngs-0.7.0/settngs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 06:03:46.000000 settngs-0.7.0/settngs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:03:46.000000 settngs-0.7.0/settngs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/settngs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 06:04:07.000000 settngs-0.7.0/settngs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-09 06:04:07.426365 settngs-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 06:03:46.000000 settngs-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.422365 settngs-0.7.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:03:46.000000 settngs-0.7.0/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-06-09 06:03:46.000000 settngs-0.7.0/testing/settngs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.426365 settngs-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:03:46.000000 settngs-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-06-09 06:03:46.000000 settngs-0.7.0/tests/settngs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:04:07.426365 settngs-0.7.0/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-09 06:03:46.000000 settngs-0.7.0/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-09 06:03:46.000000 settngs-0.7.0/workflows/package.yaml
```

### Comparing `settngs-0.6.5/.github/workflows/build.yaml` & `settngs-0.7.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.6.5/.gitignore` & `settngs-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `settngs-0.6.5/.pre-commit-config.yaml` & `settngs-0.7.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,42 +6,42 @@
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: debug-statements
     -   id: double-quote-string-fixer
     -   id: name-tests-test
     -   id: requirements-txt-fixer
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
     -   id: setup-cfg-fmt
--   repo: https://github.com/asottile/reorder_python_imports
+-   repo: https://github.com/asottile/reorder-python-imports
     rev: v3.9.0
     hooks:
     -   id: reorder-python-imports
         args: [--py38-plus, --add-import, 'from __future__ import annotations']
 -   repo: https://github.com/asottile/add-trailing-comma
     rev: v2.4.0
     hooks:
     -   id: add-trailing-comma
         args: [--py36-plus]
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.0
+    rev: v1.5.1
     hooks:
     -   id: dead
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pre-commit/mirrors-autopep8
     rev: v2.0.2
     hooks:
     -   id: autopep8
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
         additional_dependencies: [flake8-encodings, flake8-warnings, flake8-builtins, flake8-length, flake8-print]
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
     -   id: mypy
```

### Comparing `settngs-0.6.5/LICENSE` & `settngs-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `settngs-0.6.5/PKG-INFO` & `settngs-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.6.5
+Version: 0.7.0
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.6.5/README.md` & `settngs-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `settngs-0.6.5/settngs/__init__.py` & `settngs-0.7.0/settngs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 
 import argparse
 import json
 import logging
 import pathlib
 import re
 import sys
+import typing
 from argparse import Namespace
 from collections import defaultdict
 from collections.abc import Sequence
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Generic
+from typing import Literal
 from typing import NoReturn
-from typing import overload
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
+
 logger = logging.getLogger(__name__)
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import NamedTuple
 else:  # pragma: no cover
     from typing import NamedTuple
 
 
 if sys.version_info < (3, 9):  # pragma: no cover
+    from typing import List
+    from typing import _GenericAlias as types_GenericAlias
+
     def removeprefix(self: str, prefix: str, /) -> str:
         if self.startswith(prefix):
             return self[len(prefix):]
         else:
             return self[:]
 
     class BooleanOptionalAction(argparse.Action):
@@ -69,27 +74,29 @@
                 metavar=metavar,
             )
 
         def __call__(self, parser, namespace, values, option_string=None):  # dead: disable
             if option_string in self.option_strings:
                 setattr(namespace, self.dest, not option_string.startswith('--no-'))
 else:  # pragma: no cover
+    List = list
+    from types import GenericAlias as types_GenericAlias
     from argparse import BooleanOptionalAction
     removeprefix = str.removeprefix
 
 
 class Setting:
     def __init__(
         self,
         # From argparse
         *names: str,
-        action: type[argparse.Action] | None = None,
+        action: type[argparse.Action] | str | None = None,
         nargs: str | int | None = None,
-        const: str | None = None,
-        default: str | None = None,
+        const: Any | None = None,
+        default: Any | None = None,
         type: Callable[..., Any] | None = None,  # noqa: A002
         choices: Sequence[Any] | None = None,
         required: bool | None = None,
         help: str | None = None,  # noqa: A002
         metavar: str | None = None,
         dest: str | None = None,
         # ComicTagger
@@ -107,15 +114,15 @@
             nargs:        Passed directly to argparse
             const:        Passed directly to argparse
             default:      Passed directly to argparse
             type:         Passed directly to argparse
             choices:      Passed directly to argparse
             required:     Passed directly to argparse
             help:         Passed directly to argparse
-            metavar:      Passed directly to argparse, defaults to `dest` uppercased
+            metavar:      Passed directly to argparse, defaults to `dest` upper-cased
             dest:         This is the name used to retrieve the value from a `Config` object as a dictionary
             display_name: This is not used by settngs. This is a human-readable name to be used when generating a GUI.
                           Defaults to `dest`.
             cmdline:      If this setting can be set via the commandline
             file:         If this setting can be set via a file
             group:        The group this option is in.
                           This is an internal argument and should only be set by settngs
@@ -176,14 +183,53 @@
         return self.__str__()
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Setting):
             return NotImplemented
         return self.__dict__ == other.__dict__
 
+    def _guess_type(self) -> type | Literal['Any'] | None:
+        if self.type is None and self.action is None:
+            if self.cmdline:
+                return str
+            else:
+                if not self.cmdline and self.default is not None:
+                    return type(self.default)
+                return 'Any'
+
+        if isinstance(self.type, type):
+            return self.type
+
+        if self.type is not None:
+            type_hints = typing.get_type_hints(self.type)
+            if 'return' in type_hints and isinstance(type_hints['return'], type):
+                return type_hints['return']
+            if self.default is not None:
+                return type(self.default)
+            return 'Any'
+
+        if self.action in ('store_true', 'store_false', BooleanOptionalAction):
+            return bool
+
+        if self.action in ('store_const',):
+            return type(self.const)
+
+        if self.action in ('count',):
+            return int
+
+        if self.action in ('append', 'extend'):
+            return List[str]
+
+        if self.action in ('append_const',):
+            return list  # list[type(self.const)]
+
+        if self.action in ('help', 'version'):
+            return None
+        return 'Any'
+
     def get_dest(self, prefix: str, names: Sequence[str], dest: str | None) -> tuple[str, str, bool]:
         dest_name = None
         flag = False
 
         for n in names:
             if n.startswith('--'):
                 flag = True
@@ -226,224 +272,274 @@
 
 
 if TYPE_CHECKING:
     ArgParser = Union[argparse._MutuallyExclusiveGroup, argparse._ArgumentGroup, argparse.ArgumentParser]
     ns = Namespace | Config[T] | None
 
 
+def generate_ns(definitions: Definitions) -> str:
+    imports = ['from __future__ import annotations', 'import typing', 'import settngs']
+    ns = 'class settngs_namespace(settngs.Namespace):\n'
+    types = []
+    for group_name, group in definitions.items():
+        for setting_name, setting in group.v.items():
+            t = setting._guess_type()
+            if t is None:
+                continue
+            type_name = 'Any'
+            if isinstance(t, str):
+                type_name = t
+            elif type(t) == types_GenericAlias:
+                type_name = str(t)
+            elif isinstance(t, type):
+                type_name = t.__name__
+                if t.__module__ != 'builtins':
+                    imports.append(f'import {t.__module__}')
+                    type_name = t.__module__ + '.' + type_name
+            if type_name == 'Any':
+                type_name = 'typing.Any'
+
+            types.append(f'    {setting.internal_name}: {type_name}')
+        if types and types[-1] != '':
+            types.append('')
+
+    if not types or all(x == '' for x in types):
+        ns += '    ...\n'
+        types = ['']
+
+    return '\n'.join(imports) + '\n\n' + ns + '\n'.join(types)
+
+
 def sanitize_name(name: str) -> str:
     return re.sub('[' + re.escape(' -_,.!@#$%^&*(){}[]\',."<>;:') + ']+', '_', name).strip('_')
 
 
 def get_option(options: Values | Namespace, setting: Setting) -> tuple[Any, bool]:
     """
-    Helper function to retrieve the value for a setting and if the value is the default value
+    Helper function to retrieve the value for a setting and if the current value is the default value
 
     Args:
         options: Dictionary or namespace of options
         setting: The setting object describing the value to retrieve
     """
     if isinstance(options, dict):
         value = options.get(setting.group, {}).get(setting.dest, setting.default)
     else:
         value = getattr(options, setting.internal_name, setting.default)
     return value, value == setting.default
 
 
-def get_options(options: Config[T], group: str) -> dict[str, Any]:
+def get_options(config: Config[T], group: str) -> dict[str, Any]:
     """
     Helper function to retrieve all of the values for a group. Only to be used on persistent groups.
 
     Args:
-        options: Dictionary or namespace of options
+        config: Dictionary or namespace of options
         group: The name of the group to retrieve
     """
-    if isinstance(options[0], dict):
-        values = options[0].get(group, {}).copy()
+    if isinstance(config[0], dict):
+        values = config[0].get(group, {}).copy()
     else:
-        internal_names = {x.internal_name: x for x in options[1][group].v.values()}
+        internal_names = {x.internal_name: x for x in config[1][group].v.values()}
         values = {}
-        v = vars(options[0])
+        v = vars(config[0])
         for name, value in v.items():
             if name.startswith(f'{group}_'):
                 if name in internal_names:
                     values[internal_names[name].dest] = value
                 else:
                     values[removeprefix(name, f'{group}_')] = value
 
     return values
 
 
 def normalize_config(
     config: Config[T],
     file: bool = False,
     cmdline: bool = False,
-    defaults: bool = True,
+    default: bool = True,
     persistent: bool = True,
 ) -> Config[Values]:
     """
     Creates an `OptionValues` dictionary with setting definitions taken from `self.definitions`
     and values taken from `raw_options` and `raw_options_2' if defined.
     Values are assigned so if the value is a dictionary mutating it will mutate the original.
 
     Args:
-        raw_options: The dict or Namespace to normalize options from
-        definitions: The definition of the options
+        config: The Config object to normalize options from
         file: Include file options
         cmdline: Include cmdline options
-        defaults: Include default values in the returned dict
+        default: Include default values in the returned Config object
         persistent: Include unknown keys in persistent groups
     """
 
+    if not file and not cmdline:
+        raise ValueError('Invalid parameters: you must set either file or cmdline to True')
+
     normalized: Values = {}
     options, definitions = config
     for group_name, group in definitions.items():
         group_options = {}
         if group.persistent and persistent:
             group_options = get_options(config, group_name)
         for setting_name, setting in group.v.items():
             if (setting.cmdline and cmdline) or (setting.file and file):
                 # Ensures the option exists with the default if not already set
-                value, default = get_option(options, setting)
-                if not default or (default and defaults):
+                value, is_default = get_option(options, setting)
+                if not is_default or default:
                     # User has set a custom value or has requested the default value
                     group_options[setting_name] = value
                 elif setting_name in group_options:
-                    # defaults have been requested to be removed
+                    # default values have been requested to be removed
                     del group_options[setting_name]
             elif setting_name in group_options:
                 # Setting type (file or cmdline) has not been requested and should be removed for persistent groups
                 del group_options[setting_name]
         normalized[group_name] = group_options
     return Config(normalized, definitions)
 
 
 def parse_file(definitions: Definitions, filename: pathlib.Path) -> tuple[Config[Values], bool]:
     """
-    Helper function to read options from a json dictionary from a file
+    Helper function to read options from a json dictionary from a file.
+    This is purely a convenience function.
+    If _anything_ more advanced is desired this should be handled by the application.
+
     Args:
+        definitions: A set of setting definitions. See `Config.definitions` and `Manager.definitions`
         filename: A pathlib.Path object to read a json dictionary from
     """
     options: Values = {}
     success = True
     if filename.exists():
         try:
             with filename.open() as file:
                 opts = json.load(file)
             if isinstance(opts, dict):
                 options = opts
-        except Exception:
+            else:  # pragma: no cover
+                raise Exception('Loaded file is not a JSON Dictionary')
+        except Exception:  # pragma: no cover
             logger.exception('Failed to load config file: %s', filename)
             success = False
     else:
         logger.info('No config file found')
         success = True
 
-    return (normalize_config(Config(options, definitions), file=True), success)
+    return normalize_config(Config(options, definitions), file=True), success
 
 
 def clean_config(
-    config: Config[T], file: bool = False, cmdline: bool = False,
+    config: Config[T], file: bool = False, cmdline: bool = False, default: bool = True, persistent: bool = True,
 ) -> Values:
     """
-    Normalizes options and then cleans up empty groups
+    Normalizes options and then cleans up empty groups. The returned value is probably JSON serializable.
     Args:
-        options:
-        file:
-        cmdline:
-
-    Returns:
-
+        config: The Config object to normalize options from
+        file: Include file options
+        cmdline: Include cmdline options
+        default: Include default values in the returned Config object
+        persistent: Include unknown keys in persistent groups
     """
 
-    clean_options, definitions = normalize_config(config, file=file, cmdline=cmdline)
-    for group in list(clean_options.keys()):
-        if not clean_options[group]:
-            del clean_options[group]
-    return clean_options
+    cleaned, _ = normalize_config(config, file=file, cmdline=cmdline, default=default, persistent=persistent)
+    for group in list(cleaned.keys()):
+        if not cleaned[group]:
+            del cleaned[group]
+    return cleaned
 
 
 def defaults(definitions: Definitions) -> Config[Values]:
     return normalize_config(Config(Namespace(), definitions), file=True, cmdline=True)
 
 
-def get_namespace(config: Config[T], defaults: bool = True, persistent: bool = True) -> Config[Namespace]:
+def get_namespace(
+    config: Config[T], file: bool = False, cmdline: bool = False, default: bool = True, persistent: bool = True,
+) -> Config[Namespace]:
     """
-    Returns an Namespace object with options in the form "{group_name}_{setting_name}"
-    `options` should already be normalized.
-    Throws an exception if the internal_name is duplicated
+    Returns a Namespace object with options in the form "{group_name}_{setting_name}"
+    `config` should already be normalized or be a `Config[Namespace]`.
 
     Args:
-        options: Normalized options to turn into a Namespace
-        defaults: Include default values in the returned dict
+        config: The Config object to turn into a namespace
+        file: Include file options
+        cmdline: Include cmdline options
+        default: Include default values in the returned Config object
         persistent: Include unknown keys in persistent groups
     """
 
+    if not file and not cmdline:
+        raise ValueError('Invalid parameters: you must set either file or cmdline to True')
+
     if isinstance(config.values, Namespace):
-        options, definitions = normalize_config(config, True, True, defaults=defaults, persistent=persistent)
+        cfg = normalize_config(config, file=file, cmdline=cmdline, default=default, persistent=persistent)
+        options, definitions = cfg
     else:
         options, definitions = config
     namespace = Namespace()
     for group_name, group in definitions.items():
+
+        group_options = get_options(config, group_name)
         if group.persistent and persistent:
-            group_options = get_options(config, group_name)
             for name, value in group_options.items():
                 if name in group.v:
-                    internal_name, default = group.v[name].internal_name, group.v[name].default == value
+                    setting_file, setting_cmdline = group.v[name].file, group.v[name].cmdline
+                    value, is_default = get_option(options, group.v[name])
+                    internal_name = group.v[name].internal_name
                 else:
-                    internal_name, default = f'{group_name}_' + sanitize_name(name), None
+                    setting_file = setting_cmdline = True
+                    internal_name, is_default = f'{group_name}_' + sanitize_name(name), None
 
-                if hasattr(namespace, internal_name):
-                    raise Exception(f'Duplicate internal name: {internal_name}')
-
-                if not default or default and defaults:
+                if ((setting_cmdline and cmdline) or (setting_file and file)) and (not is_default or default):
                     setattr(namespace, internal_name, value)
 
-        else:
-            for setting_name, setting in group.v.items():
-                if hasattr(namespace, setting.internal_name):
-                    raise Exception(f'Duplicate internal name: {setting.internal_name}')
-                value, default = get_option(options, setting)
+        for setting in group.v.values():
+            if (setting.cmdline and cmdline) or (setting.file and file):
+                value, is_default = get_option(options, setting)
 
-                if not default or default and defaults:
+                if not is_default or default:
+                    # User has set a custom value or has requested the default value
                     setattr(namespace, setting.internal_name, value)
     return Config(namespace, definitions)
 
 
 def save_file(
     config: Config[T], filename: pathlib.Path,
 ) -> bool:
     """
     Helper function to save options from a json dictionary to a file
+    This is purely a convenience function.
+    If _anything_ more advanced is desired this should be handled by the application.
+
     Args:
-        options: The options to save to a json dictionary
+        config: The options to save to a json dictionary
         filename: A pathlib.Path object to save the json dictionary to
     """
     file_options = clean_config(config, file=True)
-    if not filename.exists():
-        filename.parent.mkdir(exist_ok=True, parents=True)
-        filename.touch()
-
     try:
+        if not filename.exists():
+            filename.parent.mkdir(exist_ok=True, parents=True)
+            filename.touch()
+
         json_str = json.dumps(file_options, indent=2)
         filename.write_text(json_str + '\n', encoding='utf-8')
     except Exception:
         logger.exception('Failed to save config file: %s', filename)
         return False
     return True
 
 
 def create_argparser(definitions: Definitions, description: str, epilog: str) -> argparse.ArgumentParser:
     """Creates an :class:`argparse.ArgumentParser` from all cmdline settings"""
     groups: dict[str, ArgParser] = {}
     argparser = argparse.ArgumentParser(
         description=description, epilog=epilog, formatter_class=argparse.RawTextHelpFormatter,
     )
-    for group_name, group in definitions.items():
-        for setting_name, setting in group.v.items():
+    for group in definitions.values():
+        for setting in group.v.values():
             if setting.cmdline:
                 argparse_args, argparse_kwargs = setting.to_argparse()
                 current_group: ArgParser = argparser
                 if setting.group:
                     if setting.group not in groups:
                         if setting.exclusive:
                             groups[setting.group] = argparser.add_argument_group(
@@ -467,23 +563,26 @@
     config: ns[T] = None,
 ) -> Config[Values]:
     """
     Creates an `argparse.ArgumentParser` from cmdline settings in `self.definitions`.
     `args` and `namespace` are passed to `argparse.ArgumentParser.parse_args`
 
     Args:
-        args: Passed to argparse.ArgumentParser.parse
-        namespace: Passed to argparse.ArgumentParser.parse
+        definitions: A set of setting definitions. See `Config.definitions` and `Manager.definitions`
+        description: Passed to argparse.ArgumentParser
+        epilog: Passed to argparse.ArgumentParser
+        args: Passed to argparse.ArgumentParser.parse_args
+        config: The Config or Namespace object to use as a Namespace passed to argparse.ArgumentParser.parse_args
     """
     namespace = None
     if isinstance(config, Config):
         if isinstance(config.values, Namespace):
             namespace = config.values
         else:
-            namespace = get_namespace(config, defaults=False)[0]
+            namespace = get_namespace(config, file=True, cmdline=True, default=False)[0]
     else:
         namespace = config
     argparser = create_argparser(definitions, description, epilog)
     ns = argparser.parse_args(args, namespace=namespace)
 
     return normalize_config(Config(ns, definitions), cmdline=True, file=True)
 
@@ -491,21 +590,33 @@
 def parse_config(
     definitions: Definitions,
     description: str,
     epilog: str,
     config_path: pathlib.Path,
     args: list[str] | None = None,
 ) -> tuple[Config[Values], bool]:
+    """
+    Convenience function to parse options from a json file and passes the resulting Config object to parse_cmdline.
+    This is purely a convenience function.
+    If _anything_ more advanced is desired this should be handled by the application.
+
+    Args:
+        definitions: A set of setting definitions. See `Config.definitions` and `Manager.definitions`
+        description: Passed to argparse.ArgumentParser
+        epilog: Passed to argparse.ArgumentParser
+        config_path: A `pathlib.Path` object
+        args: Passed to argparse.ArgumentParser.parse_args
+    """
     file_options, success = parse_file(definitions, config_path)
     cmdline_options = parse_cmdline(
-        definitions, description, epilog, args, get_namespace(file_options, defaults=False),
+        definitions, description, epilog, args, file_options,
     )
 
     final_options = normalize_config(cmdline_options, file=True, cmdline=True)
-    return (final_options, success)
+    return final_options, success
 
 
 class Manager:
     """docstring for Manager"""
 
     def __init__(self, description: str = '', epilog: str = '', definitions: Definitions | Config[T] | None = None):
         # This one is never used, it just makes MyPy happy
@@ -517,19 +628,22 @@
             self.definitions = definitions.definitions
         else:
             self.definitions = defaultdict(lambda: Group(False, {}), definitions or {})
 
         self.exclusive_group = False
         self.current_group_name = ''
 
+    def generate_ns(self) -> str:
+        return generate_ns(self.definitions)
+
     def create_argparser(self) -> None:
         self.argparser = create_argparser(self.definitions, self.description, self.epilog)
 
     def add_setting(self, *args: Any, **kwargs: Any) -> None:
-        """Takes passes all arguments through to `Setting`, `group` and `exclusive` are already set"""
+        """Passes all arguments through to `Setting`, `group` and `exclusive` are already set"""
         setting = Setting(*args, **kwargs, group=self.current_group_name, exclusive=self.exclusive_group)
         self.definitions[self.current_group_name].v[setting.dest] = setting
 
     def add_group(self, name: str, group: Callable[[Manager], None], exclusive_group: bool = False) -> None:
         """
         The primary way to add define options on this class.
 
@@ -558,15 +672,15 @@
         """
         if self.current_group_name != '':
             raise ValueError('Sub groups are not allowed')
         self.current_group_name = name
         self.exclusive_group = exclusive_group
         if self.current_group_name in self.definitions:
             if not self.definitions[self.current_group_name].persistent:
-                raise ValueError('Group already existis and is not persistent')
+                raise ValueError('Group already exists and is not persistent')
         else:
             self.definitions[self.current_group_name] = Group(True, {})
         group(self)
         self.current_group_name = ''
         self.exclusive_group = False
 
     def exit(self, *args: Any, **kwargs: Any) -> NoReturn:
@@ -574,71 +688,159 @@
         self.argparser.exit(*args, **kwargs)
         raise SystemExit(99)
 
     def defaults(self) -> Config[Values]:
         return defaults(self.definitions)
 
     def clean_config(
-        self, options: T | Config[T], file: bool = False, cmdline: bool = False,
+        self, config: T | Config[T], file: bool = False, cmdline: bool = False,
     ) -> Values:
-        if isinstance(options, Config):
-            config = options
-        else:
-            config = Config(options, self.definitions)
+        """
+        Normalizes options and then cleans up empty groups. The returned value is probably JSON serializable.
+        Args:
+            config: The Config object to normalize options from
+            file: Include file options
+            cmdline: Include cmdline options
+        """
+
+        if not isinstance(config, Config):
+            config = Config(config, self.definitions)
         return clean_config(config, file=file, cmdline=cmdline)
 
     def normalize_config(
         self,
-        options: T | Config[T],
+        config: T | Config[T],
         file: bool = False,
         cmdline: bool = False,
-        defaults: bool = True,
+        default: bool = True,
+        persistent: bool = True,
     ) -> Config[Values]:
-        if isinstance(options, Config):
-            config = options
-        else:
-            config = Config(options, self.definitions)
+        """
+        Creates an `OptionValues` dictionary with setting definitions taken from `self.definitions`
+        and values taken from `raw_options` and `raw_options_2' if defined.
+        Values are assigned so if the value is a dictionary mutating it will mutate the original.
+
+        Args:
+            config: The Config object to normalize options from
+            file: Include file options
+            cmdline: Include cmdline options
+            default: Include default values in the returned Config object
+            persistent: Include unknown keys in persistent groups
+        """
+
+        if not isinstance(config, Config):
+            config = Config(config, self.definitions)
         return normalize_config(
             config=config,
             file=file,
             cmdline=cmdline,
-            defaults=defaults,
+            default=default,
+            persistent=persistent,
         )
 
-    @overload
-    def get_namespace(self, options: Values, defaults: bool = True) -> Namespace:
-        ...
-
-    @overload
-    def get_namespace(self, options: Config[Values], defaults: bool = True) -> Config[Namespace]:
-        ...
-
-    def get_namespace(self, options: Values | Config[Values], defaults: bool = True) -> Config[Namespace] | Namespace:
-        if isinstance(options, Config):
-            self.definitions = options[1]
-            return get_namespace(options, defaults=defaults)
+    def get_namespace(
+        self,
+        config: Values | Config[Values],
+        file: bool = False,
+        cmdline: bool = False,
+        default: bool = True,
+        persistent: bool = True,
+    ) -> Config[Namespace]:
+        """
+        Returns a Namespace object with options in the form "{group_name}_{setting_name}"
+        `options` should already be normalized or be a `Config[Namespace]`.
+        Throws an exception if the internal_name is duplicated
+
+        Args:
+            config: The Config object to turn into a namespace
+            file: Include file options
+            cmdline: Include cmdline options
+            default: Include default values in the returned Config object
+            persistent: Include unknown keys in persistent groups
+        """
+
+        if isinstance(config, Config):
+            self.definitions = config[1]
         else:
-            return get_namespace(Config(options, self.definitions), defaults=defaults)
+            config = Config(config, self.definitions)
+        return get_namespace(config, file=file, cmdline=cmdline, default=default, persistent=persistent)
 
     def parse_file(self, filename: pathlib.Path) -> tuple[Config[Values], bool]:
+        """
+        Helper function to read options from a json dictionary from a file.
+        This is purely a convenience function.
+        If _anything_ more advanced is desired this should be handled by the application.
+
+        Args:
+            filename: A pathlib.Path object to read a JSON dictionary from
+        """
         return parse_file(filename=filename, definitions=self.definitions)
 
-    def save_file(self, options: T | Config[T], filename: pathlib.Path) -> bool:
-        if isinstance(options, Config):
-            return save_file(options, filename=filename)
-        return save_file(Config(options, self.definitions), filename=filename)
+    def save_file(self, config: T | Config[T], filename: pathlib.Path) -> bool:
+        """
+        Helper function to save options from a json dictionary to a file.
+        This is purely a convenience function.
+        If _anything_ more advanced is desired this should be handled by the application.
+
+        Args:
+            config: The options to save to a json dictionary
+            filename: A pathlib.Path object to save the json dictionary to
+        """
+        if not isinstance(config, Config):
+            config = Config(config, self.definitions)
+        return save_file(config, filename=filename)
+
+    def parse_cmdline(self, args: list[str] | None = None, config: ns[T] = None) -> Config[Values]:
+        """
+        Creates an `argparse.ArgumentParser` from cmdline settings in `self.definitions`.
+        `args` and `config` are passed to `argparse.ArgumentParser.parse_args`
 
-    def parse_cmdline(self, args: list[str] | None = None, namespace: ns[T] = None) -> Config[Values]:
-        return parse_cmdline(self.definitions, self.description, self.epilog, args, namespace)
+        Args:
+            args: Passed to argparse.ArgumentParser.parse_args
+            config: The Config or Namespace object to use as a Namespace passed to argparse.ArgumentParser.parse_args
+        """
+        return parse_cmdline(self.definitions, self.description, self.epilog, args, config)
 
     def parse_config(self, config_path: pathlib.Path, args: list[str] | None = None) -> tuple[Config[Values], bool]:
+        """
+        Convenience function to parse options from a json file and passes the resulting Config object to parse_cmdline.
+        This is purely a convenience function.
+        If _anything_ more advanced is desired this should be handled by the application.
+
+        Args:
+            config_path: A `pathlib.Path` object
+            args: Passed to argparse.ArgumentParser.parse_args
+        """
         return parse_config(self.definitions, self.description, self.epilog, config_path, args)
 
 
-def example(manager: Manager) -> None:
+__all__ = [
+    'Setting',
+    'Group',
+    'Values',
+    'Definitions',
+    'Config',
+    'generate_settings',
+    'sanitize_name',
+    'get_option',
+    'get_options',
+    'normalize_config',
+    'parse_file',
+    'clean_config',
+    'defaults',
+    'get_namespace',
+    'save_file',
+    'create_argparser',
+    'parse_cmdline',
+    'parse_config',
+    'Manager',
+]
+
+
+def example_group(manager: Manager) -> None:
     manager.add_setting(
         '--hello',
         default='world',
     )
     manager.add_setting(
         '--save', '-s',
         default=False,
@@ -648,34 +850,34 @@
     manager.add_setting(
         '--verbose', '-v',
         default=False,
         action=BooleanOptionalAction,  # Added in Python 3.9
     )
 
 
-def persistent(manager: Manager) -> None:
+def persistent_group(manager: Manager) -> None:
     manager.add_setting(
         '--test', '-t',
         default=False,
         action=BooleanOptionalAction,  # Added in Python 3.9
     )
 
 
 def _main(args: list[str] | None = None) -> None:
     settings_path = pathlib.Path('./settings.json')
     manager = Manager(description='This is an example', epilog='goodbye!')
 
-    manager.add_group('example', example)
-    manager.add_persistent_group('persistent', persistent)
+    manager.add_group('example', example_group)
+    manager.add_persistent_group('persistent', persistent_group)
 
     file_config, success = manager.parse_file(settings_path)
-    file_namespace = manager.get_namespace(file_config)
+    file_namespace = manager.get_namespace(file_config, file=True, cmdline=True)
 
-    merged_config = manager.parse_cmdline(args=args, namespace=file_namespace)
-    merged_namespace = manager.get_namespace(merged_config)
+    merged_config = manager.parse_cmdline(args=args, config=file_namespace)
+    merged_namespace = manager.get_namespace(merged_config, file=True, cmdline=True)
 
     print(f'Hello {merged_config.values["example"]["hello"]}')  # noqa: T201
     if merged_namespace.values.example_save:
         if manager.save_file(merged_config, settings_path):
             print(f'Successfully saved settings to {settings_path}')  # noqa: T201
         else:
             print(f'Failed saving settings to a {settings_path}')  # noqa: T201
```

### Comparing `settngs-0.6.5/settngs.egg-info/PKG-INFO` & `settngs-0.7.0/settngs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.6.5
+Version: 0.7.0
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.6.5/setup.cfg` & `settngs-0.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 [pep8]
 ignore = E265,E501
 max_line_length = 120
 
 [flake8]
 extend-ignore = E501, A003
 max_line_length = 120
+per-file-ignores = 
+	*_test.py: LN001
 
 [coverage:run]
 plugins = covdefaults
 
 [coverage:report]
 fail_under = 95
```

### Comparing `settngs-0.6.5/testing/settngs.py` & `settngs-0.7.0/testing/settngs.py`

 * *Files identical despite different names*

### Comparing `settngs-0.6.5/tests/settngs_test.py` & `settngs-0.7.0/tests/settngs_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 from __future__ import annotations
 
 import argparse
+import ast
 import json
+import pathlib
+import sys
 from collections import defaultdict
+from typing import Generator
 
 import pytest
 
 import settngs
 from settngs import Group
 from testing.settngs import example
 from testing.settngs import failure
 from testing.settngs import success
 
 
+if sys.version_info < (3, 9):  # pragma: no cover
+    from typing import List
+else:
+    List = list
+
+
 @pytest.fixture
-def settngs_manager():
+def settngs_manager() -> Generator[settngs.Manager, None, None]:
     manager = settngs.Manager()
     yield manager
 
 
 def test_settngs_manager():
     manager = settngs.Manager()
     defaults = manager.defaults()
@@ -49,100 +59,182 @@
         settngs.Setting(*arguments[0], **arguments[1])
 
 
 def test_add_setting(settngs_manager):
     assert settngs_manager.add_setting('--test') is None
 
 
-def test_get_defaults(settngs_manager):
-    settngs_manager.add_setting('--test', default='hello')
-    defaults, _ = settngs_manager.defaults()
-    assert defaults['']['test'] == 'hello'
+class TestValues:
 
+    def test_invalid_normalize(self, settngs_manager):
+        with pytest.raises(ValueError) as excinfo:
+            settngs_manager.add_setting('--test', default='hello')
+            defaults, _ = settngs_manager.normalize_config({}, file=False, cmdline=False)
+        assert str(excinfo.value) == 'Invalid parameters: you must set either file or cmdline to True'
 
-def test_get_defaults_namespace(settngs_manager):
-    settngs_manager.add_setting('--test', default='hello')
-    defaults, _ = settngs_manager.get_namespace(settngs_manager.defaults())
-    assert defaults.test == 'hello'
+    def test_get_defaults(self, settngs_manager):
+        settngs_manager.add_setting('--test', default='hello')
+        defaults, _ = settngs_manager.defaults()
+        assert defaults['']['test'] == 'hello'
 
+    def test_get_defaults_group(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+        defaults, _ = settngs_manager.defaults()
+        assert defaults['tst']['test'] == 'hello'
 
-def test_get_namespace_with_namespace(settngs_manager):
-    settngs_manager.add_setting('--test', default='hello')
-    defaults, _ = settngs_manager.get_namespace(argparse.Namespace(test='success'))
-    assert defaults.test == 'success'
+    def test_cmdline_only(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello', file=False))
+        settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', cmdline=False))
 
+        file_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), file=True)
+        cmdline_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), cmdline=True)
 
-def test_get_defaults_group(settngs_manager):
-    settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
-    defaults, _ = settngs_manager.defaults()
-    assert defaults['tst']['test'] == 'hello'
+        assert 'test' not in file_normalized['tst']  # cmdline option not in normalized config
+        assert 'test2' in file_normalized['tst2']  # file option in normalized config
 
+        assert 'test' in cmdline_normalized['tst']  # cmdline option in normalized config
+        assert 'test2' not in cmdline_normalized['tst2']  # file option not in normalized config
 
-def test_get_namespace_group(settngs_manager):
-    settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
-    defaults, _ = settngs_manager.get_namespace(settngs_manager.defaults())
-    assert defaults.tst_test == 'hello'
+    def test_cmdline_only_persistent_group(self, settngs_manager):
+        settngs_manager.add_persistent_group('tst', lambda parser: parser.add_setting('--test', default='hello', file=False))
+        settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', cmdline=False))
 
+        file_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), file=True)
+        cmdline_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), cmdline=True)
 
-def test_cmdline_only(settngs_manager):
-    settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello', file=False))
-    settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', cmdline=False))
+        assert 'test' not in file_normalized['tst']
+        assert 'test2' in file_normalized['tst2']
 
-    file_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), file=True)
-    cmdline_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), cmdline=True)
+        assert 'test' in cmdline_normalized['tst']
+        assert 'test2' not in cmdline_normalized['tst2']
 
-    assert 'test' in cmdline_normalized['tst']
-    assert 'test2' not in cmdline_normalized['tst2']
+    def test_normalize_defaults(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test2', default='hello'))
+        settngs_manager.add_persistent_group('tst_persistent', lambda parser: parser.add_setting('--test', default='hello'))
 
-    assert 'test' not in file_normalized['tst']
-    assert 'test2' in file_normalized['tst2']
+        defaults = settngs_manager.defaults()
+        defaults_normalized = settngs_manager.normalize_config(defaults, file=True, default=False)
+        assert defaults_normalized.values['tst'] == {}
+        assert defaults_normalized.values['tst_persistent'] == {}
 
+        non_defaults = settngs_manager.defaults()
+        non_defaults.values['tst']['test'] = 'world'
+        non_defaults.values['tst_persistent']['test'] = 'world'
+        non_defaults_normalized = settngs_manager.normalize_config(non_defaults, file=True, default=False)
 
-def test_cmdline_only_persistent_group(settngs_manager):
-    settngs_manager.add_persistent_group('tst', lambda parser: parser.add_setting('--test', default='hello', file=False))
-    settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', cmdline=False))
+        assert non_defaults_normalized.values['tst'] == {'test': 'world'}
+        assert non_defaults_normalized.values['tst_persistent'] == {'test': 'world'}
 
-    file_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), file=True)
-    cmdline_normalized, _ = settngs_manager.normalize_config(settngs_manager.defaults(), cmdline=True)
+    def test_normalize(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+        settngs_manager.add_persistent_group('persistent', lambda parser: parser.add_setting('--world', default='world'))
 
-    assert 'test' in cmdline_normalized['tst']
-    assert 'test2' not in cmdline_normalized['tst2']
+        defaults = settngs_manager.defaults()
+        defaults.values['test'] = 'fail'  # Not defined in settngs_manager, should be removed
+        defaults.values['persistent']['hello'] = 'success'  # Not defined in settngs_manager, should stay
 
-    assert 'test' not in file_normalized['tst']
-    assert 'test2' in file_normalized['tst2']
+        normalized, _ = settngs_manager.normalize_config(defaults, file=True)
 
+        assert 'test' not in normalized
+        assert 'tst' in normalized
+        assert 'test' in normalized['tst']
+        assert normalized['tst']['test'] == 'hello'
+        assert normalized['persistent']['hello'] == 'success'
+        assert normalized['persistent']['world'] == 'world'
 
-def test_normalize(settngs_manager):
-    settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
-    settngs_manager.add_persistent_group('persistent', lambda parser: parser.add_setting('--world', default='world'))
 
-    defaults = settngs_manager.defaults()
-    defaults.values['test'] = 'fail'  # Not defined in settngs_manager, should be removed
-    defaults.values['persistent']['hello'] = 'success'  # Not defined in settngs_manager, should stay
-
-    defaults_namespace = settngs_manager.get_namespace(settngs_manager.defaults())
-    defaults_namespace.values.test = 'fail'  # Not defined in settngs_manager, should be removed
-    defaults_namespace.values.persistent_hello = 'success'  # Not defined in settngs_manager, should stay
-
-    normalized, _ = settngs_manager.normalize_config(defaults, file=True)
-    normalized_from_namespace = settngs_manager.normalize_config(defaults_namespace, file=True)
-    normalized_namespace, _ = settngs_manager.get_namespace(normalized_from_namespace)
+class TestNamespace:
 
-    assert 'test' not in normalized
-    assert 'tst' in normalized
-    assert 'test' in normalized['tst']
-    assert normalized['tst']['test'] == 'hello'
-    assert normalized['persistent']['hello'] == 'success'
-    assert normalized['persistent']['world'] == 'world'
-
-    assert not hasattr(normalized_namespace, 'test')
-    assert hasattr(normalized_namespace, 'tst_test')
-    assert normalized_namespace.tst_test == 'hello'
-    assert normalized_namespace.persistent_hello == 'success'
-    assert normalized_namespace.persistent_world == 'world'
+    def test_invalid_normalize(self, settngs_manager):
+        with pytest.raises(ValueError) as excinfo:
+            settngs_manager.add_setting('--test', default='hello')
+            defaults, _ = settngs_manager.get_namespace(settngs_manager.defaults(), file=False, cmdline=False)
+        assert str(excinfo.value) == 'Invalid parameters: you must set either file or cmdline to True'
+
+    def test_get_defaults(self, settngs_manager):
+        settngs_manager.add_setting('--test', default='hello')
+        defaults, _ = settngs_manager.get_namespace(settngs_manager.defaults(), file=True, cmdline=True)
+        assert defaults.test == 'hello'
+
+    def test_get_defaults_group(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+        defaults, _ = settngs_manager.get_namespace(settngs_manager.defaults(), file=True, cmdline=True)
+        assert defaults.tst_test == 'hello'
+
+    def test_cmdline_only(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello', file=False))
+        settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', cmdline=False))
+
+        file_normalized, _ = settngs_manager.get_namespace(settngs_manager.normalize_config(settngs_manager.defaults(), file=True), file=True)
+        cmdline_normalized, _ = settngs_manager.get_namespace(settngs_manager.normalize_config(settngs_manager.defaults(), cmdline=True), cmdline=True)
+
+        assert 'tst_test' not in file_normalized.__dict__
+        assert 'tst2_test2' in file_normalized.__dict__
+
+        assert 'tst_test' in cmdline_normalized.__dict__
+        assert 'tst2_test2' not in cmdline_normalized.__dict__
+
+    def test_cmdline_only_persistent_group(self, settngs_manager):
+        settngs_manager.add_persistent_group('tst', lambda parser: parser.add_setting('--test', default='hello', file=False))
+        settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', cmdline=False))
+
+        file_normalized, _ = settngs_manager.get_namespace(settngs_manager.normalize_config(settngs_manager.defaults(), file=True), file=True)
+        cmdline_normalized, _ = settngs_manager.get_namespace(settngs_manager.normalize_config(settngs_manager.defaults(), cmdline=True), cmdline=True)
+
+        assert 'tst_test' not in file_normalized.__dict__
+        assert 'tst2_test2' in file_normalized.__dict__
+
+        assert 'tst_test' in cmdline_normalized.__dict__
+        assert 'tst2_test2' not in cmdline_normalized.__dict__
+
+    def test_normalize_defaults(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test2', default='hello'))
+        settngs_manager.add_persistent_group('tst_persistent', lambda parser: parser.add_setting('--test', default='hello'))
+
+        defaults = settngs_manager.defaults()
+        defaults_normalized = settngs_manager.get_namespace(settngs_manager.normalize_config(defaults, file=True, default=False), file=True, default=False)
+        assert defaults_normalized.values.__dict__ == {}
+
+        non_defaults = settngs_manager.get_namespace(settngs_manager.defaults(), file=True, cmdline=True)
+        non_defaults.values.tst_test = 'world'
+        non_defaults.values.tst_persistent_test = 'world'
+        non_defaults_normalized = settngs_manager.get_namespace(settngs_manager.normalize_config(non_defaults, file=True, default=False), file=True, default=False)
+
+        assert non_defaults_normalized.values.tst_test == 'world'
+        assert non_defaults_normalized.values.tst_persistent_test == 'world'
+
+    def test_normalize(self, settngs_manager):
+        settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+        settngs_manager.add_persistent_group('persistent', lambda parser: parser.add_setting('--world', default='world'))
+
+        defaults = settngs_manager.get_namespace(settngs_manager.defaults(), file=True, cmdline=True)
+        defaults.values.test = 'fail'  # Not defined in settngs_manager, should be removed
+        defaults.values.persistent_hello = 'success'  # Not defined in settngs_manager, should stay
+
+        normalized, _ = settngs_manager.get_namespace(settngs_manager.normalize_config(defaults, file=True), file=True)
+
+        assert not hasattr(normalized, 'test')
+        assert hasattr(normalized, 'tst_test')
+        assert normalized.tst_test == 'hello'
+        assert normalized.persistent_hello == 'success'
+        assert normalized.persistent_world == 'world'
+
+
+def test_get_namespace_with_namespace(settngs_manager):
+    settngs_manager.add_setting('--test', default='hello')
+    defaults, _ = settngs_manager.get_namespace(argparse.Namespace(test='success'), file=True)
+    assert defaults.test == 'success'
+
+
+def test_get_namespace_group(settngs_manager):
+    settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello'))
+    defaults, _ = settngs_manager.get_namespace(settngs_manager.defaults(), file=True)
+    assert defaults.tst_test == 'hello'
 
 
 def test_clean_config(settngs_manager):
     settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello', cmdline=False))
     settngs_manager.add_group('tst2', lambda parser: parser.add_setting('--test2', default='hello', file=False))
     settngs_manager.add_persistent_group('persistent', lambda parser: parser.add_setting('--world', default='world'))
     normalized, _ = settngs_manager.defaults()
@@ -176,15 +268,15 @@
 
 @pytest.mark.parametrize('ns', namespaces)
 def test_parse_cmdline_with_namespace(settngs_manager, ns):
     settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test', default='hello', cmdline=True))
     settngs_manager.add_group('tst', lambda parser: parser.add_setting('--test2', default='fail', cmdline=True))
 
     normalized, _ = settngs_manager.parse_cmdline(
-        ['--test', 'success'], namespace=ns(settngs_manager.definitions),
+        ['--test', 'success'], config=ns(settngs_manager.definitions),
     )
 
     assert 'test' in normalized['tst']
     assert normalized['tst']['test'] == 'success'
     assert normalized['tst']['test2'] == 'success'
 
 
@@ -327,15 +419,15 @@
 
     settngs_manager2 = settngs.Manager()
     settngs_manager2.add_group('tst', tst)
 
     assert default_to_regular(settngs_manager.definitions) == default_to_regular(settngs_manager2.definitions)
 
 
-def test_adding_to_existing_persistent_group(settngs_manager, tmp_path):
+def test_adding_to_existing_persistent_group(settngs_manager: settngs.Manager, tmp_path: pathlib.Path) -> None:
     def default_to_regular(d):
         if isinstance(d, defaultdict):
             d = {k: default_to_regular(v) for k, v in d.items()}
         return d
     settngs_manager.add_persistent_group('tst', lambda parser: parser.add_setting('--test', default='success'))
     settngs_manager.add_persistent_group('tst', lambda parser: parser.add_setting('--test2', default='success'))
 
@@ -345,23 +437,139 @@
 
     settngs_manager2 = settngs.Manager()
     settngs_manager2.add_persistent_group('tst', tst)
 
     assert default_to_regular(settngs_manager.definitions) == default_to_regular(settngs_manager2.definitions)
 
 
+class test_type(int):
+    ...
+
+
+def _typed_function(something: str) -> test_type:  # pragma: no cover
+    return test_type()
+
+
+def _untyped_function(something):
+    ...
+
+
+class _customAction(argparse.Action):  # pragma: no cover
+
+    def __init__(
+        self,
+        option_strings,
+        dest,
+        const=None,
+        default=None,
+        required=False,
+        help=None,  # noqa: A002
+        metavar=None,
+    ):
+        super().__init__(
+            option_strings=option_strings,
+            dest=dest,
+            nargs=0,
+            const=const,
+            default=default,
+            required=required,
+            help=help,
+        )
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        setattr(namespace, self.dest, 'Something')
+
+
+types = (
+    (settngs.Setting('-t', '--test'), str),
+    (settngs.Setting('-t', '--test', cmdline=False), 'Any'),
+    (settngs.Setting('-t', '--test', default=1, file=True, cmdline=False), int),
+    (settngs.Setting('-t', '--test', action='count'), int),
+    (settngs.Setting('-t', '--test', action='append'), List[str]),
+    (settngs.Setting('-t', '--test', action='extend'), List[str]),
+    (settngs.Setting('-t', '--test', action='store_const', const=1), int),
+    (settngs.Setting('-t', '--test', action='append_const', const=1), list),
+    (settngs.Setting('-t', '--test', action='store_true'), bool),
+    (settngs.Setting('-t', '--test', action='store_false'), bool),
+    (settngs.Setting('-t', '--test', action=settngs.BooleanOptionalAction), bool),
+    (settngs.Setting('-t', '--test', action=_customAction), 'Any'),
+    (settngs.Setting('-t', '--test', action='help'), None),
+    (settngs.Setting('-t', '--test', action='version'), None),
+    (settngs.Setting('-t', '--test', type=int), int),
+    (settngs.Setting('-t', '--test', type=_typed_function), test_type),
+    (settngs.Setting('-t', '--test', type=_untyped_function, default=1), int),
+    (settngs.Setting('-t', '--test', type=_untyped_function), 'Any'),
+)
+
+
+@pytest.mark.parametrize('setting,typ', types)
+def test_guess_type(setting, typ):
+    guessed_type = setting._guess_type()
+    assert guessed_type == typ
+
+
+settings = (
+    (lambda parser: parser.add_setting('-t', '--test'), 'str'),
+    (lambda parser: parser.add_setting('-t', '--test', cmdline=False), 'typing.Any'),
+    (lambda parser: parser.add_setting('-t', '--test', default=1, file=True, cmdline=False), 'int'),
+    (lambda parser: parser.add_setting('-t', '--test', action='count'), 'int'),
+    (lambda parser: parser.add_setting('-t', '--test', action='append'), List[str]),
+    (lambda parser: parser.add_setting('-t', '--test', action='extend'), List[str]),
+    (lambda parser: parser.add_setting('-t', '--test', action='store_const', const=1), 'int'),
+    (lambda parser: parser.add_setting('-t', '--test', action='append_const', const=1), 'list'),
+    (lambda parser: parser.add_setting('-t', '--test', action='store_true'), 'bool'),
+    (lambda parser: parser.add_setting('-t', '--test', action='store_false'), 'bool'),
+    (lambda parser: parser.add_setting('-t', '--test', action=settngs.BooleanOptionalAction), 'bool'),
+    (lambda parser: parser.add_setting('-t', '--test', action=_customAction), 'typing.Any'),
+    (lambda parser: parser.add_setting('-t', '--test', action='help'), None),
+    (lambda parser: parser.add_setting('-t', '--test', action='version'), None),
+    (lambda parser: parser.add_setting('-t', '--test', type=int), 'int'),
+    (lambda parser: parser.add_setting('-t', '--test', type=_typed_function), 'tests.settngs_test.test_type'),
+    (lambda parser: parser.add_setting('-t', '--test', type=_untyped_function, default=1), 'int'),
+    (lambda parser: parser.add_setting('-t', '--test', type=_untyped_function), 'typing.Any'),
+)
+
+
+@pytest.mark.parametrize('set_options,typ', settings)
+def test_generate_ns(settngs_manager, set_options, typ):
+    settngs_manager.add_group('test', set_options)
+
+    src = '''\
+from __future__ import annotations
+import typing
+import settngs
+'''
+    if typ == 'tests.settngs_test.test_type':
+        src += 'import tests.settngs_test\n'
+    src += '''
+class settngs_namespace(settngs.Namespace):
+'''
+    if typ is None:
+        src += '    ...\n'
+    else:
+        src += f'    {settngs_manager.definitions["test"].v["test"].internal_name}: {typ}\n'
+
+    generated_src = settngs_manager.generate_ns()
+
+    assert generated_src == src
+
+    ast.parse(generated_src)
+
+
 def test_example(capsys, tmp_path, monkeypatch):
     monkeypatch.chdir(tmp_path)
     settings_file = tmp_path / 'settings.json'
     settings_file.touch()
 
     i = 0
     for args, expected_out, expected_file in example:
         if args == ['manual settings.json']:
             settings_file.unlink()
             settings_file.write_text('{\n  "example": {\n    "hello": "lordwelch",\n    "verbose": true\n  },\n  "persistent": {\n    "test": false,\n    "hello": "world"\n  }\n}\n')
+            i += 1
+            continue
         else:
             settngs._main(args)
             captured = capsys.readouterr()
         assert captured.out == expected_out, f'{i}, {args}'
         assert settings_file.read_text() == expected_file, f'{i}, {args}'
         i += 1
```

### Comparing `settngs-0.6.5/workflows/build.yaml` & `settngs-0.7.0/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.6.5/workflows/package.yaml` & `settngs-0.7.0/workflows/package.yaml`

 * *Files identical despite different names*

