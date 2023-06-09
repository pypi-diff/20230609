# Comparing `tmp/systemrdl-compiler-1.8.0.tar.gz` & `tmp/systemrdl-compiler-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/systemrdl-compiler-1.8.0.tar", last modified: Fri Sep 13 05:00:21 2019, max compression
+gzip compressed data, was "dist/systemrdl-compiler-1.9.0.tar", last modified: Fri Nov  1 05:37:35 2019, max compression
```

## Comparing `systemrdl-compiler-1.8.0.tar` & `systemrdl-compiler-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1608 2019-09-12 04:13:39.000000 systemrdl-compiler-1.8.0/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2019-05-07 04:08:52.000000 systemrdl-compiler-1.8.0/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)       41 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       10 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)     1210 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)     3184 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/setup.cfg
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1103 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    31120 2019-09-13 03:47:29.000000 systemrdl-compiler-1.8.0/systemrdl/node.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12188 2019-09-11 04:18:31.000000 systemrdl-compiler-1.8.0/systemrdl/messages.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      443 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15856 2019-08-20 04:10:55.000000 systemrdl-compiler-1.8.0/systemrdl/rdltypes.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5307 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/walker.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13343 2019-09-13 03:46:56.000000 systemrdl-compiler-1.8.0/systemrdl/compiler.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl/preprocessor/
--rw-rw-r--   0 alex      (1000) alex      (1000)    12536 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/preprocessor/preprocessor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3530 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/preprocessor/segment_map.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/preprocessor/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1781 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/preprocessor/ppp_runner.pl
--rw-rw-r--   0 alex      (1000) alex      (1000)     1556 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/importer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2019-09-13 04:59:50.000000 systemrdl-compiler-1.8.0/systemrdl/__about__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl/core/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3436 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/StructVisitor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14099 2019-09-13 03:01:27.000000 systemrdl-compiler-1.8.0/systemrdl/core/validate.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    53357 2019-09-13 03:52:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/properties.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      967 2019-09-13 03:39:54.000000 systemrdl-compiler-1.8.0/systemrdl/core/helpers.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21874 2019-05-07 04:05:30.000000 systemrdl-compiler-1.8.0/systemrdl/core/elaborate.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/core/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4248 2019-09-11 04:45:33.000000 systemrdl-compiler-1.8.0/systemrdl/core/parameter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4388 2019-09-13 04:00:24.000000 systemrdl-compiler-1.8.0/systemrdl/core/EnumVisitor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3323 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/namespace.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     8825 2019-09-13 03:38:18.000000 systemrdl-compiler-1.8.0/systemrdl/core/rdlformatcode.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    44154 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/ComponentVisitor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    38455 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/expressions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6028 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/UDPVisitor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3699 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/BaseVisitor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3457 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/core/backports.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17187 2019-02-11 05:56:22.000000 systemrdl-compiler-1.8.0/systemrdl/core/ExprVisitor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/systemrdl/parser/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/parser/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)   246933 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/parser/SystemRDLParser.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    39649 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/parser/SystemRDLLexer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17284 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/systemrdl/parser/SystemRDLVisitor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7371 2019-08-21 05:59:52.000000 systemrdl-compiler-1.8.0/systemrdl/component.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       69 2019-02-11 05:47:19.000000 systemrdl-compiler-1.8.0/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)     3184 2019-09-13 05:00:21.000000 systemrdl-compiler-1.8.0/PKG-INFO
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1608 2019-09-12 04:13:39.000000 systemrdl-compiler-1.9.0/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2019-05-07 04:08:52.000000 systemrdl-compiler-1.9.0/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       10 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1248 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3184 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1103 2019-02-11 05:56:22.000000 systemrdl-compiler-1.9.0/systemrdl/warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32434 2019-10-22 04:55:16.000000 systemrdl-compiler-1.9.0/systemrdl/node.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12204 2019-10-22 04:54:22.000000 systemrdl-compiler-1.9.0/systemrdl/messages.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      443 2019-02-11 05:56:22.000000 systemrdl-compiler-1.9.0/systemrdl/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16284 2019-10-22 04:53:51.000000 systemrdl-compiler-1.9.0/systemrdl/rdltypes.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5310 2019-10-22 04:52:21.000000 systemrdl-compiler-1.9.0/systemrdl/walker.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13903 2019-10-22 04:52:02.000000 systemrdl-compiler-1.9.0/systemrdl/compiler.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl/preprocessor/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12537 2019-10-22 04:51:01.000000 systemrdl-compiler-1.9.0/systemrdl/preprocessor/preprocessor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3528 2019-10-22 04:50:42.000000 systemrdl-compiler-1.9.0/systemrdl/preprocessor/segment_map.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2019-02-11 05:47:19.000000 systemrdl-compiler-1.9.0/systemrdl/preprocessor/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1781 2019-02-11 05:56:22.000000 systemrdl-compiler-1.9.0/systemrdl/preprocessor/ppp_runner.pl
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1560 2019-10-22 04:51:20.000000 systemrdl-compiler-1.9.0/systemrdl/importer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2019-11-01 05:36:19.000000 systemrdl-compiler-1.9.0/systemrdl/__about__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl/core/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3439 2019-10-22 04:45:08.000000 systemrdl-compiler-1.9.0/systemrdl/core/StructVisitor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14099 2019-09-20 02:44:53.000000 systemrdl-compiler-1.9.0/systemrdl/core/validate.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    54067 2019-10-23 04:49:08.000000 systemrdl-compiler-1.9.0/systemrdl/core/properties.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      967 2019-09-20 02:44:53.000000 systemrdl-compiler-1.9.0/systemrdl/core/helpers.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23405 2019-10-23 04:50:32.000000 systemrdl-compiler-1.9.0/systemrdl/core/elaborate.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2019-02-11 05:47:19.000000 systemrdl-compiler-1.9.0/systemrdl/core/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      968 2019-09-25 04:34:53.000000 systemrdl-compiler-1.9.0/systemrdl/core/parameter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4391 2019-10-22 04:48:32.000000 systemrdl-compiler-1.9.0/systemrdl/core/EnumVisitor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3328 2019-10-22 04:48:22.000000 systemrdl-compiler-1.9.0/systemrdl/core/namespace.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     8825 2019-09-20 02:44:53.000000 systemrdl-compiler-1.9.0/systemrdl/core/rdlformatcode.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    44980 2019-10-22 04:43:33.000000 systemrdl-compiler-1.9.0/systemrdl/core/ComponentVisitor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    38459 2019-10-22 04:48:01.000000 systemrdl-compiler-1.9.0/systemrdl/core/expressions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6033 2019-10-22 04:45:44.000000 systemrdl-compiler-1.9.0/systemrdl/core/UDPVisitor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3708 2019-10-22 04:45:13.000000 systemrdl-compiler-1.9.0/systemrdl/core/BaseVisitor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4265 2019-10-23 04:37:12.000000 systemrdl-compiler-1.9.0/systemrdl/core/value_normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3457 2019-02-11 05:47:19.000000 systemrdl-compiler-1.9.0/systemrdl/core/backports.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17215 2019-10-22 04:44:30.000000 systemrdl-compiler-1.9.0/systemrdl/core/ExprVisitor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/systemrdl/parser/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2019-02-11 05:47:19.000000 systemrdl-compiler-1.9.0/systemrdl/parser/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)   247018 2019-10-23 05:14:14.000000 systemrdl-compiler-1.9.0/systemrdl/parser/SystemRDLParser.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    39650 2019-10-23 05:14:13.000000 systemrdl-compiler-1.9.0/systemrdl/parser/SystemRDLLexer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17284 2019-10-23 05:14:14.000000 systemrdl-compiler-1.9.0/systemrdl/parser/SystemRDLVisitor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8681 2019-10-02 03:00:10.000000 systemrdl-compiler-1.9.0/systemrdl/component.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       69 2019-02-11 05:47:19.000000 systemrdl-compiler-1.9.0/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3184 2019-11-01 05:37:35.000000 systemrdl-compiler-1.9.0/PKG-INFO
```

### Comparing `systemrdl-compiler-1.8.0/README.md` & `systemrdl-compiler-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/setup.py` & `systemrdl-compiler-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/SOURCES.txt` & `systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 systemrdl/core/expressions.py
 systemrdl/core/helpers.py
 systemrdl/core/namespace.py
 systemrdl/core/parameter.py
 systemrdl/core/properties.py
 systemrdl/core/rdlformatcode.py
 systemrdl/core/validate.py
