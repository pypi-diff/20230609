# Comparing `tmp/pyCANape-0.6.0.tar.gz` & `tmp/pyCANape-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCANape-0.6.0.tar", last modified: Sun Mar 19 16:53:54 2023, max compression
+gzip compressed data, was "pyCANape-0.6.1.tar", last modified: Fri Jun  9 12:28:15 2023, max compression
```

## Comparing `pyCANape-0.6.0.tar` & `pyCANape-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 16:53:54.984669 pyCANape-0.6.0/
--rw-rw-rw-   0        0        0     1112 2023-03-19 16:53:05.000000 pyCANape-0.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2961 2023-03-19 16:53:54.984669 pyCANape-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2242 2023-03-19 16:53:05.000000 pyCANape-0.6.0/README.md
--rw-rw-rw-   0        0        0     2464 2023-03-19 16:53:05.000000 pyCANape-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-19 16:53:54.984669 pyCANape-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-19 16:53:54.969044 pyCANape-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-19 16:53:54.969044 pyCANape-0.6.0/src/pyCANape.egg-info/
--rw-rw-rw-   0        0        0     2961 2023-03-19 16:53:54.000000 pyCANape-0.6.0/src/pyCANape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      624 2023-03-19 16:53:54.000000 pyCANape-0.6.0/src/pyCANape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 16:53:54.000000 pyCANape-0.6.0/src/pyCANape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-03-19 16:53:54.000000 pyCANape-0.6.0/src/pyCANape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-19 16:53:54.000000 pyCANape-0.6.0/src/pyCANape.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-19 16:53:54.969044 pyCANape-0.6.0/src/pycanape/
--rw-rw-rw-   0        0        0      768 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/__init__.py
--rw-rw-rw-   0        0        0    13292 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/calibration_object.py
--rw-rw-rw-   0        0        0    17741 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/canape.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:53:54.984669 pyCANape-0.6.0/src/pycanape/cnp_api/
--rw-rw-rw-   0        0        0      114 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/cnp_api/__init__.py
--rw-rw-rw-   0        0        0     9629 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/cnp_api/cnp_class.py
--rw-rw-rw-   0        0        0    20101 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/cnp_api/cnp_constants.py
--rw-rw-rw-   0        0        0    30066 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/cnp_api/cnp_prototype.py
--rw-rw-rw-   0        0        0      229 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/config.py
--rw-rw-rw-   0        0        0     4032 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/daq.py
--rw-rw-rw-   0        0        0     5339 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/ecu_task.py
--rw-rw-rw-   0        0        0    11744 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/module.py
--rw-rw-rw-   0        0        0        0 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/py.typed
--rw-rw-rw-   0        0        0     4559 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/recorder.py
--rw-rw-rw-   0        0        0     3453 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/script.py
--rw-rw-rw-   0        0        0     3743 2023-03-19 16:53:05.000000 pyCANape-0.6.0/src/pycanape/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:28:15.299025 pyCANape-0.6.1/
+-rw-rw-rw-   0        0        0     1112 2023-06-09 12:27:41.000000 pyCANape-0.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2961 2023-06-09 12:28:15.299025 pyCANape-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2242 2023-06-09 12:27:41.000000 pyCANape-0.6.1/README.md
+-rw-rw-rw-   0        0        0     2361 2023-06-09 12:27:41.000000 pyCANape-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 12:28:15.299025 pyCANape-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 12:28:15.283401 pyCANape-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 12:28:15.283401 pyCANape-0.6.1/src/pyCANape.egg-info/
+-rw-rw-rw-   0        0        0     2961 2023-06-09 12:28:15.000000 pyCANape-0.6.1/src/pyCANape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      624 2023-06-09 12:28:15.000000 pyCANape-0.6.1/src/pyCANape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 12:28:15.000000 pyCANape-0.6.1/src/pyCANape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-06-09 12:28:15.000000 pyCANape-0.6.1/src/pyCANape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 12:28:15.000000 pyCANape-0.6.1/src/pyCANape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 12:28:15.283401 pyCANape-0.6.1/src/pycanape/
+-rw-rw-rw-   0        0        0     1544 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/__init__.py
+-rw-rw-rw-   0        0        0    13292 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/calibration_object.py
+-rw-rw-rw-   0        0        0    17741 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/canape.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:28:15.299025 pyCANape-0.6.1/src/pycanape/cnp_api/
+-rw-rw-rw-   0        0        0      194 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/cnp_api/__init__.py
+-rw-rw-rw-   0        0        0     9629 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/cnp_api/cnp_class.py
+-rw-rw-rw-   0        0        0    20101 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/cnp_api/cnp_constants.py
+-rw-rw-rw-   0        0        0    30247 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/cnp_api/cnp_prototype.py
+-rw-rw-rw-   0        0        0      229 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/config.py
+-rw-rw-rw-   0        0        0     4032 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/daq.py
+-rw-rw-rw-   0        0        0     5339 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/ecu_task.py
+-rw-rw-rw-   0        0        0    11743 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/module.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/py.typed
+-rw-rw-rw-   0        0        0     4559 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/recorder.py
+-rw-rw-rw-   0        0        0     4221 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/script.py
+-rw-rw-rw-   0        0        0     3765 2023-06-09 12:27:41.000000 pyCANape-0.6.1/src/pycanape/utils.py
```

### Comparing `pyCANape-0.6.0/LICENSE.txt` & `pyCANape-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/PKG-INFO` & `pyCANape-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCANape
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pythonic wrapper around the VECTOR CANape API
 Author-email: Artur Drogunow <artur.drogunow@zf.com>
 License: MIT
 Project-URL: Documentation, https://pycanape.readthedocs.io
 Project-URL: Issues, https://github.com/zariiii9003/pycanape/issues
 Project-URL: Source, https://github.com/zariiii9003/pycanape
 Project-URL: Homepage, https://github.com/zariiii9003/pycanape
