# Comparing `tmp/cbirds-0.0.12.tar.gz` & `tmp/cbirds-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbirds-0.0.12.tar", last modified: Fri Jun  9 00:13:27 2023, max compression
+gzip compressed data, was "cbirds-0.1.0.tar", last modified: Fri Jun  9 00:23:00 2023, max compression
```

## Comparing `cbirds-0.0.12.tar` & `cbirds-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:13:27.764513 cbirds-0.0.12/
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     1068 2023-06-04 19:12:12.000000 cbirds-0.0.12/LICENSE
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     3373 2023-06-09 00:13:27.764513 cbirds-0.0.12/PKG-INFO
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     2917 2023-06-09 00:12:58.000000 cbirds-0.0.12/README.md
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)      531 2023-06-09 00:13:13.000000 cbirds-0.0.12/pyproject.toml
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)       38 2023-06-09 00:13:27.764513 cbirds-0.0.12/setup.cfg
-drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:13:27.761179 cbirds-0.0.12/src/
-drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:13:27.761179 cbirds-0.0.12/src/cbirds/
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     8318 2023-06-06 14:00:36.000000 cbirds-0.0.12/src/cbirds/birds.py
-drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:13:27.761179 cbirds-0.0.12/src/cbirds.egg-info/
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     3373 2023-06-09 00:13:27.000000 cbirds-0.0.12/src/cbirds.egg-info/PKG-INFO
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)      221 2023-06-09 00:13:27.000000 cbirds-0.0.12/src/cbirds.egg-info/SOURCES.txt
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)        1 2023-06-09 00:13:27.000000 cbirds-0.0.12/src/cbirds.egg-info/dependency_links.txt
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)       10 2023-06-09 00:13:27.000000 cbirds-0.0.12/src/cbirds.egg-info/requires.txt
--rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)        7 2023-06-09 00:13:27.000000 cbirds-0.0.12/src/cbirds.egg-info/top_level.txt
+drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:23:00.712616 cbirds-0.1.0/
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     1068 2023-06-04 19:12:12.000000 cbirds-0.1.0/LICENSE
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     3372 2023-06-09 00:23:00.712616 cbirds-0.1.0/PKG-INFO
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     2917 2023-06-09 00:12:58.000000 cbirds-0.1.0/README.md
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)      531 2023-06-09 00:22:49.000000 cbirds-0.1.0/pyproject.toml
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)       38 2023-06-09 00:23:00.712616 cbirds-0.1.0/setup.cfg
+drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:23:00.709282 cbirds-0.1.0/src/
+drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:23:00.709282 cbirds-0.1.0/src/cbirds/
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     8318 2023-06-06 14:00:36.000000 cbirds-0.1.0/src/cbirds/birds.py
+drwxr-xr-x   0 jotaalvim  (1000) jotaalvim  (1001)        0 2023-06-09 00:23:00.712616 cbirds-0.1.0/src/cbirds.egg-info/
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)     3372 2023-06-09 00:23:00.000000 cbirds-0.1.0/src/cbirds.egg-info/PKG-INFO
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)      221 2023-06-09 00:23:00.000000 cbirds-0.1.0/src/cbirds.egg-info/SOURCES.txt
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)        1 2023-06-09 00:23:00.000000 cbirds-0.1.0/src/cbirds.egg-info/dependency_links.txt
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)       10 2023-06-09 00:23:00.000000 cbirds-0.1.0/src/cbirds.egg-info/requires.txt
+-rw-r--r--   0 jotaalvim  (1000) jotaalvim  (1001)        7 2023-06-09 00:23:00.000000 cbirds-0.1.0/src/cbirds.egg-info/top_level.txt
```

### Comparing `cbirds-0.0.12/LICENSE` & `cbirds-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cbirds-0.0.12/PKG-INFO` & `cbirds-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbirds
-Version: 0.0.12
+Version: 0.1.0
 Summary: Combinatory Birds
 Author-email: João Alvim <joaoafonsoalvim@gmail.com>
 Project-URL: repository, https://github.com/jotaalvim/cbirds
 Project-URL: Bug Tracker, https://github.com/jotaalvim/cbirds/issues
 Keywords: cbirds,combinator,birds,combinator birds,logic
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `cbirds-0.0.12/README.md` & `cbirds-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cbirds-0.0.12/pyproject.toml` & `cbirds-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cbirds"
-version = "0.0.12"
+version = "0.1.00"
 keywords = ["cbirds", "combinator", "birds", "combinator birds","logic"]
 
 authors = [
   { name="João Alvim", email="joaoafonsoalvim@gmail.com" },
 ]
 
 description = "Combinatory Birds"
```

### Comparing `cbirds-0.0.12/src/cbirds/birds.py` & `cbirds-0.1.0/src/cbirds/birds.py`

 * *Files identical despite different names*

### Comparing `cbirds-0.0.12/src/cbirds.egg-info/PKG-INFO` & `cbirds-0.1.0/src/cbirds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbirds
-Version: 0.0.12
+Version: 0.1.0
 Summary: Combinatory Birds
 Author-email: João Alvim <joaoafonsoalvim@gmail.com>
 Project-URL: repository, https://github.com/jotaalvim/cbirds
 Project-URL: Bug Tracker, https://github.com/jotaalvim/cbirds/issues
 Keywords: cbirds,combinator,birds,combinator birds,logic
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