+systemrdl/core/value_normalization.py
 systemrdl/parser/SystemRDLLexer.py
 systemrdl/parser/SystemRDLParser.py
 systemrdl/parser/SystemRDLVisitor.py
 systemrdl/parser/__init__.py
 systemrdl/preprocessor/__init__.py
 systemrdl/preprocessor/ppp_runner.pl
 systemrdl/preprocessor/preprocessor.py
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl_compiler.egg-info/PKG-INFO` & `systemrdl-compiler-1.9.0/systemrdl_compiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemrdl-compiler
-Version: 1.8.0
+Version: 1.9.0
 Summary: Parse and elaborate front-end for SystemRDL 2.0
 Home-page: https://github.com/SystemRDL/systemrdl-compiler
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 License: UNKNOWN
 Project-URL: Documentation, http://systemrdl-compiler.readthedocs.io
 Project-URL: Source, https://github.com/SystemRDL/systemrdl-compiler
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/warnings.py` & `systemrdl-compiler-1.9.0/systemrdl/warnings.py`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl/node.py` & `systemrdl-compiler-1.9.0/systemrdl/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 
     def __deepcopy__(self, memo):
         """
         Deepcopy the node overlay.
         Members that are not part of the overlay (component tree) are not
         deepcopied.
+
+        .. versionadded:: 1.8
         """
         copy_by_ref = ["inst", "env"]
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k in copy_by_ref:
@@ -270,29 +272,29 @@
         """
         pathparts = path.split('.')
         current_node = self
         for pathpart in pathparts:
             m = re.fullmatch(r'^(\w+)((?:\[(?:\d+|0[xX][\da-fA-F]+)\])*)$', pathpart)
             if not m:
                 raise ValueError("Invalid path")
-            inst_name, array_suffix = m.group(1,2)
-            idx_list = [ int(s,0) for s in re.findall(r'\[(\d+|0[xX][\da-fA-F]+)\]', array_suffix) ]
+            inst_name, array_suffix = m.group(1, 2)
+            idx_list = [int(s, 0) for s in re.findall(r'\[(\d+|0[xX][\da-fA-F]+)\]', array_suffix)]
 
             current_node = current_node.get_child_by_name(inst_name)
             if current_node is None:
                 return None
 
             if idx_list:
                 if (isinstance(current_node, AddressableNode)) and current_node.inst.is_array:
                     # is an array
                     if len(idx_list) != len(current_node.inst.array_dimensions):
                         raise IndexError("Wrong number of array dimensions")
 
                     current_node.current_idx = [] # pylint: disable=attribute-defined-outside-init
-                    for i,idx in enumerate(idx_list):
+                    for i, idx in enumerate(idx_list):
                         if idx >= current_node.inst.array_dimensions[i]:
                             raise IndexError("Array index out of range")
                         current_node.current_idx.append(idx)
                 else:
                     raise IndexError("Index attempted on non-array component")
 
         return current_node
@@ -375,18 +377,18 @@
         ----------
         list_all: bool
             If true, lists all valid properties of this component type.
         """
 
         if list_all:
             props = []
-            for k,v in self.env.property_rules.rdl_properties.items():
+            for k, v in self.env.property_rules.rdl_properties.items():
                 if type(self.inst) in v.bindable_to:
                     props.append(k)
-            for k,v in self.env.property_rules.user_properties.items():
+            for k, v in self.env.property_rules.user_properties.items():
                 if type(self.inst) in v.bindable_to:
                     props.append(k)
             return props
         else:
             return list(self.inst.properties.keys())
 
 
@@ -404,15 +406,17 @@
         """
         # pylint: disable=unused-argument
         return self.inst.inst_name
 
 
     def get_path_segments(self, array_suffix="[{index:d}]", empty_array_suffix="[]"):
         """
-        Gets a list of path segments that represent the hierarchical path
+        Gets a list of path segments that represent the hierarchical path.
+
+        .. versionadded:: 1.8
         """
         if self.parent and not isinstance(self.parent, RootNode):
             segs = self.parent.get_path_segments(array_suffix, empty_array_suffix)
             segs.append(self.get_path_segment(array_suffix, empty_array_suffix))
         else:
             segs = [self.get_path_segment(array_suffix, empty_array_suffix)]
         return segs
@@ -464,14 +468,17 @@
             Override the string that denotes traversing up by one parent
         hier_separator: str
             Override the hierarchy separator
         array_suffix: str
             Override how array suffixes are represented when the index is known
         empty_array_suffix: str
             Override how array suffixes are represented when the index is not known
+
+
+        .. versionadded:: 1.8
         """
 
         # Collect path segments using default args to ensure paths can be compared
         ref_segs = ref.get_path_segments()
         self_segs = self.get_path_segments()
 
         # collect segments as-specified by the user
@@ -511,14 +518,17 @@
 
         Returns
         -------
         str or None
             HTML formatted string.
             If node does not have a description, returns ``None``
 
+
+        .. versionchanged:: 1.6
+            Added ``markdown_inst`` option.
         """
         desc_str = self.get_property("desc")
         if desc_str is None:
             return None
         return rdlformatcode.rdlfc_to_html(desc_str, self, md=markdown_inst)
 
 
@@ -530,28 +540,67 @@
 
         Returns
         -------
         str or None
             HTML formatted string.
             If node does not have an explicitly set name, returns ``None``
 
+
+        .. versionadded:: 1.8
         """
         name_str = self.get_property("name", default=None)
         if name_str is None:
             return None
         return rdlformatcode.rdlfc_to_html(name_str, self, is_desc=False)
 
 
     @property
     def inst_name(self):
         """
         Name of instantiated element
         """
         return self.inst.inst_name
 
+    @property
+    def type_name(self):
+        """
+        Named definition identifier.
+        If declaration was anonymous, inherits the first instance's name.
+        The type name of parameterized components is normalized based on the
+        instance's parameter values.
+
+        Importers may leave this as ``None``
+
+        .. versionadded:: 1.9
+        """
+        return self.inst.type_name
+
+    @property
+    def orig_type_name(self):
+        """
+        Named definition identifier prior to type name normalization.
+        If the declaration was anonymous, this reads as None.
+
+        .. versionadded:: 1.9
+        """
+        if self.inst.original_def is None:
+            # Component originated from an external importer
+            return None
+        else:
+            return self.inst.original_def.type_name
+
+    @property
+    def external(self):
+        """
+        True if instance type is external. False if internal.
+
+        .. versionadded:: 1.9
+        """
+        return self.inst.external
+
 
     def __eq__(self, other):
         """
         Node equality checks determine whether the other node represents the
         same position in the register model's hierarchy.
         """
         return self.get_path() == other.get_path()
@@ -589,26 +638,30 @@
             return path_segment
 
 
     def clear_lineage_index(self):
         """
         Resets this node's, as well as all parent node array indexes to
         the 'unknown index' state.
+
+        .. versionadded:: 1.7
         """
         if self.inst.is_array:
             self.current_idx = None
 
         if isinstance(self.parent, AddressableNode):
             self.parent.clear_lineage_index()
 
 
     def zero_lineage_index(self):
         """
         Resets this node's, as well as all parent node array indexes to
         zero.
+
+        .. versionadded:: 1.7
         """
         if self.inst.is_array:
             self.current_idx = [0] * len(self.array_dimensions)
 
         if isinstance(self.parent, AddressableNode):
             self.parent.zero_lineage_index()
 
@@ -670,14 +723,15 @@
         """
         Get the absolute byte address of this node excluding array stride of
         all parent.
 
         If this node, and all parents are not an array, then this is equivalent
         to :attr:`absolute_address`
 
+        .. versionadded:: 1.7
         """
         if self.parent and not isinstance(self.parent, RootNode):
             return self.parent.raw_absolute_address + self.raw_address_offset
         else:
             return self.raw_address_offset
 
 
@@ -961,15 +1015,15 @@
 
 #===============================================================================
 def get_group_node_size(node):
     """
     Shared getter for AddrmapNode and RegfileNode's "size" property
     """
     # After structural placement, children are sorted
-    if( not node.inst.children
+    if(not node.inst.children
         or (not isinstance(node.inst.children[-1], comp.AddressableComponent))
     ):
         # No addressable child exists.
         return 0
 
     # Current node's size is based on last child
     last_child_node = Node._factory(node.inst.children[-1], node.env, node)
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/messages.py` & `systemrdl-compiler-1.9.0/systemrdl/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -299,51 +299,56 @@
                 + color + severity.name.lower() + ": "
                 + Style.RESET_ALL
                 + text
             )
 
         # If src_ref highlights a span within a single line of text, print it
         if (src_ref.start_line is not None) and (src_ref.end_line is not None):
+            line_text = src_ref.start_line_text.rstrip()
+            start_col = src_ref.start_col
+            end_col = src_ref.end_col
+
+            # Normalize whitespace in line snippet (convert tabs to spaces)
+            TPS = 4
+            new_line_text = ""
+            i = 0
+            for char in line_text:
+                if char == "\t":
+                    new_line_text += " " * TPS
+                    if i < start_col:
+                        start_col += TPS-1
+                    if i < end_col:
+                        end_col += TPS-1
+                    i += TPS-1
+                else:
+                    new_line_text += char
+                i += 1
+            line_text = new_line_text
+
             if src_ref.start_line != src_ref.end_line:
                 # multi-line reference
                 # Select remainder of the line
-                width = len(src_ref.start_line_text) - src_ref.start_col
+                end_col = len(line_text)-1
+
+            width = end_col - start_col + 1
 
-                lines.append(
-                    src_ref.start_line_text[:src_ref.start_col]
-                    + color + Style.BRIGHT
-                    + src_ref.start_line_text[src_ref.start_col:]
-                    + Style.RESET_ALL
-                )
-
-                lines.append(
-                    " "*src_ref.start_col
-                    + color + Style.BRIGHT
-                    + "^"*width
-                    + Style.RESET_ALL
-                )
-
-            else:
-                # Single line
-                width = src_ref.end_col - src_ref.start_col + 1
-
-                lines.append(
-                    src_ref.start_line_text[:src_ref.start_col]
-                    + color + Style.BRIGHT
-                    + src_ref.start_line_text[src_ref.start_col : src_ref.end_col+1]
-                    + Style.RESET_ALL
-                    + src_ref.start_line_text[src_ref.end_col+1:]
-                )
-
-                lines.append(
-                    " "*src_ref.start_col
-                    + color + Style.BRIGHT
-                    + "^"*width
-                    + Style.RESET_ALL
-                )
+            lines.append(
+                line_text[:start_col]
+                + color + Style.BRIGHT
+                + line_text[start_col : end_col+1]
+                + Style.RESET_ALL
+                + line_text[end_col+1:]
+            )
+
+            lines.append(
+                " "*start_col
+                + color + Style.BRIGHT
+                + "^"*width
+                + Style.RESET_ALL
+            )
 
         return lines
 
 
     def emit_message(self, lines):
         """
         Emit message.
@@ -364,15 +369,15 @@
     def print_message(self, severity, text, src_ref):
         if severity >= Severity.ERROR:
             raise ValueError(text)
 
 #===============================================================================
 # Antlr error listener
 #===============================================================================
-class RDLAntlrErrorListener(ErrorListener) :
+class RDLAntlrErrorListener(ErrorListener):
 
     def __init__(self, msg_handler):
         self.msg = msg_handler
 
     def syntaxError(self, recognizer, offendingSymbol, line, column, msg, e):
         if offendingSymbol is not None:
             src_ref = SourceRef.from_antlr(offendingSymbol)
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/rdltypes.py` & `systemrdl-compiler-1.9.0/systemrdl/rdltypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,85 +11,85 @@
         obj = object.__new__(cls)
         obj._value_ = value
         return obj
 
 #===============================================================================
 class AccessType(AutoEnum):
     #: Not Accessible
-    na  = ()
+    na = ()
 
     #: Readable and writable
-    rw  = ()
+    rw = ()
 
     #: Read-only
-    r   = ()
+    r = ()
 
     #: Write-only
-    w   = ()
+    w = ()
 
     #: Readable and writable. After a reset occurs, can only be written once.
     rw1 = ()
 
     #: Write-only. After a reset occurs, can only be written once.
-    w1  = ()
+    w1 = ()
 
 class OnReadType(AutoEnum):
     #: Cleared on read
-    rclr    = ()
+    rclr = ()
 
     #: Set on read
-    rset    = ()
+    rset = ()
 
     #: User-defined read side-effect
-    ruser   = ()
+    ruser = ()
 
 class OnWriteType(AutoEnum):
     #: Bitwise write one to set
-    woset   = ()
+    woset = ()
 
     #: Bitwise write one to clear
-    woclr   = ()
+    woclr = ()
 
     #: Bitwise write one to toggle
-    wot     = ()
+    wot = ()
 
     #: Bitwise write zero to set
-    wzs     = ()
+    wzs = ()
 
     #: Bitwise write zero to clear
-    wzc     = ()
+    wzc = ()
 
     #: Bitwise write zero to toggle
-    wzt     = ()
+    wzt = ()
 
     #: All bits are cleared on write
-    wclr    = ()
+    wclr = ()
 
     #: All bits are set on write
-    wset    = ()
+    wset = ()
 
     #: Write modification is user-defined
-    wuser   = ()
+    wuser = ()
 
 class AddressingType(AutoEnum):
     #: Components are packed tightly together
-    compact     = ()
+    compact = ()
 
     #: Components are packed so each component’s start address is a multiple of its size
-    regalign    = ()
+    regalign = ()
 
     #: Same as regalign, except arrays are aligned to their entire size
-    fullalign   = ()
+    fullalign = ()
 
 class PrecedenceType(AutoEnum):
     #: Hardware writes take precedence over software
-    hw  = ()
+    hw = ()
 
     #: Software writes take precedence over hardware
-    sw  = ()
+    sw = ()
 
 class InterruptType(AutoEnum):
     """
     A field's interrupt type is set when using an RDL interrupt property modifier:
 
     .. code-block:: systemrdl
 
@@ -103,24 +103,24 @@
 
     .. code-block:: python
 
         intr_type = my_field_node.get_property("intr type")
 
     """
     #: Interrupt when asserted and maintained
-    level  = ()
+    level = ()
 
     #: Interrupt on low-to-high transition
-    posedge  = ()
+    posedge = ()
 
     #: Interrupt on high-to-low transition
-    negedge  = ()
+    negedge = ()
 
     #: Interrupt on any transition
-    bothedge  = ()
+    bothedge = ()
 
 #===============================================================================
 class UserEnum(enum.Enum):
     """
     All user-defined enumerations are based on this class.
 
     UserEnum types can be identified using: :meth:`is_user_enum`
@@ -163,14 +163,18 @@
             for more details.
 
         Returns
         -------
         str or None
             HTML formatted string.
             If enum entry does not have a description, returns ``None``
+
+
+        .. versionchanged:: 1.6
+            Added ``markdown_inst`` option.
         """
         desc_str = self._rdl_desc_
         if desc_str is None:
             return None
         return rdlformatcode.rdlfc_to_html(desc_str, md=markdown_inst)
 
     def get_html_name(self):
@@ -180,14 +184,17 @@
         Any RDLFormatCode tags used are converted to HTML.
 
         Returns
         -------
         str or None
             HTML formatted string.
             If enum entry does not have an explicitly set name, returns ``None``
+
+
+        .. versionadded:: 1.8
         """
         name_str = self._rdl_name_
         if name_str is None:
             return None
         return rdlformatcode.rdlfc_to_html(name_str, is_desc=False)
 
     @classmethod
@@ -208,28 +215,34 @@
         scope.
 
         Parameters
         ----------
         scope_separator: str
             Override the separator between namespace scopes
         """
-        if cls.get_parent_scope() is None:
+        parent_scope = cls.get_parent_scope()
+        if parent_scope is None:
+            # Importer likely never set the scope
             return ""
-        elif isinstance(cls.get_parent_scope(), comp.Root):
+        elif isinstance(parent_scope, comp.Root):
+            # Declaration was in root scope
             return ""
         else:
-            parent_path = cls.get_parent_scope().get_scope_path(scope_separator)
+            # Get parent definition's scope path
+            parent_path = parent_scope.get_scope_path(scope_separator)
+
+            # Extend it with its scope name
             if parent_path:
                 return(
                     parent_path
                     + scope_separator
-                    + cls.get_parent_scope().type_name
+                    + parent_scope._scope_name
                 )
             else:
-                return cls.get_parent_scope().type_name
+                return parent_scope._scope_name
 
 
     def __int__(self):
         return self.value
 
     def __bool__(self):
         return bool(self.value)
@@ -356,28 +369,34 @@
         scope.
 
         Parameters
         ----------
         scope_separator: str
             Override the separator between namespace scopes
         """
-        if cls.get_parent_scope() is None:
+        parent_scope = cls.get_parent_scope()
+        if parent_scope is None:
+            # Importer likely never set the scope
             return ""
-        elif isinstance(cls.get_parent_scope(), comp.Root):
+        elif isinstance(parent_scope, comp.Root):
+            # Declaration was in root scope
             return ""
         else:
-            parent_path = cls.get_parent_scope().get_scope_path(scope_separator)
+            # Get parent definition's scope path
+            parent_path = parent_scope.get_scope_path(scope_separator)
+
+            # Extend it with its scope name
             if parent_path:
                 return(
                     parent_path
                     + scope_separator
-                    + cls.get_parent_scope().type_name
+                    + parent_scope._scope_name
                 )
             else:
-                return cls.get_parent_scope().type_name
+                return parent_scope._scope_name
 
     def __repr__(self):
         return "<struct '%s' %s at 0x%x>" % (
             self.__class__.__qualname__,
             "(%s)" % ", ".join(self._members.keys()),
             id(self)
         )
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/walker.py` & `systemrdl-compiler-1.9.0/systemrdl/walker.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             If True, walker skips nodes whose 'ispresent' property is set
             to False
         """
         self.unroll = unroll
         self.skip_not_present = skip_not_present
 
 
-    def walk(self, node, *listeners:RDLListener):
+    def walk(self, node, *listeners: RDLListener):
         """
         Initiates the walker to traverse the current ``node`` and its children.
         Calls the corresponding callback for each of the ``listeners`` provided in
         the order that they are listed.
 
         Parameters
         ----------
@@ -120,15 +120,15 @@
             self.do_enter(node, listener)
         for child in node.children(unroll=self.unroll, skip_not_present=self.skip_not_present):
             self.walk(child, *listeners)
         for listener in listeners:
             self.do_exit(node, listener)
 
 
-    def do_enter(self, node, listener:RDLListener):
+    def do_enter(self, node, listener: RDLListener):
 
         # Skip RootNode since it isn't really a component
         if not isinstance(node, RootNode):
             listener.enter_Component(node)
 
         if isinstance(node, AddressableNode):
             listener.enter_AddressableComponent(node)
@@ -145,15 +145,15 @@
             listener.enter_Addrmap(node)
         elif isinstance(node, MemNode):
             listener.enter_Mem(node)
         elif isinstance(node, SignalNode):
             listener.enter_Signal(node)
 
 
-    def do_exit(self, node, listener:RDLListener):
+    def do_exit(self, node, listener: RDLListener):
         if isinstance(node, FieldNode):
             listener.exit_Field(node)
         elif isinstance(node, RegNode):
             listener.exit_Reg(node)
         elif isinstance(node, RegfileNode):
             listener.exit_Regfile(node)
         elif isinstance(node, AddrmapNode):
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/compiler.py` & `systemrdl-compiler-1.9.0/systemrdl/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,27 @@
         error_flags: int
             Same as ``warning_flags`` but promote them to errors instead.
         dedent_desc: bool
             Automatically remove any common indentation from multi-line
             ``desc`` properties.
 
             Set to True by default.
+        extended_dpa_type_names: bool
+            Enable extended type name generation that accounts for dynamic
+            property assignments augmenting the type.
+
+            Set to True by default.
+
+            See :ref:`dpa_type_generation` for more details.
+
+
+        .. versionchanged:: 1.8
+            Added ``dedent_desc`` option.
+        .. versionchanged:: 1.9
+            Added ``extended_dpa_type_names`` option.
         """
         self.env = RDLEnvironment(kwargs)
 
         # Check for stray kwargs
         if kwargs:
             raise TypeError("got an unexpected keyword argument '%s'" % list(kwargs.keys())[0])
 
@@ -271,28 +284,28 @@
         )
 
         # Resolve address and field placement
         walker.RDLWalker(skip_not_present=False).walk(
             root_node,
             PrePlacementValidateListener(self.msg),
             StructuralPlacementListener(self.msg),
-            LateElabListener(self.msg)
+            LateElabListener(self.msg, self.env)
         )
 
         # Validate design
         # Only need to validate nodes that are present
         walker.RDLWalker(skip_not_present=True).walk(root_node, ValidateListener(self.env))
 
         if self.msg.had_error:
             self.msg.fatal("Elaborate aborted due to previous errors")
 
         return root_node
 
 
-    def eval(self, expression:str):
+    def eval(self, expression: str):
         """
         Evaluate an RDL expression string and return its compiled value.
         This function is provided as a helper to simplify overriding top-level
         parameters during elaboration.
 
         Parameters
         ----------
@@ -301,14 +314,17 @@
             Any references used in the expression are resolved using the
             current contents of the root namespace.
 
         Raises
         ------
         ValueError
             If any parse or evaluation error occurs.
+
+
+        .. versionadded:: 1.8
         """
         # Create local message handler that suppresses the usual ouput
         # to stderr.
         # Instead raises ValueError on any error
         msg_printer = messages.MessageExceptionRaiser()
         msg_handler = messages.MessageHandler(msg_printer)
 
@@ -344,14 +360,15 @@
     def __init__(self, args_dict):
 
         # Collect args
         message_printer = args_dict.pop('message_printer', messages.MessagePrinter())
         w_flags = args_dict.pop('warning_flags', 0)
         e_flags = args_dict.pop('error_flags', 0)
         self.dedent_desc = args_dict.pop('dedent_desc', True)
+        self.use_extended_type_name_gen = args_dict.pop('extended_dpa_type_names', True)
 
         self.chk_missing_reset = self.chk_flag_severity(warnings.MISSING_RESET, w_flags, e_flags)
         self.chk_implicit_field_pos = self.chk_flag_severity(warnings.IMPLICIT_FIELD_POS, w_flags, e_flags)
         self.chk_implicit_addr = self.chk_flag_severity(warnings.IMPLICIT_ADDR, w_flags, e_flags)
         self.chk_stride_not_pow2 = self.chk_flag_severity(warnings.STRIDE_NOT_POW2, w_flags, e_flags)
         self.chk_strict_self_align = self.chk_flag_severity(warnings.STRICT_SELF_ALIGN, w_flags, e_flags)
         self.chk_sparse_reg_stride = self.chk_flag_severity(warnings.SPARSE_REG_STRIDE, w_flags, e_flags)
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/preprocessor/preprocessor.py` & `systemrdl-compiler-1.9.0/systemrdl/preprocessor/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         if shutil.which("perl") is None:
             self.env.msg.fatal(
                 "Input contains Perl preprocessor tags, but an installation of Perl could not be found"
             )
 
         # Generate minimal perl script that captures activities described in the source file
         lines = []
-        for i,pp_seg in enumerate(segments):
+        for i, pp_seg in enumerate(segments):
             if isinstance(pp_seg, PPPUnalteredSegment):
                 # Text outside preprocessor tags that should remain unaltered
                 # Insert command to emit reference to this text segment
                 lines.append("rdlppp_utils::emit_ref(%d);" % i)
 
             elif isinstance(pp_seg, PPPPerlSegment):
                 # Perl code snippet. Insert directly
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/preprocessor/segment_map.py` & `systemrdl-compiler-1.9.0/systemrdl/preprocessor/segment_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 class Segment:
     """
     Base class for various segment map segments.
     Not to be used directly
     """
-    def __init__(self, start, end, src_start, src_end, src, incl_ref = None):
+    def __init__(self, start, end, src_start, src_end, src, incl_ref=None):
 
         # start/end offset of resulting text
         self.start = start
         self.end = end
 
         # start/end offset of original text
         # Offsets are relative to src
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/preprocessor/ppp_runner.pl` & `systemrdl-compiler-1.9.0/systemrdl/preprocessor/ppp_runner.pl`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl/importer.py` & `systemrdl-compiler-1.9.0/systemrdl/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from .compiler import RDLCompiler
 from .component import Component
 
 class RDLImporter:
     """
     Base class for external parsers to import data into the register model
     """
