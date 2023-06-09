# Comparing `tmp/lofigui-0.2.1.tar.gz` & `tmp/lofigui-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lofigui-0.2.1.tar", max compression
+gzip compressed data, was "lofigui-0.2.2.tar", max compression
```

## Comparing `lofigui-0.2.1.tar` & `lofigui-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1981 2023-06-09 11:54:12.200982 lofigui-0.2.1/README.md
--rw-r--r--   0        0        0      117 2023-06-09 11:23:33.589841 lofigui-0.2.1/lofigui/__init__.py
--rw-r--r--   0        0        0      752 2023-06-09 11:23:33.589841 lofigui-0.2.1/lofigui/context.py
--rw-r--r--   0        0        0     1247 2023-06-09 11:23:33.589841 lofigui-0.2.1/lofigui/markdown.py
--rw-r--r--   0        0        0      748 2023-06-09 11:23:33.589841 lofigui-0.2.1/lofigui/options.py
--rw-r--r--   0        0        0      281 2023-06-09 11:23:33.589841 lofigui-0.2.1/lofigui/print.py
--rw-r--r--   0        0        0      340 2023-06-09 11:54:12.200982 lofigui-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 lofigui-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1981 2023-06-09 11:54:12.200982 lofigui-0.2.2/README.md
+-rw-r--r--   0        0        0      118 2023-06-09 11:55:58.042620 lofigui-0.2.2/lofigui/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-09 11:55:58.053453 lofigui-0.2.2/lofigui/context.py
+-rw-r--r--   0        0        0     1233 2023-06-09 11:55:58.064287 lofigui-0.2.2/lofigui/markdown.py
+-rw-r--r--   0        0        0      702 2023-06-09 11:55:58.042620 lofigui-0.2.2/lofigui/options.py
+-rw-r--r--   0        0        0      280 2023-06-09 11:55:58.053453 lofigui-0.2.2/lofigui/print.py
+-rw-r--r--   0        0        0      396 2023-06-09 11:56:07.630117 lofigui-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 lofigui-0.2.2/PKG-INFO
```

### Comparing `lofigui-0.2.1/README.md` & `lofigui-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lofigui-0.2.1/lofigui/context.py` & `lofigui-0.2.2/lofigui/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,19 @@
             self.queue.task_done()
         self.buffer += response
 
 
 # Slightly more involved but allows both single threaded use and option multithreaded
 _ctx = PrintContext()
 
+
 def buffer(ctx=None):
     if ctx is None:
         ctx = _ctx
     ctx.read()  # drain buffer
     return ctx.buffer
 
+
 def reset(ctx=None):
     if ctx is None:
         ctx = _ctx
-    ctx.buffer = ""
+    ctx.buffer = ""
```

### Comparing `lofigui-0.2.1/lofigui/markdown.py` & `lofigui-0.2.2/lofigui/markdown.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import markdown as mkdwn
 
 from .context import _ctx
 
+
 def markdown(msg="", ctx=None):
     if ctx is None:
         ctx = _ctx
     md = mkdwn.markdown(msg)
     ctx.queue.put_nowait(md)
 
 
-def html(msg='', ctx=None):
+def html(msg="", ctx=None):
     if ctx is None:
         ctx = _ctx
     ctx.queue.put_nowait(msg)
 
 
-def table(table, header = [], ctx=None):
+def table(table, header=[], ctx=None):
     if ctx is None:
         ctx = _ctx
     result = '<table class="table is-bordered is-striped">\n'
     if header:
-        result += '  <thead><tr>\n'
+        result += "  <thead><tr>\n"
         for field in header:
-            result += f'    <th>{field}</th>\n'
-        result += '  </tr></thead>\n'
+            result += f"    <th>{field}</th>\n"
+        result += "  </tr></thead>\n"
     if table:
-        result += '  <tbody>\n'
+        result += "  <tbody>\n"
         for row in table:
             # Make last field expand eg use one field to go alway across
-            extend_last_field = header and len(header) > len(row)                
-            result += '    <tr>\n'
-            for i,field in enumerate(row):
-                if extend_last_field and i == len(row)-1:
+            extend_last_field = header and len(header) > len(row)
+            result += "    <tr>\n"
+            for i, field in enumerate(row):
+                if extend_last_field and i == len(row) - 1:
                     result += f'      <td colspan="{len(header)-i}">{field}</td>\n'
                 else:
-                    result += f'      <td>{field}</td>\n'
-            result += '    </tr>\n'
-        result += '  </tbody>\n'
-    result += '</table>\n'
+                    result += f"      <td>{field}</td>\n"
+            result += "    </tr>\n"
+        result += "  </tbody>\n"
+    result += "</table>\n"
     ctx.queue.put_nowait(result)
```

### Comparing `lofigui-0.2.1/lofigui/options.py` & `lofigui-0.2.2/lofigui/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-
-
 # <div class = "checkbox">
 #                <label class = "is-size-5">Fruits</label>
 #                <br>
 #                <label class = "checkbox">
 #                   <input type = "checkbox">
 #                   Orange
 #                </label>
-               
+
 #                <label class = "checkbox">
 #                   <input type = "checkbox">
 #                   Apple
 #                </label>
-               
+
 #                <label class = "checkbox">
 #                   <input type = "checkbox">
 #                   Grapes
 #                </label>
-               
+
 #                <label class = "checkbox">
 #                   <input type = "checkbox">
 #                   Mango
 #                </label>
-#             </div>
+#             </div>
```

### Comparing `lofigui-0.2.1/PKG-INFO` & `lofigui-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lofigui
-Version: 0.2.1
+Version: 0.2.2
 Summary: Lofi GUI tooling
 License: MIT
 Author: Humphrey Drummond
 Author-email: hum3@drummond.info
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

