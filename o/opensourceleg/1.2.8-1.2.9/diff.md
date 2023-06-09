# Comparing `tmp/opensourceleg-1.2.8.tar.gz` & `tmp/opensourceleg-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.8.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.9.tar", max compression
```

## Comparing `opensourceleg-1.2.8.tar` & `opensourceleg-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.8/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.8/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.8/opensourceleg/__init__.py
--rw-r--r--   0        0        0    22954 2023-06-08 20:35:27.080440 opensourceleg-1.2.8/opensourceleg/actuators.py
--rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.8/opensourceleg/ankle_encoder_map.npy
--rw-r--r--   0        0        0     1156 2023-06-08 20:36:58.593678 opensourceleg-1.2.8/opensourceleg/constants.py
--rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.8/opensourceleg/control.py
--rw-r--r--   0        0        0     7480 2023-06-08 20:40:33.324884 opensourceleg-1.2.8/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.8/opensourceleg/example.py
--rw-r--r--   0        0        0    12114 2023-06-08 20:40:33.361500 opensourceleg-1.2.8/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.8/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.8/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3715 2023-06-08 20:37:48.671909 opensourceleg-1.2.8/opensourceleg/logger.py
--rw-r--r--   0        0        0    17657 2023-06-08 20:40:33.336090 opensourceleg-1.2.8/opensourceleg/osl.py
--rw-r--r--   0        0        0    15011 2023-06-08 20:34:58.232056 opensourceleg-1.2.8/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.8/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21242 2023-06-07 02:24:24.140310 opensourceleg-1.2.8/opensourceleg/tui.py
--rw-r--r--   0        0        0     4341 2023-06-07 17:03:13.722676 opensourceleg-1.2.8/opensourceleg/units.py
--rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.8/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-06-08 20:42:26.928688 opensourceleg-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.9/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.9/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.9/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    22954 2023-06-08 20:35:27.080440 opensourceleg-1.2.9/opensourceleg/actuators.py
+-rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.9/opensourceleg/ankle_encoder_map.npy
+-rw-r--r--   0        0        0     1156 2023-06-08 20:36:58.593678 opensourceleg-1.2.9/opensourceleg/constants.py
+-rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.9/opensourceleg/control.py
+-rw-r--r--   0        0        0     7467 2023-06-08 21:22:22.592686 opensourceleg-1.2.9/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.9/opensourceleg/example.py
+-rw-r--r--   0        0        0    12114 2023-06-08 20:40:33.361500 opensourceleg-1.2.9/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.9/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.9/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3715 2023-06-08 20:37:48.671909 opensourceleg-1.2.9/opensourceleg/logger.py
+-rw-r--r--   0        0        0    17657 2023-06-08 20:54:43.797417 opensourceleg-1.2.9/opensourceleg/osl.py
+-rw-r--r--   0        0        0    15011 2023-06-08 20:34:58.232056 opensourceleg-1.2.9/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.9/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21249 2023-06-08 21:23:29.300687 opensourceleg-1.2.9/opensourceleg/tui.py
+-rw-r--r--   0        0        0     4341 2023-06-07 17:03:13.722676 opensourceleg-1.2.9/opensourceleg/units.py
+-rw-r--r--   0        0        0    11587 2023-06-08 21:22:53.520289 opensourceleg-1.2.9/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-08 21:23:44.428681 opensourceleg-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.9/PKG-INFO
```

### Comparing `opensourceleg-1.2.8/LICENSE` & `opensourceleg-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/README.md` & `opensourceleg-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/actuators.py` & `opensourceleg-1.2.9/opensourceleg/actuators.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/constants.py` & `opensourceleg-1.2.9/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/control.py` & `opensourceleg-1.2.9/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/demo.py` & `opensourceleg-1.2.9/opensourceleg/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import time
-
 from opensourceleg.osl import OpenSourceLeg
 from opensourceleg.state_machine import Event, State
 
 # ------------- FSM PARAMETERS ---------------- #
 
 BODY_WEIGHT = 60
```

### Comparing `opensourceleg-1.2.8/opensourceleg/joints.py` & `opensourceleg-1.2.9/opensourceleg/joints.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/loadcell.py` & `opensourceleg-1.2.9/opensourceleg/loadcell.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/logger.py` & `opensourceleg-1.2.9/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/osl.py` & `opensourceleg-1.2.9/opensourceleg/osl.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/state_machine.py` & `opensourceleg-1.2.9/opensourceleg/state_machine.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/thermal.py` & `opensourceleg-1.2.9/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/tui.py` & `opensourceleg-1.2.9/opensourceleg/tui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable
 
 import threading
 import time
+from dataclasses import dataclass
 
 import TermTk as ttk
-from attr import dataclass
 from TermTk.TTkCore.string import TTkString
 
 
 # create a dataclass for various colors (str: hex codes)
 @dataclass
 class Colors:
     red: str = "#ff0000"
```

### Comparing `opensourceleg-1.2.8/opensourceleg/units.py` & `opensourceleg-1.2.9/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/opensourceleg/utilities.py` & `opensourceleg-1.2.9/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.8/pyproject.toml` & `opensourceleg-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.8"
+version = "1.2.9"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.8/PKG-INFO` & `opensourceleg-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.8
+Version: 1.2.9
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

