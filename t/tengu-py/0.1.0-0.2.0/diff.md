# Comparing `tmp/tengu_py-0.1.0.tar.gz` & `tmp/tengu_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tengu_py-0.1.0.tar", max compression
+gzip compressed data, was "tengu_py-0.2.0.tar", max compression
```

## Comparing `tengu_py-0.1.0.tar` & `tengu_py-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      750 2023-05-31 05:29:35.613982 tengu_py-0.1.0/README.md
--rw-r--r--   0        0        0     1555 2023-05-31 05:38:09.792875 tengu_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-05-31 05:29:35.614982 tengu_py-0.1.0/tengu/__init__.py
--rw-r--r--   0        0        0     8617 2023-05-31 05:29:35.614982 tengu_py-0.1.0/tengu/api.py
--rw-r--r--   0        0        0     7311 2023-05-31 05:29:35.614982 tengu_py-0.1.0/tengu/calcq.py
--rw-r--r--   0        0        0     4434 2023-05-31 05:29:35.614982 tengu_py-0.1.0/tengu/data.py
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 tengu_py-0.1.0/setup.py
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 tengu_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2263 2023-06-08 09:23:36.145850 tengu_py-0.2.0/README.md
+-rw-r--r--   0        0        0     1555 2023-06-08 09:24:23.506267 tengu_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-05-31 05:29:35.614982 tengu_py-0.2.0/tengu/__init__.py
+-rw-r--r--   0        0        0    12563 2023-06-08 09:22:52.450464 tengu_py-0.2.0/tengu/api.py
+-rw-r--r--   0        0        0     7311 2023-05-31 05:29:35.614982 tengu_py-0.2.0/tengu/calcq.py
+-rw-r--r--   0        0        0     4434 2023-05-31 05:29:35.614982 tengu_py-0.2.0/tengu/data.py
+-rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 tengu_py-0.2.0/setup.py
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 tengu_py-0.2.0/PKG-INFO
```

### Comparing `tengu_py-0.1.0/pyproject.toml` & `tengu_py-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 [tool.setuptools.packages]
 [tool.setuptools.packages.find]
 exclude = ["test", "tests"]
 where = [""]
 
 [tool.poetry]
 name = "tengu-py"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python SDK for interacting with the QDX Tengu API"
 authors = ["Ryan Swart <ryan@talosystems.com>"]
 readme = "README.md"
 packages = [{include = "tengu"}]
 
 [tool.poetry.scripts]
 # tengu = "tengu.__main__:main"
```

### Comparing `tengu_py-0.1.0/tengu/calcq.py` & `tengu_py-0.2.0/tengu/calcq.py`

 * *Files identical despite different names*

### Comparing `tengu_py-0.1.0/tengu/data.py` & `tengu_py-0.2.0/tengu/data.py`

 * *Files identical despite different names*