-    def __init__(self, compiler:RDLCompiler):
+    def __init__(self, compiler: RDLCompiler):
         self.compiler = compiler
         self.msg = compiler.env.msg
 
-    def import_file(self, path:str):
+    def import_file(self, path: str):
         raise NotImplementedError
 
-    def register_root_component(self, definition:Component):
+    def register_root_component(self, definition: Component):
 
         if definition.type_name is None:
             raise ValueError("Component must have a type_name")
 
         if definition.is_instance:
             raise ValueError("Component cannot already be instantiated")
 
@@ -30,15 +30,15 @@
             definition,
             definition.def_src_ref
         )
 
         # Add to root component definition list
         self.compiler.root.comp_defs[definition.type_name] = definition
 
-    def lookup_root_component(self, type_name:str):
+    def lookup_root_component(self, type_name: str):
         return self.compiler.root.comp_defs.get(type_name, None)
 
     def assign_property(self, component, prop_name, value, src_ref):
         rule = self.compiler.env.property_rules.lookup_property(prop_name)
         if rule is None:
             self.msg.fatal(
                 "Unrecognized property '%s'" % prop_name,
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/StructVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/core/StructVisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .. import component as comp
 from ..messages import SourceRef
 from .. import rdltypes
 
 class StructVisitor(BaseVisitor):
 
-    def visitStruct_def(self, ctx:SystemRDLParser.Struct_defContext):
+    def visitStruct_def(self, ctx: SystemRDLParser.Struct_defContext):
         self.compiler.namespace.enter_scope()
 
         is_abstract = (ctx.ABSTRACT_kw() is not None)
         struct_name = get_ID_text(ctx.name)
 
         if ctx.base is not None:
             # Get the base struct type
@@ -61,15 +61,15 @@
         # Create Struct type
         struct_type = base_type.define_new(struct_name, members, is_abstract)
 
         self.compiler.namespace.exit_scope()
         return struct_type, struct_name, SourceRef.from_antlr(ctx.name)
 
 
-    def visitStruct_elem(self, ctx:SystemRDLParser.Struct_elemContext):
+    def visitStruct_elem(self, ctx: SystemRDLParser.Struct_elemContext):
 
         member_name = get_ID_text(ctx.ID())
         member_src_ref = SourceRef.from_antlr(ctx.ID())
 
         member_type = self.visit(ctx.struct_type())
 
         if ctx.array_type_suffix() is not None:
@@ -82,15 +82,15 @@
         SystemRDLParser.FIELD_kw    : comp.Field,
         SystemRDLParser.REG_kw      : comp.Reg,
         SystemRDLParser.REGFILE_kw  : comp.Regfile,
         SystemRDLParser.ADDRMAP_kw  : comp.Addrmap,
         SystemRDLParser.SIGNAL_kw   : comp.Signal,
         SystemRDLParser.MEM_kw      : comp.Mem
     }
-    def visitStruct_type(self, ctx:SystemRDLParser.Struct_typeContext):
+    def visitStruct_type(self, ctx: SystemRDLParser.Struct_typeContext):
         if ctx.data_type() is not None:
             data_type_token = self.visit(ctx.data_type())
             member_type = self.datatype_from_token(data_type_token)
         elif ctx.component_type() is not None:
             type_token = self.visit(ctx.component_type())
             member_type = self._CompType_Map[type_token.type]
         else:
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/validate.py` & `systemrdl-compiler-1.9.0/systemrdl/core/validate.py`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/properties.py` & `systemrdl-compiler-1.9.0/systemrdl/core/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,27 @@
 
         self.user_properties[udp.name] = udp
 
 #===============================================================================
 # Base property
 #===============================================================================
 class PropertyRule:
+    # List of components this property can be bound to
     bindable_to = []
+
+    # List of valid assignment types. In order of cast preference
     valid_types = []
+
+    # Default value if not assigned
     default = None
+
+    # Whether dynamic assignments are allowed to be made to this property
     dyn_assign_allowed = True
+
+    # Group string in which this property is mutually exclusive
     mutex_group = None
 
     #---------------------------------------------------------------------------
     def __init__(self, env):
         self.env = env
 
     #---------------------------------------------------------------------------
@@ -113,14 +122,18 @@
         else:
             # Value is already evaluated
             assign_type = type(value)
 
         # Check if value's type is compatible
         for valid_type in self.valid_types:
             if expressions.is_castable(assign_type, valid_type):
+                if isinstance(value, expressions.Expr):
+                    # Found a type-compatible match. (first match is best match)
+                    # Wrap the expression with an explicit assignment cast
+                    value = expressions.AssignmentCast(self.env, src_ref, value, valid_type)
                 break
         else:
             self.env.msg.fatal(
                 "Incompatible assignment to property '%s'" % self.get_name(),
                 src_ref
             )
 
@@ -243,15 +256,15 @@
 class Prop_dontcompare(PropertyRule):
     """
     Indicates the components read data shall be discarded and not compared
     against expected results.
     (5.2.2)
     """
     bindable_to = (comp.Addrmap, comp.Reg, comp.Regfile, comp.Field,)
-    valid_types = (bool, int,)
+    valid_types = (int, bool,)
     default = False
     dyn_assign_allowed = True
     mutex_group = "O"
 
     def validate(self, node, value):
         donttest = node.get_property("donttest")
 
@@ -287,15 +300,15 @@
                 self.env.msg.error(
                     "A field's bit cannot have both 'dontcompare' and 'donttest' properties enabled",
                     node.inst.inst_src_ref
                 )
 
         else:
             # A boolean may end up cast as an int. Normalize 0 or 1 to boolean
-            if isinstance(value, int) and value in (0,1):
+            if isinstance(value, int) and value in (0, 1):
                 value = bool(value)
 
             # 5.2.2.1-b: can also be applied to reg, regfile, and addrmap
             # components, but only as a boolean
             if not isinstance(value, bool):
                 self.env.msg.error(
                     "Property 'dontcompare' expects a boolean for non-field types. Got an integer in '%s'"
@@ -315,15 +328,15 @@
 
 class Prop_donttest(PropertyRule):
     """
     Indicates the component is not included in structural testing.
     (5.2.2)
     """
     bindable_to = (comp.Addrmap, comp.Reg, comp.Regfile, comp.Field,)
-    valid_types = (bool, int,)
+    valid_types = (int, bool,)
     default = False
     dyn_assign_allowed = True
     mutex_group = "O"
 
     def validate(self, node, value):
         if isinstance(node, m_node.FieldNode):
             # 5.2.2.1-a: If value is a bit mask, the mask shall have the same width
@@ -333,15 +346,15 @@
                     self.env.msg.error(
                         "Bit mask (%d) of property 'donttest' exceeds width (%d) of field '%s'"
                         % (value, node.inst.width, node.inst.inst_name),
                         node.inst.inst_src_ref
                     )
         else:
             # A boolean may end up cast as an int. Normalize 0 or 1 to boolean
-            if isinstance(value, int) and value in (0,1):
+            if isinstance(value, int) and value in (0, 1):
                 value = bool(value)
 
             # 5.2.2.1-b: can also be applied to reg, regfile, and addrmap
             # components, but only as a boolean
             if not isinstance(value, bool):
                 self.env.msg.error(
                     "Property 'donttest' expects a boolean for non-field types. Got an integer in '%s'"
@@ -1050,70 +1063,70 @@
     mutex_group = "E"
 
 class Prop_threshold(PropertyRule):
     """
     alias of incrthreshold.
     """
     bindable_to = (comp.Field,)
-    valid_types = (bool, int, comp.Signal, comp.Field,)
+    valid_types = (int, bool, comp.Signal, comp.Field,)
     default = False
     dyn_assign_allowed = True
     mutex_group = "incrthreshold alias"
 
     def assign_value(self, comp_def, value, src_ref):
         """
         Set both alias and actual value
         """
         super().assign_value(comp_def, value, src_ref)
-        comp_def.properties['incrthreshold'] = value
+        comp_def.properties['incrthreshold'] = comp_def.properties['threshold']
 
 class Prop_saturate(PropertyRule):
     """
     alias of incrsaturate.
     """
     bindable_to = (comp.Field,)
-    valid_types = (bool, int, comp.Signal, comp.Field,)
+    valid_types = (int, bool, comp.Signal, comp.Field,)
     default = False
     dyn_assign_allowed = True
     mutex_group = "incrsaturate alias"
 
     def assign_value(self, comp_def, value, src_ref):
         """
         Set both alias and actual value
         """
         super().assign_value(comp_def, value, src_ref)
-        comp_def.properties['incrsaturate'] = value
+        comp_def.properties['incrsaturate'] = comp_def.properties['saturate']
 
 class Prop_incrthreshold(PropertyRule):
     bindable_to = (comp.Field,)
-    valid_types = (bool, int, comp.Signal, comp.Field,)
+    valid_types = (int, bool, comp.Signal, comp.Field,)
     default = False
     dyn_assign_allowed = True
     mutex_group = "incrthreshold alias"
 
     def assign_value(self, comp_def, value, src_ref):
         """
         Set both alias and actual value
         """
         super().assign_value(comp_def, value, src_ref)
-        comp_def.properties['incrthreshold'] = value
+        comp_def.properties['threshold'] = comp_def.properties['incrthreshold']
 
 class Prop_incrsaturate(PropertyRule):
     bindable_to = (comp.Field,)
-    valid_types = (bool, int, comp.Signal, comp.Field,)
+    valid_types = (int, bool, comp.Signal, comp.Field,)
     default = False
     dyn_assign_allowed = True
     mutex_group = "incrsaturate alias"
 
     def assign_value(self, comp_def, value, src_ref):
         """
         Set both alias and actual value
         """
         super().assign_value(comp_def, value, src_ref)
-        comp_def.properties['incrsaturate'] = value
+        comp_def.properties['saturate'] = comp_def.properties['incrsaturate']
 
 class Prop_overflow(PropertyRule):
     bindable_to = (comp.Field,)
     valid_types = (bool,)
     default = False
     dyn_assign_allowed = True
     mutex_group = None
@@ -1165,22 +1178,22 @@
     valid_types = (int,)
     default = None
     dyn_assign_allowed = True
     mutex_group = "G"
 
 class Prop_decrsaturate(PropertyRule):
     bindable_to = (comp.Field,)
-    valid_types = (bool, int, comp.Signal, comp.Field,)
+    valid_types = (int, bool, comp.Signal, comp.Field,)
     default = False
     dyn_assign_allowed = True
     mutex_group = None
 
 class Prop_decrthreshold(PropertyRule):
     bindable_to = (comp.Field,)
-    valid_types = (bool, int, comp.Signal, comp.Field,)
+    valid_types = (int, bool, comp.Signal, comp.Field,)
     default = False
     dyn_assign_allowed = True
     mutex_group = None
 
 #-------------------------------------------------------------------------------
 # Field access interrupt properties
 #-------------------------------------------------------------------------------
@@ -1460,15 +1473,15 @@
     mutex_group = None
 
 #===============================================================================
 # User-defined property
 #===============================================================================
 
 class UserProperty(PropertyRule):
-    def __init__(self, env, name, bindable_to, valid_types, default = None, constr_componentwidth=False):
+    def __init__(self, env, name, bindable_to, valid_types, default=None, constr_componentwidth=False):
         super().__init__(env)
 
         self.name = name
         self.bindable_to = bindable_to
         self.valid_types = valid_types
         self.default = default
         self.constr_componentwidth = constr_componentwidth
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/helpers.py` & `systemrdl-compiler-1.9.0/systemrdl/core/helpers.py`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/elaborate.py` & `systemrdl-compiler-1.9.0/systemrdl/core/elaborate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import hashlib
 
 from .expressions import Expr
 from .helpers import is_pow2, roundup_pow2, roundup_to
+from .value_normalization import normalize
 
 from .. import component as comp
 from .. import walker
 from .. import rdltypes
 from ..node import AddressableNode, RegNode
 
 
