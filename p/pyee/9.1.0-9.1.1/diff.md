# Comparing `tmp/pyee-9.1.0.tar.gz` & `tmp/pyee-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyee-9.1.0.tar", last modified: Sun Apr 30 22:14:02 2023, max compression
+gzip compressed data, was "pyee-9.1.1.tar", last modified: Fri Jun  9 06:09:06 2023, max compression
```

## Comparing `pyee-9.1.0.tar` & `pyee-9.1.1.tar`

### file list

```diff
@@ -1,36 +1,51 @@
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.412626 pyee-9.1.0/
--rw-r--r--   0 josh      (1000) josh      (1000)     7159 2023-04-30 22:13:43.000000 pyee-9.1.0/CHANGELOG.rst
--rw-r--r--   0 josh      (1000) josh      (1000)      518 2023-04-30 21:23:40.000000 pyee-9.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 josh      (1000) josh      (1000)     2518 2023-04-30 21:23:40.000000 pyee-9.1.0/DEVELOPMENT.rst
--rw-r--r--   0 josh      (1000) josh      (1000)     1080 2023-04-30 21:23:40.000000 pyee-9.1.0/LICENSE
--rw-r--r--   0 josh      (1000) josh      (1000)      177 2023-04-30 21:23:40.000000 pyee-9.1.0/MANIFEST.in
--rw-r--r--   0 josh      (1000) josh      (1000)     1699 2023-04-30 22:14:02.412626 pyee-9.1.0/PKG-INFO
--rw-r--r--   0 josh      (1000) josh      (1000)      811 2023-04-30 21:23:40.000000 pyee-9.1.0/README.rst
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.411626 pyee-9.1.0/pyee/
--rw-r--r--   0 josh      (1000) josh      (1000)     3728 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/__init__.py
--rw-r--r--   0 josh      (1000) josh      (1000)     2607 2023-04-30 22:03:07.000000 pyee-9.1.0/pyee/asyncio.py
--rw-r--r--   0 josh      (1000) josh      (1000)     8099 2023-04-30 21:55:18.000000 pyee-9.1.0/pyee/base.py
--rw-r--r--   0 josh      (1000) josh      (1000)     2913 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/cls.py
--rw-r--r--   0 josh      (1000) josh      (1000)     2463 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/executor.py
--rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/py.typed
--rw-r--r--   0 josh      (1000) josh      (1000)     4520 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/trio.py
--rw-r--r--   0 josh      (1000) josh      (1000)     3005 2023-04-30 21:55:18.000000 pyee-9.1.0/pyee/twisted.py
--rw-r--r--   0 josh      (1000) josh      (1000)     6611 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/uplift.py
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.411626 pyee-9.1.0/pyee.egg-info/
--rw-r--r--   0 josh      (1000) josh      (1000)     1699 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/PKG-INFO
--rw-r--r--   0 josh      (1000) josh      (1000)      543 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/SOURCES.txt
--rw-r--r--   0 josh      (1000) josh      (1000)        1 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/dependency_links.txt
--rw-r--r--   0 josh      (1000) josh      (1000)       18 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/requires.txt
--rw-r--r--   0 josh      (1000) josh      (1000)        5 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/top_level.txt
--rw-r--r--   0 josh      (1000) josh      (1000)       98 2023-04-30 21:23:40.000000 pyee-9.1.0/pyproject.toml
--rw-r--r--   0 josh      (1000) josh      (1000)       90 2023-04-30 22:14:02.412626 pyee-9.1.0/setup.cfg
--rw-r--r--   0 josh      (1000) josh      (1000)     1324 2023-04-30 22:13:43.000000 pyee-9.1.0/setup.py
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.412626 pyee-9.1.0/tests/
--rw-r--r--   0 josh      (1000) josh      (1000)      235 2023-04-30 21:23:40.000000 pyee-9.1.0/tests/conftest.py
--rw-r--r--   0 josh      (1000) josh      (1000)     4018 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_async.py
--rw-r--r--   0 josh      (1000) josh      (1000)     1003 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_cls.py
--rw-r--r--   0 josh      (1000) josh      (1000)     1245 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_executor.py
--rw-r--r--   0 josh      (1000) josh      (1000)     6297 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_sync.py
--rw-r--r--   0 josh      (1000) josh      (1000)     2444 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_trio.py
--rw-r--r--   0 josh      (1000) josh      (1000)     1860 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_twisted.py
--rw-r--r--   0 josh      (1000) josh      (1000)     6318 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_uplift.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.716785 pyee-9.1.1/
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.711785 pyee-9.1.1/.github/
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.714785 pyee-9.1.1/.github/workflows/
+-rw-r--r--   0 josh      (1000) josh      (1000)      893 2023-06-09 05:56:39.000000 pyee-9.1.1/.github/workflows/qa.yaml
+-rw-r--r--   0 josh      (1000) josh      (1000)      146 2023-04-30 21:23:40.000000 pyee-9.1.1/.gitignore
+-rw-r--r--   0 josh      (1000) josh      (1000)      147 2023-06-09 05:56:39.000000 pyee-9.1.1/.readthedocs.yaml
+-rw-r--r--   0 josh      (1000) josh      (1000)     7244 2023-06-09 06:08:07.000000 pyee-9.1.1/CHANGELOG.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)      518 2023-06-09 05:56:39.000000 pyee-9.1.1/CONTRIBUTORS.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)     2518 2023-06-09 05:56:39.000000 pyee-9.1.1/DEVELOPMENT.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)     1080 2023-04-30 21:23:40.000000 pyee-9.1.1/LICENSE
+-rw-r--r--   0 josh      (1000) josh      (1000)      177 2023-04-30 21:23:40.000000 pyee-9.1.1/MANIFEST.in
+-rw-r--r--   0 josh      (1000) josh      (1000)     1699 2023-06-09 06:09:06.716785 pyee-9.1.1/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)      811 2023-06-09 05:56:39.000000 pyee-9.1.1/README.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)      222 2023-06-09 05:56:39.000000 pyee-9.1.1/environment.yml
+-rw-r--r--   0 josh      (1000) josh      (1000)     1010 2023-04-30 21:32:47.000000 pyee-9.1.1/package-lock.json
+-rw-r--r--   0 josh      (1000) josh      (1000)      523 2023-04-30 21:23:40.000000 pyee-9.1.1/package.json
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.714785 pyee-9.1.1/pyee/
+-rw-r--r--   0 josh      (1000) josh      (1000)     3728 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/__init__.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2732 2023-06-09 06:08:07.000000 pyee-9.1.1/pyee/asyncio.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     8099 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/base.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2913 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/cls.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2463 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/executor.py
+-rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-04-30 21:23:40.000000 pyee-9.1.1/pyee/py.typed
+-rw-r--r--   0 josh      (1000) josh      (1000)     4520 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/trio.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     3005 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/twisted.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6611 2023-06-09 05:56:39.000000 pyee-9.1.1/pyee/uplift.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.715785 pyee-9.1.1/pyee.egg-info/
+-rw-r--r--   0 josh      (1000) josh      (1000)     1699 2023-06-09 06:09:06.000000 pyee-9.1.1/pyee.egg-info/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)      726 2023-06-09 06:09:06.000000 pyee-9.1.1/pyee.egg-info/SOURCES.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        1 2023-06-09 06:09:06.000000 pyee-9.1.1/pyee.egg-info/dependency_links.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       18 2023-06-09 06:09:06.000000 pyee-9.1.1/pyee.egg-info/requires.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        5 2023-06-09 06:09:06.000000 pyee-9.1.1/pyee.egg-info/top_level.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       98 2023-06-09 05:56:39.000000 pyee-9.1.1/pyproject.toml
+-rw-r--r--   0 josh      (1000) josh      (1000)       25 2023-06-09 05:56:39.000000 pyee-9.1.1/requirements.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)      279 2023-06-09 05:56:39.000000 pyee-9.1.1/requirements_dev.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       90 2023-06-09 06:09:06.716785 pyee-9.1.1/setup.cfg
+-rw-r--r--   0 josh      (1000) josh      (1000)     1324 2023-06-09 06:08:07.000000 pyee-9.1.1/setup.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.715785 pyee-9.1.1/tests/
+-rw-r--r--   0 josh      (1000) josh      (1000)      235 2023-04-30 21:23:40.000000 pyee-9.1.1/tests/conftest.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     4051 2023-06-09 06:08:07.000000 pyee-9.1.1/tests/test_async.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1003 2023-04-30 21:55:18.000000 pyee-9.1.1/tests/test_cls.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1245 2023-04-30 21:55:18.000000 pyee-9.1.1/tests/test_executor.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6297 2023-04-30 21:55:18.000000 pyee-9.1.1/tests/test_sync.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2444 2023-04-30 21:55:18.000000 pyee-9.1.1/tests/test_trio.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1860 2023-04-30 21:55:18.000000 pyee-9.1.1/tests/test_twisted.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6318 2023-04-30 21:55:18.000000 pyee-9.1.1/tests/test_uplift.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      121 2023-06-09 05:56:39.000000 pyee-9.1.1/tox.ini
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.712785 pyee-9.1.1/typings/
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.712785 pyee-9.1.1/typings/twisted/
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-06-09 06:09:06.715785 pyee-9.1.1/typings/twisted/python/
+-rw-r--r--   0 josh      (1000) josh      (1000)       98 2023-04-30 21:23:40.000000 pyee-9.1.1/typings/twisted/python/failure.pyi
```

### Comparing `pyee-9.1.0/CHANGELOG.rst` & `pyee-9.1.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2023/06/08 Version 9.1.1
+------------------------
+
+- Store AsyncIO Futures in a set
+
 2023/04/30 Version 9.1.0
 ------------------------
 - ``EventEmitter`` supports pickling
 - Development dependencies updated to latest
 - Dependency on mock removed in favor of unittest.mock
 - Additional type hints so pyright check passes on latest
 - Drop 3.7 support
