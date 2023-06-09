# Comparing `tmp/example_helloworld-0.1.tar.gz` & `tmp/example_helloworld-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_helloworld-0.1.tar", last modified: Fri Jun  9 10:56:30 2023, max compression
+gzip compressed data, was "example_helloworld-1.0.tar", last modified: Fri Jun  9 12:05:53 2023, max compression
```

## Comparing `example_helloworld-0.1.tar` & `example_helloworld-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 10:56:30.233954 example_helloworld-0.1/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)     1073 2023-06-09 10:52:21.000000 example_helloworld-0.1/LICENSE
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      601 2023-06-09 10:56:30.233954 example_helloworld-0.1/PKG-INFO
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       51 2023-06-09 10:49:23.000000 example_helloworld-0.1/README.md
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 10:56:30.229954 example_helloworld-0.1/example_helloworld.egg-info/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      601 2023-06-09 10:56:30.000000 example_helloworld-0.1/example_helloworld.egg-info/PKG-INFO
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      232 2023-06-09 10:56:30.000000 example_helloworld-0.1/example_helloworld.egg-info/SOURCES.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)        1 2023-06-09 10:56:30.000000 example_helloworld-0.1/example_helloworld.egg-info/dependency_links.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       11 2023-06-09 10:56:30.000000 example_helloworld-0.1/example_helloworld.egg-info/top_level.txt
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 10:56:30.233954 example_helloworld-0.1/helloworld/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       22 2023-06-09 10:41:03.000000 example_helloworld-0.1/helloworld/__init__.py
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      520 2023-06-09 10:54:18.000000 example_helloworld-0.1/pyproject.toml
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       38 2023-06-09 10:56:30.233954 example_helloworld-0.1/setup.cfg
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      238 2023-06-09 10:40:36.000000 example_helloworld-0.1/setup.py
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 12:05:53.773954 example_helloworld-1.0/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)     1073 2023-06-09 10:52:21.000000 example_helloworld-1.0/LICENSE
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      602 2023-06-09 12:05:53.769954 example_helloworld-1.0/PKG-INFO
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       52 2023-06-09 11:55:20.000000 example_helloworld-1.0/README.md
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 12:05:53.769954 example_helloworld-1.0/example_helloworld.egg-info/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      602 2023-06-09 12:05:53.000000 example_helloworld-1.0/example_helloworld.egg-info/PKG-INFO
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      232 2023-06-09 12:05:53.000000 example_helloworld-1.0/example_helloworld.egg-info/SOURCES.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)        1 2023-06-09 12:05:53.000000 example_helloworld-1.0/example_helloworld.egg-info/dependency_links.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       11 2023-06-09 12:05:53.000000 example_helloworld-1.0/example_helloworld.egg-info/top_level.txt
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 12:05:53.769954 example_helloworld-1.0/helloworld/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       22 2023-06-09 10:41:03.000000 example_helloworld-1.0/helloworld/__init__.py
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      608 2023-06-09 12:03:09.000000 example_helloworld-1.0/pyproject.toml
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       38 2023-06-09 12:05:53.773954 example_helloworld-1.0/setup.cfg
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      317 2023-06-09 12:04:09.000000 example_helloworld-1.0/setup.py
```

### Comparing `example_helloworld-0.1/LICENSE` & `example_helloworld-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `example_helloworld-0.1/PKG-INFO` & `example_helloworld-1.0/example_helloworld.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: example_helloworld
-Version: 0.1
+Name: example-helloworld
+Version: 1.0
 Summary: Example hello world script
 Author: mishpro
 Author-email: mishpro <root@venusbiser.ru>
 Project-URL: Homepage, https://github.com/mishpro-programm/example_helloworld
 Project-URL: Bug Tracker, https://github.com/mishpro-programm/example_helloworld/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Hello world package
+Hello world package\
 Usage: ```import helloworld```
```

### Comparing `example_helloworld-0.1/example_helloworld.egg-info/PKG-INFO` & `example_helloworld-1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: example-helloworld
-Version: 0.1
+Name: example_helloworld
+Version: 1.0
 Summary: Example hello world script
 Author: mishpro
 Author-email: mishpro <root@venusbiser.ru>
 Project-URL: Homepage, https://github.com/mishpro-programm/example_helloworld
 Project-URL: Bug Tracker, https://github.com/mishpro-programm/example_helloworld/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Hello world package
+Hello world package\
 Usage: ```import helloworld```
```