@@ -24,25 +26,18 @@
     Also elaborates parameterized component type names
     """
 
     def __init__(self, msg_handler):
         self.msg = msg_handler
 
     def enter_Component(self, node):
-        if node.inst.original_def is not None:
-            # Generate the elaborated type name as per 5.1.1.4
-            new_type_name = node.inst.original_def.type_name
-
-            for i in range(len(node.inst.parameters)):
-                orig_param_value = node.inst.original_def.parameters[i].get_value()
-                new_param_value = node.inst.parameters[i].get_value()
-                if new_param_value != orig_param_value:
-                    new_type_name = new_type_name + "_" + node.inst.parameters[i].get_normalized_parameter()
-            node.inst.type_name = new_type_name
-
+        # Evaluate component properties
+        for prop_name, prop_value in node.inst.properties.items():
+            if isinstance(prop_value, Expr):
+                node.inst.properties[prop_name] = prop_value.get_value()
 
     def enter_AddressableComponent(self, node):
         # Evaluate instance object expressions
         if isinstance(node.inst.addr_offset, Expr):
             node.inst.addr_offset = node.inst.addr_offset.get_value()
 
         if isinstance(node.inst.addr_align, Expr):
@@ -83,19 +78,16 @@
 
         if isinstance(node.inst.msb, Expr):
             node.inst.msb = node.inst.msb.get_value()
 
         if isinstance(node.inst.lsb, Expr):
             node.inst.lsb = node.inst.lsb.get_value()
 
-    def exit_Component(self, node):
-        # Evaluate component properties
-        for prop_name, prop_value in node.inst.properties.items():
-            if isinstance(prop_value, Expr):
-                node.inst.properties[prop_name] = prop_value.get_value()
+
+
 
 #-------------------------------------------------------------------------------
 class PrePlacementValidateListener(walker.RDLListener):
     """
     Performs value checks of some properties prior to StructuralPlacementListener
     """
     def __init__(self, msg_handler):
@@ -400,14 +392,21 @@
 
 
     def exit_AddressableComponent(self, node):
         # Resolve array stride if needed
         if node.inst.is_array and (node.inst.array_stride is None):
             node.inst.array_stride = node.size
 
+            if node.env.chk_implicit_addr:
+                node.env.msg.message(
+                    node.env.chk_implicit_addr,
+                    "Array stride of component '%s' is not explicitly set" % node.inst.inst_name,
+                    node.inst.inst_src_ref
+                )
+
 
     def resolve_addresses(self, node):
         """
         Resolve addresses of children of Addrmap and Regfile components
         """
 
         # Get alignment based on 'alignment' property
@@ -488,16 +487,17 @@
         node.inst.children.sort(key=get_child_sort_key)
 
 #-------------------------------------------------------------------------------
 class LateElabListener(walker.RDLListener):
     """
     Elaboration listener for misc late-stage things
     """
-    def __init__(self, msg_handler):
+    def __init__(self, msg_handler, env):
         self.msg = msg_handler
+        self.env = env
         self.coerce_external_to = None
         self.coerce_end_regfile = None
 
 
     def enter_Field(self, node):
 
         # 9.6.1-d: swwe and swwel have precedence over the software access
@@ -570,7 +570,42 @@
 
 
     def exit_Regfile(self, node):
         if node is self.coerce_end_regfile:
             # Exiting inst type coercion
             self.coerce_external_to = None
             self.coerce_end_regfile = None
+
+    def exit_Component(self, node):
+        # Generate elaborated type name
+        extra_type_name_segments = []
+
+        # Augment based on paramter overrides as per 5.1.1.4
+        if node.inst.original_def is not None:
+            for i in range(len(node.inst.parameters)):
+                orig_param_value = node.inst.original_def.parameters[i].get_value()
+                new_param_value = node.inst.parameters[i].get_value()
+                if new_param_value != orig_param_value:
+                    extra_type_name_segments.append(node.inst.parameters[i].get_normalized_parameter())
+
+        # Further augment type name as per extended type generation from DPAs
+        if self.env.use_extended_type_name_gen:
+            # Strip duplicates and sort alphabetically
+            node.inst._dyn_assigned_props = sorted(set(node.inst._dyn_assigned_props))
+            node.inst._dyn_assigned_children = sorted(set(node.inst._dyn_assigned_children))
+
+            # assignments made 'through' the component
+            for child_name in node.inst._dyn_assigned_children:
+                child = node.inst.get_child_by_name(child_name)
+
+                # <child_name>_<hash of child type name>
+                norm_name = hashlib.md5(child.type_name.encode('utf-8')).hexdigest()[:8]
+                extra_type_name_segments.append(child_name + "_" + norm_name)
+
+            # this component's DPAs
+            for prop_name in node.inst._dyn_assigned_props:
+                # <prop_name>_<norm prop value>
+                norm_name = normalize(node.get_property(prop_name), owner_node=node)
+                extra_type_name_segments.append(prop_name + "_" + norm_name)
+
+        if extra_type_name_segments:
+            node.inst.type_name += "_" + "_".join(extra_type_name_segments)
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/parameter.py` & `systemrdl-compiler-1.9.0/systemrdl/core/value_normalization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,36 @@
 import hashlib
 import enum
 from .. import rdltypes
+from .. import node
 
-
-class Parameter:
-    def __init__(self, param_type, name, default_expr=None):
-        self.name = name
-        self.param_type = param_type
-
-        self.expr = default_expr
-
-        # Stores the evaluated result of self.expr so that subsequent queries do
-        # not need to repeatedly re-evaluate it
-        self._value = None
-
-    def get_value(self):
-        """
-        Evaluate self.expr to get the parameter's value
-        """
-        if (self._value is None) and (self.expr is not None):
-            self._value = self.expr.get_value()
-
-        return self._value
-
-
-    def get_normalized_parameter(self):
-        """
-        Converts the parameter to the normalized type name segment as defined in
-        SystemRDL 2.0 Section 5.1.1.4-c
-
-        Returns the whole parameter string:
-            <parameter name> + "_" + <normalized value>
-        """
-        return self.name + "_" + normalize(self.get_value())
-
-#===============================================================================
-# Parameter value normalizing functions (5.1.1.4-c)
-#===============================================================================
-def normalize(value):
-    # Determine what type it is supposed to be
+def normalize(value, owner_node=None):
+    """
+    Flatten an RDL value into a unique string that is used for type
+    normalization.
+    """
+    # Determine what type is being flattened
     if type(value) == int:
         return normalize_scalar(value)
     elif type(value) == bool:
         return normalize_boolean(value)
     elif type(value) == str:
         return normalize_string(value)
     elif type(value) == list:
         return normalize_array(value)
     elif isinstance(value, enum.Enum):
         return normalize_enum(value)
     elif isinstance(value, rdltypes.UserStruct):
         return normalize_struct(value)
+    elif isinstance(value, node.Node):
+        return normalize_component_ref(value, owner_node)
+    elif isinstance(value, rdltypes.PropertyReference):
+        return normalize_property_ref(value, owner_node)
+    elif rdltypes.is_user_enum(value):
+        return normalize_user_enum_type(value)
     else:
         # Should never get here
         raise RuntimeError
 
 
 def normalize_scalar(value):
     """
@@ -133,7 +109,33 @@
     norm_elements = []
     for member_name, member_value in value._values.items():
         norm_elements.append("%s_%s" % (member_name, normalize(member_value)))
 
     norm_str = "_".join(norm_elements)
     md5 = hashlib.md5(norm_str.encode('utf-8')).hexdigest()
     return md5[:8]
+
+
+def normalize_component_ref(value, owner_node):
+    """
+    Hash of relative path from owner of the property to the target component
+    """
+    path = value.get_rel_path(owner_node)
+    md5 = hashlib.md5(path.encode('utf-8')).hexdigest()
+    return md5[:8]
+
+
+def normalize_property_ref(value, owner_node):
+    """
+    Hash of relative path from owner of the property to the target component's
+    property
+    """
+    path = "%s->%s" % (value.node.get_rel_path(owner_node), value.name)
+    md5 = hashlib.md5(path.encode('utf-8')).hexdigest()
+    return md5[:8]
+
+
+def normalize_user_enum_type(value):
+    """
+    Enum type references shall be rendered using their enumeration type name.
+    """
+    return value.__name__
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/EnumVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/core/EnumVisitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from . import expressions, helpers
 
 from ..messages import SourceRef
 from .. import rdltypes
 
 class EnumVisitor(BaseVisitor):
 
-    def visitEnum_def(self, ctx:SystemRDLParser.Enum_defContext):
+    def visitEnum_def(self, ctx: SystemRDLParser.Enum_defContext):
         self.compiler.namespace.enter_scope()
 
         enum_name = get_ID_text(ctx.ID())
 
         # Collect entries
         entry_values = []
         entries = OrderedDict()
@@ -61,15 +61,15 @@
 
         # Create Enum type
         enum_type = rdltypes.UserEnum(enum_name, entries) #pylint: disable=no-value-for-parameter
 
         self.compiler.namespace.exit_scope()
         return enum_type, get_ID_text(ctx.ID()), SourceRef.from_antlr(ctx.ID())
 
-    def visitEnum_entry(self, ctx:SystemRDLParser.Enum_entryContext):
+    def visitEnum_entry(self, ctx: SystemRDLParser.Enum_entryContext):
         name_token = ctx.ID()
         value_expr_ctx = ctx.expr()
 
         rdl_name = None
         rdl_desc = None
 
         for pa_ctx in ctx.getTypedRuleContexts(SystemRDLParser.Enum_prop_assignContext):
@@ -99,15 +99,15 @@
                 self.msg.fatal(
                     "Illegal enum property assignment '%s'" % prop_name,
                     SourceRef.from_antlr(prop_token)
                 )
 
         return name_token, value_expr_ctx, rdl_name, rdl_desc
 
-    def visitEnum_prop_assign(self, ctx:SystemRDLParser.Enum_prop_assignContext):
+    def visitEnum_prop_assign(self, ctx: SystemRDLParser.Enum_prop_assignContext):
         prop_token = ctx.ID()
 
         visitor = ExprVisitor(self.compiler)
         prop_expr = visitor.visit(ctx.expr())
         prop_expr = expressions.AssignmentCast(self.compiler.env, ctx.expr(), prop_expr, str)
         prop_expr.predict_type()
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/namespace.py` & `systemrdl-compiler-1.9.0/systemrdl/core/namespace.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,47 +6,47 @@
         self.env = env
         self.msg = env.msg
 
         self.type_ns_stack = [{}]
         self.element_ns_stack = [{}]
         self.default_property_ns_stack = [{}]
 
-    def register_type(self, name:str, ref, src_ref):
+    def register_type(self, name: str, ref, src_ref):
         if name in self.type_ns_stack[-1]:
             self.msg.fatal(
                 "Multiple declarations of type '%s'" % name,
                 src_ref
             )
         self.type_ns_stack[-1][name] = ref
 
-    def register_element(self, name:str, ref, parent_comp_def, src_ref):
+    def register_element(self, name: str, ref, parent_comp_def, src_ref):
         if name in self.element_ns_stack[-1]:
             self.msg.fatal(
                 "Multiple declarations of instance '%s'" % name,
                 src_ref
             )
         self.element_ns_stack[-1][name] = (ref, parent_comp_def)
 
-    def register_default_property(self, name:str, ref, src_ref, overwrite_ok=False):
+    def register_default_property(self, name: str, ref, src_ref, overwrite_ok=False):
         if not overwrite_ok:
             if name in self.default_property_ns_stack[-1]:
                 self.msg.fatal(
                     "Default property '%s' was already assigned in this scope" % name,
                     src_ref
                 )
 
         self.default_property_ns_stack[-1][name] = (src_ref, ref)
 
-    def lookup_type(self, name:str):
+    def lookup_type(self, name: str):
         for scope in reversed(self.type_ns_stack):
             if name in scope:
                 return scope[name]
         return None
 
