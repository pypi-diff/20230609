# Comparing `tmp/dbt-databricks-1.5.2.tar.gz` & `tmp/dbt-databricks-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.5.2.tar", last modified: Wed May 17 18:32:04 2023, max compression
+gzip compressed data, was "dbt-databricks-1.5.3.tar", last modified: Thu Jun  8 16:30:30 2023, max compression
```

## Comparing `dbt-databricks-1.5.2.tar` & `dbt-databricks-1.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.169320 dbt-databricks-1.5.2/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/MANIFEST.in
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-05-17 18:32:04.169047 dbt-databricks-1.5.2/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-05-17 18:30:31.000000 dbt-databricks-1.5.2/README.md
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.141534 dbt-databricks-1.5.2/dbt/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.141125 dbt-databricks-1.5.2/dbt/adapters/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.153442 dbt-databricks-1.5.2/dbt/adapters/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       22 2023-05-17 18:32:01.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2708 2023-05-02 22:11:51.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/auth.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/column.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    26590 2023-05-10 23:51:18.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/connections.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    19041 2023-05-17 18:30:31.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/impl.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    17731 2023-05-17 18:30:27.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/relation.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.141825 dbt-databricks-1.5.2/dbt/include/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.155606 dbt-databricks-1.5.2/dbt/include/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/dbt/include/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.158149 dbt-databricks-1.5.2/dbt/include/databricks/macros/
--rw-r--r--   0 andre.furlan   (502) staff       (20)    10178 2023-05-02 22:12:17.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.162063 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.163666 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-05-02 16:19:19.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-05-02 16:19:19.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-05-02 16:19:19.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/seed.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.165013 dbt-databricks-1.5.2/dbt/include/databricks/macros/utils/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.5.2/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      535 2023-05-02 22:11:51.000000 dbt-databricks-1.5.2/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-17 18:32:04.168583 dbt-databricks-1.5.2/dbt_databricks.egg-info/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-05-17 18:32:04.000000 dbt-databricks-1.5.2/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1421 2023-05-17 18:32:04.000000 dbt-databricks-1.5.2/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-17 18:32:04.000000 dbt-databricks-1.5.2/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:20:40.000000 dbt-databricks-1.5.2/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 andre.furlan   (502) staff       (20)      105 2023-05-17 18:32:04.000000 dbt-databricks-1.5.2/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-05-17 18:32:04.000000 dbt-databricks-1.5.2/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-05-17 18:32:04.169406 dbt-databricks-1.5.2/setup.cfg
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2607 2023-05-17 18:31:34.000000 dbt-databricks-1.5.2/setup.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.983027 dbt-databricks-1.5.3/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/MANIFEST.in
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-06-08 16:30:30.982803 dbt-databricks-1.5.3/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-05-17 18:30:31.000000 dbt-databricks-1.5.3/README.md
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.948316 dbt-databricks-1.5.3/dbt/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.948000 dbt-databricks-1.5.3/dbt/adapters/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.957564 dbt-databricks-1.5.3/dbt/adapters/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       22 2023-06-08 16:30:00.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2708 2023-05-02 22:11:51.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/column.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    26590 2023-06-08 16:20:11.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    19041 2023-05-17 18:30:31.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    17731 2023-05-17 18:30:27.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.948811 dbt-databricks-1.5.3/dbt/include/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.961070 dbt-databricks-1.5.3/dbt/include/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/dbt/include/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.965612 dbt-databricks-1.5.3/dbt/include/databricks/macros/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    10178 2023-05-02 22:12:17.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.971328 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.975884 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-05-02 16:19:19.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-05-02 16:19:19.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-05-02 16:19:19.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/seed.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.977778 dbt-databricks-1.5.3/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.5.3/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      535 2023-05-02 22:11:51.000000 dbt-databricks-1.5.3/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-08 16:30:30.982198 dbt-databricks-1.5.3/dbt_databricks.egg-info/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-06-08 16:30:30.000000 dbt-databricks-1.5.3/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1421 2023-06-08 16:30:30.000000 dbt-databricks-1.5.3/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-06-08 16:30:30.000000 dbt-databricks-1.5.3/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:20:40.000000 dbt-databricks-1.5.3/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      105 2023-06-08 16:30:30.000000 dbt-databricks-1.5.3/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-06-08 16:30:30.000000 dbt-databricks-1.5.3/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-06-08 16:30:30.983074 dbt-databricks-1.5.3/setup.cfg
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2607 2023-06-08 16:27:34.000000 dbt-databricks-1.5.3/setup.py
```

### Comparing `dbt-databricks-1.5.2/PKG-INFO` & `dbt-databricks-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.5.2/README.md` & `dbt-databricks-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/column.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.5.3/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/seed.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.5.3/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.5.3/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.5.3/dbt_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.5.2/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.5.3/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.2/setup.py` & `dbt-databricks-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     long_description_content_type="text/markdown",
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-spark>=1.5.0",
-        "databricks-sql-connector>=2.5.0",
+        "dbt-spark~=1.5.0",
+        "databricks-sql-connector~=2.5.0",
         "databricks-sdk==0.1.6",
         "keyring>=23.13.0",
         "protobuf>=4.21.0" # workaround for dbt-core issue
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

