# Comparing `tmp/many_migrations-0.1.0.tar.gz` & `tmp/many_migrations-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many_migrations-0.1.0.tar", max compression
+gzip compressed data, was "many_migrations-0.2.tar", max compression
```

## Comparing `many_migrations-0.1.0.tar` & `many_migrations-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-06-09 09:03:19.805059 many_migrations-0.1.0/LICENSE
--rw-r--r--   0        0        0     2258 2023-06-09 09:03:19.805059 many_migrations-0.1.0/README.md
--rw-r--r--   0        0        0      512 2023-06-09 09:03:19.809059 many_migrations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1802 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/__init__.py
--rw-r--r--   0        0        0      172 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/default-config.ini
--rw-r--r--   0        0        0      440 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/engine.py
--rw-r--r--   0        0        0     2847 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/migrate.py
--rw-r--r--   0        0        0     2777 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/revise.py
--rw-r--r--   0        0        0      389 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/templates/__init__.py
--rw-r--r--   0        0        0      191 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/templates/base.py.mako
--rw-r--r--   0        0        0      272 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/templates/elasticsearch.py.mako
--rw-r--r--   0        0        0      261 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/templates/spark.py.mako
--rw-r--r--   0        0        0      249 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/templates/sqlalchemy.py.mako
--rw-r--r--   0        0        0       96 2023-06-09 09:03:19.809059 many_migrations-0.1.0/src/many/utils.py
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 many_migrations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-09 09:38:57.415614 many_migrations-0.2/LICENSE
+-rw-r--r--   0        0        0     2264 2023-06-09 09:38:57.415614 many_migrations-0.2/README.md
+-rw-r--r--   0        0        0      509 2023-06-09 09:38:57.419615 many_migrations-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1802 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/default-config.ini
+-rw-r--r--   0        0        0      440 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/engine.py
+-rw-r--r--   0        0        0     2847 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/migrate.py
+-rw-r--r--   0        0        0     2777 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/revise.py
+-rw-r--r--   0        0        0      389 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/base.py.mako
+-rw-r--r--   0        0        0      272 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/elasticsearch.py.mako
+-rw-r--r--   0        0        0      261 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/spark.py.mako
+-rw-r--r--   0        0        0      249 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/templates/sqlalchemy.py.mako
+-rw-r--r--   0        0        0       96 2023-06-09 09:38:57.419615 many_migrations-0.2/src/many/utils.py
+-rw-r--r--   0        0        0     2789 1970-01-01 00:00:00.000000 many_migrations-0.2/PKG-INFO
```

### Comparing `many_migrations-0.1.0/LICENSE` & `many_migrations-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `many_migrations-0.1.0/README.md` & `many_migrations-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 To create your own migration application for your data store:
 1. Subclass the `MigrationEngine` class and implement its methods.
 2. Optionally, create a customized migration template by using `Mako` templates.
 3. Initialize your application using `init_app` function with your customized `MigrationEngine` and `Template`
 4. Run you application.
 
 How this would look like:
-```
+```python
 # migration_app.py
 
 from many import MigrationEngine, init_app
 
 class CustomEngine(MigrationEngine):
     def init_remote(self):
         # Add logic to initialize a place where the state can be maintained (e.g. a table).
```

### Comparing `many_migrations-0.1.0/src/many/__init__.py` & `many_migrations-0.2/src/many/__init__.py`

 * *Files identical despite different names*

### Comparing `many_migrations-0.1.0/src/many/migrate.py` & `many_migrations-0.2/src/many/migrate.py`

 * *Files identical despite different names*

### Comparing `many_migrations-0.1.0/src/many/revise.py` & `many_migrations-0.2/src/many/revise.py`

 * *Files identical despite different names*

### Comparing `many_migrations-0.1.0/PKG-INFO` & `many_migrations-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: many-migrations
-Version: 0.1.0
+Version: 0.2
 Summary: 
 Author: Thijsvandepoll
 Author-email: thijsvandepoll@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mako (>=1.2.4,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Many: A library to migrate anything!
@@ -19,15 +21,15 @@
 To create your own migration application for your data store:
 1. Subclass the `MigrationEngine` class and implement its methods.
 2. Optionally, create a customized migration template by using `Mako` templates.
 3. Initialize your application using `init_app` function with your customized `MigrationEngine` and `Template`
 4. Run you application.
 
 How this would look like:
-```
+```python
 # migration_app.py
 
 from many import MigrationEngine, init_app
 
 class CustomEngine(MigrationEngine):
     def init_remote(self):
         # Add logic to initialize a place where the state can be maintained (e.g. a table).
```