-    def lookup_element(self, name:str):
+    def lookup_element(self, name: str):
         for idx, scope in enumerate(reversed(self.element_ns_stack)):
             if name in scope:
                 el, parent_def = scope[name]
                 if idx == 0:
                     # Return anything from local namespace
                     return (el, parent_def)
                 elif isinstance(el, comp.Signal):
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/rdlformatcode.py` & `systemrdl-compiler-1.9.0/systemrdl/core/rdlformatcode.py`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/ComponentVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/core/ComponentVisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         # Scratchpad to pass stuff down between visitor functions
         self._tmp = None
 
     #---------------------------------------------------------------------------
     # Component Definitions
     #---------------------------------------------------------------------------
-    def visitComponent_body(self, ctx:SystemRDLParser.Component_bodyContext):
+    def visitComponent_body(self, ctx: SystemRDLParser.Component_bodyContext):
         self.compiler.namespace.enter_scope()
 
         self.component.def_src_ref = SourceRef.from_antlr(ctx)
 
         # Re-Load any parameters into the local scope
         for param in self.component.parameters:
             self.compiler.namespace.register_element(param.name, param, None, None)
@@ -69,15 +69,15 @@
 
         self.apply_local_properties()
         self.apply_dynamic_properties()
 
         self.compiler.namespace.exit_scope()
         return self.component
 
-    def visitComponent_def(self, ctx:SystemRDLParser.Component_defContext):
+    def visitComponent_def(self, ctx: SystemRDLParser.Component_defContext):
         """
         Create, and possibly instantiate a component
         """
 
         # Get definition. Returns Component
         if ctx.component_anon_def() is not None:
             comp_def = self.visit(ctx.component_anon_def())
@@ -103,15 +103,15 @@
 
                 # Pass some temporary info to visitComponent_insts
                 self._tmp = (comp_def, inst_type, None)
                 self.visit(ctx.component_insts())
 
         return None
 
-    def visitComponent_named_def(self, ctx:SystemRDLParser.Component_named_defContext):
+    def visitComponent_named_def(self, ctx: SystemRDLParser.Component_named_defContext):
         type_token = self.visit(ctx.component_type())
 
         self.check_comp_def_allowed(type_token)
 
         def_name = get_ID_text(ctx.ID())
         # Get any parameters for the component
         if ctx.param_def() is not None:
@@ -122,18 +122,21 @@
         # Recurse into the component definition body
         body = ctx.component_body()
         comp_def = self.define_component(body, type_token, def_name, param_defs)
 
         # Since the definition is named, register it with the namespace
         self.compiler.namespace.register_type(def_name, comp_def, SourceRef.from_antlr(ctx.ID()))
 
+        # A named component's scope name is the same as it's type name
+        comp_def._scope_name = def_name
+
         return comp_def
 
 
-    def visitComponent_anon_def(self, ctx:SystemRDLParser.Component_anon_defContext):
+    def visitComponent_anon_def(self, ctx: SystemRDLParser.Component_anon_defContext):
         type_token = self.visit(ctx.component_type())
 
         self.check_comp_def_allowed(type_token)
 
         body = ctx.component_body()
         comp_def = self.define_component(body, type_token, None, [])
 
@@ -160,15 +163,15 @@
                 visitor = subclass(self.compiler, def_name, param_defs)
                 return visitor.visit(body)
         raise RuntimeError
 
     #---------------------------------------------------------------------------
     # Component Instantiation
     #---------------------------------------------------------------------------
-    def visitExplicit_component_inst(self, ctx:SystemRDLParser.Explicit_component_instContext):
+    def visitExplicit_component_inst(self, ctx: SystemRDLParser.Explicit_component_instContext):
         if ctx.component_inst_type() is not None:
             inst_type = self.visit(ctx.component_inst_type())
         else:
             inst_type = None
 
         comp_def = self.component_def_from_token(ctx.ID())
 
@@ -187,15 +190,15 @@
 
         # Pass some temporary info to visitComponent_insts
         self._tmp = (comp_def, inst_type, alias_primary_inst)
         self.visit(ctx.component_insts())
 
         return None
 
-    def visitComponent_inst_alias(self, ctx:SystemRDLParser.Component_inst_aliasContext):
+    def visitComponent_inst_alias(self, ctx: SystemRDLParser.Component_inst_aliasContext):
         name = get_ID_text(ctx.ID())
         inst, _ = self.compiler.namespace.lookup_element(name)
         if inst is None:
             self.msg.fatal(
                 "Reference to '%s' not found" % name,
                 SourceRef.from_antlr(ctx.ID())
             )
@@ -207,37 +210,35 @@
         if inst.is_alias:
             self.msg.fatal(
                 "Alias primary register '%s' cannot be another alias" % name,
                 SourceRef.from_antlr(ctx.ID())
             )
         return inst
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # Unpack instance def info from parent
         comp_def, inst_type, alias_primary_inst = self._tmp
 
-        if comp_def.type_name is not None:
-            # Instantiating a named definition.
-            # Make a copy of the component def to preserve original definition
-            # in case it is being parameterized or gets altered
-            # with a dynamic property assign
-            comp_inst_template = deepcopy(comp_def)
-            comp_inst_template.original_def = comp_def
-        else:
-            # Anonymous declaration.
-            # No need to copy since declaration is single-use
-            comp_inst_template = comp_def
-            comp_inst_template.original_def = comp_def
-
         # Get a dictionary of parameter assignments
         if ctx.param_inst() is not None:
             param_assigns = self.visit(ctx.param_inst())
         else:
             param_assigns = {}
 
+        if param_assigns:
+            # Component definition is being parameterized.
+            # Make a copy of the definition prior to applying the parameters
+            # in order to preserve the original definition
+            comp_inst_template = deepcopy(comp_def)
+            comp_inst_template.original_def = comp_def
+        else:
+            # Component is not being parameterized. No need to copy it
+            comp_inst_template = comp_def
+            comp_inst_template.original_def = comp_def
+
         # Assign any parameter overrides to the instance template
         # Keep track of any override expressions as they are external references
         # to outside the instance's tree, and shall not be deepcopied.
         external_refs = []
         for param_name, (assign_expr, src_ref) in param_assigns.items():
             # Lookup corresponding parameter in component
             for comp_param in comp_inst_template.parameters:
@@ -247,15 +248,15 @@
             else:
                 self.msg.fatal(
                     "Parameter '%s' not found in definition for component '%s'"
                     % (param_name, comp_inst_template.name),
                     src_ref
                 )
 
-            # Override the value
+            # Override the parameter's value
             assign_expr = expressions.AssignmentCast(self.compiler.env, src_ref, assign_expr, param.param_type)
             assign_expr.predict_type()
             param.expr = assign_expr
             external_refs.append(assign_expr)
 
 
         # Resolve internal/external instance type
@@ -291,21 +292,35 @@
                     comp_inst_template.external = False
             else:
                 # Leave as None. Elaborate step will resolve later.
                 comp_inst_template.external = None
 
 
         # Do instantiations
+        common_type_name = comp_inst_template.type_name
         for inst in ctx.getTypedRuleContexts(SystemRDLParser.Component_instContext):
             # Make a copy of the template so that the instance is unique
+            # in case any dynamic property assignments are made to it.
+
             # Use a pre-loaded memo dictionary for this deepcopy to force
             # any external reference objects to be copied by reference only
             copy_by_ref_memo = {id(obj):obj for obj in external_refs}
             comp_inst = deepcopy(comp_inst_template, copy_by_ref_memo)
 
+            if common_type_name is None:
+                # 5.1.1-f: The first instance name of an anonymous definition is
+                #   also used as the component type name.
+                common_type_name = get_ID_text(inst.ID())
+            comp_inst.type_name = common_type_name
+
+            # If scope name was unset, then this was an anonymous declaration.
+            # Use the common type name inherited by the first instantiation
+            if comp_inst.original_def._scope_name is None:
+                comp_inst.original_def._scope_name = common_type_name
+
             # Pass some temporary info to visitComponent_inst
             self._tmp = comp_inst, alias_primary_inst
             self.visit(inst)
 
         return None
 
     def get_instance_assignment(self, ctx):
@@ -318,30 +333,22 @@
 
         visitor = ExprVisitor(self.compiler)
         expr = visitor.visit(ctx.expr())
         expr = expressions.AssignmentCast(self.compiler.env, SourceRef.from_antlr(ctx.op), expr, int)
         expr.predict_type()
         return expr
 
-    def visitComponent_inst(self, ctx:SystemRDLParser.Component_instContext):
+    def visitComponent_inst(self, ctx: SystemRDLParser.Component_instContext):
         # Unpack instance def info from parent
         comp_inst, alias_primary_inst = self._tmp
 
         inst_name = get_ID_text(ctx.ID())
         comp_inst.inst_name = inst_name
         comp_inst.inst_src_ref = SourceRef.from_antlr(ctx.ID())
 
-        if comp_inst.type_name is None:
-            if comp_inst.original_def.type_name is None:
-                # 5.1.1-f: The first instance name of an anonymous definition is
-                #   also used as the component type name.
-                comp_inst.original_def.type_name = inst_name
-            comp_inst.type_name = comp_inst.original_def.type_name
-
-
         # Get array or range suffix
         array_suffixes = []
         for as_ctx in ctx.getTypedRuleContexts(SystemRDLParser.Array_suffixContext):
             array_suffixes.append(self.visit(as_ctx))
 
         if ctx.range_suffix() is not None:
             range_suffix = self.visit(ctx.range_suffix())
@@ -419,15 +426,15 @@
                     SourceRef.from_antlr(ctx.field_inst_reset().start)
                 )
 
 
         # Specifying stride is only allowed if an array suffix is used
         if (inst_addr_stride is not None) and (not array_suffixes):
             self.msg.fatal(
-                "Unexpected address stride allocator '%=' on non-array instance",
+                "Unexpected address stride allocator '+=' on non-array instance",
                 SourceRef.from_antlr(ctx.inst_addr_stride().start)
             )
 
         # Do instantiation
         comp_inst.is_instance = True
         if isinstance(comp_inst, comp.VectorComponent):
             if range_suffix is not None:
@@ -464,29 +471,29 @@
         )
 
         return None
 
     #---------------------------------------------------------------------------
     # Parameters
     #---------------------------------------------------------------------------
-    def visitParam_def(self, ctx:SystemRDLParser.Param_defContext):
+    def visitParam_def(self, ctx: SystemRDLParser.Param_defContext):
         """
         Parameter Definition block
         """
         self.compiler.namespace.enter_scope()
 
         param_defs = []
         for elem in ctx.getTypedRuleContexts(SystemRDLParser.Param_def_elemContext):
             param_def = self.visit(elem)
             param_defs.append(param_def)
 
         self.compiler.namespace.exit_scope()
         return param_defs
 
-    def visitParam_def_elem(self, ctx:SystemRDLParser.Param_def_elemContext):
+    def visitParam_def_elem(self, ctx: SystemRDLParser.Param_def_elemContext):
         """
         Individual parameter definition elements
         """
 
         # Construct parameter type
         data_type_token = self.visit(ctx.data_type())
         param_data_type = self.datatype_from_token(data_type_token)
@@ -513,15 +520,15 @@
         param = Parameter(param_type, param_name, default_expr)
 
         # Register it in the parameter def namespace scope
         self.compiler.namespace.register_element(param_name, param, None, SourceRef.from_antlr(ctx.ID()))
 
         return param
 
-    def visitParam_inst(self, ctx:SystemRDLParser.Param_instContext):
+    def visitParam_inst(self, ctx: SystemRDLParser.Param_instContext):
         param_assigns = {}
         for assignment in ctx.getTypedRuleContexts(SystemRDLParser.Param_assignmentContext):
             param_name, assign_expr = self.visit(assignment)
 
             src_ref = SourceRef.from_antlr(assignment.ID())
 
             if param_name in param_assigns:
@@ -529,26 +536,26 @@
                     "Duplicate assignment to parameter '%s'" % param_name,
                     src_ref
                 )
 
             param_assigns[param_name] = (assign_expr, src_ref)
         return param_assigns
 
-    def visitParam_assignment(self, ctx:SystemRDLParser.Param_assignmentContext):
+    def visitParam_assignment(self, ctx: SystemRDLParser.Param_assignmentContext):
         param_name = get_ID_text(ctx.ID())
 
         visitor = ExprVisitor(self.compiler)
         # Note: AssignmentCast is handled in the visitComponent_insts Visitor
         assign_expr = visitor.visit(ctx.expr())
         return param_name, assign_expr
 
     #---------------------------------------------------------------------------
     # Property Assignments
     #---------------------------------------------------------------------------
-    def visitLocal_property_assignment(self, ctx:SystemRDLParser.Local_property_assignmentContext):
+    def visitLocal_property_assignment(self, ctx: SystemRDLParser.Local_property_assignmentContext):
 
         default = (ctx.DEFAULT_kw() is not None)
 
         if ctx.normal_prop_assign() is not None:
             prop_src_ref, prop_name, rhs = self.visit(ctx.normal_prop_assign())
         elif ctx.encode_prop_assign() is not None:
             prop_src_ref, prop_name, rhs = self.visit(ctx.encode_prop_assign())
@@ -589,15 +596,15 @@
                 self.msg.fatal(
                     "Property '%s' was already assigned in this scope" % prop_name,
                     prop_src_ref
                 )
             else:
                 self.property_dict[prop_name] = (prop_src_ref, rhs)
 
-    def visitDynamic_property_assignment(self, ctx:SystemRDLParser.Dynamic_property_assignmentContext):
+    def visitDynamic_property_assignment(self, ctx: SystemRDLParser.Dynamic_property_assignmentContext):
 
         # List of component instance names in the hierarchical path
         name_tokens = self.visit(ctx.instance_ref())
 
         if ctx.normal_prop_assign() is not None:
             prop_src_ref, prop_name, rhs = self.visit(ctx.normal_prop_assign())
         elif ctx.encode_prop_assign() is not None:
@@ -605,14 +612,21 @@
         else:
             raise RuntimeError
 
         # Lookup component instance being assigned
         target_inst = self.component
         for name_token in name_tokens:
             inst_name = get_ID_text(name_token)
+
+            if target_inst is not self.component:
+                # target_inst is an intermediate component in the hier path
+                # mark the child that is being modified
+                target_inst._dyn_assigned_children.append(inst_name)
+
+            # Traverse to next child in token list
             target_inst = target_inst.get_child_by_name(inst_name)
             if target_inst is None:
                 # Not found!
                 self.msg.fatal(
                     "Could not resolve hierarchical reference to '%s'" % inst_name,
                     SourceRef.from_antlr(name_token)
                 )
@@ -625,35 +639,38 @@
                 % (prop_name, get_ID_text(name_tokens[-1])),
                 prop_src_ref
             )
         else:
             target_inst_dict[prop_name] = (prop_src_ref, rhs)
         self.dynamic_property_dict[target_inst] = target_inst_dict
 
+        # Mark the property as dynamically assigned
+        target_inst._dyn_assigned_props.append(prop_name)
+
 
-    def visitInstance_ref(self, ctx:SystemRDLParser.Instance_refContext):
+    def visitInstance_ref(self, ctx: SystemRDLParser.Instance_refContext):
         name_tokens = []
         for ref_elem in ctx.getTypedRuleContexts(SystemRDLParser.Instance_ref_elementContext):
             name_tokens.append(self.visit(ref_elem))
         return name_tokens
 
-    def visitInstance_ref_element(self, ctx:SystemRDLParser.Instance_ref_elementContext):
+    def visitInstance_ref_element(self, ctx: SystemRDLParser.Instance_ref_elementContext):
         name_token = ctx.ID()
 
         # Intentionally not supporting array references in dynamic assignments
         # due to heterogeneous array complications.
         for as_ctx in ctx.getTypedRuleContexts(SystemRDLParser.Array_suffixContext):
             self.msg.fatal(
                 "Use of array suffixes in dynamic property assignments is not supported",
                 SourceRef.from_antlr(as_ctx)
             )
 
         return name_token
 
-    def visitNormal_prop_assign(self, ctx:SystemRDLParser.Normal_prop_assignContext):
+    def visitNormal_prop_assign(self, ctx: SystemRDLParser.Normal_prop_assignContext):
 
         # Get property string
         if ctx.prop_keyword() is not None:
             prop_token = self.visit(ctx.prop_keyword())
             prop_name = prop_token.text
         else:
             prop_token = ctx.ID()
@@ -664,15 +681,15 @@
         else:
             # No explicit RHS
             # What this implies is resolved later
             rhs = None
 
         return SourceRef.from_antlr(prop_token), prop_name, rhs
 
-    def visitEncode_prop_assign(self, ctx:SystemRDLParser.Encode_prop_assignContext):
+    def visitEncode_prop_assign(self, ctx: SystemRDLParser.Encode_prop_assignContext):
         # Get property string
         prop_token = ctx.ENCODE_kw()
         prop_name = get_ID_text(prop_token)
 
         enum_name = get_ID_text(ctx.ID())
 
         enum_type = self.compiler.namespace.lookup_type(enum_name)
@@ -687,39 +704,39 @@
                 SourceRef.from_antlr(ctx.ID())
             )
         rhs = enum_type
 
         return SourceRef.from_antlr(prop_token), prop_name, rhs
 
 
-    def visitProp_mod_assign(self, ctx:SystemRDLParser.Prop_mod_assignContext):
+    def visitProp_mod_assign(self, ctx: SystemRDLParser.Prop_mod_assignContext):
         prop_mod_token = self.visit(ctx.prop_mod())
         prop_mod = prop_mod_token.text
 
         intr_token = ctx.ID()
 
         if intr_token.getText() != "intr":
             self.msg.fatal(
                 "extraneous input '%s' expecting 'intr'" % intr_token.getText(),
                 SourceRef.from_antlr(intr_token)
             )
 
         return SourceRef.from_antlr(prop_mod_token), prop_mod
 
-    def visitProp_assignment_rhs(self, ctx:SystemRDLParser.Prop_assignment_rhsContext):
+    def visitProp_assignment_rhs(self, ctx: SystemRDLParser.Prop_assignment_rhsContext):
 
         if ctx.expr() is not None:
             visitor = ExprVisitor(self.compiler)
             rhs = visitor.visit(ctx.expr())
         else:
             rhs = self.visit(ctx.precedencetype_literal())
 
         return rhs
 
-    def visitPrecedencetype_literal(self, ctx:SystemRDLParser.Precedencetype_literalContext):
+    def visitPrecedencetype_literal(self, ctx: SystemRDLParser.Precedencetype_literalContext):
         return rdltypes.PrecedenceType[ctx.kw.text]
 
     def apply_local_properties(self):
 
         # First, apply default property assignments inherited from namespace
         for prop_name, (prop_src_ref, prop_rhs) in self.compiler.namespace.get_default_properties(type(self.component)).items():
             rule = self.compiler.env.property_rules.lookup_property(prop_name)
@@ -796,27 +813,27 @@
 
         # Clear out pending assignments now that they have been resolved
         self.dynamic_property_dict = {}
 
     #---------------------------------------------------------------------------
     # Array and Range suffixes
     #---------------------------------------------------------------------------
-    def visitRange_suffix(self, ctx:SystemRDLParser.Range_suffixContext):
+    def visitRange_suffix(self, ctx: SystemRDLParser.Range_suffixContext):
         visitor = ExprVisitor(self.compiler)
         expr1 = visitor.visit(ctx.expr(0))
         expr1 = expressions.AssignmentCast(self.compiler.env, SourceRef.from_antlr(ctx.expr(0)), expr1, int)
         expr1.predict_type()
 
         expr2 = visitor.visit(ctx.expr(1))
         expr2 = expressions.AssignmentCast(self.compiler.env, SourceRef.from_antlr(ctx.expr(1)), expr2, int)
         expr2.predict_type()
 
         return expr1, expr2
 
-    def visitArray_suffix(self, ctx:SystemRDLParser.Array_suffixContext):
+    def visitArray_suffix(self, ctx: SystemRDLParser.Array_suffixContext):
         visitor = ExprVisitor(self.compiler)
         expr = visitor.visit(ctx.expr())
         expr = expressions.AssignmentCast(self.compiler.env, SourceRef.from_antlr(ctx.expr()), expr, int)
         expr.predict_type()
         return expr
 
     #---------------------------------------------------------------------------
@@ -838,65 +855,65 @@
             )
 
         return comp_def
 
     #---------------------------------------------------------------------------
     # User-defined enum
     #---------------------------------------------------------------------------
-    def visitEnum_def(self, ctx:SystemRDLParser.Enum_defContext):
+    def visitEnum_def(self, ctx: SystemRDLParser.Enum_defContext):
         visitor = EnumVisitor(self.compiler)
         enum_type, name, src_ref = visitor.visit(ctx)
         enum_type._set_parent_scope(self.component)
         self.compiler.namespace.register_type(name, enum_type, src_ref)
 
     #---------------------------------------------------------------------------
     # User-defined struct
     #---------------------------------------------------------------------------
-    def visitStruct_def(self, ctx:SystemRDLParser.Struct_defContext):
+    def visitStruct_def(self, ctx: SystemRDLParser.Struct_defContext):
         visitor = StructVisitor(self.compiler)
         struct_type, name, src_ref = visitor.visit(ctx)
         struct_type._set_parent_scope(self.component)
         self.compiler.namespace.register_type(name, struct_type, src_ref)
 
     #---------------------------------------------------------------------------
     # Constraint Definition
     #---------------------------------------------------------------------------
-    def visitConstraint_def(self, ctx:SystemRDLParser.Constraint_defContext):
+    def visitConstraint_def(self, ctx: SystemRDLParser.Constraint_defContext):
         # TODO: Implement constraints
         pass
 
 #===============================================================================
 # Root meta-component visitor
 #===============================================================================
 class RootVisitor(ComponentVisitor):
     comp_type = comp.Root
 
-    def visitRoot(self, ctx:SystemRDLParser.RootContext):
+    def visitRoot(self, ctx: SystemRDLParser.RootContext):
         self.visitChildren(ctx)
         self.apply_dynamic_properties()
 
 
     def define_component(self, body, type_token, def_name, param_defs):
         comp_def = super().define_component(body, type_token, def_name, param_defs)
 
         if def_name is not None:
             self.component.comp_defs[def_name] = comp_def
 
         return comp_def
 
-    def visitComponent_anon_def(self, ctx:SystemRDLParser.Component_anon_defContext):
+    def visitComponent_anon_def(self, ctx: SystemRDLParser.Component_anon_defContext):
         type_token = self.visit(ctx.component_type())
         if type_token.type == SystemRDLParser.ADDRMAP_kw:
             self.msg.fatal(
                 "Definitions of addrmap components in the root namespace must declare a type name.",
                 SourceRef.from_antlr(type_token)
             )
         return super().visitComponent_anon_def(ctx)
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # Unpack instance def info from parent
         comp_def, inst_type, alias_primary_inst = self._tmp #pylint: disable=unused-variable
 
         if not isinstance(comp_def, comp.Signal):
             self.msg.fatal(
                 "Instantiation of '%s' components not allowed in the root namespace"
                 % type(comp_def).__name__.lower(),
@@ -904,25 +921,25 @@
             )
 
         return super().visitComponent_insts(ctx)
 
     #---------------------------------------------------------------------------
     # User-defined Properties
     #---------------------------------------------------------------------------
-    def visitUdp_def(self, ctx:SystemRDLParser.Udp_defContext):
+    def visitUdp_def(self, ctx: SystemRDLParser.Udp_defContext):
         visitor = UDPVisitor(self.compiler)
         visitor.visit(ctx)
 
 #===============================================================================
 # Field Component visitor
 #===============================================================================
 class FieldComponentVisitor(ComponentVisitor):
     comp_type = comp.Field
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # 9.2-a: No other types of structural components shall be defined within a field component.
         self.msg.fatal(
             "Instantiation of components not allowed inside a field definition",
             SourceRef.from_antlr(ctx.component_inst(0).ID())
         )
 
     def check_comp_def_allowed(self, type_token):
@@ -933,15 +950,15 @@
 
 #===============================================================================
 # Reg Component visitor
 #===============================================================================
 class RegComponentVisitor(ComponentVisitor):
     comp_type = comp.Reg
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # Unpack instance def info from parent
         comp_def, inst_type, alias_primary_inst = self._tmp #pylint: disable=unused-variable
 
         # 10.2-b-1-ii: Component instantiations are limited to field, constraint, and signal instances
         if not isinstance(comp_def, (comp.Signal, comp.Field)):
             self.msg.fatal(
                 "Instantiation of '%s' components not allowed inside a reg definition"
@@ -963,15 +980,15 @@
 
 #===============================================================================
 # Regfile Component visitor
 #===============================================================================
 class RegfileComponentVisitor(ComponentVisitor):
     comp_type = comp.Regfile
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # Unpack instance def info from parent
         comp_def, inst_type, alias_primary_inst = self._tmp #pylint: disable=unused-variable
 
         # 12.1-b-1-ii: Component instantiations are limited to reg, regfile, constraint, and signal instances
         if not isinstance(comp_def, (comp.Signal, comp.Reg, comp.Regfile)):
             self.msg.fatal(
                 "Instantiation of '%s' components not allowed inside a regfile definition"
@@ -992,15 +1009,15 @@
             )
 #===============================================================================
 # Addrmap Component visitor
 #===============================================================================
 class AddrmapComponentVisitor(ComponentVisitor):
     comp_type = comp.Addrmap
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # Unpack instance def info from parent
         comp_def, inst_type, alias_primary_inst = self._tmp #pylint: disable=unused-variable
 
         # 13.3-a: The components instantiated within an address map shall be
         #   registers, register files, memories, address maps, or signals.
         if not isinstance(comp_def, (comp.Reg, comp.Regfile, comp.Mem, comp.Addrmap, comp.Signal)):
             self.msg.fatal(
@@ -1012,15 +1029,15 @@
 
 #===============================================================================
 # Mem Component visitor
 #===============================================================================
 class MemComponentVisitor(ComponentVisitor):
     comp_type = comp.Mem
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         # Unpack instance def info from parent
         comp_def, inst_type, alias_primary_inst = self._tmp #pylint: disable=unused-variable
 
         # 11.1-b-a-ii: Component instantiations are limited to reg and constraint instances.
         if not isinstance(comp_def, comp.Reg):
             self.msg.fatal(
                 "Instantiation of '%s' components not allowed inside a mem definition"
@@ -1041,15 +1058,15 @@
             )
 #===============================================================================
 # Signal Component visitor
 #===============================================================================
 class SignalComponentVisitor(ComponentVisitor):
     comp_type = comp.Signal
 
-    def visitComponent_insts(self, ctx:SystemRDLParser.Component_instsContext):
+    def visitComponent_insts(self, ctx: SystemRDLParser.Component_instsContext):
         self.msg.fatal(
             "Instantiation of components not allowed inside a signal definition",
             SourceRef.from_antlr(ctx.component_inst(0).ID())
         )
 
     def check_comp_def_allowed(self, type_token):
         self.msg.fatal(
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/expressions.py` & `systemrdl-compiler-1.9.0/systemrdl/core/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     def predict_type(self):
 
         if not self.elements:
             # Empty array. Element type is indeterminate
             return rdltypes.ArrayPlaceholder(None)
 
         # Get type of first element
-        element_iter = iter( self.elements)
+        element_iter = iter(self.elements)
         element_type = next(element_iter).predict_type()
 
         # All remaining elements shall match
         for element in element_iter:
             if element_type != element.predict_type():
                 self.msg.fatal(
                     "Elements of an array shall be the same type",
@@ -322,15 +322,15 @@
             self.reps_value = self.reps.get_value()
 
         if self.type == int:
             width = self.concat.get_min_eval_width()
             val = int(self.concat.get_value())
 
             result = 0
-            for i in range(self.reps_value):
+            for _ in range(self.reps_value):
                 result <<= width
                 result |= val
 
             return result
 
         elif self.type == str:
             result = self.concat.get_value()
@@ -545,15 +545,15 @@
             r = int(self.r.get_value(eval_width))
         elif not self.is_numeric:
             l = self.l.get_value()
             r = self.r.get_value()
         else:
             raise RuntimeError
 
-        return l,r
+        return l, r
 
 class _NumericRelationalExpr(_RelationalExpr):
 
     def predict_type(self):
         l_type = self.l.predict_type()
         r_type = self.r.predict_type()
 
@@ -571,40 +571,40 @@
             )
         return bool
 
 
 
 class Eq(_RelationalExpr):
     def get_value(self, eval_width=None):
-        l,r = self.get_ops()
+        l, r = self.get_ops()
         return l == r
 
 class Neq(_RelationalExpr):
     def get_value(self, eval_width=None):
-        l,r = self.get_ops()
+        l, r = self.get_ops()
         return l != r
 
 class Lt(_NumericRelationalExpr):
     def get_value(self, eval_width=None):
-        l,r = self.get_ops()
+        l, r = self.get_ops()
         return l < r
 
 class Gt(_NumericRelationalExpr):
     def get_value(self, eval_width=None):
-        l,r = self.get_ops()
+        l, r = self.get_ops()
         return l > r
 
 class Leq(_NumericRelationalExpr):
     def get_value(self, eval_width=None):
-        l,r = self.get_ops()
+        l, r = self.get_ops()
         return l <= r
 
 class Geq(_NumericRelationalExpr):
     def get_value(self, eval_width=None):
-        l,r = self.get_ops()
+        l, r = self.get_ops()
         return l >= r
 
 #-------------------------------------------------------------------------------
 # Reduction operators:
 #   &  ~&  |  ~|  ^  ^~  !
 # Result is always 1 bit bool
 # Creates a new evaluation context
@@ -1104,15 +1104,15 @@
         """
         Build a resolved ComponentRef container that describes the relative path
         """
 
         resolved_ref_elements = []
 
         for name, array_suffixes, name_src_ref in self.ref_elements:
-            idx_list = [ suffix.get_value() for suffix in array_suffixes ]
+            idx_list = [suffix.get_value() for suffix in array_suffixes]
             resolved_ref_elements.append((name, idx_list, name_src_ref))
 
         # Create container
         cref = rdltypes.ComponentRef(self.ref_root, resolved_ref_elements)
 
         return cref
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/UDPVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/core/UDPVisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class UDPVisitor(BaseVisitor):
     def __init__(self, compiler):
         super().__init__(compiler)
 
         # Attributes
         self.attr = {}
 
-    def visitUdp_def(self, ctx:SystemRDLParser.Udp_defContext):
+    def visitUdp_def(self, ctx: SystemRDLParser.Udp_defContext):
         udp_name = get_ID_text(ctx.ID())
 
         # Collect all attributes
         for attr_ctx in ctx.getTypedRuleContexts(SystemRDLParser.Udp_attrContext):
             self.visit(attr_ctx)
 
         # Check attribute rules
@@ -75,15 +75,15 @@
             self.attr['default'] = expr.get_value()
 
         # Create and register the new property rule
         udp = properties.UserProperty(self.compiler.env, udp_name, **self.attr)
         self.compiler.env.property_rules.register_udp(udp, SourceRef.from_antlr(ctx.ID()))
 
 
-    def visitUdp_type(self, ctx:SystemRDLParser.Udp_typeContext):
+    def visitUdp_type(self, ctx: SystemRDLParser.Udp_typeContext):
         # Determine which type this property can hold
         if 'valid_types' in self.attr:
             self.msg.fatal(
                 "More than one 'type' attribute specified for user-defined property",
                 SourceRef.from_antlr(ctx.TYPE_kw())
             )
 
@@ -114,15 +114,15 @@
         SystemRDLParser.REG_kw      : comp.Reg,
         SystemRDLParser.REGFILE_kw  : comp.Regfile,
         SystemRDLParser.ADDRMAP_kw  : comp.Addrmap,
         SystemRDLParser.MEM_kw      : comp.Mem,
         SystemRDLParser.SIGNAL_kw   : comp.Signal,
         #SystemRDLParser.CONSTRAINT_kw   : TODO,
     }
-    def visitUdp_usage(self, ctx:SystemRDLParser.Udp_usageContext):
+    def visitUdp_usage(self, ctx: SystemRDLParser.Udp_usageContext):
         # Determine which components the UDP can be bound to
         if 'bindable_to' in self.attr:
             self.msg.fatal(
                 "More than one 'component' attribute specified for user-defined property",
                 SourceRef.from_antlr(ctx.COMPONENT_kw())
             )
 
@@ -136,26 +136,26 @@
 
         comp_types = list(set(comp_types))
 
 
         self.attr['bindable_to'] = comp_types
 
 
-    def visitUdp_default(self, ctx:SystemRDLParser.Udp_defaultContext):
+    def visitUdp_default(self, ctx: SystemRDLParser.Udp_defaultContext):
         if 'default' in self.attr:
             self.msg.fatal(
                 "More than one 'default' attribute specified for user-defined property",
                 SourceRef.from_antlr(ctx.DEFAULT_kw())
             )
 
         # defer expr evaluation until later
         self.attr['default'] = ctx.expr()
 
 
-    def visitUdp_constraint(self, ctx:SystemRDLParser.Udp_constraintContext):
+    def visitUdp_constraint(self, ctx: SystemRDLParser.Udp_constraintContext):
         # There is only one type of constraint even allowed by the grammar
         # no need to explore further
         if 'constr_componentwidth' in self.attr:
             self.msg.fatal(
                 "More than one 'constraint' attribute specified for user-defined property",
                 SourceRef.from_antlr(ctx.CONSTRAINT_kw())
             )
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/BaseVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/core/BaseVisitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,33 +64,33 @@
 
     def passthru_kw_token(self, ctx):
         if ctx.kw is not None:
             return ctx.kw
         else:
             return self.visitChildren(ctx)
 
-    def visitComponent_inst_type(self, ctx:SystemRDLParser.Component_inst_typeContext):
+    def visitComponent_inst_type(self, ctx: SystemRDLParser.Component_inst_typeContext):
         return self.passthru_kw_token(ctx)
 
-    def visitComponent_type(self, ctx:SystemRDLParser.Component_typeContext):
+    def visitComponent_type(self, ctx: SystemRDLParser.Component_typeContext):
         return self.passthru_kw_token(ctx)
 
-    def visitComponent_type_primary(self, ctx:SystemRDLParser.Component_type_primaryContext):
+    def visitComponent_type_primary(self, ctx: SystemRDLParser.Component_type_primaryContext):
         return self.passthru_kw_token(ctx)
 
-    def visitData_type(self, ctx:SystemRDLParser.Data_typeContext):
+    def visitData_type(self, ctx: SystemRDLParser.Data_typeContext):
         return self.passthru_kw_token(ctx)
 
-    def visitBasic_data_type(self, ctx:SystemRDLParser.Basic_data_typeContext):
+    def visitBasic_data_type(self, ctx: SystemRDLParser.Basic_data_typeContext):
         return self.passthru_kw_token(ctx)
 
-    def visitProp_keyword(self, ctx:SystemRDLParser.Prop_keywordContext):
+    def visitProp_keyword(self, ctx: SystemRDLParser.Prop_keywordContext):
         return self.passthru_kw_token(ctx)
 
-    def visitProp_mod(self, ctx:SystemRDLParser.Prop_modContext):
+    def visitProp_mod(self, ctx: SystemRDLParser.Prop_modContext):
         return self.passthru_kw_token(ctx)
 
-    def visitUdp_data_type(self, ctx:SystemRDLParser.Udp_data_typeContext):
+    def visitUdp_data_type(self, ctx: SystemRDLParser.Udp_data_typeContext):
         return self.passthru_kw_token(ctx)
 
-    def visitUdp_comp_type(self, ctx:SystemRDLParser.Udp_comp_typeContext):
+    def visitUdp_comp_type(self, ctx: SystemRDLParser.Udp_comp_typeContext):
         return self.passthru_kw_token(ctx)
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/backports.py` & `systemrdl-compiler-1.9.0/systemrdl/core/backports.py`

 * *Files identical despite different names*

