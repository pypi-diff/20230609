# Comparing `tmp/easyprofile-0.0.0.tar.gz` & `tmp/easyprofile-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyprofile-0.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "easyprofile-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easyprofile-0.0.0.tar` & `easyprofile-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-05-24 11:34:30.411457 easyprofile-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     3249 2023-05-24 11:34:30.411457 easyprofile-0.0.0/README.md
--rw-r--r--   0        0        0     3668 2023-05-24 11:34:30.411457 easyprofile-0.0.0/easyprofile.py
--rw-r--r--   0        0        0      532 2023-05-24 11:34:30.411457 easyprofile-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 easyprofile-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-23 00:06:38.657308 easyprofile-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3249 2023-05-24 11:18:41.678737 easyprofile-0.1.0/README.md
+-rw-r--r--   0        0        0     4065 2023-06-09 13:15:57.554758 easyprofile-0.1.0/easyprofile.py
+-rw-r--r--   0        0        0      532 2023-05-24 11:23:53.275865 easyprofile-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 easyprofile-0.1.0/PKG-INFO
```

### Comparing `easyprofile-0.0.0/LICENSE.txt` & `easyprofile-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyprofile-0.0.0/README.md` & `easyprofile-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easyprofile-0.0.0/easyprofile.py` & `easyprofile-0.1.0/easyprofile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''Easy context-based profiling with logging support'''
 
 from __future__ import annotations
 
-__version__ = '0.0.0'
+__version__ = '0.1.0'
 
 __all__ = (
     'BaseProfile',
     'LogProfile',
     'ignore',
     'ignored',
     'log',
@@ -65,23 +65,26 @@
                         else:
                             in_scope = frame.f_back is scope
 
                         if in_scope and frame.f_code not in PROFILE_IGNORE:
                             func(frame, event, arg)
 
                     setprofile(prof)
+                    func(scope, 'attach', None)
         else:
             trap = None
 
         self.stack.append(getprofile())
         setprofile(trap)
         return func
 
     @ignored
     def __exit__(self, *args: Any) -> None:
+        if self.func is not None:
+            self.func(None, 'detach', None)
         setprofile(self.stack.pop())
 
 
 ignore = profile(None)
 
 
 class BaseProfile:
@@ -97,14 +100,21 @@
 
 
 class LogProfile(BaseProfile):
 
     def __init__(self, log: Callable[[str], Any]) -> None:
         self.log = log
         self.counts: dict[FrameType, float] = {}
+        self.frame: FrameType | None = None
+
+    def _attach(self, frame: FrameType, arg: Any) -> None:
+        self.frame = frame
+
+    def _detach(self, frame: FrameType, arg: Any) -> None:
+        self.frame = None
 
     def _call(self, frame: FrameType, arg: Any) -> None:
         self.counts[frame] = perf_counter()
 
     def _return(self, frame: FrameType, arg: Any) -> None:
         count = perf_counter()
         delta = count - self.counts.get(frame, count)
@@ -116,14 +126,16 @@
             try:
                 qualname = f.f_code.co_qualname
             except AttributeError:
                 qualname = name
             if qualname.endswith(name):
                 name = qualname
             names.append(name)
+            if f == self.frame:
+                break
             f = f.f_back
         name = ' > '.join(names[-2::-1])
 
         parr = []
         if delta > 0:
             parr += [f'{timedelta(seconds=delta)!s}']
         if tracemalloc.is_tracing():
```

### Comparing `easyprofile-0.0.0/pyproject.toml` & `easyprofile-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyprofile-0.0.0/PKG-INFO` & `easyprofile-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyprofile
-Version: 0.0.0
+Version: 0.1.0
 Summary: Easy context-based profiling with logging support
 Author-email: Nicolas Tessore <n.tessore@ucl.ac.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Homepage, https://github.com/ntessore/easyprofile
 Project-URL: Issues, https://github.com/ntessore/easyprofile/issues
```

