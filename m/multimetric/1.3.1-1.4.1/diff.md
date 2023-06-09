# Comparing `tmp/multimetric-1.3.1.tar.gz` & `tmp/multimetric-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimetric-1.3.1.tar", last modified: Mon Mar 27 09:24:09 2023, max compression
+gzip compressed data, was "multimetric-1.4.1.tar", last modified: Fri Jun  9 19:33:56 2023, max compression
```

## Comparing `multimetric-1.3.1.tar` & `multimetric-1.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.652600 multimetric-1.3.1/
--rw-r--r--   0 jason     (1000) jason     (1000)     1455 2023-03-27 09:19:53.000000 multimetric-1.3.1/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)       59 2023-03-27 09:12:10.000000 multimetric-1.3.1/MANIFEST.in
--rw-r--r--   0 jason     (1000) jason     (1000)     1008 2023-03-27 09:24:09.652600 multimetric-1.3.1/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     7393 2023-03-27 09:12:25.000000 multimetric-1.3.1/README.md
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.630933 multimetric-1.3.1/multimetric/
--rw-r--r--   0 jason     (1000) jason     (1000)       18 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4386 2023-03-27 09:12:25.000000 multimetric-1.3.1/multimetric/__main__.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.641766 multimetric-1.3.1/multimetric/cls/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)      722 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/base.py
--rw-r--r--   0 jason     (1000) jason     (1000)      278 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/base_calc.py
--rw-r--r--   0 jason     (1000) jason     (1000)      284 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/base_stats.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.641766 multimetric-1.3.1/multimetric/cls/calc/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/calc/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3377 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/calc/halstead.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1967 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/calc/maintenance.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2192 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/calc/pylint.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4628 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/calc/tiobe.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.641766 multimetric-1.3.1/multimetric/cls/importer/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1061 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/base.py
--rw-r--r--   0 jason     (1000) jason     (1000)      375 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/filtered.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.641766 multimetric-1.3.1/multimetric/cls/importer/mods/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/mods/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)      534 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/mods/csv.py
--rw-r--r--   0 jason     (1000) jason     (1000)      686 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/mods/json.py
--rw-r--r--   0 jason     (1000) jason     (1000)      553 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/importer/pick.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.652600 multimetric-1.3.1/multimetric/cls/metric/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1714 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/comments.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1681 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/cyclomatic.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4257 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/fanout.py
--rw-r--r--   0 jason     (1000) jason     (1000)      907 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/loc.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2394 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/operands.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1583 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/metric/operators.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2107 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/modules.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.652600 multimetric-1.3.1/multimetric/cls/stats/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/stats/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1357 2023-03-27 09:12:10.000000 multimetric-1.3.1/multimetric/cls/stats/stats.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1680 2023-03-27 09:12:25.000000 multimetric-1.3.1/multimetric/fp.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-03-27 09:24:09.641766 multimetric-1.3.1/multimetric.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)     1008 2023-03-27 09:24:09.000000 multimetric-1.3.1/multimetric.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     1197 2023-03-27 09:24:09.000000 multimetric-1.3.1/multimetric.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-03-27 09:24:09.000000 multimetric-1.3.1/multimetric.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       58 2023-03-27 09:24:09.000000 multimetric-1.3.1/multimetric.egg-info/entry_points.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       31 2023-03-27 09:24:09.000000 multimetric-1.3.1/multimetric.egg-info/requires.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       12 2023-03-27 09:24:09.000000 multimetric-1.3.1/multimetric.egg-info/top_level.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       30 2023-03-27 09:12:10.000000 multimetric-1.3.1/requirements.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-03-27 09:24:09.652600 multimetric-1.3.1/setup.cfg
--rw-r--r--   0 jason     (1000) jason     (1000)     1757 2023-03-27 09:17:16.000000 multimetric-1.3.1/setup.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/
+-rw-r--r--   0 jason     (1000) jason     (1000)     1455 2023-03-27 09:19:53.000000 multimetric-1.4.1/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)       59 2023-03-27 09:12:10.000000 multimetric-1.4.1/MANIFEST.in
+-rw-r--r--   0 jason     (1000) jason     (1000)     1008 2023-06-09 19:33:56.156608 multimetric-1.4.1/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)     7393 2023-03-27 09:12:25.000000 multimetric-1.4.1/README.md
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/
+-rw-r--r--   0 jason     (1000) jason     (1000)       18 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     4386 2023-03-27 09:12:25.000000 multimetric-1.4.1/multimetric/__main__.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      722 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/base.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      278 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/base_calc.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      284 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/base_stats.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/calc/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     3377 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/halstead.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1967 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/maintenance.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2192 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/pylint.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     4628 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/tiobe.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/importer/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1061 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/base.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      375 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/filtered.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/importer/mods/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/mods/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      534 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/mods/csv.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      686 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/mods/json.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      553 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/pick.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/metric/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1714 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/comments.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1681 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/cyclomatic.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     4257 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/fanout.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      907 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/loc.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2394 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/operands.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1583 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/operators.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2107 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/modules.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/stats/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/stats/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1357 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/stats/stats.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1680 2023-03-27 09:12:25.000000 multimetric-1.4.1/multimetric/fp.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric.egg-info/
+-rw-r--r--   0 jason     (1000) jason     (1000)     1008 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)     1197 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       58 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/entry_points.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/requires.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       12 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/top_level.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-09 19:24:40.000000 multimetric-1.4.1/requirements.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-06-09 19:33:56.156608 multimetric-1.4.1/setup.cfg
+-rw-r--r--   0 jason     (1000) jason     (1000)     1757 2023-06-09 19:30:02.000000 multimetric-1.4.1/setup.py
```

### Comparing `multimetric-1.3.1/LICENSE` & `multimetric-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/PKG-INFO` & `multimetric-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 1.3.1
+Version: 1.4.1
 Summary: Calculate code metrics in various languages
