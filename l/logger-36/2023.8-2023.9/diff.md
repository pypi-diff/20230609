# Comparing `tmp/logger-36-2023.8.tar.gz` & `tmp/logger-36-2023.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-36-2023.8.tar", last modified: Wed Mar 15 15:19:30 2023, max compression
+gzip compressed data, was "logger-36-2023.9.tar", last modified: Thu Mar 16 14:50:57 2023, max compression
```

## Comparing `logger-36-2023.8.tar` & `logger-36-2023.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:19:30.082509 logger-36-2023.8/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2023.8/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4221 2023-03-15 15:19:30.082509 logger-36-2023.8/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2023.8/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2023.8/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2023.8/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:19:30.082509 logger-36-2023.8/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:19:30.082509 logger-36-2023.8/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1852 2023-02-17 08:45:51.000000 logger-36-2023.8/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:19:30.082509 logger-36-2023.8/logger_36/
--rw-r--r--   0 eric      (1000) users      (984)     1763 2023-03-14 16:09:12.000000 logger-36-2023.8/logger_36/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)    13061 2023-03-15 15:12:19.000000 logger-36-2023.8/logger_36/main.py
--rw-r--r--   0 eric      (1000) users      (984)     2599 2023-03-15 15:14:51.000000 logger-36-2023.8/logger_36/test.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-03-15 14:58:16.000000 logger-36-2023.8/logger_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-15 15:19:30.082509 logger-36-2023.8/logger_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4221 2023-03-15 15:19:30.000000 logger-36-2023.8/logger_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      379 2023-03-15 15:19:30.000000 logger-36-2023.8/logger_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-03-15 15:19:30.000000 logger-36-2023.8/logger_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        5 2023-03-15 15:19:30.000000 logger-36-2023.8/logger_36.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2023-03-15 15:19:30.000000 logger-36-2023.8/logger_36.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2023.8/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-03-15 15:19:30.082509 logger-36-2023.8/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5340 2023-02-17 09:13:12.000000 logger-36-2023.8/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-16 14:50:57.991479 logger-36-2023.9/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2023.9/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4221 2023-03-16 14:50:57.991479 logger-36-2023.9/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2023.9/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2023.9/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2023.9/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-16 14:50:57.988145 logger-36-2023.9/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-16 14:50:57.991479 logger-36-2023.9/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1852 2023-02-17 08:45:51.000000 logger-36-2023.9/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-16 14:50:57.991479 logger-36-2023.9/logger_36/
+-rw-r--r--   0 eric      (1000) users      (984)     1780 2023-03-16 09:06:08.000000 logger-36-2023.9/logger_36/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)    14300 2023-03-16 14:49:31.000000 logger-36-2023.9/logger_36/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     3534 2023-03-16 14:41:42.000000 logger-36-2023.9/logger_36/test.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-03-16 14:43:57.000000 logger-36-2023.9/logger_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-16 14:50:57.991479 logger-36-2023.9/logger_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4221 2023-03-16 14:50:57.000000 logger-36-2023.9/logger_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      379 2023-03-16 14:50:57.000000 logger-36-2023.9/logger_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-03-16 14:50:57.000000 logger-36-2023.9/logger_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        5 2023-03-16 14:50:57.000000 logger-36-2023.9/logger_36.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2023-03-16 14:50:57.000000 logger-36-2023.9/logger_36.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2023.9/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-03-16 14:50:57.991479 logger-36-2023.9/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5340 2023-02-17 09:13:12.000000 logger-36-2023.9/setup.py
```

### Comparing `logger-36-2023.8/PKG-INFO` & `logger-36-2023.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2023.8
+Version: 2023.9
 Summary: Simple logger using rich_
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
```

### Comparing `logger-36-2023.8/README-COPYRIGHT-utf8.txt` & `logger-36-2023.9/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2023.8/README-LICENCE-utf8.txt` & `logger-36-2023.9/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2023.8/README.rst` & `logger-36-2023.9/README.rst`

 * *Files identical despite different names*

### Comparing `logger-36-2023.8/documentation/wiki/description.asciidoc` & `logger-36-2023.9/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `logger-36-2023.8/logger_36/__init__.py` & `logger-36-2023.9/logger_36/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,10 +32,11 @@
 from logger_36.main import (
     LOGGER,
     AddFileHandler,
     ElapsedTime,
     LogSystemDetails,
     MaximumMemoryUsage,
     SaveLOGasHTML,
+    SetLOGLevel,
     SetShowMemoryUsage,
 )
 from logger_36.version import __version__
```

