# Comparing `tmp/speakleash-0.1.0.tar.gz` & `tmp/speakleash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.1.0.tar", last modified: Fri Jun  9 19:40:35 2023, max compression
+gzip compressed data, was "speakleash-0.1.1.tar", last modified: Fri Jun  9 19:59:57 2023, max compression
```

## Comparing `speakleash-0.1.0.tar` & `speakleash-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:40:35.836345 speakleash-0.1.0/
--rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.1.0/LICENSE
--rw-r--r--   0 skondracki   (502) staff       (20)     2293 2023-06-09 19:40:35.836052 speakleash-0.1.0/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)     1994 2023-06-09 19:37:08.000000 speakleash-0.1.0/README.md
--rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-06-09 19:40:35.836440 speakleash-0.1.0/setup.cfg
--rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-06-09 19:38:43.000000 speakleash-0.1.0/setup.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:40:35.833885 speakleash-0.1.0/speakleash/
--rw-r--r--   0 skondracki   (502) staff       (20)     6586 2023-06-09 19:27:17.000000 speakleash-0.1.0/speakleash/__init__.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:40:35.835672 speakleash-0.1.0/speakleash.egg-info/
--rw-r--r--   0 skondracki   (502) staff       (20)     2293 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/SOURCES.txt
--rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/dependency_links.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/requires.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/top_level.txt
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:59:57.196217 speakleash-0.1.1/
+-rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.1.1/LICENSE
+-rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-06-09 19:59:57.195922 speakleash-0.1.1/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)     1995 2023-06-09 19:57:52.000000 speakleash-0.1.1/README.md
+-rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-06-09 19:59:57.196313 speakleash-0.1.1/setup.cfg
+-rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-06-09 19:59:30.000000 speakleash-0.1.1/setup.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:59:57.193348 speakleash-0.1.1/speakleash/
+-rw-r--r--   0 skondracki   (502) staff       (20)     6586 2023-06-09 19:27:17.000000 speakleash-0.1.1/speakleash/__init__.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:59:57.195537 speakleash-0.1.1/speakleash.egg-info/
+-rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/SOURCES.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/dependency_links.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/requires.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.1.0/LICENSE` & `speakleash-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.1.0/PKG-INFO` & `speakleash-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.1.0
+Version: 0.1.1
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -89,15 +89,15 @@
 ```
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
-sl = Speakleash(replicate_t, "hr")
+sl = Speakleash(replicate_to, "hr")
 
 for d in sl.datasets:
     print(d.name)
     for doc in d.data:
         size_mb = round(d.characters/1024/1024)
         print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
```

### Comparing `speakleash-0.1.0/README.md` & `speakleash-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 ```
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
-sl = Speakleash(replicate_t, "hr")
+sl = Speakleash(replicate_to, "hr")
 
 for d in sl.datasets:
     print(d.name)
     for doc in d.data:
         size_mb = round(d.characters/1024/1024)
         print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
```

### Comparing `speakleash-0.1.0/setup.py` & `speakleash-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="speakleash",
-    version="0.1.0",
+    version="0.1.1",
     author="SpeakLeash Team",
     author_email="team@speakleash.org",
     description="SpeakLeash agnostic dataset for Polish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speakleash/speakleash",
     packages = ["speakleash"],
```

### Comparing `speakleash-0.1.0/speakleash/__init__.py` & `speakleash-0.1.1/speakleash/__init__.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.1.0/speakleash.egg-info/PKG-INFO` & `speakleash-0.1.1/speakleash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.1.0
+Version: 0.1.1
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -89,15 +89,15 @@
 ```
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
-sl = Speakleash(replicate_t, "hr")
+sl = Speakleash(replicate_to, "hr")
 
 for d in sl.datasets:
     print(d.name)
     for doc in d.data:
         size_mb = round(d.characters/1024/1024)
         print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
```

