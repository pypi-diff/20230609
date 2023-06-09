# Comparing `tmp/GeneralSQL-1.0.6.tar.gz` & `tmp/GeneralSQL-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeneralSQL-1.0.6.tar", last modified: Fri Jun  9 12:01:14 2023, max compression
+gzip compressed data, was "GeneralSQL-1.0.7.tar", last modified: Fri Jun  9 12:22:47 2023, max compression
```

## Comparing `GeneralSQL-1.0.6.tar` & `GeneralSQL-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL/
--rw-r--r--   0 joker     (1000) joker     (1000)     2321 2022-12-18 15:36:05.000000 GeneralSQL-1.0.6/GeneralSQL/Error.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL/Template/
--rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-06-09 10:46:01.000000 GeneralSQL-1.0.6/GeneralSQL/Template/__init__.py
--rw-r--r--   0 joker     (1000) joker     (1000)     3024 2023-06-09 10:45:33.000000 GeneralSQL-1.0.6/GeneralSQL/Template/base.py
--rw-r--r--   0 joker     (1000) joker     (1000)     2155 2023-06-09 11:56:15.000000 GeneralSQL-1.0.6/GeneralSQL/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL/db/
--rw-r--r--   0 joker     (1000) joker     (1000)    14741 2023-06-09 11:16:08.000000 GeneralSQL-1.0.6/GeneralSQL/db/Jmysql.py
--rw-r--r--   0 joker     (1000) joker     (1000)       57 2022-12-18 15:36:05.000000 GeneralSQL-1.0.6/GeneralSQL/db/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL.egg-info/
--rw-r--r--   0 joker     (1000) joker     (1000)      750 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)      321 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/SOURCES.txt
--rw-r--r--   0 joker     (1000) joker     (1000)        1 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/dependency_links.txt
--rw-r--r--   0 joker     (1000) joker     (1000)       11 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/top_level.txt
--rwxr-xr-x   0 joker     (1000) joker     (1000)    35149 2022-12-18 15:40:21.000000 GeneralSQL-1.0.6/LICENSE
--rw-r--r--   0 joker     (1000) joker     (1000)      750 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)      230 2022-12-18 16:34:16.000000 GeneralSQL-1.0.6/README.md
--rwxr-xr-x   0 joker     (1000) joker     (1000)      510 2023-06-09 04:52:15.000000 GeneralSQL-1.0.6/pyproject.toml
--rw-r--r--   0 joker     (1000) joker     (1000)       38 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/setup.cfg
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/GeneralSQL/
+-rw-r--r--   0 joker     (1000) joker     (1000)     2321 2022-12-18 15:36:05.000000 GeneralSQL-1.0.7/GeneralSQL/Error.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/GeneralSQL/Template/
+-rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-06-09 10:46:01.000000 GeneralSQL-1.0.7/GeneralSQL/Template/__init__.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     3024 2023-06-09 10:45:33.000000 GeneralSQL-1.0.7/GeneralSQL/Template/base.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     2155 2023-06-09 11:56:15.000000 GeneralSQL-1.0.7/GeneralSQL/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/GeneralSQL/db/
+-rw-r--r--   0 joker     (1000) joker     (1000)    14741 2023-06-09 11:16:08.000000 GeneralSQL-1.0.7/GeneralSQL/db/Jmysql.py
+-rw-r--r--   0 joker     (1000) joker     (1000)       57 2022-12-18 15:36:05.000000 GeneralSQL-1.0.7/GeneralSQL/db/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/GeneralSQL.egg-info/
+-rw-r--r--   0 joker     (1000) joker     (1000)     1838 2023-06-09 12:22:47.000000 GeneralSQL-1.0.7/GeneralSQL.egg-info/PKG-INFO
+-rw-r--r--   0 joker     (1000) joker     (1000)      321 2023-06-09 12:22:47.000000 GeneralSQL-1.0.7/GeneralSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)        1 2023-06-09 12:22:47.000000 GeneralSQL-1.0.7/GeneralSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)       11 2023-06-09 12:22:47.000000 GeneralSQL-1.0.7/GeneralSQL.egg-info/top_level.txt
+-rwxr-xr-x   0 joker     (1000) joker     (1000)    35149 2022-12-18 15:40:21.000000 GeneralSQL-1.0.7/LICENSE
+-rw-r--r--   0 joker     (1000) joker     (1000)     1838 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/PKG-INFO
+-rw-r--r--   0 joker     (1000) joker     (1000)     1318 2023-06-09 12:20:50.000000 GeneralSQL-1.0.7/README.md
+-rwxr-xr-x   0 joker     (1000) joker     (1000)      510 2023-06-09 12:21:11.000000 GeneralSQL-1.0.7/pyproject.toml
+-rw-r--r--   0 joker     (1000) joker     (1000)       38 2023-06-09 12:22:47.063558 GeneralSQL-1.0.7/setup.cfg
```

### Comparing `GeneralSQL-1.0.6/GeneralSQL/Error.py` & `GeneralSQL-1.0.7/GeneralSQL/Error.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.0.6/GeneralSQL/Template/__init__.py` & `GeneralSQL-1.0.7/GeneralSQL/Template/__init__.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.0.6/GeneralSQL/Template/base.py` & `GeneralSQL-1.0.7/GeneralSQL/Template/base.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.0.6/GeneralSQL/__init__.py` & `GeneralSQL-1.0.7/GeneralSQL/__init__.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.0.6/GeneralSQL/db/Jmysql.py` & `GeneralSQL-1.0.7/GeneralSQL/db/Jmysql.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.0.6/LICENSE` & `GeneralSQL-1.0.7/LICENSE`

 * *Files identical despite different names*

