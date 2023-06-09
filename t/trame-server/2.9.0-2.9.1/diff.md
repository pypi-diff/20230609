# Comparing `tmp/trame-server-2.9.0.tar.gz` & `tmp/trame-server-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-server-2.9.0.tar", last modified: Wed Feb  8 17:37:10 2023, max compression
+gzip compressed data, was "trame-server-2.9.1.tar", last modified: Wed Feb 15 18:48:29 2023, max compression
```

## Comparing `trame-server-2.9.0.tar` & `trame-server-2.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 17:37:10.428373 trame-server-2.9.0/
--rw-r--r--   0 root         (0) root         (0)      552 2023-02-08 17:37:07.000000 trame-server-2.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-08 17:37:07.000000 trame-server-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4318 2023-02-08 17:37:10.428373 trame-server-2.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3585 2023-02-08 17:37:07.000000 trame-server-2.9.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      888 2023-02-08 17:37:10.428373 trame-server-2.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-08 17:37:07.000000 trame-server-2.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 17:37:10.428373 trame-server-2.9.0/trame_server/
--rw-r--r--   0 root         (0) root         (0)      552 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/LICENSE
--rw-r--r--   0 root         (0) root         (0)      170 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10410 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/controller.py
--rw-r--r--   0 root         (0) root         (0)    20512 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/core.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/protocol.py
--rw-r--r--   0 root         (0) root         (0)     6754 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/state.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 17:37:10.428373 trame-server-2.9.0/trame_server/utils/
--rw-r--r--   0 root         (0) root         (0)     2636 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/browser.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/desktop.py
--rw-r--r--   0 root         (0) root         (0)     9859 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/hot_reload.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/server.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-02-08 17:37:07.000000 trame-server-2.9.0/trame_server/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 17:37:10.428373 trame-server-2.9.0/trame_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4318 2023-02-08 17:37:10.000000 trame-server-2.9.0/trame_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      635 2023-02-08 17:37:10.000000 trame-server-2.9.0/trame_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 17:37:10.000000 trame-server-2.9.0/trame_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-08 17:37:10.000000 trame-server-2.9.0/trame_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-08 17:37:10.000000 trame-server-2.9.0/trame_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.024079 trame-server-2.9.1/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-02-15 18:48:25.000000 trame-server-2.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-02-15 18:48:25.000000 trame-server-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-02-15 18:48:29.024079 trame-server-2.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-02-15 18:48:25.000000 trame-server-2.9.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      888 2023-02-15 18:48:29.024079 trame-server-2.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 18:48:25.000000 trame-server-2.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.020079 trame-server-2.9.1/trame_server/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      170 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10511 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/controller.py
+-rw-r--r--   0 root         (0) root         (0)    20952 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/core.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/state.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.024079 trame-server-2.9.1/trame_server/utils/
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/browser.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/desktop.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/hot_reload.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/server.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.020079 trame-server-2.9.1/trame_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      635 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/top_level.txt
```

### Comparing `trame-server-2.9.0/LICENSE` & `trame-server-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/PKG-INFO` & `trame-server-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-server
-Version: 2.9.0
+Version: 2.9.1
 Summary: Internal server side implementation of trame
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-server-2.9.0/README.rst` & `trame-server-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/setup.cfg` & `trame-server-2.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-server
-version = 2.9.0
+version = 2.9.1
 description = Internal server side implementation of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-server-2.9.0/trame_server/LICENSE` & `trame-server-2.9.1/trame_server/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/controller.py` & `trame-server-2.9.1/trame_server/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         self.name = name
         self.func = func
         self.funcs = set()
         self.task_funcs = set()
         self.funcs_once = set()
 
     def __call__(self, *args, **kwargs):
-        if self.func is None and len(self.funcs) == 0:
+        if self.func is None and len(self.funcs) + len(self.task_funcs) == 0:
             raise FunctionNotImplementedError(self.name)
 
         copy_list = list(self.funcs) + list(self.funcs_once)
         self.funcs_once.clear()
 
         # Exec main function first
         result = None
@@ -283,21 +283,23 @@
         results = list(map(lambda f: f(*args, **kwargs), copy_list))
 
         # Schedule any task
         for task_fn in list(self.task_funcs):
             if self.hot_reload:
                 task_fn = reload(task_fn)
 
-            asynchronous.create_task(task_fn(*args, **kwargs))
+            results.append(asynchronous.create_task(task_fn(*args, **kwargs)))
 
         # Figure out return
         if self.func is None:
             return results
         elif len(copy_list):
             return [result, *results]
+        elif len(self.task_funcs):
+            return results
         return result
 
     def once(self, func):
         """
         Add function to the set of functions to be called when
         the current ControllerFunction is called.
         After first execution, the function will automatically be removed.
```

### Comparing `trame-server-2.9.0/trame_server/core.py` & `trame-server-2.9.1/trame_server/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import asyncio
+import inspect
 import logging
 import os
 import sys
 
 from . import utils
 
 from .state import State
@@ -555,15 +556,24 @@
             },
         )
 
         # Manage exit life cycle unless coroutine
         if exec_mode == "main":
             self._running_stage = 0
             if self.controller.on_server_exited.exists():
-                self.controller.on_server_exited(**self.state.to_dict())
+                loop = asyncio.get_event_loop()
+                for exit_task in self.controller.on_server_exited(
+                    **self.state.to_dict()
+                ):
+                    if inspect.isawaitable(exit_task):
+                        loop.run_until_complete(exit_task)
+                    elif callable(exit_task):
+                        result = exit_task()
+                        if inspect.isawaitable(result):
+                            loop.run_until_complete(result)
         elif hasattr(task, "add_done_callback"):
 
             def on_done(task: asyncio.Task) -> None:
                 try:
                     task.result()
                     self._running_stage = 0
                     if self.controller.on_server_exited.exists():
```

### Comparing `trame-server-2.9.0/trame_server/protocol.py` & `trame-server-2.9.1/trame_server/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/state.py` & `trame-server-2.9.1/trame_server/state.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/ui.py` & `trame-server-2.9.1/trame_server/ui.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/__init__.py` & `trame-server-2.9.1/trame_server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/asynchronous.py` & `trame-server-2.9.1/trame_server/utils/asynchronous.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/desktop.py` & `trame-server-2.9.1/trame_server/utils/desktop.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/hot_reload.py` & `trame-server-2.9.1/trame_server/utils/hot_reload.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/logger.py` & `trame-server-2.9.1/trame_server/utils/logger.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/server.py` & `trame-server-2.9.1/trame_server/utils/server.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server/utils/version.py` & `trame-server-2.9.1/trame_server/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.0/trame_server.egg-info/PKG-INFO` & `trame-server-2.9.1/trame_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-server
-Version: 2.9.0
+Version: 2.9.1
 Summary: Internal server side implementation of trame
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-server-2.9.0/trame_server.egg-info/SOURCES.txt` & `trame-server-2.9.1/trame_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

