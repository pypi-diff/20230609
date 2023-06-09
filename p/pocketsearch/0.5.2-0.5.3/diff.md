# Comparing `tmp/pocketsearch-0.5.2.tar.gz` & `tmp/pocketsearch-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.5.2.tar", last modified: Fri Jun  9 17:49:09 2023, max compression
+gzip compressed data, was "pocketsearch-0.5.3.tar", last modified: Fri Jun  9 18:36:25 2023, max compression
```

## Comparing `pocketsearch-0.5.2.tar` & `pocketsearch-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.326173 pocketsearch-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.233747 pocketsearch-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.233747 pocketsearch-0.5.3/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 18:36:14.000000 pocketsearch-0.5.3/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:36:25.237747 pocketsearch-0.5.3/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:36:25.000000 pocketsearch-0.5.3/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.5.2/LICENSE` & `pocketsearch-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.2/PKG-INFO` & `pocketsearch-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.2
+Version: 0.5.3
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -65,15 +65,20 @@
 to the search index, as each insert is followed by a database commit.
 
 Be ware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
 FTS extension in sqlite and showing how relevant a document is to a 
 given query. 
 
+The API also supports iteration:
 
+```Python
+for document in pocket_search.search(text="hello"):
+    print(document.text)
+```
 
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query: 
 
@@ -165,25 +170,43 @@
 * is_id_field - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
 
 With respect to naming your fields following restrictions apply:
 
 * Fields may not start with an underscore.
 * Fields may not contain double underscores.
 
+> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
+
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
 # Searches documents that contain "world" in text and have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
+# Handling updates and deletes
+
+Using the id of a document, you can run updates:
+
+```Python
+pocket_search.update(rowid=1, text="The updated text.")
+```
+
+If want to update more fields, simply provide them as keyword arguments.
+
+To delete a document, use:
+
+```Python
+pocket_search.delete(rowid=1)
+```
+
 Please note that by default an AND query is performed, thus only documents are
 matched where text contains the word "world" and the filename is "a.txt"
 
 # Searching numeric data
 
 You can also search for numeric data:
 
@@ -217,25 +240,28 @@
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
     published=Datetime()
 
-pocket_search = PocketSearch(schema=self.Product)
+pocket_search = PocketSearch(schema=Product)
 # Search documents published in year 2023
 pocket_search.search(published__year=2023)
 # Search document published after 2020
 pocket_search.search(published__year__gt=2023)
 # Search documents published in month 6
 pocket_search.search(published__month=6)
 # Search documents published on 21/6/2023:
 pocket_search.search(published__month=21,published__month=6,published_year=2023)
 ```
 
+> **_NOTE:_**  In search results, datefields are automatically converted to datetime and date objects respectivley. 
+
+
 # Making your database persistent
 
 The previous examples use an in-memory sqlite database. If you want to actually store 
 the database, you have to provide a name:
 
 ```Python
 pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
```

### Comparing `pocketsearch-0.5.2/README.md` & `pocketsearch-0.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,20 @@
 to the search index, as each insert is followed by a database commit.
 
 Be ware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
 FTS extension in sqlite and showing how relevant a document is to a 
 given query. 
 
+The API also supports iteration:
 
+```Python
+for document in pocket_search.search(text="hello"):
+    print(document.text)
+```
 
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query: 
 
@@ -142,25 +147,43 @@
 * is_id_field - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
 
 With respect to naming your fields following restrictions apply:
 
 * Fields may not start with an underscore.
 * Fields may not contain double underscores.
 
+> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
+
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
 # Searches documents that contain "world" in text and have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
+# Handling updates and deletes
+
+Using the id of a document, you can run updates:
+
+```Python
+pocket_search.update(rowid=1, text="The updated text.")
+```
+
+If want to update more fields, simply provide them as keyword arguments.
+
+To delete a document, use:
+
+```Python
+pocket_search.delete(rowid=1)
+```
+
 Please note that by default an AND query is performed, thus only documents are
 matched where text contains the word "world" and the filename is "a.txt"
 
 # Searching numeric data
 
 You can also search for numeric data:
 
@@ -194,25 +217,28 @@
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
     published=Datetime()
 
-pocket_search = PocketSearch(schema=self.Product)
+pocket_search = PocketSearch(schema=Product)
 # Search documents published in year 2023
 pocket_search.search(published__year=2023)
 # Search document published after 2020
 pocket_search.search(published__year__gt=2023)
 # Search documents published in month 6
 pocket_search.search(published__month=6)
 # Search documents published on 21/6/2023:
 pocket_search.search(published__month=21,published__month=6,published_year=2023)
 ```
 
+> **_NOTE:_**  In search results, datefields are automatically converted to datetime and date objects respectivley. 
+
+
 # Making your database persistent
 
 The previous examples use an in-memory sqlite database. If you want to actually store 
 the database, you have to provide a name:
 
 ```Python
 pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
```

### Comparing `pocketsearch-0.5.2/setup.py` & `pocketsearch-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.5.2",
+    version = "0.5.3",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.5.2/src/pocketsearch/__init__.py` & `pocketsearch-0.5.3/src/pocketsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.2/src/pocketsearch/tests.py` & `pocketsearch-0.5.3/src/pocketsearch/tests.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.2/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.5.3/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.2
+Version: 0.5.3
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -65,15 +65,20 @@
 to the search index, as each insert is followed by a database commit.
 
 Be ware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
 FTS extension in sqlite and showing how relevant a document is to a 
 given query. 
 
+The API also supports iteration:
 
+```Python
+for document in pocket_search.search(text="hello"):
+    print(document.text)
+```
 
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query: 
 
@@ -165,25 +170,43 @@
 * is_id_field - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
 
 With respect to naming your fields following restrictions apply:
 
 * Fields may not start with an underscore.
 * Fields may not contain double underscores.
 
+> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
+
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
 # Searches documents that contain "world" in text and have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
+# Handling updates and deletes
+
+Using the id of a document, you can run updates:
+
+```Python
+pocket_search.update(rowid=1, text="The updated text.")
+```
+
+If want to update more fields, simply provide them as keyword arguments.
+
+To delete a document, use:
+
+```Python
+pocket_search.delete(rowid=1)
+```
+
 Please note that by default an AND query is performed, thus only documents are
 matched where text contains the word "world" and the filename is "a.txt"
 
 # Searching numeric data
 
 You can also search for numeric data:
 
@@ -217,25 +240,28 @@
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
     published=Datetime()
 
-pocket_search = PocketSearch(schema=self.Product)
+pocket_search = PocketSearch(schema=Product)
 # Search documents published in year 2023
 pocket_search.search(published__year=2023)
 # Search document published after 2020
 pocket_search.search(published__year__gt=2023)
 # Search documents published in month 6
 pocket_search.search(published__month=6)
 # Search documents published on 21/6/2023:
 pocket_search.search(published__month=21,published__month=6,published_year=2023)
 ```
 
+> **_NOTE:_**  In search results, datefields are automatically converted to datetime and date objects respectivley. 
+
+
 # Making your database persistent
 
 The previous examples use an in-memory sqlite database. If you want to actually store 
 the database, you have to provide a name:
 
 ```Python
 pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
```

