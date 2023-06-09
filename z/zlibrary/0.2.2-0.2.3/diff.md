# Comparing `tmp/zlibrary-0.2.2.tar.gz` & `tmp/zlibrary-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlibrary-0.2.2.tar", last modified: Sun Mar 26 14:42:55 2023, max compression
+gzip compressed data, was "zlibrary-0.2.3.tar", last modified: Fri Jun  9 15:57:12 2023, max compression
```

## Comparing `zlibrary-0.2.2.tar` & `zlibrary-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-03-26 14:42:55.049889 zlibrary-0.2.2/
--rw-r--r--   0 desu      (1000) desu      (1000)    35149 2023-03-10 21:32:56.000000 zlibrary-0.2.2/LICENSE
--rw-r--r--   0 desu      (1000) desu      (1000)     6699 2023-03-26 14:42:55.049889 zlibrary-0.2.2/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)     6187 2023-03-26 14:35:22.000000 zlibrary-0.2.2/README.md
--rw-r--r--   0 desu      (1000) desu      (1000)      104 2023-03-10 21:32:56.000000 zlibrary-0.2.2/pyproject.toml
--rw-r--r--   0 desu      (1000) desu      (1000)      759 2023-03-26 14:42:55.049889 zlibrary-0.2.2/setup.cfg
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-03-26 14:42:55.046556 zlibrary-0.2.2/src/
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-03-26 14:42:55.049889 zlibrary-0.2.2/src/zlibrary/
--rw-r--r--   0 desu      (1000) desu      (1000)       84 2023-03-11 00:54:21.000000 zlibrary-0.2.2/src/zlibrary/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)    19396 2023-03-11 01:48:40.000000 zlibrary-0.2.2/src/zlibrary/abs.py
--rw-r--r--   0 desu      (1000) desu      (1000)      852 2023-03-11 00:50:09.000000 zlibrary-0.2.2/src/zlibrary/booklists.py
--rw-r--r--   0 desu      (1000) desu      (1000)     4945 2023-03-11 00:52:56.000000 zlibrary-0.2.2/src/zlibrary/const.py
--rw-r--r--   0 desu      (1000) desu      (1000)      769 2023-03-10 23:56:48.000000 zlibrary-0.2.2/src/zlibrary/exception.py
--rw-r--r--   0 desu      (1000) desu      (1000)     7892 2023-03-26 14:21:28.000000 zlibrary-0.2.2/src/zlibrary/libasync.py
--rw-r--r--   0 desu      (1000) desu      (1000)       96 2023-03-10 21:32:56.000000 zlibrary-0.2.2/src/zlibrary/logger.py
--rw-r--r--   0 desu      (1000) desu      (1000)     2664 2023-03-26 14:40:03.000000 zlibrary-0.2.2/src/zlibrary/profile.py
--rw-r--r--   0 desu      (1000) desu      (1000)     2497 2023-03-26 14:22:57.000000 zlibrary-0.2.2/src/zlibrary/util.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-03-26 14:42:55.049889 zlibrary-0.2.2/src/zlibrary.egg-info/
--rw-r--r--   0 desu      (1000) desu      (1000)     6699 2023-03-26 14:42:55.000000 zlibrary-0.2.2/src/zlibrary.egg-info/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      433 2023-03-26 14:42:55.000000 zlibrary-0.2.2/src/zlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        1 2023-03-26 14:42:55.000000 zlibrary-0.2.2/src/zlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       90 2023-03-26 14:42:55.000000 zlibrary-0.2.2/src/zlibrary.egg-info/requires.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        9 2023-03-26 14:42:55.000000 zlibrary-0.2.2/src/zlibrary.egg-info/top_level.txt
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-06-09 15:57:12.247912 zlibrary-0.2.3/
+-rw-r--r--   0 desu      (1000) desu      (1000)    35149 2023-06-09 15:42:39.000000 zlibrary-0.2.3/LICENSE
+-rw-r--r--   0 desu      (1000) desu      (1000)     6699 2023-06-09 15:57:12.247912 zlibrary-0.2.3/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)     6187 2023-06-09 15:42:39.000000 zlibrary-0.2.3/README.md
+-rw-r--r--   0 desu      (1000) desu      (1000)      104 2023-06-09 15:42:39.000000 zlibrary-0.2.3/pyproject.toml
+-rw-r--r--   0 desu      (1000) desu      (1000)      759 2023-06-09 15:57:12.247912 zlibrary-0.2.3/setup.cfg
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-06-09 15:57:12.244578 zlibrary-0.2.3/src/
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-06-09 15:57:12.247912 zlibrary-0.2.3/src/zlibrary/
+-rw-r--r--   0 desu      (1000) desu      (1000)       84 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)    19396 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/abs.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      852 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/booklists.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     4945 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/const.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      769 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/exception.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     7896 2023-06-09 15:56:40.000000 zlibrary-0.2.3/src/zlibrary/libasync.py
+-rw-r--r--   0 desu      (1000) desu      (1000)       96 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/logger.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     2664 2023-06-09 15:42:39.000000 zlibrary-0.2.3/src/zlibrary/profile.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     2500 2023-06-09 15:48:51.000000 zlibrary-0.2.3/src/zlibrary/util.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-06-09 15:57:12.247912 zlibrary-0.2.3/src/zlibrary.egg-info/
+-rw-r--r--   0 desu      (1000) desu      (1000)     6699 2023-06-09 15:57:12.000000 zlibrary-0.2.3/src/zlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      433 2023-06-09 15:57:12.000000 zlibrary-0.2.3/src/zlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        1 2023-06-09 15:57:12.000000 zlibrary-0.2.3/src/zlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       90 2023-06-09 15:57:12.000000 zlibrary-0.2.3/src/zlibrary.egg-info/requires.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        9 2023-06-09 15:57:12.000000 zlibrary-0.2.3/src/zlibrary.egg-info/top_level.txt
```

### Comparing `zlibrary-0.2.2/LICENSE` & `zlibrary-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/PKG-INFO` & `zlibrary-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlibrary
-Version: 0.2.2
+Version: 0.2.3
 Summary: Unofficial Z-Library API
 Home-page: https://github.com/sertraline/zlibrary
 Author: Toshiro Iwa
 Author-email: iwa@acid.im
 Project-URL: Bug Tracker, https://github.com/sertraline/zlibrary/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `zlibrary-0.2.2/README.md` & `zlibrary-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/setup.cfg` & `zlibrary-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zlibrary
