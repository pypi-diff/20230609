# Comparing `tmp/dbt-spark-1.6.0b2.tar.gz` & `tmp/dbt-spark-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.6.0b2.tar", last modified: Thu May 25 20:00:18 2023, max compression
+gzip compressed data, was "dbt-spark-1.6.0b3.tar", last modified: Fri Jun  9 01:08:22 2023, max compression
```

## Comparing `dbt-spark-1.6.0b2.tar` & `dbt-spark-1.6.0b3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.755314 dbt-spark-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:00:18.755314 dbt-spark-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.078732 dbt-spark-1.6.0b3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.078732 dbt-spark-1.6.0b3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.078732 dbt-spark-1.6.0b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/setup.py
```

### Comparing `dbt-spark-1.6.0b2/PKG-INFO` & `dbt-spark-1.6.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ODBC
 Provides-Extra: PyHive
 Provides-Extra: session
 Provides-Extra: all
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b2 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b3 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: ODBC Provides-Extra:
-PyHive Provides-Extra: session Provides-Extra: all
+Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+ODBC Provides-Extra: PyHive Provides-Extra: session Provides-Extra: all
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-spark The `dbt-spark` package contains all of the
```

### Comparing `dbt-spark-1.6.0b2/README.md` & `dbt-spark-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/adapters/spark/column.py` & `dbt-spark-1.6.0b3/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/adapters/spark/connections.py` & `dbt-spark-1.6.0b3/dbt/adapters/spark/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import contextmanager
+from typing import Tuple
 
 import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import ConnectionState, AdapterResponse
 from dbt.events import AdapterLogger
 from dbt.utils import DECIMALS
@@ -143,15 +144,15 @@
     def type(self):
         return "spark"
 
     @property
     def unique_field(self):
         return self.host
 
-    def _connection_keys(self):
+    def _connection_keys(self) -> Tuple[str, ...]:
         return ("host", "port", "cluster", "endpoint", "schema", "organization")
 
 
 class PyhiveConnectionWrapper(object):
     """Wrap a Spark connection in a way that no-ops transactions"""
 
     # https://forums.databricks.com/questions/2157/in-apache-spark-sql-can-we-roll-back-the-transacti.html  # noqa
```

### Comparing `dbt-spark-1.6.0b2/dbt/adapters/spark/impl.py` & `dbt-spark-1.6.0b3/dbt/adapters/spark/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,14 +473,18 @@
             if object_type == "TABLE" and privilege != "OWN":
                 if privilege in grants_dict.keys():
                     grants_dict[privilege].append(grantee)
                 else:
                     grants_dict.update({privilege: [grantee]})
         return grants_dict
 
+    def debug_query(self):
+        """Override for DebugTask method"""
+        self.execute("select 1 as id")
+
 
 # spark does something interesting with joins when both tables have the same
 # static values for the join condition and complains that the join condition is
 # "trivial". Which is true, though it seems like an unreasonable cause for
 # failure! It also doesn't like the `from foo, bar` syntax as opposed to
 # `from foo cross join bar`.
 COLUMNS_EQUAL_SQL = """
```

### Comparing `dbt-spark-1.6.0b2/dbt/adapters/spark/python_submissions.py` & `dbt-spark-1.6.0b3/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/adapters/spark/relation.py` & `dbt-spark-1.6.0b3/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/adapters/spark/session.py` & `dbt-spark-1.6.0b3/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/adapters.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 {% endmacro %}
 
 {% macro spark__alter_table_add_constraints(relation, constraints) %}
   {% for constraint in constraints %}
     {% if constraint.type == 'check' and not is_incremental() %}
       {%- set constraint_hash = local_md5(column_name ~ ";" ~ constraint.expression ~ ";" ~ loop.index) -%}
       {% call statement() %}
-        alter table {{ relation }} add constraint {{ constraint.name if constraint.name else constraint_hash }} check {{ constraint.expression }};
+        alter table {{ relation }} add constraint {{ constraint.name if constraint.name else constraint_hash }} check ({{ constraint.expression }});
       {% endcall %}
     {% endif %}
   {% endfor %}
 {% endmacro %}
 
 {% macro alter_column_set_constraints(relation, column_dict) %}
   {{ return(adapter.dispatch('alter_column_set_constraints', 'dbt')(relation, column_dict)) }}
```

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/apply_grants.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/seed.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/table.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/dateadd.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/datediff.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/listagg.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/split_part.sql` & `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt/include/spark/profile_template.yml` & `dbt-spark-1.6.0b3/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/dbt_spark.egg-info/PKG-INFO` & `dbt-spark-1.6.0b3/dbt_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ODBC
 Provides-Extra: PyHive
 Provides-Extra: session
 Provides-Extra: all
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b2 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b3 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: ODBC Provides-Extra:
-PyHive Provides-Extra: session Provides-Extra: all
+Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+ODBC Provides-Extra: PyHive Provides-Extra: session Provides-Extra: all
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-spark The `dbt-spark` package contains all of the
```

### Comparing `dbt-spark-1.6.0b2/dbt_spark.egg-info/SOURCES.txt` & `dbt-spark-1.6.0b3/dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b2/setup.py` & `dbt-spark-1.6.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 import os
 import sys
 import re
 
-# require python 3.7 or newer
-if sys.version_info < (3, 7):
+# require python 3.8 or newer
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-spark"
-package_version = "1.6.0b2"
+package_version = "1.6.0b3"
 dbt_core_version = _get_dbt_core_version()
 description = """The Apache Spark adapter plugin for dbt"""
 
 odbc_extras = ["pyodbc~=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
@@ -86,14 +86,13 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