-Home-page: https://github.com/aylustltd/multimetric
+Home-page: https://github.com/startupos/multimetric
 Author: Jason Nichols
 Author-email: jn@ayl.us
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -18,8 +18,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/plain
 License-File: LICENSE
 
-See https://github.com/aylustltd/multimetric for documentation
+See https://github.com/startupos/multimetric for documentation
```

### Comparing `multimetric-1.3.1/README.md` & `multimetric-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/__main__.py` & `multimetric-1.4.1/multimetric/__main__.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/base.py` & `multimetric-1.4.1/multimetric/cls/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/calc/halstead.py` & `multimetric-1.4.1/multimetric/cls/calc/halstead.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/calc/maintenance.py` & `multimetric-1.4.1/multimetric/cls/calc/maintenance.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/calc/pylint.py` & `multimetric-1.4.1/multimetric/cls/calc/pylint.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/calc/tiobe.py` & `multimetric-1.4.1/multimetric/cls/calc/tiobe.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/importer/base.py` & `multimetric-1.4.1/multimetric/cls/importer/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/importer/mods/csv.py` & `multimetric-1.4.1/multimetric/cls/importer/mods/csv.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/importer/mods/json.py` & `multimetric-1.4.1/multimetric/cls/importer/mods/json.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/importer/pick.py` & `multimetric-1.4.1/multimetric/cls/importer/pick.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/metric/comments.py` & `multimetric-1.4.1/multimetric/cls/metric/comments.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/metric/cyclomatic.py` & `multimetric-1.4.1/multimetric/cls/metric/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/metric/fanout.py` & `multimetric-1.4.1/multimetric/cls/metric/fanout.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/metric/loc.py` & `multimetric-1.4.1/multimetric/cls/metric/loc.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/metric/operands.py` & `multimetric-1.4.1/multimetric/cls/metric/operands.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/metric/operators.py` & `multimetric-1.4.1/multimetric/cls/metric/operators.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/modules.py` & `multimetric-1.4.1/multimetric/cls/modules.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/cls/stats/stats.py` & `multimetric-1.4.1/multimetric/cls/stats/stats.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric/fp.py` & `multimetric-1.4.1/multimetric/fp.py`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/multimetric.egg-info/PKG-INFO` & `multimetric-1.4.1/multimetric.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 1.3.1
+Version: 1.4.1
 Summary: Calculate code metrics in various languages
-Home-page: https://github.com/aylustltd/multimetric
+Home-page: https://github.com/startupos/multimetric
 Author: Jason Nichols
 Author-email: jn@ayl.us
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -18,8 +18,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/plain
 License-File: LICENSE
 
-See https://github.com/aylustltd/multimetric for documentation
+See https://github.com/startupos/multimetric for documentation
```

### Comparing `multimetric-1.3.1/multimetric.egg-info/SOURCES.txt` & `multimetric-1.4.1/multimetric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multimetric-1.3.1/setup.py` & `multimetric-1.4.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import subprocess
 import setuptools
 
-_long_description = "See https://github.com/aylustltd/multimetric for documentation"
+_long_description = "See https://github.com/startupos/multimetric for documentation"
 _long_description_content_type = "text/plain"
 try:
     _long_description = subprocess.check_output(
         ["pandoc", "--from", "markdown", "--to", "rst", "README.md"]).decode("utf-8")
     _long_description_content_type = "text/x-rst"
 except (subprocess.CalledProcessError, FileNotFoundError):
     pass
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="multimetric",
-    version="1.3.1",
+    version="1.4.1",
     author="Jason Nichols",
     author_email="jn@ayl.us",
     description="Calculate code metrics in various languages",
     long_description=_long_description,
     long_description_content_type=_long_description_content_type,
-    url="https://github.com/aylustltd/multimetric",
+    url="https://github.com/startupos/multimetric",
     packages=setuptools.find_packages(),
     install_requires=requirements,
         entry_points={
         "console_scripts": [
             "multimetric = multimetric.__main__:main",
         ]
     },
```