### Comparing `systemrdl-compiler-1.8.0/systemrdl/core/ExprVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/core/ExprVisitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,61 +49,61 @@
         SystemRDLParser.OR      : e.OrReduce,
         SystemRDLParser.NOR     : e.NorReduce,
         SystemRDLParser.XOR     : e.XorReduce,
         SystemRDLParser.XNOR    : e.XnorReduce
     }
 
     # Visit a parse tree produced by SystemRDLParser#BinaryExpr.
-    def visitBinaryExpr(self, ctx:SystemRDLParser.BinaryExprContext):
+    def visitBinaryExpr(self, ctx: SystemRDLParser.BinaryExprContext):
         l = self.visit(ctx.expr(0))
         r = self.visit(ctx.expr(1))
         expr_class = self._BinaryExpr_map[ctx.op.type]
         return expr_class(self.compiler.env, SourceRef.from_antlr(ctx.op), l, r)
 
 
     # Visit a parse tree produced by SystemRDLParser#UnaryExpr.
-    def visitUnaryExpr(self, ctx:SystemRDLParser.UnaryExprContext):
+    def visitUnaryExpr(self, ctx: SystemRDLParser.UnaryExprContext):
         n = self.visit(ctx.expr_primary())
         expr_class = self._UnaryExpr_map[ctx.op.type]
         return expr_class(self.compiler.env, SourceRef.from_antlr(ctx.op), n)
 
 
     # Visit a parse tree produced by SystemRDLParser#TernaryExpr.