```

### Comparing `pyCANape-0.6.0/README.md` & `pyCANape-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/pyproject.toml` & `pyCANape-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     "numpy>=1.21",
     "typing-extensions;python_version<'3.8'",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-    "black==23.1.*",
-    "ruff==0.0.257",
-    "mypy==1.1.*",
+    "black==23.3.*",
+    "ruff==0.0.271",
+    "mypy==1.3.*",
     "types-backports;python_version<'3.8'",
     "pre-commit",
 ]
 doc = [
     "furo",
     "sphinx==6.1.*",
 ]
@@ -105,12 +105,7 @@
 line-length = 100
 
 # Assume Python 3.7.
 target-version = "py37"
 
 [tool.ruff.isort]
 known-first-party = ["pycanape"]
-
-[tool.ruff.per-file-ignores]
-"src/pycanape/__init__.py" = [
-    "F401",  # imported but unused
-]
```

### Comparing `pyCANape-0.6.0/src/pyCANape.egg-info/PKG-INFO` & `pyCANape-0.6.1/src/pyCANape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCANape
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pythonic wrapper around the VECTOR CANape API
 Author-email: Artur Drogunow <artur.drogunow@zf.com>
 License: MIT
 Project-URL: Documentation, https://pycanape.readthedocs.io
 Project-URL: Issues, https://github.com/zariiii9003/pycanape/issues
 Project-URL: Source, https://github.com/zariiii9003/pycanape
 Project-URL: Homepage, https://github.com/zariiii9003/pycanape
