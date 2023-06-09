# Comparing `tmp/autodox-0.0.2.1.tar.gz` & `tmp/autodox-0.0.3.0.tar.gz`

## Comparing `autodox-0.0.2.1.tar` & `autodox-0.0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 autodox-0.0.2.1/autodox/__init__.py
--rw-r--r--   0        0        0    13833 2020-02-02 00:00:00.000000 autodox-0.0.2.1/autodox/functions.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.2.1/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.2.1/license
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 autodox-0.0.2.1/readme.md
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 autodox-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.3.0/autodox/__init__.py
+-rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 autodox-0.0.3.0/autodox/functions.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.3.0/tests/context.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.3.0/tests/test_hooks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.3.0/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.3.0/license
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 autodox-0.0.3.0/readme.md
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 autodox-0.0.3.0/PKG-INFO
```

### Comparing `autodox-0.0.2.1/autodox/functions.py` & `autodox-0.0.3.0/autodox/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,87 @@
+from enum import Enum, auto
 from types import ModuleType
 from typing import Any, Callable
 
 
+
+class Event(Enum):
+    AFTER_HEADER = auto()
+    AFTER_PARAGRAPH = auto()
+    AFTER_LIST = auto()
+    BEFORE_VALUE = auto()
+    AFTER_VALUE = auto()
+    BEFORE_FUNCTION = auto()
+    AFTER_FUNCTION = auto()
+    BEFORE_CLASS = auto()
+    AFTER_CLASS = auto()
+    BEFORE_MODULE = auto()
+    AFTER_MODULE = auto()
+
+
+_handlers = {}
+
+
+def _set_handler(event: Event, function: Callable) -> None:
+    """Set a handler for a specific event."""
+    if not callable(function):
+        raise TypeError('function must be callable')
+
+    if event.name in _handlers:
+        first = _handlers[event.name]
+        second = function
+        _handlers[event.name] = lambda *args: second(first(*args))
+    else:
+        _handlers[event.name] = function
+
+
+def set_before_handler(event: Event, function: Callable[[Any, dict], tuple[Any, dict]]) -> None:
+    """Sets a handler for a BEFORE_ event."""
+    if type(event) is not Event:
+        raise TypeError('event must be Event')
+    if 'BEFORE_' not in event.name:
+        raise ValueError('event must be a BEFORE_ event')
+
+    _set_handler(event, function)
+
+
+def set_after_handler(event: Event, function: Callable[[str], str]) -> None:
+    """Sets a handler for an AFTER_ event."""
+    if type(event) is not Event:
+        raise TypeError('event must be Event')
+    if 'AFTER_' not in event.name:
+        raise ValueError('event must be an AFTER_ event')
+
+    _set_handler(event, function)
+
+
+def unset_handler(event: Event) -> None:
+    """Unset an event handling handler."""
+    if type(event) is not Event:
+        raise TypeError('event must be Event')
+    if event.name in _handlers:
+        del _handlers[event.name]
+
+
+def _invoke_handler(event: Event, *args) -> None:
+    """Invokes the handler for the event if set, otherwise return the
+        parameters.
+    """
+    if event.name in _handlers:
+        val = _handlers[event.name](*args)
+        return val[0] if len(val) == 1 else val
+    return args[0] if len(args) == 1 else args
+
+
 def _header(line: str, header_level: int = 0) -> str:
     """Takes a line and returns it formatted as a header with the proper
         number of hashtags for the given header_level.
     """
-    return ''.join(['#' for _ in range(header_level+1)]) + f' {line}\n\n'
+    doc = ''.join(['#' for _ in range(header_level+1)]) + f' {line}\n\n'
+    return _invoke_handler(Event.AFTER_HEADER, doc)
 
 
 def _paragraph(docstring: str) -> str:
     """Takes a docstring, tokenizes it, and returns a str formatted to
         72 chars or fewer per line without splitting tokens.
     """
     def make_line(tokens: list[str]) -> tuple[str, list[str]]:
@@ -23,27 +94,30 @@
     tokens = docstring.split()
     lines = []
 
     while len(tokens):
         line, tokens = make_line(tokens)
         lines.append(line)
 
-    return '\n'.join(lines) + '\n\n'
+    doc = '\n'.join(lines) + '\n\n'
+    return _invoke_handler(Event.AFTER_PARAGRAPH, doc)
 
 
 def _list(line: str) -> str:
     """Takes a line and returns a formatted list item."""
-    return _paragraph(f'- {line}')[:-1]
+    doc = _paragraph(f'- {line}')[:-1]
+    return _invoke_handler(Event.AFTER_LIST, doc)
 
 
 def dox_a_module(module: ModuleType, options: dict = {}) -> str:
     """Iterates over a module, collects information about its parts, and
         returns a str containing markdown documentation generated from
         types, annotations, and docstrings.
     """
