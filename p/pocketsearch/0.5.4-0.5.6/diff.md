# Comparing `tmp/pocketsearch-0.5.4.tar.gz` & `tmp/pocketsearch-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.5.4.tar", last modified: Fri Jun  9 18:55:05 2023, max compression
+gzip compressed data, was "pocketsearch-0.5.6.tar", last modified: Fri Jun  9 18:58:33 2023, max compression
```

## Comparing `pocketsearch-0.5.4.tar` & `pocketsearch-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.920593 pocketsearch-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:58:33.396350 pocketsearch-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:58:24.000000 pocketsearch-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-09 18:58:33.396350 pocketsearch-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-06-09 18:58:24.000000 pocketsearch-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:58:33.396350 pocketsearch-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 18:58:24.000000 pocketsearch-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:58:33.392350 pocketsearch-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:58:33.396350 pocketsearch-0.5.6/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 18:58:24.000000 pocketsearch-0.5.6/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 18:58:24.000000 pocketsearch-0.5.6/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:58:33.396350 pocketsearch-0.5.6/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-09 18:58:33.000000 pocketsearch-0.5.6/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 18:58:33.000000 pocketsearch-0.5.6/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:58:33.000000 pocketsearch-0.5.6/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:58:33.000000 pocketsearch-0.5.6/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.5.4/LICENSE` & `pocketsearch-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.4/PKG-INFO` & `pocketsearch-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.4
+Version: 0.5.6
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -188,19 +188,21 @@
 ```
 
 > **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
 
 However, you can join 2 queries (resulting in a UNION statement in SQL):
 
 ```Python
-q = pocket_search.search(text="world") | pocket_search.search(filename="world")
+q = pocket_search.search(text="world") | pocket_search.search(filename="a.txt")
 for result in q:
     print(result.text)
 ```
 
+The result will contain all documents containing either "world" or where the filename is "a.text".
+
 This option is currently experimental and still has issues, espcially when accessing results through indexing. 
 
 # Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
```

### Comparing `pocketsearch-0.5.4/README.md` & `pocketsearch-0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -165,19 +165,21 @@
 ```
 
 > **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
 
 However, you can join 2 queries (resulting in a UNION statement in SQL):
 
 ```Python
-q = pocket_search.search(text="world") | pocket_search.search(filename="world")
+q = pocket_search.search(text="world") | pocket_search.search(filename="a.txt")
 for result in q:
     print(result.text)
 ```
 
+The result will contain all documents containing either "world" or where the filename is "a.text".
+
 This option is currently experimental and still has issues, espcially when accessing results through indexing. 
 
 # Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
```

### Comparing `pocketsearch-0.5.4/setup.py` & `pocketsearch-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.5.4",
+    version = "0.5.6",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.5.4/src/pocketsearch/__init__.py` & `pocketsearch-0.5.6/src/pocketsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.4/src/pocketsearch/tests.py` & `pocketsearch-0.5.6/src/pocketsearch/tests.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.4/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.5.6/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.4
+Version: 0.5.6
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -188,19 +188,21 @@
 ```
 
 > **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
 
 However, you can join 2 queries (resulting in a UNION statement in SQL):
 
 ```Python
-q = pocket_search.search(text="world") | pocket_search.search(filename="world")
+q = pocket_search.search(text="world") | pocket_search.search(filename="a.txt")
 for result in q:
     print(result.text)
 ```
 
+The result will contain all documents containing either "world" or where the filename is "a.text".
+
 This option is currently experimental and still has issues, espcially when accessing results through indexing. 
 
 # Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
```