```

### Comparing `pyCANape-0.6.0/src/pyCANape.egg-info/SOURCES.txt` & `pyCANape-0.6.1/src/pyCANape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/calibration_object.py` & `pyCANape-0.6.1/src/pycanape/calibration_object.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/canape.py` & `pyCANape-0.6.1/src/pycanape/canape.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/cnp_api/cnp_class.py` & `pyCANape-0.6.1/src/pycanape/cnp_api/cnp_class.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/cnp_api/cnp_constants.py` & `pyCANape-0.6.1/src/pycanape/cnp_api/cnp_constants.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/cnp_api/cnp_prototype.py` & `pyCANape-0.6.1/src/pycanape/cnp_api/cnp_prototype.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
 
 Asap3GetScriptResultString = CANAPEAPI.map_symbol(
     func_name="Asap3GetScriptResultString",
     restype=ctypes.c_bool,
     argtypes=[
         cnp_class.TAsap3Hdl,                    # > TAsap3Hdl hdl
         cnp_class.TScriptHdl,                   # > TScriptHdl hScript
-        ctypes.POINTER(ctypes.c_char_p),        # < char *resultString
+        ctypes.POINTER(ctypes.c_char),          # < char *resultString
         ctypes.POINTER(ctypes.c_ulong),         # < DWORD *sizeofBuffer
     ],
     errcheck=get_last_error,
 )
 
 Asap3GetScriptResultValue = CANAPEAPI.map_symbol(
     func_name="Asap3GetScriptResultValue",
@@ -790,15 +790,15 @@
 Asap3GetScriptState = CANAPEAPI.map_symbol(
     func_name="Asap3GetScriptState",
     restype=ctypes.c_bool,
     argtypes=[
         cnp_class.TAsap3Hdl,                    # > TAsap3Hdl hdl
         cnp_class.TScriptHdl,                   # > TScriptHdl hScript
         ctypes.POINTER(cnp_class.enum_type),    # < TScriptStatus *scrstate
-        ctypes.POINTER(ctypes.c_char_p),        # < char *textBuffer
+        ctypes.POINTER(ctypes.c_char),          # < char *textBuffer
         ctypes.POINTER(ctypes.c_ulong),         # < DWORD *sizeofBuffer
     ],
     errcheck=get_last_error,
 )
 
 Asap3ReleaseScript = CANAPEAPI.map_symbol(
     func_name="Asap3ReleaseScript",
@@ -812,14 +812,16 @@
 
 Asap3StartScript = CANAPEAPI.map_symbol(
     func_name="Asap3StartScript",
     restype=ctypes.c_bool,
     argtypes=[
         cnp_class.TAsap3Hdl,                    # > TAsap3Hdl hdl
         cnp_class.TScriptHdl,                   # > TScriptHdl hScript
+        ctypes.c_char_p,                        # > char *  Commandline = NULL
+        cnp_class.TModulHdl,                    # > TModulHdl  moduleHdl = ASAP3_INVALID_MODULE_HDL
     ],
     errcheck=get_last_error,
 )
 
 Asap3StopScript = CANAPEAPI.map_symbol(
     func_name="Asap3StopScript",
     restype=ctypes.c_bool,
```

### Comparing `pyCANape-0.6.0/src/pycanape/daq.py` & `pyCANape-0.6.1/src/pycanape/daq.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/ecu_task.py` & `pyCANape-0.6.1/src/pycanape/ecu_task.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/module.py` & `pyCANape-0.6.1/src/pycanape/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         :param script_file:
             Declares interpretation of parameter script.
             If 'script_file' is true, parameter 'script' is
             interpreted as the file name of the script file
             to be executed. If 'script_file' is false,
             'script' is interpreted as a single script command
         :param script:
-            A script filename or an single script command
+            A script filename or a single script command
         :return:
             The instance of the Script class
         """
         script_handle = TScriptHdl()
         cnp_prototype.Asap3ExecuteScriptEx(
             self.asap3_handle,
             self.module_handle,
```

### Comparing `pyCANape-0.6.0/src/pycanape/recorder.py` & `pyCANape-0.6.1/src/pycanape/recorder.py`

 * *Files identical despite different names*

### Comparing `pyCANape-0.6.0/src/pycanape/script.py` & `pyCANape-0.6.1/src/pycanape/script.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import ctypes
+from typing import TYPE_CHECKING, Optional
 
 from .cnp_api import cnp_class, cnp_constants
+from .cnp_api.cnp_constants import ASAP3_INVALID_MODULE_HDL
 from .config import RC
 
 try:
     from .cnp_api import cnp_prototype
 except FileNotFoundError:
     cnp_prototype = None  # type: ignore[assignment]
 
+if TYPE_CHECKING:
+    from .module import Module
+
 
 class Script:
     def __init__(
         self,
         asap3_handle: cnp_class.TAsap3Hdl,  # type: ignore[valid-type]
         script_handle: cnp_class.TScriptHdl,
     ) -> None:
@@ -45,19 +50,38 @@
             self.script_handle,
             ctypes.byref(scrstate),
             None,
             ctypes.byref(max_size),
         )
         return cnp_constants.TScriptStatus(scrstate.value)
 
-    def start_script(self) -> None:
-        """Starts the script."""
+    def start_script(
+        self,
+        *,
+        command_line: Optional[str] = None,
+        current_device: Optional["Module"] = None,
+    ) -> None:
+        """Starts the script.
+
+        :param command_line:
+            Set a commandline for the script.
+        :param current_device:
+            Set a module as current_device.
+        """
+        module_handle = (
+            current_device.module_handle
+            if current_device
+            else cnp_class.TModulHdl(ASAP3_INVALID_MODULE_HDL)
+        )
+        _command_line = command_line.encode(RC["ENCODING"]) if command_line else None
         cnp_prototype.Asap3StartScript(
             self.asap3_handle,
             self.script_handle,
+            _command_line,
+            module_handle,
         )
 
     def stop_script(self) -> None:
         """Stop the script."""
         cnp_prototype.Asap3StopScript(
             self.asap3_handle,
             self.script_handle,
```

### Comparing `pyCANape-0.6.0/src/pycanape/utils.py` & `pyCANape-0.6.1/src/pycanape/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,14 @@
             pass
         else:
             if proc_name.lower() in ("canape.exe", "canape64.exe"):
                 proc.kill()
 
 
 def get_canape_path() -> str:
-    key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, "SOFTWARE\\VECTOR\\CANape")
-    return winreg.QueryValueEx(key, "Path")[0]
+    with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, "SOFTWARE\\VECTOR\\CANape") as key:
+        return winreg.QueryValueEx(key, "Path")[0]
 
 
 def get_canape_datapath() -> str:
-    key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, "SOFTWARE\\VECTOR\\CANape")
-    return winreg.QueryValueEx(key, "DataPath")[0]
+    with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, "SOFTWARE\\VECTOR\\CANape") as key:
+        return winreg.QueryValueEx(key, "DataPath")[0]
```

