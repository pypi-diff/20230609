# Comparing `tmp/sphinx_link_fixer-1.1.0.tar.gz` & `tmp/sphinx_link_fixer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_link_fixer-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_link_fixer-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_link_fixer-1.1.0.tar` & `sphinx_link_fixer-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      346 2023-06-03 14:08:07.236725 sphinx_link_fixer-1.1.0/.gitignore
--rw-r--r--   0        0        0      657 2023-06-03 11:21:11.173363 sphinx_link_fixer-1.1.0/LICENSE
--rw-r--r--   0        0        0     4195 2023-06-03 13:19:20.726706 sphinx_link_fixer-1.1.0/README.md
--rw-r--r--   0        0        0       82 2023-06-03 13:35:16.856712 sphinx_link_fixer-1.1.0/mypy.ini
--rw-r--r--   0        0        0      667 2023-06-03 13:03:39.216700 sphinx_link_fixer-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0    13435 2023-06-03 14:11:44.590060 sphinx_link_fixer-1.1.0/release.sh
--rw-r--r--   0        0        0        5 2022-07-22 16:42:44.109466 sphinx_link_fixer-1.1.0/requirements-release.txt
--rw-r--r--   0        0        0       11 2023-06-03 13:37:39.666713 sphinx_link_fixer-1.1.0/requirements-test.txt
--rw-r--r--   0        0        0        0 2022-07-22 16:42:44.109466 sphinx_link_fixer-1.1.0/requirements.txt
--rw-r--r--   0        0        0       45 2023-06-03 12:59:34.336698 sphinx_link_fixer-1.1.0/src/sphinx_link_fixer/__init__.py
--rwxr-xr-x   0        0        0    20394 2023-06-03 14:54:14.480076 sphinx_link_fixer-1.1.0/src/sphinx_link_fixer/main.py
--rw-r--r--   0        0        0      433 2023-06-03 14:04:36.503390 sphinx_link_fixer-1.1.0/tox.ini
--rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 sphinx_link_fixer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      346 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/.gitignore
+-rw-r--r--   0        0        0      657 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4195 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/README.md
+-rw-r--r--   0        0        0       82 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/mypy.ini
+-rw-r--r--   0        0        0      667 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0    13435 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/release.sh
+-rw-r--r--   0        0        0        5 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/requirements-release.txt
+-rw-r--r--   0        0        0       11 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/requirements-test.txt
+-rw-r--r--   0        0        0        0 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/requirements.txt
+-rw-r--r--   0        0        0       45 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/src/sphinx_link_fixer/__init__.py
+-rwxr-xr-x   0        0        0    20623 2023-06-09 19:27:17.982316 sphinx_link_fixer-1.1.1/src/sphinx_link_fixer/main.py
+-rw-r--r--   0        0        0      433 2023-06-07 08:49:16.337278 sphinx_link_fixer-1.1.1/tox.ini
+-rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 sphinx_link_fixer-1.1.1/PKG-INFO
```

### Comparing `sphinx_link_fixer-1.1.0/LICENSE` & `sphinx_link_fixer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_link_fixer-1.1.0/README.md` & `sphinx_link_fixer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_link_fixer-1.1.0/pyproject.toml` & `sphinx_link_fixer-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_link_fixer-1.1.0/release.sh` & `sphinx_link_fixer-1.1.1/release.sh`

 * *Files identical despite different names*

### Comparing `sphinx_link_fixer-1.1.0/src/sphinx_link_fixer/main.py` & `sphinx_link_fixer-1.1.1/src/sphinx_link_fixer/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 In order to figure out the correct references this script tries to import and inspect the code
 for which the documentation should be fixed. Therefore this script must be run in an environment
 where this code is installed. If --in-venv is not passed thris script runs itself in venv.
 If venv does not exist it is created.
 '''
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 
 import os
 import sys
 import argparse
 import re
 import importlib
@@ -449,14 +449,19 @@
 			if self.has_object(tgt, DefinitionType.PARAM):
 				return [tgt]
 			#else:
 				# When referencing the parameter of a constructor from a different method
 				# ref.tgt is 'ClassName.param' and ref.nested_defs is 'pkg.mod.ClassName.meth'
 				# resulting in tgt = 'pkg.mod.ClassName.ClassName.param' which is invalid because the class is duplicated.
 				# In this case the usual algorithm should be tried instead.
+		elif ref.role in ROLES_PARAMREF:
+			func_name, param_name = ref.tgt.rsplit('.', 1)
+			if func_name in self.functions_with_kw:
+				# I cannot check whether ref.tgt is valid or not, I'll leave that to sphinx
+				return [ref.tgt]
 
 		elif ref.role in ROLES_MEMBER and '.' not in ref.tgt and ref.nested_defs:
 			if ref.nested_defs[-1].definition_type is DefinitionType.METH:
 				i1 = -1
 			else:
 				i1 = None
```

### Comparing `sphinx_link_fixer-1.1.0/PKG-INFO` & `sphinx_link_fixer-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-link-fixer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Convert all relative references to absolute references in .py and .rst files
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
```

