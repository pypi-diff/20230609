# Comparing `tmp/satellitevu-1.5.1.tar.gz` & `tmp/satellitevu-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellitevu-1.5.1.tar", max compression
+gzip compressed data, was "satellitevu-1.6.0.tar", max compression
```

## Comparing `satellitevu-1.5.1.tar` & `satellitevu-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1080 2023-04-25 11:16:02.648422 satellitevu-1.5.1/LICENSE
--rw-r--r--   0        0        0     3859 2023-06-09 09:59:59.328597 satellitevu-1.5.1/README.md
--rw-r--r--   0        0        0     1082 2023-06-09 09:59:59.329377 satellitevu-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-25 11:16:02.654100 satellitevu-1.5.1/satellitevu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:16:02.654475 satellitevu-1.5.1/satellitevu/apis/__init__.py
--rw-r--r--   0        0        0     2838 2023-04-25 11:16:02.654773 satellitevu-1.5.1/satellitevu/apis/archive.py
--rw-r--r--   0        0        0     2440 2023-04-25 11:16:02.655075 satellitevu-1.5.1/satellitevu/apis/archive_test.py
--rw-r--r--   0        0        0     1175 2023-04-25 11:16:02.655329 satellitevu-1.5.1/satellitevu/apis/base.py
--rw-r--r--   0        0        0     1287 2023-04-25 11:16:02.655584 satellitevu-1.5.1/satellitevu/apis/base_test.py
--rw-r--r--   0        0        0     5617 2023-04-25 11:16:02.655864 satellitevu-1.5.1/satellitevu/apis/orders.py
--rw-r--r--   0        0        0    10041 2023-04-25 11:16:02.656154 satellitevu-1.5.1/satellitevu/apis/orders_test.py
--rw-r--r--   0        0        0     7124 2023-06-05 11:02:00.398119 satellitevu-1.5.1/satellitevu/apis/otm.py
--rw-r--r--   0        0        0      149 2023-04-25 11:16:02.656814 satellitevu-1.5.1/satellitevu/auth/__init__.py
--rw-r--r--   0        0        0     2799 2023-04-25 11:16:02.657060 satellitevu-1.5.1/satellitevu/auth/auth.py
--rw-r--r--   0        0        0     1664 2023-04-25 11:16:02.657296 satellitevu-1.5.1/satellitevu/auth/auth_test.py
--rw-r--r--   0        0        0     1956 2023-04-25 11:16:02.657552 satellitevu-1.5.1/satellitevu/auth/cache.py
--rw-r--r--   0        0        0     2144 2023-04-25 11:16:02.657786 satellitevu-1.5.1/satellitevu/auth/cache_test.py
--rw-r--r--   0        0        0      122 2023-04-25 11:16:02.658168 satellitevu-1.5.1/satellitevu/auth/exc.py
--rw-r--r--   0        0        0     2622 2023-05-19 14:19:02.843967 satellitevu-1.5.1/satellitevu/client.py
--rw-r--r--   0        0        0     1363 2023-04-25 11:16:02.659391 satellitevu-1.5.1/satellitevu/config.py
--rw-r--r--   0        0        0     2406 2023-04-25 11:16:02.659787 satellitevu-1.5.1/satellitevu/conftest.py
--rw-r--r--   0        0        0      148 2023-04-25 11:16:02.660323 satellitevu-1.5.1/satellitevu/http/__init__.py
--rw-r--r--   0        0        0     2038 2023-04-25 11:16:02.661129 satellitevu-1.5.1/satellitevu/http/base.py
--rw-r--r--   0        0        0     3327 2023-04-25 11:16:02.661491 satellitevu-1.5.1/satellitevu/http/http_test.py
--rw-r--r--   0        0        0     1305 2023-04-25 11:16:02.661854 satellitevu-1.5.1/satellitevu/http/httpx.py
--rw-r--r--   0        0        0     1334 2023-04-25 11:16:02.662154 satellitevu-1.5.1/satellitevu/http/requests.py
--rw-r--r--   0        0        0     1744 2023-04-25 11:16:02.662427 satellitevu-1.5.1/satellitevu/http/urllib.py
--rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 satellitevu-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-25 11:16:02.648422 satellitevu-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3859 2023-06-09 09:59:59.328597 satellitevu-1.6.0/README.md
+-rw-r--r--   0        0        0     1082 2023-06-09 16:31:53.860924 satellitevu-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-25 11:16:02.654100 satellitevu-1.6.0/satellitevu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:16:02.654475 satellitevu-1.6.0/satellitevu/apis/__init__.py
+-rw-r--r--   0        0        0     2838 2023-04-25 11:16:02.654773 satellitevu-1.6.0/satellitevu/apis/archive.py
+-rw-r--r--   0        0        0     2440 2023-04-25 11:16:02.655075 satellitevu-1.6.0/satellitevu/apis/archive_test.py
+-rw-r--r--   0        0        0     1175 2023-04-25 11:16:02.655329 satellitevu-1.6.0/satellitevu/apis/base.py
+-rw-r--r--   0        0        0     1287 2023-04-25 11:16:02.655584 satellitevu-1.6.0/satellitevu/apis/base_test.py
+-rw-r--r--   0        0        0     5617 2023-04-25 11:16:02.655864 satellitevu-1.6.0/satellitevu/apis/orders.py
+-rw-r--r--   0        0        0    10041 2023-04-25 11:16:02.656154 satellitevu-1.6.0/satellitevu/apis/orders_test.py
+-rw-r--r--   0        0        0     7124 2023-06-05 11:02:00.398119 satellitevu-1.6.0/satellitevu/apis/otm.py
+-rw-r--r--   0        0        0      149 2023-04-25 11:16:02.656814 satellitevu-1.6.0/satellitevu/auth/__init__.py
+-rw-r--r--   0        0        0     2799 2023-04-25 11:16:02.657060 satellitevu-1.6.0/satellitevu/auth/auth.py
+-rw-r--r--   0        0        0     1664 2023-04-25 11:16:02.657296 satellitevu-1.6.0/satellitevu/auth/auth_test.py
+-rw-r--r--   0        0        0     1956 2023-04-25 11:16:02.657552 satellitevu-1.6.0/satellitevu/auth/cache.py
+-rw-r--r--   0        0        0     2144 2023-04-25 11:16:02.657786 satellitevu-1.6.0/satellitevu/auth/cache_test.py
+-rw-r--r--   0        0        0      122 2023-04-25 11:16:02.658168 satellitevu-1.6.0/satellitevu/auth/exc.py
+-rw-r--r--   0        0        0     2622 2023-05-19 14:19:02.843967 satellitevu-1.6.0/satellitevu/client.py
+-rw-r--r--   0        0        0     1363 2023-04-25 11:16:02.659391 satellitevu-1.6.0/satellitevu/config.py
+-rw-r--r--   0        0        0     2406 2023-04-25 11:16:02.659787 satellitevu-1.6.0/satellitevu/conftest.py
+-rw-r--r--   0        0        0      148 2023-04-25 11:16:02.660323 satellitevu-1.6.0/satellitevu/http/__init__.py
+-rw-r--r--   0        0        0     2038 2023-04-25 11:16:02.661129 satellitevu-1.6.0/satellitevu/http/base.py
+-rw-r--r--   0        0        0     3327 2023-04-25 11:16:02.661491 satellitevu-1.6.0/satellitevu/http/http_test.py
+-rw-r--r--   0        0        0     1305 2023-04-25 11:16:02.661854 satellitevu-1.6.0/satellitevu/http/httpx.py
+-rw-r--r--   0        0        0     1334 2023-04-25 11:16:02.662154 satellitevu-1.6.0/satellitevu/http/requests.py
+-rw-r--r--   0        0        0     1744 2023-04-25 11:16:02.662427 satellitevu-1.6.0/satellitevu/http/urllib.py
+-rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 satellitevu-1.6.0/PKG-INFO
```

### Comparing `satellitevu-1.5.1/LICENSE` & `satellitevu-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/README.md` & `satellitevu-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/pyproject.toml` & `satellitevu-1.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satellitevu"
-version = "1.5.1"
+version = "1.6.0"
 description = "Client SDK for SatelliteVu's platform APIs"
 authors = ["Christian Wygoda <christian.wygoda@satellitevu.com>", "Zhelini Sivanesan <zhelini.sivanesan@satellitevu.com>", "James Harrison <james.harrison@satellitevu.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `satellitevu-1.5.1/satellitevu/apis/archive.py` & `satellitevu-1.6.0/satellitevu/apis/archive.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/apis/archive_test.py` & `satellitevu-1.6.0/satellitevu/apis/archive_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/apis/base.py` & `satellitevu-1.6.0/satellitevu/apis/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/apis/base_test.py` & `satellitevu-1.6.0/satellitevu/apis/base_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/apis/orders.py` & `satellitevu-1.6.0/satellitevu/apis/orders.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/apis/orders_test.py` & `satellitevu-1.6.0/satellitevu/apis/orders_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/apis/otm.py` & `satellitevu-1.6.0/satellitevu/apis/otm.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/auth/auth.py` & `satellitevu-1.6.0/satellitevu/auth/auth.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/auth/auth_test.py` & `satellitevu-1.6.0/satellitevu/auth/auth_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/auth/cache.py` & `satellitevu-1.6.0/satellitevu/auth/cache.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/auth/cache_test.py` & `satellitevu-1.6.0/satellitevu/auth/cache_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/client.py` & `satellitevu-1.6.0/satellitevu/client.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/config.py` & `satellitevu-1.6.0/satellitevu/config.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/conftest.py` & `satellitevu-1.6.0/satellitevu/conftest.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/http/base.py` & `satellitevu-1.6.0/satellitevu/http/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/http/http_test.py` & `satellitevu-1.6.0/satellitevu/http/http_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/http/httpx.py` & `satellitevu-1.6.0/satellitevu/http/httpx.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/http/requests.py` & `satellitevu-1.6.0/satellitevu/http/requests.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/satellitevu/http/urllib.py` & `satellitevu-1.6.0/satellitevu/http/urllib.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.5.1/PKG-INFO` & `satellitevu-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellitevu
-Version: 1.5.1
+Version: 1.6.0
 Summary: Client SDK for SatelliteVu's platform APIs
 License: MIT
 Author: Christian Wygoda
 Author-email: christian.wygoda@satellitevu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

