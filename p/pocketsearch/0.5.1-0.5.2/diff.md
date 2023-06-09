# Comparing `tmp/pocketsearch-0.5.1.tar.gz` & `tmp/pocketsearch-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.5.1.tar", last modified: Fri Jun  9 16:31:10 2023, max compression
+gzip compressed data, was "pocketsearch-0.5.2.tar", last modified: Fri Jun  9 17:49:09 2023, max compression
```

## Comparing `pocketsearch-0.5.1.tar` & `pocketsearch-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.249450 pocketsearch-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-09 16:31:10.245450 pocketsearch-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:31:10.249450 pocketsearch-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.241450 pocketsearch-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.245450 pocketsearch-0.5.1/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 16:30:56.000000 pocketsearch-0.5.1/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:31:10.245450 pocketsearch-0.5.1/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 16:31:10.000000 pocketsearch-0.5.1/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.326173 pocketsearch-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    40372 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-06-09 17:49:00.000000 pocketsearch-0.5.2/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:49:09.330173 pocketsearch-0.5.2/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:49:09.000000 pocketsearch-0.5.2/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.5.1/LICENSE` & `pocketsearch-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.1/PKG-INFO` & `pocketsearch-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.1
+Version: 0.5.2
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Indexing
-Classifier: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
@@ -56,24 +55,25 @@
 ```Python
 from pocketsearch import PocketSearch
 
 pocket_search = PocketSearch()
 pocket_search.insert(text="Hello World !")
 print(pocket_search.search(text="hello")[0].text)
 Hello World !
+```
 
 From a database perspective, the new document will be immediately available 
 to the search index, as each insert is followed by a database commit.
 
 Be ware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
 FTS extension in sqlite and showing how relevant a document is to a 
 given query. 
 
-```
+
 
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query:
```

### Comparing `pocketsearch-0.5.1/README.md` & `pocketsearch-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,24 +32,25 @@
 ```Python
 from pocketsearch import PocketSearch
 
 pocket_search = PocketSearch()
 pocket_search.insert(text="Hello World !")
 print(pocket_search.search(text="hello")[0].text)
 Hello World !
+```
 
 From a database perspective, the new document will be immediately available 
 to the search index, as each insert is followed by a database commit.
 
 Be ware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
 FTS extension in sqlite and showing how relevant a document is to a 
 given query. 
 
-```
+
 
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query:
```

### Comparing `pocketsearch-0.5.1/setup.py` & `pocketsearch-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.5.1",
+    version = "0.5.2",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
@@ -22,14 +22,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Text Processing :: Indexing",        
-        ""
+        "Topic :: Text Processing :: Indexing"
     ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.8"
 )
```

### Comparing `pocketsearch-0.5.1/src/pocketsearch/__init__.py` & `pocketsearch-0.5.2/src/pocketsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.1/src/pocketsearch/tests.py` & `pocketsearch-0.5.2/src/pocketsearch/tests.py`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.5.1/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.5.2/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.5.1
+Version: 0.5.2
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Indexing
-Classifier: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pocketsearch
 pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
 
@@ -56,24 +55,25 @@
 ```Python
 from pocketsearch import PocketSearch
 
 pocket_search = PocketSearch()
 pocket_search.insert(text="Hello World !")
 print(pocket_search.search(text="hello")[0].text)
 Hello World !
+```
 
 From a database perspective, the new document will be immediately available 
 to the search index, as each insert is followed by a database commit.
 
 Be ware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
 FTS extension in sqlite and showing how relevant a document is to a 
 given query. 
 
-```
+
 
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query:
```

