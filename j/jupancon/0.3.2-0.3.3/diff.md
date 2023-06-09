# Comparing `tmp/jupancon-0.3.2.tar.gz` & `tmp/jupancon-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupancon-0.3.2.tar", last modified: Thu Nov 17 08:17:27 2022, max compression
+gzip compressed data, was "jupancon-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jupancon-0.3.2.tar` & `jupancon-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1996 2021-11-11 11:42:36.367913 jupancon-0.3.2/.gitignore
--rw-r--r--   0        0        0     1070 2022-07-27 14:05:28.345576 jupancon-0.3.2/LICENSE
--rw-r--r--   0        0        0     4651 2022-11-17 08:15:35.931124 jupancon-0.3.2/README.md
--rw-r--r--   0        0        0      675 2022-11-17 08:16:03.350384 jupancon-0.3.2/jupancon/__init__.py
--rw-r--r--   0        0        0     5145 2022-11-17 08:15:35.931124 jupancon-0.3.2/jupancon/config.py
--rw-r--r--   0        0        0     3295 2022-11-17 08:15:35.931124 jupancon-0.3.2/jupancon/core.py
--rw-r--r--   0        0        0      110 2022-11-16 22:45:24.773564 jupancon-0.3.2/jupancon/defaults.py
--rw-r--r--   0        0        0        0 2022-11-17 08:15:35.931124 jupancon-0.3.2/jupancon/engine/__init__.py
--rw-r--r--   0        0        0      513 2022-11-17 08:15:35.931124 jupancon-0.3.2/jupancon/engine/databricks.py
--rw-r--r--   0        0        0     1594 2022-01-09 20:21:44.042958 jupancon-0.3.2/jupancon/magic.py
--rw-r--r--   0        0        0      946 2022-11-17 08:15:35.931124 jupancon-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      484 2021-11-02 20:57:50.060991 jupancon-0.3.2/test/test_config.py
--rw-r--r--   0        0        0      127 2021-11-02 20:50:41.652234 jupancon-0.3.2/test/test_configfile.yml
--rw-r--r--   0        0        0     5695 1970-01-01 00:00:00.000000 jupancon-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1996 2022-09-05 06:18:49.308982 jupancon-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1072 2023-06-09 16:11:42.531226 jupancon-0.3.3/LICENSE.md
+-rw-r--r--   0        0        0     4651 2023-03-02 16:40:56.739388 jupancon-0.3.3/README.md
+-rw-r--r--   0        0        0      675 2023-06-09 16:35:17.049728 jupancon-0.3.3/jupancon/__init__.py
+-rw-r--r--   0        0        0     5145 2023-03-02 16:40:56.743389 jupancon-0.3.3/jupancon/config.py
+-rw-r--r--   0        0        0     4614 2023-03-02 16:40:56.743389 jupancon-0.3.3/jupancon/core.py
+-rw-r--r--   0        0        0      110 2022-09-05 06:18:49.308982 jupancon-0.3.3/jupancon/defaults.py
+-rw-r--r--   0        0        0        0 2023-03-02 16:40:56.743389 jupancon-0.3.3/jupancon/engine/__init__.py
+-rw-r--r--   0        0        0      513 2023-03-02 16:40:56.743389 jupancon-0.3.3/jupancon/engine/databricks.py
+-rw-r--r--   0        0        0     1594 2022-09-05 06:18:49.308982 jupancon-0.3.3/jupancon/magic.py
+-rw-r--r--   0        0        0      830 2023-06-09 16:00:34.437384 jupancon-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      484 2022-09-05 06:18:49.308982 jupancon-0.3.3/test/test_config.py
+-rw-r--r--   0        0        0      127 2022-09-05 06:18:49.308982 jupancon-0.3.3/test/test_configfile.yml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 jupancon-0.3.3/PKG-INFO
```

### Comparing `jupancon-0.3.2/.gitignore` & `jupancon-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupancon-0.3.2/LICENSE` & `jupancon-0.3.3/LICENSE.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 multilayer-io
+Copyright (c) 2023 multilayer-labs
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jupancon-0.3.2/README.md` & `jupancon-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jupancon-0.3.2/jupancon/__init__.py` & `jupancon-0.3.3/jupancon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Jupancon, connector to several DBs that returns pandas. Magic included."""
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 
 from .core import (change, df_to_table, list_schemas, list_tables, peek,
                    peek_schema, query, query_raw)
 
 
 # snippet to check if the environment is interactive
```

### Comparing `jupancon-0.3.2/jupancon/config.py` & `jupancon-0.3.3/jupancon/config.py`

 * *Files identical despite different names*

### Comparing `jupancon-0.3.2/jupancon/engine/databricks.py` & `jupancon-0.3.3/jupancon/engine/databricks.py`

 * *Files identical despite different names*

### Comparing `jupancon-0.3.2/jupancon/magic.py` & `jupancon-0.3.3/jupancon/magic.py`

 * *Files identical despite different names*

### Comparing `jupancon-0.3.2/pyproject.toml` & `jupancon-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 name = "jupancon"
 authors = [{name = "Juan Gonz\u00e1lez-Vallinas", email = "juan@multilayer.io"}]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 
 dependencies = [
-    "pandas>=1.5.1",
+    "pandas<2.0.0",
     "sshtunnel>=0.4.0",
     "pyparsing>=3.0.9",
-    "sqlalchemy-redshift>=0.8.11", 
-    "redshift-connector>=2.0.909",
-    "databricks-sql-connector>=2.1.0"
+    "sqlalchemy-redshift>=0.8.14", 
+    "redshift-connector>=2.0.911",
+    "databricks-sql-connector>=2.6.1",
+    "sqlalchemy-bigquery>=1.6.1", 
+    "google-cloud-bigquery-storage>=2.20.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=6.2.5",
     "jupyter>=1.0.0",
     "jupyterlab>=3.1.14",
     "black>=21.9b0",
     "flake8>=3.9.2",
     "isort>=5.9.3"
 ]
 
-bigquery = [
-    "sqlalchemy-bigquery==1.4.4", # this package is problematic because it requires an old version of pyarrow and conflicts with others
-    "google-cloud-bigquery-storage>=2.16.2"
-]
 
 [project.urls]
 Home = "https://github.com/multilayer-io/jupancon"
```

### Comparing `jupancon-0.3.2/PKG-INFO` & `jupancon-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: jupancon
-Version: 0.3.2
+Version: 0.3.3
 Summary: Jupancon, connector to several DBs that returns pandas. Magic included.
 Author-email: Juan González-Vallinas <juan@multilayer.io>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: pandas>=1.5.1
+Requires-Dist: pandas<2.0.0
 Requires-Dist: sshtunnel>=0.4.0
 Requires-Dist: pyparsing>=3.0.9
-Requires-Dist: sqlalchemy-redshift>=0.8.11
-Requires-Dist: redshift-connector>=2.0.909
-Requires-Dist: databricks-sql-connector>=2.1.0
-Requires-Dist: sqlalchemy-bigquery==1.4.4 ; extra == "bigquery"
-Requires-Dist: google-cloud-bigquery-storage>=2.16.2 ; extra == "bigquery"
+Requires-Dist: sqlalchemy-redshift>=0.8.14
+Requires-Dist: redshift-connector>=2.0.911
+Requires-Dist: databricks-sql-connector>=2.6.1
+Requires-Dist: sqlalchemy-bigquery>=1.6.1
+Requires-Dist: google-cloud-bigquery-storage>=2.20.0
 Requires-Dist: pytest>=6.2.5 ; extra == "test"
 Requires-Dist: jupyter>=1.0.0 ; extra == "test"
 Requires-Dist: jupyterlab>=3.1.14 ; extra == "test"
 Requires-Dist: black>=21.9b0 ; extra == "test"
 Requires-Dist: flake8>=3.9.2 ; extra == "test"
 Requires-Dist: isort>=5.9.3 ; extra == "test"
 Project-URL: Home, https://github.com/multilayer-io/jupancon
-Provides-Extra: bigquery
 Provides-Extra: test
 
 # jupancon
 
 Database Connectors and SQL magics for [Jupyter](https://docs.jupyter.org/en/latest/). `jupancon` = Jupyter + Pandas + Connectors. 
 
 ### Features
```