### Comparing `logger-36-2023.8/logger_36/main.py` & `logger-36-2023.9/logger_36/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 import datetime as dttm
 import logging as lggg
 import platform as pltf
 import sys as sstm
 import time
 from pathlib import Path as path_t
-from typing import Any, Callable, ClassVar, TextIO
+from typing import ClassVar, TextIO
+from types import FunctionType, MethodType
 
 from rich.color import Color as color_t
 from rich.console import Console as console_t
 from rich.style import Style as style_t
 from rich.text import Text as text_t
 
 try:
@@ -50,14 +51,17 @@
     _MEGA_UNIT = _KILO_UNIT * 1024.0
     _GIGA_UNIT = _MEGA_UNIT * 1024.0
 except ModuleNotFoundError:
     _PROCESS = None
     _KILO_UNIT = _MEGA_UNIT = _GIGA_UNIT = 0.0
 
 
+LOGGER_NAME = "logger-36"
+
+
 # This module is certainly imported early. Therefore, the current time should be close enough to the real start time.
 _START_TIME = time.time()
 
 _TAB_SIZE = 5  # So that _CONTEXT_SEPARATOR is aligned for all log levels
 _DATE_TIME_LENGTH = 19
 _LOG_LEVEL_LENGTH = 10  # Max length, including _LEVEL_OPENING and _LEVEL_CLOSING
 
@@ -165,24 +169,24 @@
 
 
 class console_handler_t(lggg.Handler, _handler_extension):
     _LEVEL_COLOR: ClassVar[dict[int, str | style_t]] = {
         lggg.DEBUG: "orchid",
         lggg.INFO: "white",
         lggg.WARNING: "yellow",
-        lggg.ERROR: "orange3",
+        lggg.ERROR: "orange1",
         lggg.CRITICAL: "red",
     }
     _GRAY_STYLE: ClassVar[style_t] = style_t(color=color_t.from_rgb(150, 150, 150))
     _ACTUAL: ClassVar[str] = r" Actual=[^.]+\."
     _EXPECTED: ClassVar[str] = r" Expected([!<>]=|: )[^.]+\."
 
     console: console_t
 
-    def __init__(self, /, *, level=lggg.NOTSET) -> None:
+    def __init__(self, /, *, level: int = lggg.NOTSET) -> None:
         """"""
         lggg.Handler.__init__(self, level=level)
         _handler_extension.__init__(self)
 
         self.setFormatter(self.formatter)
         self.console = console_t(record=True, force_terminal=True, tab_size=_TAB_SIZE)
 
@@ -217,17 +221,17 @@
         highlighted.highlight_words((cls._ACTUAL,), style="red")
         highlighted.highlight_words((cls._EXPECTED,), style="green")
 
         self.console.print(highlighted, crop=False, overflow="ignore", highlight=False)
 
 
 class file_handler_t(lggg.FileHandler, _handler_extension):
-    def __init__(self, file: str | path_t, *args, **kwargs) -> None:
+    def __init__(self, path: str | path_t, /, *args, **kwargs) -> None:
         """"""
-        lggg.FileHandler.__init__(self, str(file), *args, **kwargs)
+        lggg.FileHandler.__init__(self, str(path), *args, **kwargs)
         _handler_extension.__init__(self)
 
         self.setFormatter(self.formatter)
 
     def emit(self, record: lggg.LogRecord, /) -> None:
         """"""
         formatted, next_lines = self.FormattedMessage(record)
@@ -237,49 +241,112 @@
         if next_lines is not None:
             message = f"{message}{next_lines}"
 
         print(message, file=self.stream)
         self.stream.flush()
 
 
