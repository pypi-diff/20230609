# Comparing `tmp/lofigui-0.1.0.tar.gz` & `tmp/lofigui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lofigui-0.1.0.tar", max compression
+gzip compressed data, was "lofigui-0.2.0.tar", max compression
```

## Comparing `lofigui-0.1.0.tar` & `lofigui-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1339 2023-06-09 10:36:32.228349 lofigui-0.1.0/README.md
--rwxr-xr-x   0        0        0       43 2023-05-12 08:49:23.228702 lofigui-0.1.0/lofigui/__init__.py
--rwxr-xr-x   0        0        0     1048 2023-05-12 13:33:22.331875 lofigui-0.1.0/lofigui/aprint.py
--rw-r--r--   0        0        0      302 2023-06-09 10:36:32.228349 lofigui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 lofigui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1339 2023-06-09 10:36:32.228349 lofigui-0.2.0/README.md
+-rw-r--r--   0        0        0      117 2023-06-09 11:23:33.589841 lofigui-0.2.0/lofigui/__init__.py
+-rw-r--r--   0        0        0      752 2023-06-09 11:23:33.589841 lofigui-0.2.0/lofigui/context.py
+-rw-r--r--   0        0        0     1247 2023-06-09 11:23:33.589841 lofigui-0.2.0/lofigui/markdown.py
+-rw-r--r--   0        0        0      748 2023-06-09 11:23:33.589841 lofigui-0.2.0/lofigui/options.py
+-rw-r--r--   0        0        0      281 2023-06-09 11:23:33.589841 lofigui-0.2.0/lofigui/print.py
+-rw-r--r--   0        0        0      322 2023-06-09 11:23:33.589841 lofigui-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lofigui-0.2.0/PKG-INFO
```

### Comparing `lofigui-0.1.0/README.md` & `lofigui-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lofigui-0.1.0/lofigui/aprint.py` & `lofigui-0.2.0/lofigui/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-import asyncio
-
-class PrintContext:
-    def __init__(self):
-        self.queue = asyncio.Queue()
-        self.buffer = ""  # This is a results buffer
-
-    def read(self):
-        if self.queue.empty():
-            return
-        response = ""
-        while not self.queue.empty():
-            # Get a "work item" out of the queue.
-            response += self.queue.get_nowait()
-            self.queue.task_done()
-        self.buffer += response
-
-
-# Slightly more involved but allows both single threaded use and option multithreaded
-_ctx = PrintContext()
-
-def aprint(msg="", ctx=None, end="\n"):
-    if ctx is None:
-        ctx = _ctx
-    if end == "\n":
-        ctx.queue.put_nowait(f"<p>{msg}</p>")
-    else:
-        ctx.queue.put_nowait(f"&nbsp;{msg}&nbsp;")
-    # await asyncio.sleep(0)  # Allow breaks
-
-def abuffer(ctx=None):
-    if ctx is None:
-        ctx = _ctx
-    ctx.read()  # drain buffer
-    return ctx.buffer
-
-def areset(ctx=None):
-    if ctx is None:
-        ctx = _ctx
-    ctx.buffer = ""
-
+import asyncio
+
+
+class PrintContext:
+    def __init__(self):
+        self.queue = asyncio.Queue()
+        self.buffer = ""  # This is a results buffer
+
+    def read(self):
+        if self.queue.empty():
+            return
+        response = ""
+        while not self.queue.empty():
+            # Get a "work item" out of the queue.
+            response += self.queue.get_nowait()
+            self.queue.task_done()
+        self.buffer += response
+
+
+# Slightly more involved but allows both single threaded use and option multithreaded
+_ctx = PrintContext()
+
+def buffer(ctx=None):
+    if ctx is None:
+        ctx = _ctx
+    ctx.read()  # drain buffer
+    return ctx.buffer
+
+def reset(ctx=None):
+    if ctx is None:
+        ctx = _ctx
+    ctx.buffer = ""
```

### Comparing `lofigui-0.1.0/PKG-INFO` & `lofigui-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: lofigui
-Version: 0.1.0
+Version: 0.2.0
 Summary: Lofi GUI tooling
 License: MIT
 Author: Humphrey Drummond
 Author-email: hum3@drummond.info
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: markdown (>=3.4.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 # lofigui
 
 This is tooling for me as a go and python programmer to provide really simple front ends.  They serve the same area as:
 
 It provides a way to build a very simple web app that can be bundled if required.
```