+    module, options = _invoke_handler(Event.BEFORE_MODULE, module, options)
     exclude_names = options['exclude_names'] if 'exclude_names' in options else []
     exclude_types = options['exclude_types'] if 'exclude_types' in options else []
     header_level = options['header_level'] if 'header_level' in options else 0
     function_format = options['function_format'] if 'function_format' in options else 'header'
     value_format = options['value_format'] if 'value_format' in options else 'list'
     include_private = 'include_private' in options
     include_dunder = 'include_dunder' in options
@@ -113,42 +187,47 @@
             doc += val
 
     if len(submodules):
         doc += _header('Submodules', header_level + 1)
         for sub in submodules:
             doc += sub
 
-    return doc
+    return _invoke_handler(Event.AFTER_MODULE, doc)
 
 
 def dox_a_value(value: Any, options: dict = {}) -> str:
     """Collects some information about a value and returns it formatted
         as specified in the options or as a list.
     """
+    value, options = _invoke_handler(Event.BEFORE_VALUE, value, options)
     header_level = options['header_level'] if 'header_level' in options else 0
     format = options['format'] if 'format' in options else 'list'
 
     name = value.__name__ if hasattr(value, '__name__') else '{unknown/unnamed}'
     if 'name' in options:
         name = options['name']
     type_str = type(value).__name__
+    doc = ''
 
     match format:
         case 'header':
-            return _header(f'{name}: {type_str}', header_level)
+            doc = _header(f'{name}: {type_str}', header_level)
         case 'paragraph':
-            return _paragraph(f'{name}: {type_str}')
+            doc = _paragraph(f'{name}: {type_str}')
         case _:
-            return _list(f'{name}: {type_str}')
+            doc = _list(f'{name}: {type_str}')
+
+    return _invoke_handler(Event.AFTER_VALUE, doc)
 
 
 def dox_a_function(function: Callable, options: dict = {}) -> str:
     """Collects some information about a function and returns it
         formatted as specified in the options or as a list.
     """
+    function, options = _invoke_handler(Event.BEFORE_FUNCTION, function, options)
     header_level = options['header_level'] if 'header_level' in options else 0
     format = options['format'] if 'format' in options else 'list'
 
     name = function.__name__ if hasattr(function, '__name__') else '{unknown/unnamed}'
     annotations = function.__annotations__ if hasattr(function, '__annotations__') else {}
     return_annotation = annotations['return'] if 'return' in annotations else None
     annotations = [
@@ -191,15 +270,15 @@
                 doc += _paragraph(docstring)
         case _:
             doc = signature
             if docstring:
                 doc += docstring
             doc = _list(doc)
 
-    return doc
+    return _invoke_handler(Event.AFTER_FUNCTION, doc)
 
 
 def _dox_properties(properties: dict, header_level: int = 0) -> str:
     """Format properties for a class."""
     doc = ''
     dunders = {
         name: value
@@ -284,14 +363,15 @@
     """Collects some information about a class and returns a formatted
         str. Any names specified in options['exclude_names'] and any
         types specified in options['exclude_types'] will be excluded.
         Private and dunder methods/properties will be included if
         options['include_private'] or options['include_dunder'] are
         specified, respectively.
     """
+    cls, options = _invoke_handler(Event.BEFORE_CLASS, cls, options)
     exclude_names = options['exclude_names'] if 'exclude_names' in options else []
     header_level = options['header_level'] if 'header_level' in options else 0
     include_private = 'include_private' in options
     include_dunder = 'include_dunder' in options
     suboptions = {**options, 'header_level': header_level + 1}
 
     parent = cls.__base__ if hasattr(cls, '__base__') else None
@@ -334,15 +414,15 @@
         doc += _header('Properties', header_level + 1)
         doc += _dox_properties(properties, header_level)
 
     if methods:
         doc += _header('Methods', header_level + 1)
         doc += _dox_methods(methods, suboptions)
 
-    return doc
+    return _invoke_handler(Event.AFTER_CLASS, doc)
 
 
 def main_cli() -> int:
     """Entry point for pip installed wrapper function to invoke via CLI."""
     from importlib import import_module
     from sys import argv
     _settings = {}
```

### Comparing `autodox-0.0.2.1/license` & `autodox-0.0.3.0/license`

 * *Files identical despite different names*

### Comparing `autodox-0.0.2.1/pyproject.toml` & `autodox-0.0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autodox"
-version = "0.0.2.1"
+version = "0.0.3.0"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Tool for generating documentation automatically from code annotations, types, and docstrings."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

