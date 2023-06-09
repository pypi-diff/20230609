# Comparing `tmp/utilki-0.4.1.tar.gz` & `tmp/utilki-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.4.1.tar", max compression
+gzip compressed data, was "utilki-0.4.2.tar", max compression
```

## Comparing `utilki-0.4.1.tar` & `utilki-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-09 11:32:15.874240 utilki-0.4.1/README.md
--rw-r--r--   0        0        0      525 2023-06-09 11:32:15.874240 utilki-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      269 2023-06-09 11:32:15.874240 utilki-0.4.1/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-06-09 11:32:15.874240 utilki-0.4.1/utilki/cli.py
--rw-r--r--   0        0        0     5249 2023-06-09 11:32:15.874240 utilki-0.4.1/utilki/log_utils.py
--rw-r--r--   0        0        0     6381 2023-06-09 11:32:15.874240 utilki-0.4.1/utilki/task_mixin.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-09 12:49:02.071124 utilki-0.4.2/README.md
+-rw-r--r--   0        0        0      525 2023-06-09 12:49:02.071124 utilki-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/cli.py
+-rw-r--r--   0        0        0     5273 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/log_utils.py
+-rw-r--r--   0        0        0     6381 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.2/PKG-INFO
```

### Comparing `utilki-0.4.1/README.md` & `utilki-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.4.1/pyproject.toml` & `utilki-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.4.1"
+version = "0.4.2"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.4.1/utilki/cli.py` & `utilki-0.4.2/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.1/utilki/log_utils.py` & `utilki-0.4.2/utilki/log_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,19 @@
 
         self.print_idx = print_idx
         self.iterator: Iterator[A] = iter(iterator)
         self.len = len(iterator)
         self.name = name
         self.num_steps = num_steps
         if self.num_steps > self.len:
-            # msg = "num_steps > len(iterator), setting num_steps to len(iterator)"
-            # err(msg)
             self.num_steps = self.len
 
+        if self.num_steps < 1:
+            self.num_steps = 1
+
         self.map = {}
         step_size = 100 / self.num_steps
         is_int = step_size.is_integer()
         for i in range(self.num_steps + 1):
             index = i * int(self.len / self.num_steps)
             percent = i * step_size
             percent_str = f"{percent:.{precision}f}%"
@@ -214,7 +215,10 @@
     set_global("ayy", "lmao")
     value = get_global("ayy")
     log(value)
 
     from datetime import datetime
 
     err(datetime.now())
+
+    for i in progress([], name="test5"):
+        time.sleep(0.001)
```

### Comparing `utilki-0.4.1/utilki/task_mixin.py` & `utilki-0.4.2/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.1/PKG-INFO` & `utilki-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.4.1
+Version: 0.4.2
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

