# Comparing `tmp/pocketsearch-0.5.3.tar.gz` & `tmp/pocketsearch-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.5.3.tar", last modified: Fri Jun  9 18:36:25 2023, max compression
+gzip compressed data, was "pocketsearch-0.5.4.tar", last modified: Fri Jun  9 18:55:05 2023, max compression
```

## Comparing `pocketsearch-0.5.3.tar` & `pocketsearch-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.233747 pocketsearch-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.233747 pocketsearch-0.5.3/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.920593 pocketsearch-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 18:54:56.000000 pocketsearch-0.5.4/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:55:05.924593 pocketsearch-0.5.4/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:55:05.000000 pocketsearch-0.5.4/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.5.3/LICENSE` & `pocketsearch-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.3/PKG-INFO` & `pocketsearch-0.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.3
+Version: 0.5.4
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
 - Support for full text search
-- A simple API for defining schemas and searching
+- A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
 - Support for text, numeric and date search
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
 # Status
 The package is currently in Beta status.
@@ -177,20 +177,32 @@
 > **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
 
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
-# Searches documents that contain "world" in text and have "a.txt" is a filename.
+# Searches documents that contain "world" in text AND have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
+> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
+
+However, you can join 2 queries (resulting in a UNION statement in SQL):
+
+```Python
+q = pocket_search.search(text="world") | pocket_search.search(filename="world")
+for result in q:
+    print(result.text)
+```
+
+This option is currently experimental and still has issues, espcially when accessing results through indexing. 
+
 # Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
 pocket_search.update(rowid=1, text="The updated text.")
 ```
@@ -312,14 +324,14 @@
 
 # Multiple indicies in one database
 
 You can have multiple indicies in one database (only databases written to disk) by setting 
 the "index_name" option:
 
 ```Python
-pocket_search = PocketSearch(index_name="Product",schema=Product)
+pocket_search = PocketSearch(db_name="my_db.db",index_name="Product",schema=Product)
 ```
 
 # Contribute
 Pull requests are welcome. If you come across any issues, please report them 
 at https://github.com/kaykay-dv/pocketsearch/issues
```

### Comparing `pocketsearch-0.5.3/README.md` & `pocketsearch-0.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
 - Support for full text search
-- A simple API for defining schemas and searching
+- A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
 - Support for text, numeric and date search
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
 # Status
 The package is currently in Beta status.
@@ -154,20 +154,32 @@
 > **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
 
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
-# Searches documents that contain "world" in text and have "a.txt" is a filename.
+# Searches documents that contain "world" in text AND have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
+> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
+
+However, you can join 2 queries (resulting in a UNION statement in SQL):
+
+```Python
+q = pocket_search.search(text="world") | pocket_search.search(filename="world")
+for result in q:
+    print(result.text)
+```
+
+This option is currently experimental and still has issues, espcially when accessing results through indexing. 
+
 # Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
 pocket_search.update(rowid=1, text="The updated text.")
 ```
@@ -289,14 +301,14 @@
 
 # Multiple indicies in one database
 
 You can have multiple indicies in one database (only databases written to disk) by setting 
 the "index_name" option:
 
 ```Python
-pocket_search = PocketSearch(index_name="Product",schema=Product)
+pocket_search = PocketSearch(db_name="my_db.db",index_name="Product",schema=Product)
 ```
 
 # Contribute
 Pull requests are welcome. If you come across any issues, please report them 
 at https://github.com/kaykay-dv/pocketsearch/issues
```

### Comparing `pocketsearch-0.5.3/setup.py` & `pocketsearch-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.5.3",
+    version = "0.5.4",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.5.3/src/pocketsearch/__init__.py` & `pocketsearch-0.5.4/src/pocketsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.3/src/pocketsearch/tests.py` & `pocketsearch-0.5.4/src/pocketsearch/tests.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.3/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.5.4/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.3
+Version: 0.5.4
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
 - Support for full text search
-- A simple API for defining schemas and searching
+- A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
 - Support for text, numeric and date search
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
 # Status
 The package is currently in Beta status.
@@ -177,20 +177,32 @@
 > **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
 
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
-# Searches documents that contain "world" in text and have "a.txt" is a filename.
+# Searches documents that contain "world" in text AND have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
+> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
+
+However, you can join 2 queries (resulting in a UNION statement in SQL):
+
+```Python
+q = pocket_search.search(text="world") | pocket_search.search(filename="world")
+for result in q:
+    print(result.text)
+```
+
+This option is currently experimental and still has issues, espcially when accessing results through indexing. 
+
 # Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
 ```Python
 pocket_search.update(rowid=1, text="The updated text.")
 ```
@@ -312,14 +324,14 @@
 
 # Multiple indicies in one database
 
 You can have multiple indicies in one database (only databases written to disk) by setting 
 the "index_name" option:
 
 ```Python
-pocket_search = PocketSearch(index_name="Product",schema=Product)
+pocket_search = PocketSearch(db_name="my_db.db",index_name="Product",schema=Product)
 ```
 
 # Contribute
 Pull requests are welcome. If you come across any issues, please report them 
 at https://github.com/kaykay-dv/pocketsearch/issues
```

