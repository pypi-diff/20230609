# Comparing `tmp/wfdsl-0.2.5.tar.gz` & `tmp/wfdsl-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfdsl-0.2.5.tar", last modified: Thu Jun  1 23:52:24 2023, max compression
+gzip compressed data, was "wfdsl-0.2.6.tar", last modified: Fri Jun  9 20:11:44 2023, max compression
```

## Comparing `wfdsl-0.2.5.tar` & `wfdsl-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:52:24.637195 wfdsl-0.2.5/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-01-19 10:37:26.000000 wfdsl-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-01 23:52:24.637195 wfdsl-0.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       72 2023-01-19 10:37:26.000000 wfdsl-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:52:24.637195 wfdsl-0.2.5/dsl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/accessrights.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-02-16 02:21:38.000000 wfdsl-0.2.5/dsl/context.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/datatype.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/exechelper.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/filemgr.py
--rw-r--r--   0 root         (0) root         (0)    18111 2023-06-01 23:48:34.000000 wfdsl-0.2.5/dsl/fileop.py
--rw-r--r--   0 root         (0) root         (0)    11878 2023-04-30 12:21:22.000000 wfdsl-0.2.5/dsl/grammar.py
--rw-r--r--   0 root         (0) root         (0)    21176 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/graphgen.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-04-29 16:01:45.000000 wfdsl-0.2.5/dsl/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    10898 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/library.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/parser.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/pygen.py
--rw-r--r--   0 root         (0) root         (0)     1231 2023-04-29 16:01:45.000000 wfdsl-0.2.5/dsl/symtab.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/taskmgr.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/wfobj.py
--rw-r--r--   0 root         (0) root         (0)      459 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/wftimer.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 23:52:24.637195 wfdsl-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-01 23:52:15.000000 wfdsl-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:52:24.637195 wfdsl-0.2.5/wfdsl.egg-info/
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:11:44.591665 wfdsl-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-01-19 10:37:26.000000 wfdsl-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-09 20:11:44.591665 wfdsl-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       72 2023-01-19 10:37:26.000000 wfdsl-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:11:44.591665 wfdsl-0.2.6/dsl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/accessrights.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-02-16 02:21:38.000000 wfdsl-0.2.6/dsl/context.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/datatype.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/exechelper.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/filemgr.py
+-rw-r--r--   0 root         (0) root         (0)    18111 2023-06-01 23:48:34.000000 wfdsl-0.2.6/dsl/fileop.py
+-rw-r--r--   0 root         (0) root         (0)    11878 2023-04-30 12:21:22.000000 wfdsl-0.2.6/dsl/grammar.py
+-rw-r--r--   0 root         (0) root         (0)    21176 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/graphgen.py
+-rw-r--r--   0 root         (0) root         (0)    16699 2023-06-09 19:43:55.000000 wfdsl-0.2.6/dsl/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    10898 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/library.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/parser.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/pygen.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-04-29 16:01:45.000000 wfdsl-0.2.6/dsl/symtab.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/taskmgr.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/wfobj.py
+-rw-r--r--   0 root         (0) root         (0)      459 2023-01-19 10:37:26.000000 wfdsl-0.2.6/dsl/wftimer.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 20:11:44.591665 wfdsl-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-09 20:11:40.000000 wfdsl-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:11:44.591665 wfdsl-0.2.6/wfdsl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-09 20:11:44.000000 wfdsl-0.2.6/wfdsl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-09 20:11:44.000000 wfdsl-0.2.6/wfdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 20:11:44.000000 wfdsl-0.2.6/wfdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 20:11:44.000000 wfdsl-0.2.6/wfdsl.egg-info/top_level.txt
```

### Comparing `wfdsl-0.2.5/LICENSE` & `wfdsl-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/PKG-INFO` & `wfdsl-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfdsl
-Version: 0.2.5
+Version: 0.2.6
 Summary: Workflow Domain Specific Language
 Home-page: https://github.com/srlabUsask/wfdsl
 Author: Muhammad Mainul Hossain
 Author-email: mainul.hossain@usask.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wfdsl-0.2.5/dsl/accessrights.py` & `wfdsl-0.2.6/dsl/accessrights.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/context.py` & `wfdsl-0.2.6/dsl/context.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/fileop.py` & `wfdsl-0.2.6/dsl/fileop.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/grammar.py` & `wfdsl-0.2.6/dsl/grammar.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/graphgen.py` & `wfdsl-0.2.6/dsl/graphgen.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/interpreter.py` & `wfdsl-0.2.6/dsl/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,16 @@
             return left < right
         elif operator == '>':
             return left > right
         elif operator == '<=':
             return left <= right
         elif operator == '>=':
             return left >= right
+        elif operator == '!=':
+            return left != right
         else:
             return left == right
     
     def doand(self, expr):
         '''
         Executes "and" expression.
         :param expr:
```

### Comparing `wfdsl-0.2.5/dsl/library.py` & `wfdsl-0.2.6/dsl/library.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/parser.py` & `wfdsl-0.2.6/dsl/parser.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/pygen.py` & `wfdsl-0.2.6/dsl/pygen.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/symtab.py` & `wfdsl-0.2.6/dsl/symtab.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/taskmgr.py` & `wfdsl-0.2.6/dsl/taskmgr.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/dsl/wfobj.py` & `wfdsl-0.2.6/dsl/wfobj.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.5/setup.py` & `wfdsl-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wfdsl",
-    version="0.2.5",
+    version="0.2.6",
     author="Muhammad Mainul Hossain",
     author_email="mainul.hossain@usask.ca",
     description="Workflow Domain Specific Language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/srlabUsask/wfdsl",
     packages=setuptools.find_packages(),
```

### Comparing `wfdsl-0.2.5/wfdsl.egg-info/PKG-INFO` & `wfdsl-0.2.6/wfdsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfdsl
-Version: 0.2.5
+Version: 0.2.6
 Summary: Workflow Domain Specific Language
 Home-page: https://github.com/srlabUsask/wfdsl
 Author: Muhammad Mainul Hossain
 Author-email: mainul.hossain@usask.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

