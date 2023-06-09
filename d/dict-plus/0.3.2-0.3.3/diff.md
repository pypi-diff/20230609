# Comparing `tmp/dict_plus-0.3.2.tar.gz` & `tmp/dict_plus-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dict_plus-0.3.2.tar", last modified: Mon May 31 21:40:59 2021, max compression
+gzip compressed data, was "dict_plus-0.3.3.tar", last modified: Fri Jun  9 17:18:14 2023, max compression
```

## Comparing `dict_plus-0.3.2.tar` & `dict_plus-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/
--rw-rw-rw-   0        0        0      374 2021-05-31 21:40:59.000000 dict_plus-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       80 2020-09-24 22:07:34.000000 dict_plus-0.3.2/README.rst
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/dict_plus/
--rw-rw-rw-   0        0        0      409 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/dict_plus/dicts/
--rw-rw-rw-   0        0        0      384 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/dicts/__init__.py
--rw-rw-rw-   0        0        0      619 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/dicts/dictlist.py
--rw-rw-rw-   0        0        0     1831 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/dicts/dictplus.py
--rw-rw-rw-   0        0        0     4239 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/dicts/hooked.py
--rw-rw-rw-   0        0        0    12076 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/dicts/insensitive.py
--rw-rw-rw-   0        0        0     4363 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/dicts/ordered.py
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/dict_plus/elements/
--rw-rw-rw-   0        0        0     1024 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/elements/__init__.py
--rw-rw-rw-   0        0        0     7575 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/elements/element.py
--rw-rw-rw-   0        0        0      435 2020-09-24 22:07:34.000000 dict_plus-0.3.2/dict_plus/etypes.py
--rw-rw-rw-   0        0        0      586 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/exceptions.py
--rw-rw-rw-   0        0        0     2026 2020-09-24 22:07:34.000000 dict_plus-0.3.2/dict_plus/funcs.py
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/dict_plus/indexes/
--rw-rw-rw-   0        0        0      121 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/indexes/__init__.py
--rw-rw-rw-   0        0        0     5423 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/indexes/index.py
--rw-rw-rw-   0        0        0     1156 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/indexes/ordered.py
--rw-rw-rw-   0        0        0    35082 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/iterable.py
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/dict_plus/lists/
--rw-rw-rw-   0        0        0       94 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/lists/__init__.py
--rw-rw-rw-   0        0        0     7652 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/lists/listdict.py
--rw-rw-rw-   0        0        0     6406 2021-05-31 21:29:27.000000 dict_plus-0.3.2/dict_plus/lists/listplus.py
-drwxrwxrwx   0        0        0        0 2021-05-31 21:40:59.000000 dict_plus-0.3.2/dict_plus.egg-info/
--rw-rw-rw-   0        0        0      374 2021-05-31 21:40:58.000000 dict_plus-0.3.2/dict_plus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      657 2021-05-31 21:40:58.000000 dict_plus-0.3.2/dict_plus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-31 21:40:58.000000 dict_plus-0.3.2/dict_plus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-05-31 21:40:58.000000 dict_plus-0.3.2/dict_plus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-31 21:40:59.000000 dict_plus-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1249 2021-05-31 21:40:31.000000 dict_plus-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.546373 dict_plus-0.3.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 16:46:36.000000 dict_plus-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      357 2023-06-09 17:18:14.546373 dict_plus-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-06-09 17:16:37.000000 dict_plus-0.3.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.536867 dict_plus-0.3.3/dict_plus/
+-rw-rw-rw-   0        0        0      409 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.541372 dict_plus-0.3.3/dict_plus/dicts/
+-rw-rw-rw-   0        0        0      384 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/dicts/__init__.py
+-rw-rw-rw-   0        0        0      619 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/dicts/dictlist.py
+-rw-rw-rw-   0        0        0     1831 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/dicts/dictplus.py
+-rw-rw-rw-   0        0        0     4239 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/dicts/hooked.py
+-rw-rw-rw-   0        0        0    12076 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/dicts/insensitive.py
+-rw-rw-rw-   0        0        0     4363 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/dicts/ordered.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.542374 dict_plus-0.3.3/dict_plus/elements/
+-rw-rw-rw-   0        0        0     1024 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/elements/__init__.py
+-rw-rw-rw-   0        0        0     7575 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/elements/element.py
+-rw-rw-rw-   0        0        0      435 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/etypes.py
+-rw-rw-rw-   0        0        0      586 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/exceptions.py
+-rw-rw-rw-   0        0        0     2026 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.543374 dict_plus-0.3.3/dict_plus/indexes/
+-rw-rw-rw-   0        0        0      121 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/indexes/__init__.py
+-rw-rw-rw-   0        0        0     5423 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/indexes/index.py
+-rw-rw-rw-   0        0        0     1156 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/indexes/ordered.py
+-rw-rw-rw-   0        0        0    35082 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/iterable.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.545383 dict_plus-0.3.3/dict_plus/lists/
+-rw-rw-rw-   0        0        0       94 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/lists/__init__.py
+-rw-rw-rw-   0        0        0     7652 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/lists/listdict.py
+-rw-rw-rw-   0        0        0     6406 2023-06-09 16:46:36.000000 dict_plus-0.3.3/dict_plus/lists/listplus.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:18:14.538370 dict_plus-0.3.3/dict_plus.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-06-09 17:18:14.000000 dict_plus-0.3.3/dict_plus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-06-09 17:18:14.000000 dict_plus-0.3.3/dict_plus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 17:18:14.000000 dict_plus-0.3.3/dict_plus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 17:18:14.000000 dict_plus-0.3.3/dict_plus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 17:18:14.546373 dict_plus-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1249 2023-06-09 17:16:37.000000 dict_plus-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dict_plus-0.3.2/dict_plus/dicts/dictlist.py` & `dict_plus-0.3.3/dict_plus/dicts/dictlist.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/dicts/dictplus.py` & `dict_plus-0.3.3/dict_plus/dicts/dictplus.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/dicts/hooked.py` & `dict_plus-0.3.3/dict_plus/dicts/hooked.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/dicts/insensitive.py` & `dict_plus-0.3.3/dict_plus/dicts/insensitive.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/dicts/ordered.py` & `dict_plus-0.3.3/dict_plus/dicts/ordered.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/elements/__init__.py` & `dict_plus-0.3.3/dict_plus/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/elements/element.py` & `dict_plus-0.3.3/dict_plus/elements/element.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/exceptions.py` & `dict_plus-0.3.3/dict_plus/exceptions.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/funcs.py` & `dict_plus-0.3.3/dict_plus/funcs.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/indexes/index.py` & `dict_plus-0.3.3/dict_plus/indexes/index.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/indexes/ordered.py` & `dict_plus-0.3.3/dict_plus/indexes/ordered.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/iterable.py` & `dict_plus-0.3.3/dict_plus/iterable.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/lists/listdict.py` & `dict_plus-0.3.3/dict_plus/lists/listdict.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus/lists/listplus.py` & `dict_plus-0.3.3/dict_plus/lists/listplus.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.2/dict_plus.egg-info/SOURCES.txt` & `dict_plus-0.3.3/dict_plus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.py
 dict_plus/__init__.py
 dict_plus/etypes.py
 dict_plus/exceptions.py
 dict_plus/funcs.py
 dict_plus/iterable.py
```

### Comparing `dict_plus-0.3.2/setup.py` & `dict_plus-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import json
 
-VERSION = "0.3.2"
+VERSION = "0.3.3"
 
 
 def check_version_info():
     try:
         with open("version.json", "r") as f:
             data = json.load(f)
             assert data["version"] == VERSION  # Assert that the versions are the same
```