-LOGGER = lggg.getLogger(name="color_w_rich")
-LOGGER.setLevel(lggg.INFO)  # Minimum desired level
-LOGGER.addHandler(console_handler_t())
+LOGGER = lggg.getLogger(name=LOGGER_NAME)
+LOGGER.setLevel(lggg.DEBUG)
+LOGGER.addHandler(console_handler_t(level=lggg.INFO))
+
+
+def AddFileHandler(
+    path: str | path_t, /, level: int = lggg.INFO, *args, **kwargs
+) -> None:
+    """"""
+    if isinstance(path, str):
+        path = path_t(path)
+    if path.exists():
+        raise ValueError(f"{path}: File already exists")
+
+    handler = file_handler_t(path, *args, **kwargs)
+    handler.setLevel(level)
+    LOGGER.addHandler(handler)
+
+
+def SetLOGLevel(level: int, /, *, which: str = "a") -> None:
+    """
+    which: c=console, f=file, a=all
+    """
+    if which not in "cfa":
+        raise ValueError(
+            f'{which}: Invalid handler specifier. Expected="c" for console, "f" for file, or "a" for all'
+        )
+
+    for handler in LOGGER.handlers:
+        if (
+            (which == "a")
+            or ((which == "c") and isinstance(handler, console_handler_t))
+            or ((which == "f") and isinstance(handler, file_handler_t))
+        ):
+            handler.setLevel(level)
 
 
 def SetShowMemoryUsage(show_memory_usage: bool, /) -> None:
     """"""
     if show_memory_usage and (_PROCESS is None):
         LOGGER.warning('Cannot show memory usage: Package "psutil" not installed')
         return
 
     for handler in LOGGER.handlers:
         if hasattr(handler, "show_memory_usage"):
             handler.show_memory_usage = show_memory_usage
 
 
-def AddFileHandler(path: str | path_t, /) -> None:
+def LogSystemDetails() -> None:
     """"""
-    if isinstance(path, str):
-        path = path_t(path)
-    if path.exists():
-        raise ValueError(f"{path}: File already exists")
+    details = "\n".join(
+        f"    {_key:>{_MAX_DETAIL_NAME_LENGTH}}: {_vle}"
+        for _key, _vle in _SYSTEM_DETAILS.items()
+    )
+
+    modules = sstm.modules
+    with_versions = []
+    for name in modules.keys():
+        if name.startswith("_") or ("." in name):
+            continue
+
+        module = modules[name]
+        version = getattr(module, "__version__", None)
+        if version is not None:
+            with_versions.append(f"{name}={version}")
+    modules = ", ".join(with_versions)
 
-    LOGGER.addHandler(file_handler_t(path))
+    LOGGER.info(
+        f"SYSTEM DETAILS\n"
+        f"{details}\n"
+        f"    {'Python Modules':>{_MAX_DETAIL_NAME_LENGTH}}:\n"
+        f"    {modules}"
+    )
 
 
-def SaveLOGasHTML(path: str | path_t | TextIO, /) -> None:
+def SaveLOGasHTML(path: str | path_t | TextIO = None) -> None:
     """"""
-    if isinstance(path, str):
+    cannot_save = "Cannot save logging record as HTML"
+
+    if path is None:
+        for handler in LOGGER.handlers:
+            if isinstance(handler, lggg.FileHandler):
+                path = path_t(handler.baseFilename).with_suffix(".htm")
+                break
+        if path is None:
+            LOGGER.warning(f"{cannot_save}: No file handler to build a filename from")
+            return
+        if path.exists():
+            LOGGER.warning(
+                f'{cannot_save}: Automatically generated path "{path}" already exists'
+            )
+            return
+    elif isinstance(path, str):
         path = path_t(path)
+
     actual_file = isinstance(path, path_t)
     if actual_file and path.exists():
-        LOGGER.warning(
-            f'Cannot save logging record as HTML: File "{path}" already exists'
-        )
+        LOGGER.warning(f'{cannot_save}: File "{path}" already exists')
         return
 
     console = None
     found = False
     for handler in LOGGER.handlers:
         console = getattr(handler, "console", None)
         if found := isinstance(console, console_t):
@@ -289,62 +356,33 @@
         html = console.export_html()
         if actual_file:
             with open(path, "w") as accessor:
                 accessor.write(html)
         else:
             path.write(html)
     else:
-        LOGGER.warning(
-            "Cannot save logging record as HTML: No handler has a RICH console"
-        )
+        LOGGER.warning(f"{cannot_save}: No handler has a RICH console")
 
 
-def WhereFunction(function: Any, /) -> str:
+def WhereFunction(function: FunctionType, /) -> str:
     """"""
     return f"{function.__module__}:{function.__name__}"
 
 
-def WhereMethod(obj: Any, method: Callable, /) -> str:
+def WhereMethod(instance: object, method: MethodType, /) -> str:
     """
     method: Could be a str instead, which would require changing method.__name__ into getattr(cls, method). But if the
         method name changes while forgetting to change the string in the call to WhereMethod accordingly, then an
         exception would be raised here.
     """
-    cls = obj.__class__
+    cls = instance.__class__
 
     return f"{cls.__module__}:{cls.__name__}:{method.__name__}"
 
 
