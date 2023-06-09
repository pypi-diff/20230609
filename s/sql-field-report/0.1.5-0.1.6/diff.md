# Comparing `tmp/sql_field_report-0.1.5.tar.gz` & `tmp/sql_field_report-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.1.5.tar", max compression
+gzip compressed data, was "sql_field_report-0.1.6.tar", max compression
```

## Comparing `sql_field_report-0.1.5.tar` & `sql_field_report-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      676 2023-04-27 15:21:47.585955 sql_field_report-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.5/sql_field_report/__init__.py
--rw-r--r--   0        0        0       68 2023-04-27 13:15:20.467845 sql_field_report-0.1.5/sql_field_report/__main__.py
--rw-r--r--   0        0        0    11751 2023-04-27 15:21:41.034351 sql_field_report-0.1.5/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 sql_field_report-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      676 2023-06-09 14:51:18.367339 sql_field_report-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.6/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-27 13:15:20.467845 sql_field_report-0.1.6/sql_field_report/__main__.py
+-rw-r--r--   0        0        0    11846 2023-06-09 14:51:10.524401 sql_field_report-0.1.6/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 sql_field_report-0.1.6/PKG-INFO
```

### Comparing `sql_field_report-0.1.5/pyproject.toml` & `sql_field_report-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `sql_field_report-0.1.5/README.md` & `sql_field_report-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.1.5/sql_field_report/sql_field_report.py` & `sql_field_report-0.1.6/sql_field_report/sql_field_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,18 +188,20 @@
 
     Params:
     str: table - the database table to query
 
     Returns:
     Tuple: file_shape - a tuple of tuples containing the file name, field name, row count for each field
     """
+    try:
+        data = pd.read_sql(text(f"SELECT * FROM [{schema}].[{table}]"), conn)
 
-    data = pd.read_sql(text(f"SELECT * FROM [{schema}].[{table}]"), conn)
-
-    file_shape = tuple((review_column(table, data, h) for h in data.columns))
+        file_shape = tuple((review_column(table, data, h) for h in data.columns))
+    except:
+        file_shape = tuple(((table, 'ERROR', 0, 0, 0, 'ERROR')))
 
     return file_shape
 
 
 def analyze_files(objects: list, schema:str, conn) -> pd.DataFrame:
     """
     Analyze Files
```

### Comparing `sql_field_report-0.1.5/PKG-INFO` & `sql_field_report-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```