-    def visitTernaryExpr(self, ctx:SystemRDLParser.TernaryExprContext):
+    def visitTernaryExpr(self, ctx: SystemRDLParser.TernaryExprContext):
         i = self.visit(ctx.expr(0))
         j = self.visit(ctx.expr(1))
         k = self.visit(ctx.expr(2))
         return e.TernaryExpr(self.compiler.env, SourceRef.from_antlr(ctx.op), i, j, k)
 
 
     # Visit a parse tree produced by SystemRDLParser#paren_expr.
-    def visitParen_expr(self, ctx:SystemRDLParser.Paren_exprContext):
+    def visitParen_expr(self, ctx: SystemRDLParser.Paren_exprContext):
         return self.visit(ctx.expr())
 
     #---------------------------------------------------------------------------
     # Numeric Literals
     #---------------------------------------------------------------------------
     # Visit a parse tree produced by SystemRDLParser#NumberInt.
-    def visitNumberInt(self, ctx:SystemRDLParser.NumberIntContext):
+    def visitNumberInt(self, ctx: SystemRDLParser.NumberIntContext):
         s = ctx.INT().getText()
-        s = s.replace("_","")
+        s = s.replace("_", "")
         return e.IntLiteral(self.compiler.env, SourceRef.from_antlr(ctx.INT()), int(s))
 
 
     # Visit a parse tree produced by SystemRDLParser#NumberHex.
-    def visitNumberHex(self, ctx:SystemRDLParser.NumberHexContext):
+    def visitNumberHex(self, ctx: SystemRDLParser.NumberHexContext):
         s = ctx.HEX_INT().getText()
-        s = s.replace("_","")
-        return e.IntLiteral(self.compiler.env, SourceRef.from_antlr(ctx.HEX_INT()), int(s,16))
+        s = s.replace("_", "")
+        return e.IntLiteral(self.compiler.env, SourceRef.from_antlr(ctx.HEX_INT()), int(s, 16))
 
 
     # Visit a parse tree produced by SystemRDLParser#NumberVerilog.
-    def visitNumberVerilog(self, ctx:SystemRDLParser.NumberVerilogContext):
+    def visitNumberVerilog(self, ctx: SystemRDLParser.NumberVerilogContext):
         s = ctx.VLOG_INT().getText()
-        s = s.replace("_","")
+        s = s.replace("_", "")
         m = re.fullmatch(r"(\d+)'(b|d|h)([\da-f]+)", s, re.IGNORECASE)
         width = int(m.group(1))
         basechar = m.group(2).lower()
         if basechar == "b":
             base = 2
         elif basechar == "d":
             base = 10
@@ -124,57 +124,57 @@
                 SourceRef.from_antlr(ctx.VLOG_INT())
             )
 
         return e.IntLiteral(self.compiler.env, SourceRef.from_antlr(ctx.VLOG_INT()), val, width)
 
 
     # Visit a parse tree produced by SystemRDLParser#boolean_literal.
-    def visitBoolean_literal(self, ctx:SystemRDLParser.Boolean_literalContext):
+    def visitBoolean_literal(self, ctx: SystemRDLParser.Boolean_literalContext):
         if ctx.val.type == SystemRDLParser.TRUE_kw:
             return e.IntLiteral(self.compiler.env, SourceRef.from_antlr(ctx.val), 1, 1)
         else:
             return e.IntLiteral(self.compiler.env, SourceRef.from_antlr(ctx.val), 0, 1)
 
     #---------------------------------------------------------------------------
     # Built-in RDL Enumeration literals
     #---------------------------------------------------------------------------
-    def visitAccesstype_literal(self, ctx:SystemRDLParser.Accesstype_literalContext):
+    def visitAccesstype_literal(self, ctx: SystemRDLParser.Accesstype_literalContext):
         if ctx.kw.text == "wr":
             # same as rw
             value = rdltypes.AccessType.rw
         else:
             value = rdltypes.AccessType[ctx.kw.text]
 
         return e.BuiltinEnumLiteral(self.compiler.env, SourceRef.from_antlr(ctx.kw), value)
 
-    def visitOnreadtype_literal(self, ctx:SystemRDLParser.Onreadtype_literalContext):
+    def visitOnreadtype_literal(self, ctx: SystemRDLParser.Onreadtype_literalContext):
         return e.BuiltinEnumLiteral(self.compiler.env, SourceRef.from_antlr(ctx.kw), rdltypes.OnReadType[ctx.kw.text])
 
-    def visitOnwritetype_literal(self, ctx:SystemRDLParser.Onwritetype_literalContext):
+    def visitOnwritetype_literal(self, ctx: SystemRDLParser.Onwritetype_literalContext):
         return e.BuiltinEnumLiteral(self.compiler.env, SourceRef.from_antlr(ctx.kw), rdltypes.OnWriteType[ctx.kw.text])
 
-    def visitAddressingtype_literal(self, ctx:SystemRDLParser.Addressingtype_literalContext):
+    def visitAddressingtype_literal(self, ctx: SystemRDLParser.Addressingtype_literalContext):
         return e.BuiltinEnumLiteral(self.compiler.env, SourceRef.from_antlr(ctx.kw), rdltypes.AddressingType[ctx.kw.text])
 
     #---------------------------------------------------------------------------
     # Misc other literals
     #---------------------------------------------------------------------------
-    def visitString_literal(self, ctx:SystemRDLParser.String_literalContext):
+    def visitString_literal(self, ctx: SystemRDLParser.String_literalContext):
         string = ctx.STRING().getText()
 
         # Remove leading and trailing quotes (guaranteed to exist)
-        string = string [1:-1]
+        string = string[1:-1]
 
         # Remove backslashes from any escaped characters
         string = re.sub(r'\\(.)', r'\1', string)
 
         return e.StringLiteral(self.compiler.env, SourceRef.from_antlr(ctx.STRING()), string)
 
 
-    def visitEnum_literal(self, ctx:SystemRDLParser.Enum_literalContext):
+    def visitEnum_literal(self, ctx: SystemRDLParser.Enum_literalContext):
         enum_type_name = get_ID_text(ctx.ID(0))
         enum_entry_name = get_ID_text(ctx.ID(1))
 
         # Lookup the enum type
         enum_type = self.compiler.namespace.lookup_type(enum_type_name)
         if enum_type is None:
             self.msg.fatal(
@@ -195,26 +195,26 @@
                 % (enum_entry_name, enum_type_name),
                 SourceRef.from_antlr(ctx.ID(1))
             )
 
         return e.EnumLiteral(self.compiler.env, SourceRef.from_antlr(ctx), enum_type[enum_entry_name])
 
 
-    def visitArray_literal(self, ctx:SystemRDLParser.Array_literalContext):
+    def visitArray_literal(self, ctx: SystemRDLParser.Array_literalContext):
         elements = []
         for expr_ctx in ctx.getTypedRuleContexts(SystemRDLParser.ExprContext):
             elm_expr = self.visit(expr_ctx)
             elements.append(elm_expr)
 
         expr = e.ArrayLiteral(self.compiler.env, SourceRef.from_antlr(ctx), elements)
         expr.predict_type()
         return expr
 
 
-    def visitStruct_literal(self, ctx:SystemRDLParser.Struct_literalContext):
+    def visitStruct_literal(self, ctx: SystemRDLParser.Struct_literalContext):
         struct_type_name = get_ID_text(ctx.ID())
 
         # Lookup the struct type
         struct_type = self.compiler.namespace.lookup_type(struct_type_name)
         if struct_type is None:
             self.msg.fatal(
                 "Struct type '%s' not found" % struct_type_name,
@@ -267,67 +267,67 @@
             struct_type,
             values
         )
         expr.predict_type()
         return expr
 
 
-    def visitStruct_kv(self, ctx:SystemRDLParser.Struct_kvContext):
+    def visitStruct_kv(self, ctx: SystemRDLParser.Struct_kvContext):
         member_name = get_ID_text(ctx.ID())
         member_name_src_ref = SourceRef.from_antlr(ctx.ID())
         member_expr = self.visit(ctx.expr())
         return member_name, member_expr, member_name_src_ref
 
     #---------------------------------------------------------------------------
     # Aggregate Operators
     #---------------------------------------------------------------------------
-    def visitConcatenate(self, ctx:SystemRDLParser.ConcatenateContext):
+    def visitConcatenate(self, ctx: SystemRDLParser.ConcatenateContext):
         elements = []
         for expr_ctx in ctx.getTypedRuleContexts(SystemRDLParser.ExprContext):
             elm_expr = self.visit(expr_ctx)
             elements.append(elm_expr)
 
         expr = e.Concatenate(self.compiler.env, SourceRef.from_antlr(ctx), elements)
         expr.predict_type()
         return expr
 
 
-    def visitReplicate(self, ctx:SystemRDLParser.ReplicateContext):
+    def visitReplicate(self, ctx: SystemRDLParser.ReplicateContext):
         reps_expr = self.visit(ctx.expr())
         concat_expr = self.visit(ctx.concatenate())
         expr = e.Replicate(self.compiler.env, SourceRef.from_antlr(ctx), reps_expr, concat_expr)
         expr.predict_type()
         return expr
 
     #---------------------------------------------------------------------------
     # Cast
     #---------------------------------------------------------------------------
     # Visit a parse tree produced by SystemRDLParser#CastType.
-    def visitCastType(self, ctx:SystemRDLParser.CastTypeContext):
+    def visitCastType(self, ctx: SystemRDLParser.CastTypeContext):
         if ctx.typ.type == SystemRDLParser.LONGINT_kw:
             # Longint gets truncated to 64-bits
             return e.WidthCast(self.compiler.env, SourceRef.from_antlr(ctx.op), self.visit(ctx.expr()), w_int=64)
         elif ctx.typ.type == SystemRDLParser.BIT_kw:
             # Cast to bit remains unaffected, but in self-determined context
             # Use assignment cast to isolate evaluation
             return e.AssignmentCast(self.compiler.env, SourceRef.from_antlr(ctx.op), self.visit(ctx.expr()), int)
         elif ctx.typ.type == SystemRDLParser.BOOLEAN_kw:
             return e.BoolCast(self.compiler.env, SourceRef.from_antlr(ctx.op), self.visit(ctx.expr()))
         else:
             raise RuntimeError
 
     # Visit a parse tree produced by SystemRDLParser#CastWidth.
-    def visitCastWidth(self, ctx:SystemRDLParser.CastWidthContext):
+    def visitCastWidth(self, ctx: SystemRDLParser.CastWidthContext):
         w = self.visit(ctx.cast_width_expr())
         return e.WidthCast(self.compiler.env, SourceRef.from_antlr(ctx.op), self.visit(ctx.expr()), w_expr=w)
 
     #---------------------------------------------------------------------------
     # References
     #---------------------------------------------------------------------------
