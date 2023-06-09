# Comparing `tmp/basic_math_operations-1.0.161.tar.gz` & `tmp/basic_math_operations-1.0.163.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_math_operations-1.0.161.tar", last modified: Fri Jun  9 12:01:53 2023, max compression
+gzip compressed data, was "basic_math_operations-1.0.163.tar", last modified: Fri Jun  9 12:28:03 2023, max compression
```

## Comparing `basic_math_operations-1.0.161.tar` & `basic_math_operations-1.0.163.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:01:53.569942 basic_math_operations-1.0.161/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 12:01:30.000000 basic_math_operations-1.0.161/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:01:53.569942 basic_math_operations-1.0.161/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-09 12:01:30.000000 basic_math_operations-1.0.161/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:01:53.569942 basic_math_operations-1.0.161/basic_math_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:01:53.000000 basic_math_operations-1.0.161/basic_math_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-09 12:01:53.000000 basic_math_operations-1.0.161/basic_math_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:01:53.000000 basic_math_operations-1.0.161/basic_math_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 12:01:53.000000 basic_math_operations-1.0.161/basic_math_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:01:53.569942 basic_math_operations-1.0.161/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-09 12:01:30.000000 basic_math_operations-1.0.161/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:01:53.569942 basic_math_operations-1.0.161/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:01:53.569942 basic_math_operations-1.0.161/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-06-09 12:01:53.000000 basic_math_operations-1.0.161/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-09 12:01:30.000000 basic_math_operations-1.0.161/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 12:01:53.000000 basic_math_operations-1.0.161/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/basic_math_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/src/python-module/version.txt
```

### Comparing `basic_math_operations-1.0.161/LICENSE` & `basic_math_operations-1.0.163/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.161/README.md` & `basic_math_operations-1.0.163/README.md`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.161/setup.py` & `basic_math_operations-1.0.163/setup.py`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.161/src/python-module/libbasic_math_operations.a` & `basic_math_operations-1.0.163/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.161/src/python-module/module.c` & `basic_math_operations-1.0.163/src/python-module/module.c`

 * *Files identical despite different names*