-version = 0.2.2
+version = 0.2.3
 author = Toshiro Iwa
 author_email = iwa@acid.im
 description = Unofficial Z-Library API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sertraline/zlibrary
 project_urls =
```

### Comparing `zlibrary-0.2.2/src/zlibrary/abs.py` & `zlibrary-0.2.3/src/zlibrary/abs.py`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/src/zlibrary/booklists.py` & `zlibrary-0.2.3/src/zlibrary/booklists.py`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/src/zlibrary/const.py` & `zlibrary-0.2.3/src/zlibrary/const.py`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/src/zlibrary/exception.py` & `zlibrary-0.2.3/src/zlibrary/exception.py`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/src/zlibrary/libasync.py` & `zlibrary-0.2.3/src/zlibrary/libasync.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from .exception import EmptyQueryError, ProxyNotMatchError, NoProfileError, NoDomainError
 from .util import GET_request, POST_request, HEAD_request
 from .abs import SearchPaginator
 from .profile import ZlibProfile
 from .const import Extension, Language
 
 
-ZLIB_DOMAIN = "https://singlelogin.me/"
-LOGIN_DOMAIN = "https://singlelogin.me/rpc.php"
+ZLIB_DOMAIN = "https://singlelogin.site/"
+LOGIN_DOMAIN = "https://singlelogin.site/rpc.php"
 
 ZLIB_TOR_DOMAIN = "http://bookszlibb74ugqojhzhg2a63w5i2atv5bqarulgczawnbmsb6s6qead.onion"
 LOGIN_TOR_DOMAIN = "http://loginzlib2vrak5zzpcocc3ouizykn6k5qecgj2tzlnab5wcbqhembyd.onion/rpc.php"
 
 
 class AsyncZlib:
     semaphore = True
```

### Comparing `zlibrary-0.2.2/src/zlibrary/profile.py` & `zlibrary-0.2.3/src/zlibrary/profile.py`

 * *Files identical despite different names*

### Comparing `zlibrary-0.2.2/src/zlibrary/util.py` & `zlibrary-0.2.3/src/zlibrary/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 HEAD = {
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36"
 }
 
 
 TIMEOUT = aiohttp.ClientTimeout(
-    total=90,
+    total=180,
     connect=0,
-    sock_connect=60,
-    sock_read=90
+    sock_connect=120,
+    sock_read=180
 )
 
 HEAD_TIMEOUT = aiohttp.ClientTimeout(
     total=4,
     connect=0,
     sock_connect=4,
     sock_read=4
```

### Comparing `zlibrary-0.2.2/src/zlibrary.egg-info/PKG-INFO` & `zlibrary-0.2.3/src/zlibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlibrary
-Version: 0.2.2
+Version: 0.2.3
 Summary: Unofficial Z-Library API
 Home-page: https://github.com/sertraline/zlibrary
 Author: Toshiro Iwa
 Author-email: iwa@acid.im
 Project-URL: Bug Tracker, https://github.com/sertraline/zlibrary/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