-    def visitInstance_ref(self, ctx:SystemRDLParser.Instance_refContext):
+    def visitInstance_ref(self, ctx: SystemRDLParser.Instance_refContext):
 
         # Get each ref element in a hierarchical chain. Each element is a tuple:
         #   (name, [index_expr, ...], SourceRef)
         ref_elements = []
         for ref_elem in ctx.getTypedRuleContexts(SystemRDLParser.Instance_ref_elementContext):
             ref_elements.append(self.visit(ref_elem))
 
@@ -359,25 +359,25 @@
                 ref_elements=ref_elements
             )
         else:
             raise RuntimeError
 
         return ref_expr
 
-    def visitInstance_ref_element(self, ctx:SystemRDLParser.Instance_ref_elementContext):
+    def visitInstance_ref_element(self, ctx: SystemRDLParser.Instance_ref_elementContext):
         name_token = ctx.ID()
         name = get_ID_text(name_token)
 
         array_suffixes = []
         for as_ctx in ctx.getTypedRuleContexts(SystemRDLParser.Array_suffixContext):
             array_suffixes.append(self.visit(as_ctx))
 
         return name, array_suffixes, SourceRef.from_antlr(name_token)
 
-    def visitProp_ref(self, ctx:SystemRDLParser.Prop_refContext):
+    def visitProp_ref(self, ctx: SystemRDLParser.Prop_refContext):
         ref_expr = self.visit(ctx.instance_ref())
 
         if ctx.prop_keyword() is not None:
             prop_token = self.visit(ctx.prop_keyword())
         else:
             prop_token = ctx.ID()
 
@@ -405,12 +405,12 @@
 
         #self.msg.fatal(
         #    "Property references in expressions are not supported.",
         #    SourceRef.from_antlr(prop_token)
         #)
         return propref_expr
 
-    def visitArray_suffix(self, ctx:SystemRDLParser.Array_suffixContext):
+    def visitArray_suffix(self, ctx: SystemRDLParser.Array_suffixContext):
         expr = self.visit(ctx.expr())
         expr = e.AssignmentCast(self.compiler.env, SourceRef.from_antlr(ctx.expr()), expr, int)
         expr.predict_type()
         return expr
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/parser/SystemRDLParser.py` & `systemrdl-compiler-1.9.0/systemrdl/parser/SystemRDLParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Generated from SystemRDL.g4 by ANTLR 4.7.1
+# Generated from SystemRDL.g4 by ANTLR 4.7.2
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 from typing.io import TextIO
 import sys
 
+
 def serializedATN():
     with StringIO() as buf:
         buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\3\177")
         buf.write("\u0321\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7\t\7")
         buf.write("\4\b\t\b\4\t\t\t\4\n\t\n\4\13\t\13\4\f\t\f\4\r\t\r\4\16")
         buf.write("\t\16\4\17\t\17\4\20\t\20\4\21\t\21\4\22\t\22\4\23\t\23")
         buf.write("\4\24\t\24\4\25\t\25\4\26\t\26\4\27\t\27\4\30\t\30\4\31")
@@ -692,20 +693,21 @@
     INC=122
     ALIGN=123
     WS=124
     ID=125
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.7.1")
+        self.checkVersion("4.7.2")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
+
     class RootContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def EOF(self):
@@ -755,14 +757,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Root_elemContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_def(self):
@@ -870,14 +873,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_named_def(self):
@@ -992,14 +996,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Explicit_component_instContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -1060,14 +1065,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_inst_aliasContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ALIAS_kw(self):
@@ -1102,14 +1108,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_named_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_type(self):
@@ -1164,14 +1171,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_anon_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_type(self):
@@ -1208,14 +1216,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_bodyContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_body_elem(self, i:int=None):
@@ -1264,14 +1273,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_body_elemContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_def(self):
@@ -1369,14 +1379,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_instsContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def component_inst(self, i:int=None):
@@ -1435,14 +1446,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_instContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -1554,14 +1566,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Field_inst_resetContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.op = None # Token
 
@@ -1598,14 +1611,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Inst_addr_fixedContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.op = None # Token
 
@@ -1642,14 +1656,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Inst_addr_strideContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.op = None # Token
 
@@ -1686,14 +1701,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Inst_addr_alignContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.op = None # Token
 
@@ -1730,14 +1746,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_inst_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -1778,14 +1795,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -1833,14 +1851,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Component_type_primaryContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -1890,14 +1909,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Param_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def param_def_elem(self, i:int=None):
@@ -1950,14 +1970,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Param_def_elemContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def data_type(self):
@@ -2023,14 +2044,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Param_instContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def param_assignment(self, i:int=None):
@@ -2083,14 +2105,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Param_assignmentContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -2132,14 +2155,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class ExprContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
@@ -2545,14 +2569,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.unrollRecursionContexts(_parentctx)
         return localctx
 
+
     class Expr_primaryContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def literal(self):
@@ -2670,14 +2695,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class ConcatenateContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expr(self, i:int=None):
@@ -2728,14 +2754,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class ReplicateContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expr(self):
@@ -2776,14 +2803,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Paren_exprContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expr(self):
@@ -2818,14 +2846,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class CastContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
@@ -2935,14 +2964,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Cast_width_exprContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def literal(self):
@@ -2990,14 +3020,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Range_suffixContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expr(self, i:int=None):
@@ -3039,14 +3070,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Array_suffixContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expr(self):
@@ -3081,14 +3113,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Array_type_suffixContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
@@ -3118,14 +3151,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Data_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -3189,14 +3223,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Basic_data_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -3276,14 +3311,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class LiteralContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def number(self):
@@ -3394,14 +3430,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class NumberContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
@@ -3496,14 +3533,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class String_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def STRING(self):
@@ -3533,14 +3571,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Boolean_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.val = None # Token
 
@@ -3581,14 +3620,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Array_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expr(self, i:int=None):
@@ -3658,14 +3698,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Struct_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -3723,14 +3764,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Struct_kvContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -3768,14 +3810,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Enum_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self, i:int=None):
@@ -3812,14 +3855,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Accesstype_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -3875,14 +3919,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Onreadtype_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -3926,14 +3971,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Onwritetype_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -3995,14 +4041,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Addressingtype_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -4046,14 +4093,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Precedencetype_literalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -4094,14 +4142,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Instance_refContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def instance_ref_element(self, i:int=None):
@@ -4148,14 +4197,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Instance_ref_elementContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -4203,14 +4253,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Prop_refContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def instance_ref(self):
@@ -4264,14 +4315,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Local_property_assignmentContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def normal_prop_assign(self):
@@ -4357,14 +4409,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Dynamic_property_assignmentContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def instance_ref(self):
@@ -4424,14 +4477,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Normal_prop_assignContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def prop_keyword(self):
@@ -4495,14 +4549,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Encode_prop_assignContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ENCODE_kw(self):
@@ -4542,14 +4597,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Prop_mod_assignContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def prop_mod(self):
@@ -4585,14 +4641,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Prop_assignment_rhsContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def precedencetype_literal(self):
@@ -4640,14 +4697,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Prop_keywordContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -4700,14 +4758,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Prop_modContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -4757,14 +4816,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def PROPERTY_kw(self):
@@ -4825,14 +4885,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_attrContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def udp_type(self):
@@ -4898,14 +4959,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def TYPE_kw(self):
@@ -4959,14 +5021,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_data_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -5033,14 +5096,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_usageContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def COMPONENT_kw(self):
@@ -5103,14 +5167,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_comp_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.kw = None # Token
 
@@ -5168,14 +5233,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_defaultContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def DEFAULT_kw(self):
@@ -5216,14 +5282,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Udp_constraintContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def CONSTRAINT_kw(self):
@@ -5263,14 +5330,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Enum_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ENUM_kw(self):
@@ -5331,14 +5399,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Enum_entryContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -5415,14 +5484,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Enum_prop_assignContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -5463,14 +5533,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Struct_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.name = None # Token
             self.base = None # Token
@@ -5555,14 +5626,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Struct_elemContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def struct_type(self):
@@ -5611,14 +5683,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Struct_typeContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def data_type(self):
@@ -5666,14 +5739,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constraint_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def constraint_named_def(self):
@@ -5736,14 +5810,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constraint_named_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def CONSTRAINT_kw(self):
@@ -5784,14 +5859,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constraint_anon_defContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def CONSTRAINT_kw(self):
@@ -5827,14 +5903,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constraint_bodyContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def constraint_body_elem(self, i:int=None):
@@ -5883,14 +5960,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constraint_body_elemContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def constr_relational(self):
@@ -5958,14 +6036,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constraint_instsContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self, i:int=None):
@@ -6011,14 +6090,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constr_relationalContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.op = None # Token
 
@@ -6082,14 +6162,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constr_prop_assignContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
@@ -6130,14 +6211,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constr_inside_valuesContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def constr_lhs(self):
@@ -6199,14 +6281,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constr_inside_enumContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def constr_lhs(self):
@@ -6247,14 +6330,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constr_lhsContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def THIS_kw(self):
@@ -6301,14 +6385,15 @@
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
+
     class Constr_inside_valueContext(ParserRuleContext):
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
             self.val = None # ExprContext
             self.l_val = None # ExprContext
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/parser/SystemRDLLexer.py` & `systemrdl-compiler-1.9.0/systemrdl/parser/SystemRDLLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Generated from SystemRDL.g4 by ANTLR 4.7.1
+# Generated from SystemRDL.g4 by ANTLR 4.7.2
 from antlr4 import *
 from io import StringIO
 from typing.io import TextIO
 import sys
 
 
+
 def serializedATN():
     with StringIO() as buf:
         buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\2\177")
         buf.write("\u03cf\b\1\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7")
         buf.write("\t\7\4\b\t\b\4\t\t\t\4\n\t\n\4\13\t\13\4\f\t\f\4\r\t\r")
         buf.write("\4\16\t\16\4\17\t\17\4\20\t\20\4\21\t\21\4\22\t\22\4\23")
         buf.write("\t\23\4\24\t\24\4\25\t\25\4\26\t\26\4\27\t\27\4\30\t\30")
@@ -625,13 +626,13 @@
                   "MULT", "EXP", "DIV", "MOD", "EQ", "ASSIGN", "NEQ", "LEQ", 
                   "LT", "GEQ", "GT", "AT", "INC", "ALIGN", "WS", "ID" ]
 
     grammarFileName = "SystemRDL.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.7.1")
+        self.checkVersion("4.7.2")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/parser/SystemRDLVisitor.py` & `systemrdl-compiler-1.9.0/systemrdl/parser/SystemRDLVisitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from SystemRDL.g4 by ANTLR 4.7.1
+# Generated from SystemRDL.g4 by ANTLR 4.7.2
 from antlr4 import *
 if __name__ is not None and "." in __name__:
     from .SystemRDLParser import SystemRDLParser
 else:
     from SystemRDLParser import SystemRDLParser
 
 # This class defines a complete generic visitor for a parse tree produced by SystemRDLParser.
```

### Comparing `systemrdl-compiler-1.8.0/systemrdl/component.py` & `systemrdl-compiler-1.9.0/systemrdl/component.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,20 +22,33 @@
         #: May remain ``None`` if scope is not known or not applicable.
         #:
         #: .. note::
         #:      This represents the parent *lexical* scope! This does *not*
         #:      refer to the hierarchical parent of this component.
         self.parent_scope = None
 
+        # Name of this component's declaration scope
+        # This field is only valid in non-instantiated components (referenced
+        # via an instance's original_def)
+        # If declaration was anonymous, inherits the first instance's name,
+        # otherwise it contains the original type name.
+        self._scope_name = None
+
         #: Named definition identifier.
-        #: If declaration was anonymous, inherits the first instance's name.
+        #: If declaration was anonymous, instantiation type names inherit
+        #: the first instance's name.
         #: The type name of parameterized components is normalized based on the
         #: instance's parameter values.
         #:
-        #: Importers may leave this as ``None``
+        #: If this is a non-instantiated component (referenced via an
+        #: instance's original_def), then it will contain either the original
+        #: type name, or None if the declaration was anonymous.
+        #:
+        #: Importers may leave this as ``None`` if an appropriate type name
+        #: cannot be imported.
         self.type_name = None
 
         #: List of :class:`~systemrdl.component.Component` instances that are
         #: direct descendants of this component.
         #:
         #: Child components are sorted as follows:
         #:
@@ -62,22 +75,33 @@
         self.is_instance = False
 
         #: Name of instantiated element
         self.inst_name = None
 
         #: Reference to original :class:`~systemrdl.component.Component`
         #: definition this instance is derived from.
+        #:
+        #: Importers may leave this as ``None`` if appropriate.
         self.original_def = None
 
         #: True if instance type is external. False if internal.
         self.external = None
 
         # SourceRef for the component instantiation.
         self.inst_src_ref = None
 
+        #------------------------------
+        # List of property names that were assigned via a dynamic property
+        # assignment.
+        self._dyn_assigned_props = []
+
+        # List of child instances that were assigned "through" this component,
+        # from outside this component's scope.
+        self._dyn_assigned_children = []
+
     def __deepcopy__(self, memo):
         """
         Deepcopy all members except for ones that should be copied by reference
         """
         copy_by_ref = ["original_def", "def_src_ref", "inst_src_ref", "parent_scope"]
         cls = self.__class__
         result = cls.__new__(cls)
@@ -116,27 +140,32 @@
 
         Parameters
         ----------
         scope_separator: str
             Override the separator between namespace scopes
         """
         if self.parent_scope is None:
+            # Importer likely never set the scope
             return ""
         elif isinstance(self.parent_scope, Root):
+            # Declaration was in root scope
             return ""
         else:
+            # Get parent definition's scope path
             parent_path = self.parent_scope.get_scope_path(scope_separator)
+
+            # Extend it with its scope name
             if parent_path:
                 return(
                     parent_path
                     + scope_separator
-                    + self.parent_scope.type_name
+                    + self.parent_scope._scope_name
                 )
             else:
-                return self.parent_scope.type_name
+                return self.parent_scope._scope_name
 
 
 class AddressableComponent(Component):
     """
     Base class for all components that can have an address
     """
 
@@ -220,14 +249,16 @@
     pass
 
 class Reg(AddressableComponent):
     def __init__(self):
         super().__init__()
 
         #: If true, fields are to be arranged in msb0 order
+        #:
+        #: .. versionadded:: 1.7
         self.is_msb0_order = False
         #------------------------------
         # Alias Register
         #------------------------------
         #: If true, then ``alias_primary_inst`` is valid
         self.is_alias = False
```

### Comparing `systemrdl-compiler-1.8.0/PKG-INFO` & `systemrdl-compiler-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemrdl-compiler
-Version: 1.8.0
+Version: 1.9.0
 Summary: Parse and elaborate front-end for SystemRDL 2.0
 Home-page: https://github.com/SystemRDL/systemrdl-compiler
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 License: UNKNOWN
 Project-URL: Documentation, http://systemrdl-compiler.readthedocs.io
 Project-URL: Source, https://github.com/SystemRDL/systemrdl-compiler
```