-def LogSystemDetails() -> None:
-    """"""
-    details = "\n".join(
-        f"    {_key:>{_MAX_DETAIL_NAME_LENGTH}}: {_vle}"
-        for _key, _vle in _SYSTEM_DETAILS.items()
-    )
-
-    modules = sstm.modules
-    with_versions = []
-    for name in modules.keys():
-        if name.startswith("_") or ("." in name):
-            continue
-
-        module = modules[name]
-        version = getattr(module, "__version__", None)
-        if version is not None:
-            with_versions.append(f"{name}={version}")
-    modules = ", ".join(with_versions)
-
-    LOGGER.info(
-        f"SYSTEM DETAILS\n"
-        f"{details}\n"
-        f"    {'Python Modules':>{_MAX_DETAIL_NAME_LENGTH}}:\n"
-        f"    {modules}"
-    )
-
-
 def TimeStamp() -> str:
     """"""
     return (
         dttm.datetime.now()
         .isoformat(timespec="milliseconds")
         .replace(".", "-")
         .replace(":", "-")
```

### Comparing `logger-36-2023.8/logger_36/test.py` & `logger-36-2023.9/logger_36/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,43 +25,84 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+import difflib as diff
+import logging as lggg
+import sys as sstm
+from html.parser import HTMLParser as html_parser_t
+from io import StringIO as fake_file_t
 from pathlib import Path as path_t
 from tempfile import TemporaryDirectory
-from io import StringIO as fake_file_t
+
 from logger_36 import (
     LOGGER,
     AddFileHandler,
     MaximumMemoryUsage,
-    SetShowMemoryUsage,
     SaveLOGasHTML,
+    SetLOGLevel,
+    SetShowMemoryUsage,
 )
 
 
+class de_htmler_t(html_parser_t):
+    inside_body: bool = False
+    text: str = ""
+
+    def handle_starttag(self, tag: str, attrs, /) -> None:
+        """"""
+        if tag.lower() == "body":
+            self.inside_body = True
+
+    def handle_data(self, data: str, /) -> None:
+        """"""
+        if self.inside_body:
+            self.text += data
+
+
 with TemporaryDirectory() as tmp_folder:
     tmp_folder = path_t(tmp_folder)
     tmp_file = tmp_folder / "log.txt"
 
     AddFileHandler(tmp_file)
+    SetLOGLevel(lggg.DEBUG, which="c")
     SetShowMemoryUsage(True)
 
     for level in ("debug", "info", "warning", "error", "critical"):
         LogMessage = getattr(LOGGER, level)
         LogMessage(f"{level.capitalize()} message")
         LogMessage(f"Multi-line\n{level.capitalize()}\nmessage")
 
     LOGGER.info("V" + 30 * "e" + "ry l" + 30 * "o" + "ng line")
     LOGGER.info("V" + 30 * "e" + "ry l" + 30 * "o" + "ng line...\n...with a newline")
 
     usage, unit = MaximumMemoryUsage(decimals=1)
     LOGGER.info(f"Max. memory usage: {usage}{unit}")
 
-    content = open(tmp_file, "r").read()
-    print(f"\n{content}")
+    content = open(tmp_file, "r").read().strip()
+    print("\n--- LOG File\n" + content)
 
 fake_file = fake_file_t()
 SaveLOGasHTML(fake_file)
-print(fake_file.getvalue())
+html = fake_file.getvalue()
+
+de_htmler = de_htmler_t()
+de_htmler.feed(html)
+de_htmled = de_htmler.text.strip()
+
+print("\n--- De HTMLed\n" + de_htmled)
+
+print("")
+sstm.stdout.writelines(
+    diff.context_diff(
+        content.splitlines(keepends=True),
+        de_htmled.splitlines(keepends=True),
+        fromfile="LOG File",
+        tofile="De HTMLed",
+        n=0,
+    )
+)
+
+print("\n--- HTML\n" + html.strip())
```

### Comparing `logger-36-2023.8/logger_36/version.py` & `logger-36-2023.9/logger_36/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.8"
+__version__ = "2023.9"
```

### Comparing `logger-36-2023.8/logger_36.egg-info/PKG-INFO` & `logger-36-2023.9/logger_36.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2023.8
+Version: 2023.9
 Summary: Simple logger using rich_
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
```

### Comparing `logger-36-2023.8/setup.py` & `logger-36-2023.9/setup.py`

 * *Files identical despite different names*

