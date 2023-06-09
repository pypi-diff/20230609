# Comparing `tmp/angola-0.12.0.tar.gz` & `tmp/angola-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.12.0.tar", last modified: Fri Jun  9 05:21:46 2023, max compression
+gzip compressed data, was "angola-0.12.1.tar", last modified: Fri Jun  9 05:24:09 2023, max compression
```

## Comparing `angola-0.12.0.tar` & `angola-0.12.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:21:46.038953 angola-0.12.0/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.0/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.0/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 05:21:46.039029 angola-0.12.0/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.0/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-09 05:21:46.039287 angola-0.12.0/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-09 05:21:38.000000 angola-0.12.0/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:21:46.033139 angola-0.12.0/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:21:46.036572 angola-0.12.0/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.0/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    48672 2023-06-09 05:21:28.000000 angola-0.12.0/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.0/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.0/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.0/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    19447 2023-06-09 03:27:14.000000 angola-0.12.0/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:21:46.037409 angola-0.12.0/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 05:21:46.000000 angola-0.12.0/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-09 05:21:46.000000 angola-0.12.0/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-09 05:21:46.000000 angola-0.12.0/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-09 05:21:46.000000 angola-0.12.0/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-09 05:21:46.000000 angola-0.12.0/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:21:46.038844 angola-0.12.0/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.0/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.0/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.0/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.0/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.0/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.205971 angola-0.12.1/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.1/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.1/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 05:24:09.206033 angola-0.12.1/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.1/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-09 05:24:09.206255 angola-0.12.1/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-09 05:24:04.000000 angola-0.12.1/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.200431 angola-0.12.1/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.203756 angola-0.12.1/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.1/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    48688 2023-06-09 05:23:54.000000 angola-0.12.1/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.1/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.1/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.1/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    19447 2023-06-09 03:27:14.000000 angola-0.12.1/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.204713 angola-0.12.1/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.205874 angola-0.12.1/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.1/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.1/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.1/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.1/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.1/tests/test_query.py
```

### Comparing `angola-0.12.0/LICENSE` & `angola-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/PKG-INFO` & `angola-0.12.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.0
+Version: 0.12.1
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.0/README.md` & `angola-0.12.1/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/setup.py` & `angola-0.12.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.12.0"
+VERSION = "0.12.1"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.12.0/src/angola/database.py` & `angola-0.12.1/src/angola/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,15 +814,15 @@
         Returns: bool
         """
         if not self.has_collection(collection_name):
             collection_name = self.prefix_collection_name(collection_name)
             col = self.db.create_collection(collection_name)
 
             # indexes
-            if _indexes := {l.get("name"):l for l in [*DEFAULT_INDEXES, *self.default_indexes, *indexes]}.values():
+            if _indexes := {l.get("name"):l for l in [*DEFAULT_INDEXES, *(self.default_indexes or []), *(indexes or [])]}.values():
                 for index in _indexes:
                     col._add_index(index) 
                     
             return True 
         return False
 
     def select_collection(self, collection_name:str, indexes:list=[], immut_keys:list=[], item_class=None, auto_create:bool=True) -> "Collection":
```

### Comparing `angola-0.12.0/src/angola/dict_mutator.py` & `angola-0.12.1/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/src/angola/dict_query.py` & `angola-0.12.1/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/src/angola/lib.py` & `angola-0.12.1/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/src/angola/lib_xql.py` & `angola-0.12.1/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/src/angola.egg-info/PKG-INFO` & `angola-0.12.1/src/angola.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.0
+Version: 0.12.1
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.0/tests/test_database.py` & `angola-0.12.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/tests/test_dict_mutator.py` & `angola-0.12.1/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.0/tests/test_lib.py` & `angola-0.12.1/tests/test_lib.py`

 * *Files identical despite different names*