```

### Comparing `pyee-9.1.0/CONTRIBUTORS.rst` & `pyee-9.1.1/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/DEVELOPMENT.rst` & `pyee-9.1.1/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/LICENSE` & `pyee-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/PKG-INFO` & `pyee-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyee
-Version: 9.1.0
+Version: 9.1.1
 Summary: A port of node.js's EventEmitter to python.
 Home-page: https://github.com/jfhbrook/pyee
 Author: Josh Holbrook
 Author-email: josh.holbrook@gmail.com
 License: MIT
 Keywords: events,emitter,node.js,node,eventemitter,event_emitter
 Platform: UNKNOWN
```

### Comparing `pyee-9.1.0/README.rst` & `pyee-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/__init__.py` & `pyee-9.1.1/pyee/__init__.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/asyncio.py` & `pyee-9.1.1/pyee/asyncio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from asyncio import AbstractEventLoop, ensure_future, Future, iscoroutine
-from typing import Any, Callable, cast, Dict, Optional, Tuple
+from typing import Any, Callable, cast, Dict, Optional, Set, Tuple
 
 from pyee.base import EventEmitter
 
 __all__ = ["AsyncIOEventEmitter"]
 
 
 class AsyncIOEventEmitter(EventEmitter):
@@ -33,14 +33,15 @@
     In other words, you do not have to await any results from emit, and the
     coroutine is scheduled in a fire-and-forget fashion.
     """
 
     def __init__(self, loop: Optional[AbstractEventLoop] = None):
         super(AsyncIOEventEmitter, self).__init__()
         self._loop: Optional[AbstractEventLoop] = loop
+        self._waiting: Set[Future] = set()
 
     def _emit_run(
         self,
         f: Callable,
         args: Tuple[Any, ...],
         kwargs: Dict[str, Any],
     ):
@@ -53,21 +54,25 @@
                 if self._loop:
                     # ensure_future is *extremely* cranky about the types here,
                     # but this is relatively well-tested and I think the types
                     # are more strict than they should be
                     fut: Any = ensure_future(cast(Any, coro), loop=self._loop)
                 else:
                     fut = ensure_future(cast(Any, coro))
+
             elif isinstance(coro, Future):
                 fut = cast(Any, coro)
             else:
                 return
 
             def callback(f):
+                self._waiting.remove(f)
+
                 if f.cancelled():
                     return
 
                 exc: Exception = f.exception()
                 if exc:
                     self.emit("error", exc)
 
             fut.add_done_callback(callback)
+            self._waiting.add(fut)
```

### Comparing `pyee-9.1.0/pyee/base.py` & `pyee-9.1.1/pyee/base.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/cls.py` & `pyee-9.1.1/pyee/cls.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/executor.py` & `pyee-9.1.1/pyee/executor.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/trio.py` & `pyee-9.1.1/pyee/trio.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/twisted.py` & `pyee-9.1.1/pyee/twisted.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee/uplift.py` & `pyee-9.1.1/pyee/uplift.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/pyee.egg-info/PKG-INFO` & `pyee-9.1.1/pyee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyee
-Version: 9.1.0
+Version: 9.1.1
 Summary: A port of node.js's EventEmitter to python.
 Home-page: https://github.com/jfhbrook/pyee
 Author: Josh Holbrook
 Author-email: josh.holbrook@gmail.com
 License: MIT
 Keywords: events,emitter,node.js,node,eventemitter,event_emitter
 Platform: UNKNOWN
```

### Comparing `pyee-9.1.0/setup.py` & `pyee-9.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README_rst = path.join(path.abspath(path.dirname(__file__)), "README.rst")
 
 with open(README_rst, "r") as f:
     long_description = f.read()
 
 setup(
     name="pyee",
-    version="9.1.0",
+    version="9.1.1",
     packages=find_packages(),
     include_package_data=True,
     description="A port of node.js's EventEmitter to python.",
     long_description=long_description,
     author="Josh Holbrook",
     author_email="josh.holbrook@gmail.com",
     url="https://github.com/jfhbrook/pyee",
```

### Comparing `pyee-9.1.0/tests/test_async.py` & `pyee-9.1.1/tests/test_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         should_call.set_result(True)
 
     ee.emit("event")
 
     result = await wait_for(should_call, 0.1)
 
     assert result is True
+    assert len(ee._waiting) == 0
 
 
 @pytest.mark.asyncio
 async def test_asyncio_once_emit(event_loop):
     """Test that AsyncIOEventEmitter also wrap coroutines when
     using once
     """
```

### Comparing `pyee-9.1.0/tests/test_cls.py` & `pyee-9.1.1/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/tests/test_executor.py` & `pyee-9.1.1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/tests/test_sync.py` & `pyee-9.1.1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/tests/test_trio.py` & `pyee-9.1.1/tests/test_trio.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/tests/test_twisted.py` & `pyee-9.1.1/tests/test_twisted.py`

 * *Files identical despite different names*

### Comparing `pyee-9.1.0/tests/test_uplift.py` & `pyee-9.1.1/tests/test_uplift.py`

 * *Files identical despite different names*

