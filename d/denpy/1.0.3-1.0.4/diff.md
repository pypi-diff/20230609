# Comparing `tmp/denpy-1.0.3.tar.gz` & `tmp/denpy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.3.tar", last modified: Fri Jun  9 21:44:56 2023, max compression
+gzip compressed data, was "denpy-1.0.4.tar", last modified: Fri Jun  9 21:50:28 2023, max compression
```

## Comparing `denpy-1.0.3.tar` & `denpy-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 21:44:56.417771 denpy-1.0.3/
--rw-rw-rw-   0        0        0      112 2023-06-09 21:44:56.417771 denpy-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 21:44:56.412784 denpy-1.0.3/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.3/denpy/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.3/denpy/color.py
--rw-rw-rw-   0        0        0     1718 2023-06-09 21:29:58.000000 denpy-1.0.3/denpy/database.py
--rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.3/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:44:56.416774 denpy-1.0.3/denpy.egg-info/
--rw-rw-rw-   0        0        0      112 2023-06-09 21:44:56.000000 denpy-1.0.3/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-09 21:44:56.000000 denpy-1.0.3/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 21:44:56.000000 denpy-1.0.3/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 21:44:56.000000 denpy-1.0.3/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 21:44:56.417771 denpy-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-09 21:44:54.000000 denpy-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:28.574699 denpy-1.0.4/
+-rw-rw-rw-   0        0        0      112 2023-06-09 21:50:28.574699 denpy-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:28.569744 denpy-1.0.4/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.4/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.4/denpy/color.py
+-rw-rw-rw-   0        0        0     1716 2023-06-09 21:49:51.000000 denpy-1.0.4/denpy/database.py
+-rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.4/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:28.573701 denpy-1.0.4/denpy.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 21:50:28.574699 denpy-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      205 2023-06-09 21:50:22.000000 denpy-1.0.4/setup.py
```

### Comparing `denpy-1.0.3/denpy/database.py` & `denpy-1.0.4/denpy/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sqlite3
 
 def connect(__file__: str) -> tuple[sqlite3.Connection, sqlite3.Cursor]:
-    path = __file__.split('\\')
+    path = __file__.split('/')
     path.pop(-1)
     path.pop(-1)
     path.append('database.db')
-    database = sqlite3.connect('\\'.join(path))
+    database = sqlite3.connect('/'.join(path))
     cursor = database.cursor()
     return database, cursor
 
 def disconnect(database: sqlite3.Connection, cursor: sqlite3.Cursor):
     database.commit()
     cursor.close()
     database.close()
```

### Comparing `denpy-1.0.3/denpy/utils.py` & `denpy-1.0.4/denpy/utils.py`

 * *Files identical despite different names*

