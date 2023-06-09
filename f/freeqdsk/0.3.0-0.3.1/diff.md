# Comparing `tmp/freeqdsk-0.3.0.tar.gz` & `tmp/freeqdsk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeqdsk-0.3.0.tar", last modified: Wed Apr  5 12:36:35 2023, max compression
+gzip compressed data, was "freeqdsk-0.3.1.tar", last modified: Fri Jun  9 07:43:00 2023, max compression
```

## Comparing `freeqdsk-0.3.0.tar` & `freeqdsk-0.3.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.168869 freeqdsk-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.168869 freeqdsk-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.168869 freeqdsk-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.168869 freeqdsk-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/source/_fileutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/source/aeqdsk.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/source/geqdsk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/docs/source/peqdsk.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.168869 freeqdsk-0.3.0/freeqdsk/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/freeqdsk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/freeqdsk/_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 12:36:35.000000 freeqdsk-0.3.0/freeqdsk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    31623 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/freeqdsk/aeqdsk.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/freeqdsk/geqdsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/freeqdsk/peqdsk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/freeqdsk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-05 12:36:35.000000 freeqdsk-0.3.0/freeqdsk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-05 12:36:35.000000 freeqdsk-0.3.0/freeqdsk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:36:35.000000 freeqdsk-0.3.0/freeqdsk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-05 12:36:35.000000 freeqdsk-0.3.0/freeqdsk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 12:36:35.000000 freeqdsk-0.3.0/freeqdsk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.168869 freeqdsk-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/tests/data/aeqdsk/
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/data/aeqdsk/test_1.aeqdsk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/tests/data/geqdsk/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/data/geqdsk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   190428 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/data/geqdsk/test_1.geqdsk
--rw-r--r--   0 runner    (1001) docker     (123)   234034 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/data/geqdsk/test_2.geqdsk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:36:35.172869 freeqdsk-0.3.0/tests/data/peqdsk/
--rw-r--r--   0 runner    (1001) docker     (123)   137393 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/data/peqdsk/test_1.peqdsk
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/test_aeqdsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/test_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/test_geqdsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/test_peqdsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-05 12:36:21.000000 freeqdsk-0.3.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.759719 freeqdsk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.739719 freeqdsk-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.743718 freeqdsk-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-09 07:43:00.759719 freeqdsk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.743718 freeqdsk-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.747719 freeqdsk-0.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/source/_fileutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/source/aeqdsk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/source/geqdsk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/docs/source/peqdsk.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.751719 freeqdsk-0.3.1/freeqdsk/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/freeqdsk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/freeqdsk/_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 07:43:00.000000 freeqdsk-0.3.1/freeqdsk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31623 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/freeqdsk/aeqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/freeqdsk/geqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/freeqdsk/peqdsk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.755719 freeqdsk-0.3.1/freeqdsk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-09 07:43:00.000000 freeqdsk-0.3.1/freeqdsk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-09 07:43:00.000000 freeqdsk-0.3.1/freeqdsk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:43:00.000000 freeqdsk-0.3.1/freeqdsk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 07:43:00.000000 freeqdsk-0.3.1/freeqdsk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 07:43:00.000000 freeqdsk-0.3.1/freeqdsk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:43:00.759719 freeqdsk-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.755719 freeqdsk-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.739719 freeqdsk-0.3.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.755719 freeqdsk-0.3.1/tests/data/aeqdsk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/data/aeqdsk/test_1.aeqdsk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.759719 freeqdsk-0.3.1/tests/data/geqdsk/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/data/geqdsk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   190428 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/data/geqdsk/test_1.geqdsk
+-rw-r--r--   0 runner    (1001) docker     (123)   234034 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/data/geqdsk/test_2.geqdsk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:43:00.759719 freeqdsk-0.3.1/tests/data/peqdsk/
+-rw-r--r--   0 runner    (1001) docker     (123)   137393 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/data/peqdsk/test_1.peqdsk
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/test_aeqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/test_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/test_geqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/test_peqdsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-09 07:42:44.000000 freeqdsk-0.3.1/tests/utils.py
```

### Comparing `freeqdsk-0.3.0/.github/workflows/black.yml` & `freeqdsk-0.3.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/.github/workflows/publish.yml` & `freeqdsk-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/.github/workflows/tests.yml` & `freeqdsk-0.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/.gitignore` & `freeqdsk-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/.readthedocs.yaml` & `freeqdsk-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/LICENSE` & `freeqdsk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/PKG-INFO` & `freeqdsk-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeqdsk
-Version: 0.3.0
+Version: 0.3.1
 Summary: GEQDSK and AEQDSK tokamak equilibrium file reader/writer
 Author: Ben Dudson, Peter Hill, Liam Pattinson
 License: Copyright 2016 Ben Dudson
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `freeqdsk-0.3.0/README.md` & `freeqdsk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/docs/Makefile` & `freeqdsk-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/docs/make.bat` & `freeqdsk-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/docs/source/_fileutils.rst` & `freeqdsk-0.3.1/docs/source/_fileutils.rst`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/docs/source/conf.py` & `freeqdsk-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/docs/source/index.rst` & `freeqdsk-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/freeqdsk/_fileutils.py` & `freeqdsk-0.3.1/freeqdsk/_fileutils.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/freeqdsk/aeqdsk.py` & `freeqdsk-0.3.1/freeqdsk/aeqdsk.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/freeqdsk/geqdsk.py` & `freeqdsk-0.3.1/freeqdsk/geqdsk.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/freeqdsk/peqdsk.py` & `freeqdsk-0.3.1/freeqdsk/peqdsk.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/freeqdsk.egg-info/PKG-INFO` & `freeqdsk-0.3.1/freeqdsk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeqdsk
-Version: 0.3.0
+Version: 0.3.1
 Summary: GEQDSK and AEQDSK tokamak equilibrium file reader/writer
 Author: Ben Dudson, Peter Hill, Liam Pattinson
 License: Copyright 2016 Ben Dudson
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `freeqdsk-0.3.0/freeqdsk.egg-info/SOURCES.txt` & `freeqdsk-0.3.1/freeqdsk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/pyproject.toml` & `freeqdsk-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
     "numpy >= 1.8",
-    "fortranformat",
+    "fortranformat ~= 2.0",
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest >= 3.3.0",
     "pytest-cov",
 ]
```

### Comparing `freeqdsk-0.3.0/tests/data/aeqdsk/test_1.aeqdsk` & `freeqdsk-0.3.1/tests/data/aeqdsk/test_1.aeqdsk`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/data/geqdsk/test_1.geqdsk` & `freeqdsk-0.3.1/tests/data/geqdsk/test_1.geqdsk`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/data/geqdsk/test_2.geqdsk` & `freeqdsk-0.3.1/tests/data/geqdsk/test_2.geqdsk`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/data/peqdsk/test_1.peqdsk` & `freeqdsk-0.3.1/tests/data/peqdsk/test_1.peqdsk`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/test_aeqdsk.py` & `freeqdsk-0.3.1/tests/test_aeqdsk.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/test_fileutils.py` & `freeqdsk-0.3.1/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/test_geqdsk.py` & `freeqdsk-0.3.1/tests/test_geqdsk.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/test_peqdsk.py` & `freeqdsk-0.3.1/tests/test_peqdsk.py`

 * *Files identical despite different names*

### Comparing `freeqdsk-0.3.0/tests/utils.py` & `freeqdsk-0.3.1/tests/utils.py`

 * *Files identical despite different names*

