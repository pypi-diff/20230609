# Comparing `tmp/macnotesapp-0.5.1.tar.gz` & `tmp/macnotesapp-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macnotesapp-0.5.1.tar", max compression
+gzip compressed data, was "macnotesapp-0.5.2.tar", max compression
```

## Comparing `macnotesapp-0.5.1.tar` & `macnotesapp-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2022-07-05 13:26:35.000000 macnotesapp-0.5.1/LICENSE
--rw-r--r--   0        0        0     6049 2023-01-02 17:47:31.455563 macnotesapp-0.5.1/README.md
--rw-r--r--   0        0        0      235 2023-01-02 17:47:31.458212 macnotesapp-0.5.1/macnotesapp/__init__.py
--rw-r--r--   0        0        0      108 2022-07-09 11:42:28.000000 macnotesapp-0.5.1/macnotesapp/__main__.py
--rw-r--r--   0        0        0       43 2023-03-14 19:52:32.880007 macnotesapp-0.5.1/macnotesapp/_version.py
--rw-r--r--   0        0        0       53 2022-07-09 11:39:36.000000 macnotesapp-0.5.1/macnotesapp/cli/__init__.py
--rw-r--r--   0        0        0    15167 2023-01-02 17:47:31.458651 macnotesapp-0.5.1/macnotesapp/cli/cli.py
--rw-r--r--   0        0        0     2555 2022-07-12 14:10:32.000000 macnotesapp-0.5.1/macnotesapp/cli/cli_config.py
--rw-r--r--   0        0        0     8287 2022-07-15 16:46:52.000000 macnotesapp-0.5.1/macnotesapp/cli/cli_help.py
--rw-r--r--   0        0        0      305 2022-07-17 16:50:09.000000 macnotesapp-0.5.1/macnotesapp/cli/cli_param_types.py
--rw-r--r--   0        0        0     8588 2022-07-15 16:31:00.000000 macnotesapp-0.5.1/macnotesapp/cli/click_rich_echo.py
--rw-r--r--   0        0        0      754 2022-07-17 15:34:08.000000 macnotesapp-0.5.1/macnotesapp/cli/readable.py
--rw-r--r--   0        0        0    13597 2023-03-14 19:52:32.880448 macnotesapp-0.5.1/macnotesapp/macnotesapp.applescript
--rw-r--r--   0        0        0    13931 2023-03-14 19:52:32.880866 macnotesapp-0.5.1/macnotesapp/macnotesapp_applescript.py
--rw-r--r--   0        0        0    28174 2023-03-14 19:52:32.881595 macnotesapp-0.5.1/macnotesapp/notesapp.py
--rw-r--r--   0        0        0      349 2023-01-02 17:47:31.460565 macnotesapp-0.5.1/macnotesapp/script_loader.py
--rw-r--r--   0        0        0      384 2023-01-02 17:47:31.460806 macnotesapp-0.5.1/macnotesapp/utils.py
--rw-r--r--   0        0        0     1329 2023-03-14 19:52:32.882361 macnotesapp-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7360 1970-01-01 00:00:00.000000 macnotesapp-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-07-05 13:26:35.000000 macnotesapp-0.5.2/LICENSE
+-rw-r--r--   0        0        0     6049 2023-01-02 17:47:31.455563 macnotesapp-0.5.2/README.md
+-rw-r--r--   0        0        0      235 2023-01-02 17:47:31.458212 macnotesapp-0.5.2/macnotesapp/__init__.py
+-rw-r--r--   0        0        0      108 2022-07-09 11:42:28.000000 macnotesapp-0.5.2/macnotesapp/__main__.py
+-rw-r--r--   0        0        0       43 2023-06-09 12:42:16.409838 macnotesapp-0.5.2/macnotesapp/_version.py
+-rw-r--r--   0        0        0       53 2022-07-09 11:39:36.000000 macnotesapp-0.5.2/macnotesapp/cli/__init__.py
+-rw-r--r--   0        0        0    15167 2023-06-09 12:22:23.557260 macnotesapp-0.5.2/macnotesapp/cli/cli.py
+-rw-r--r--   0        0        0     2970 2023-06-09 12:34:38.053851 macnotesapp-0.5.2/macnotesapp/cli/cli_config.py
+-rw-r--r--   0        0        0     8287 2022-07-15 16:46:52.000000 macnotesapp-0.5.2/macnotesapp/cli/cli_help.py
+-rw-r--r--   0        0        0      305 2022-07-17 16:50:09.000000 macnotesapp-0.5.2/macnotesapp/cli/cli_param_types.py
+-rw-r--r--   0        0        0     8588 2022-07-15 16:31:00.000000 macnotesapp-0.5.2/macnotesapp/cli/click_rich_echo.py
+-rw-r--r--   0        0        0      754 2022-07-17 15:34:08.000000 macnotesapp-0.5.2/macnotesapp/cli/readable.py
+-rw-r--r--   0        0        0    13597 2023-03-14 19:52:32.880448 macnotesapp-0.5.2/macnotesapp/macnotesapp.applescript
+-rw-r--r--   0        0        0    13931 2023-03-14 19:52:32.880866 macnotesapp-0.5.2/macnotesapp/macnotesapp_applescript.py
+-rw-r--r--   0        0        0    28174 2023-06-09 12:21:56.529276 macnotesapp-0.5.2/macnotesapp/notesapp.py
+-rw-r--r--   0        0        0      349 2023-01-02 17:47:31.460565 macnotesapp-0.5.2/macnotesapp/script_loader.py
+-rw-r--r--   0        0        0      384 2023-01-02 17:47:31.460806 macnotesapp-0.5.2/macnotesapp/utils.py
+-rw-r--r--   0        0        0     1354 2023-06-09 12:42:16.410156 macnotesapp-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7321 1970-01-01 00:00:00.000000 macnotesapp-0.5.2/PKG-INFO
```

### Comparing `macnotesapp-0.5.1/LICENSE` & `macnotesapp-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/README.md` & `macnotesapp-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/cli/cli.py` & `macnotesapp-0.5.2/macnotesapp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/cli/cli_config.py` & `macnotesapp-0.5.2/macnotesapp/cli/cli_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Simple config loader/writer for macnotesapp CLI"""
 
+from __future__ import annotations
+
 import os
 import pathlib
-from typing import Dict
 
 import toml
 
 from macnotesapp import NotesApp
 
 CONFIG_DIR = pathlib.Path("~/.config/macnotesapp").expanduser()
 CONFIG_FILE = CONFIG_DIR / "macnotesapp.toml"
@@ -16,28 +17,37 @@
 FORMAT_HTML = "HTML"
 FORMAT_MARKDOWN = "Markdown"
 FORMAT_OPTIONS = [FORMAT_PLAINTEXT, FORMAT_HTML, FORMAT_MARKDOWN]
 DEFAULT_FORMAT = FORMAT_PLAINTEXT
 DEFAULT_EDITOR = "$EDITOR"
 
 
+def fix_unicode(text: str) -> str:
+    """Fix unicode characters in text that on Ventura cause toml.dump to treat str as a list (#26)"""
+    return text.encode("utf-8").decode()
+
+
 class ConfigSettings:
     config_file = CONFIG_FILE
 
     def __init__(self):
         if not self.config_file.is_file():
             self._create_config_file()
 
-    def read(self) -> Dict:
+    def read(self) -> dict[str, str]:
         """Read data from config file"""
         data = toml.load(self.config_file)
-        return data.get("defaults", dict())
+        return data.get("defaults", {})
 
-    def write(self, settings: Dict):
+    def write(self, settings: dict[str, str]):
         """Write settings dict to config file"""
+        # on Ventura, unicode encoding can cause toml.dump to treat str as a list (#26)
+        settings = {
+            k: fix_unicode(v) if isinstance(v, str) else v for k, v in settings.items()
+        }
         data = {"defaults": settings}
         if not self.config_file.is_file():
             self._create_config_file()
         with open(self.config_file, "w") as fp:
             toml.dump(data, fp)
 
     @property
```

### Comparing `macnotesapp-0.5.1/macnotesapp/cli/cli_help.py` & `macnotesapp-0.5.2/macnotesapp/cli/cli_help.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/cli/click_rich_echo.py` & `macnotesapp-0.5.2/macnotesapp/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/cli/readable.py` & `macnotesapp-0.5.2/macnotesapp/cli/readable.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/macnotesapp.applescript` & `macnotesapp-0.5.2/macnotesapp/macnotesapp.applescript`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/macnotesapp_applescript.py` & `macnotesapp-0.5.2/macnotesapp/macnotesapp_applescript.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/macnotesapp/notesapp.py` & `macnotesapp-0.5.2/macnotesapp/notesapp.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.1/pyproject.toml` & `macnotesapp-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "macnotesapp"
-version = "0.5.1"
+version = "0.5.2"
 description = "Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code."
 authors = ["Rhet Turnbull <rturnbull@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/RhetTbull/macnotesapp"
 repository = "https://github.com/RhetTbull/macnotesapp"
 keywords = ["cli", "mac", "macos"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12" # pyinstaller requires python < 3.12
 py-applescript = "^1.0.3"
 click = "^8.1.2"
 rich = "^12.4.4"
 markdown2 = "^2.4.3"
 toml = "^0.10.2"
 questionary = "^1.10.0"
 wheel = "^0.37.1"
 readability-lxml = "^0.8.1"
 requests = "^2.28.1"
 validators = "^0.20.0"
-textual = "^0.8.1"
 markdownify = "^0.11.6"
 pyobjc-framework-ScriptingBridge = "^9.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 cogapp = "^3.3.0"
 wheel = "^0.37.1"
```

### Comparing `macnotesapp-0.5.1/PKG-INFO` & `macnotesapp-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: macnotesapp
-Version: 0.5.1
+Version: 0.5.2
 Summary: Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code.
 Home-page: https://github.com/RhetTbull/macnotesapp
 License: MIT
 Keywords: cli,mac,macos
 Author: Rhet Turnbull
 Author-email: rturnbull@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: markdown2 (>=2.4.3,<3.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: py-applescript (>=1.0.3,<2.0.0)
 Requires-Dist: pyobjc-framework-ScriptingBridge (>=9.0.1,<10.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: readability-lxml (>=0.8.1,<0.9.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
-Requires-Dist: textual (>=0.8.1,<0.9.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: wheel (>=0.37.1,<0.38.0)
 Project-URL: Repository, https://github.com/RhetTbull/macnotesapp
 Description-Content-Type: text/markdown
 
 # MacNotesApp
```

