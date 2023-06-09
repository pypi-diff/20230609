# Comparing `tmp/many_migrations-0.2.tar.gz` & `tmp/many_migrations-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many_migrations-0.2.tar", max compression
+gzip compressed data, was "many_migrations-0.3.tar", max compression
```

## Comparing `many_migrations-0.2.tar` & `many_migrations-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-06-09 09:38:57.415614 many_migrations-0.2/LICENSE
--rw-r--r--   0        0        0     2264 2023-06-09 09:38:57.415614 many_migrations-0.2/README.md
--rw-r--r--   0        0        0      509 2023-06-09 09:38:57.419615 many_migrations-0.2/pyproject.toml
--rw-r--r--   0        0        0     1802 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/__init__.py
--rw-r--r--   0        0        0      172 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/default-config.ini
--rw-r--r--   0        0        0      440 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/engine.py
--rw-r--r--   0        0        0     2847 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/migrate.py
--rw-r--r--   0        0        0     2777 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/revise.py
--rw-r--r--   0        0        0      389 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/__init__.py
--rw-r--r--   0        0        0      191 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/base.py.mako
--rw-r--r--   0        0        0      272 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/elasticsearch.py.mako
--rw-r--r--   0        0        0      261 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/spark.py.mako
--rw-r--r--   0        0        0      249 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/sqlalchemy.py.mako
--rw-r--r--   0        0        0       96 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/utils.py
--rw-r--r--   0        0        0     2789 1970-01-01 00:00:00.000000 many_migrations-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-09 10:10:39.527938 many_migrations-0.3/LICENSE
+-rw-r--r--   0        0        0     2264 2023-06-09 10:10:39.527938 many_migrations-0.3/README.md
+-rw-r--r--   0        0        0     1802 2023-06-09 10:10:39.531938 many_migrations-0.3/many/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-09 10:10:39.531938 many_migrations-0.3/many/default-config.ini
+-rw-r--r--   0        0        0      440 2023-06-09 10:10:39.531938 many_migrations-0.3/many/engine.py
+-rw-r--r--   0        0        0     2847 2023-06-09 10:10:39.531938 many_migrations-0.3/many/migrate.py
+-rw-r--r--   0        0        0     2777 2023-06-09 10:10:39.531938 many_migrations-0.3/many/revise.py
+-rw-r--r--   0        0        0      389 2023-06-09 10:10:39.531938 many_migrations-0.3/many/templates/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-09 10:10:39.531938 many_migrations-0.3/many/templates/base.py.mako
+-rw-r--r--   0        0        0      272 2023-06-09 10:10:39.531938 many_migrations-0.3/many/templates/elasticsearch.py.mako
+-rw-r--r--   0        0        0      261 2023-06-09 10:10:39.531938 many_migrations-0.3/many/templates/spark.py.mako
+-rw-r--r--   0        0        0      249 2023-06-09 10:10:39.531938 many_migrations-0.3/many/templates/sqlalchemy.py.mako
+-rw-r--r--   0        0        0       96 2023-06-09 10:10:39.531938 many_migrations-0.3/many/utils.py
+-rw-r--r--   0        0        0      522 2023-06-09 10:10:39.531938 many_migrations-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2789 1970-01-01 00:00:00.000000 many_migrations-0.3/PKG-INFO
```

### Comparing `many_migrations-0.2/LICENSE` & `many_migrations-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `many_migrations-0.2/README.md` & `many_migrations-0.3/README.md`

 * *Files identical despite different names*

### Comparing `many_migrations-0.2/src/many/__init__.py` & `many_migrations-0.3/many/__init__.py`

 * *Files identical despite different names*

### Comparing `many_migrations-0.2/src/many/migrate.py` & `many_migrations-0.3/many/migrate.py`

 * *Files identical despite different names*

### Comparing `many_migrations-0.2/src/many/revise.py` & `many_migrations-0.3/many/revise.py`

 * *Files identical despite different names*

### Comparing `many_migrations-0.2/PKG-INFO` & `many_migrations-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: many-migrations
-Version: 0.2
+Version: 0.3
 Summary: 
 Author: Thijsvandepoll
 Author-email: thijsvandepoll@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

