# Comparing `tmp/vertica-sqlalchemy-dialect-0.0.4.tar.gz` & `tmp/vertica-sqlalchemy-dialect-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.4.tar", last modified: Tue Jun  6 17:05:22 2023, max compression
+gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.5.tar", last modified: Fri Jun  9 14:25:23 2023, max compression
```

## Comparing `vertica-sqlalchemy-dialect-0.0.4.tar` & `vertica-sqlalchemy-dialect-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.978170 vertica-sqlalchemy-dialect-0.0.4/
--rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5749 2023-06-06 17:05:22.980141 vertica-sqlalchemy-dialect-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5402 2023-06-06 16:57:33.000000 vertica-sqlalchemy-dialect-0.0.4/README.rst
--rw-rw-rw-   0        0        0      211 2023-06-06 17:05:22.984145 vertica-sqlalchemy-dialect-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1922 2023-06-06 16:58:01.000000 vertica-sqlalchemy-dialect-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.884139 vertica-sqlalchemy-dialect-0.0.4/test/
--rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/test/test_core.py
--rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/test/test_integration.py
--rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/test/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.929143 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/
--rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/__init__.py
--rw-rw-rw-   0        0        0    68805 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/base.py
--rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_pyodbc.py
--rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_vertica_python.py
--rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/requirements.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.973138 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/
--rw-rw-rw-   0        0        0     5749 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.873414 vertica-sqlalchemy-dialect-0.0.5/
+-rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5749 2023-06-09 14:25:23.875414 vertica-sqlalchemy-dialect-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2023-06-06 16:57:33.000000 vertica-sqlalchemy-dialect-0.0.5/README.rst
+-rw-rw-rw-   0        0        0      211 2023-06-09 14:25:23.880445 vertica-sqlalchemy-dialect-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2023-06-09 13:48:02.000000 vertica-sqlalchemy-dialect-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.698413 vertica-sqlalchemy-dialect-0.0.5/test/
+-rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/test/test_core.py
+-rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/test/test_integration.py
+-rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.818415 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/
+-rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/__init__.py
+-rw-rw-rw-   0        0        0    68765 2023-06-09 14:23:32.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/base.py
+-rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_pyodbc.py
+-rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_vertica_python.py
+-rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/requirements.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.866415 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/
+-rw-rw-rw-   0        0        0     5749 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/top_level.txt
```

### Comparing `vertica-sqlalchemy-dialect-0.0.4/LICENSE` & `vertica-sqlalchemy-dialect-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.4
+Version: 0.0.5
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.4/README.rst` & `vertica-sqlalchemy-dialect-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/setup.py` & `vertica-sqlalchemy-dialect-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from setuptools import setup
 
 with open("README.rst", "r") as f:
     description = f.read()
 
 
-version_info = (0, 0, 4)
+version_info = (0, 0, 5)
 
 version = '.'.join(map(str, version_info))
 
 setup(
     name='vertica-sqlalchemy-dialect',
     version=version,
     description='Official Vertica dialect for SQLalchemy',
```

### Comparing `vertica-sqlalchemy-dialect-0.0.4/test/test_core.py` & `vertica-sqlalchemy-dialect-0.0.5/test/test_core.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/test/test_integration.py` & `vertica-sqlalchemy-dialect-0.0.5/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/test/test_suite.py` & `vertica-sqlalchemy-dialect-0.0.5/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/base.py` & `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1148,56 +1148,56 @@
 
     @reflection.cache
     def get_projection_comment(self, connection, schema=None, **kw):
         
         src = sql.text(dedent("""
                 SELECT ros_count , LOWER(projection_name)
                 FROM v_monitor.projection_storage
-                WHERE lower(projection_schema) = '%(schema)s'
+                WHERE projection_schema = '%(schema)s'
 
             """ % {'schema': schema}))
         
         projection_type =sql.text(dedent("""
-                SELECT is_super_projection,is_key_constraint_projection,is_aggregate_projection,has_expressions ,LOWER(projection_name)
+                SELECT DISTINCT is_super_projection,is_key_constraint_projection,is_aggregate_projection,has_expressions ,LOWER(projection_name)
                 FROM v_catalog.projections
-                WHERE lower(projection_schema) = '%(schema)s' 
+                WHERE projection_schema = '%(schema)s' 
                 """ % {'schema': schema}))
         
         
         is_segmented = sql.text(dedent("""
                 SELECT is_segmented , segment_expression , LOWER(projection_name)
                 FROM v_catalog.projections 
-                WHERE lower(projection_schema) = '%(schema)s'
+                WHERE projection_schema = '%(schema)s'
             """ % {'schema': schema}))
         
         
         partition_key = sql.text(dedent("""
                 SELECT  DISTINCT LOWER(projection_name) ,  partition_key 
                 FROM v_monitor.partitions
-                WHERE lower(table_schema) = '%(schema)s'
+                WHERE table_schema = '%(schema)s'
               
             """ % {'schema': schema}))
         
         partition_num = sql.text(dedent("""
                 SELECT  COUNT(ros_id) , LOWER(projection_name)
                 FROM v_monitor.partitions
-                WHERE lower(table_schema) = '%(schema)s'
+                WHERE table_schema = '%(schema)s'
                 GROUP BY projection_name
             """ % {'schema': schema}))
         
         projection_size = sql.text(dedent("""
             SELECT used_bytes , LOWER(projection_name) 
             from v_monitor.projection_storage
-            WHERE lower(projection_schema) = '%(schema)s'
+            WHERE projection_schema = '%(schema)s'
         """ % {'schema': schema}))
         
         projection_cache = sql.text(dedent("""
             SELECT COUNT(*) , object_name
             FROM DEPOT_PIN_POLICIES
-            WHERE lower(schema_name) = '%(schema)s'
+            WHERE schema_name = '%(schema)s'
             GROUP BY object_name 
             """ % {'schema': schema}))
         
         projection_comment = []
       
         ros_count = {}
         for data in connection.execute(src):
```

### Comparing `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_pyodbc.py` & `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_pyodbc.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_vertica_python.py` & `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_vertica_python.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/requirements.py` & `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/requirements.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.4
+Version: 0.0.5
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt` & `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

