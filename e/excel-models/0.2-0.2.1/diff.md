# Comparing `tmp/excel-models-0.2.tar.gz` & `tmp/excel-models-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-models-0.2.tar", last modified: Fri Jun  2 18:01:14 2023, max compression
+gzip compressed data, was "excel-models-0.2.1.tar", last modified: Thu Jun  8 22:01:26 2023, max compression
```

## Comparing `excel-models-0.2.tar` & `excel-models-0.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.333166 excel-models-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-02 18:01:07.000000 excel-models-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 18:01:14.333166 excel-models-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-02 18:01:07.000000 excel-models-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/column_inst/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/remainder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/columns/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/basic_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/collection_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/models/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/models/_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/_inst.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/assignable_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/class_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/validators/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/validators/comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:01:14.333166 excel-models-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-02 18:01:04.000000 excel-models-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.333166 excel-models-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_cell_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_cell_access_many.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_cell_access_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_custom_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_custom_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_model_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_open_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.118219 excel-models-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-08 22:01:18.000000 excel-models-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:01:26.118219 excel-models-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-08 22:01:18.000000 excel-models-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.110219 excel-models-0.2.1/excel_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/column_inst/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/remainder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/basic_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/collection_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/models/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/_inst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/assignable_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/class_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/validators/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/validators/comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:01:26.118219 excel-models-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-08 22:01:12.000000 excel-models-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.118219 excel-models-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_cell_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_cell_access_many.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_cell_access_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_custom_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_custom_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_model_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_open_modes.py
```

### Comparing `excel-models-0.2/LICENSE` & `excel-models-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/PKG-INFO` & `excel-models-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-models
-Version: 0.2
+Version: 0.2.1
 Summary: Model-style Excel File Accessor
 Home-page: https://github.com/MichaelKim0407/excel-models
 Author: Zheng Jin
 Author-email: mkim0407@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `excel-models-0.2/README.md` & `excel-models-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/column_inst/_base.py` & `excel-models-0.2.1/excel_models/column_inst/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/column_inst/_std.py` & `excel-models-0.2.1/excel_models/column_inst/_std.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/column_inst/array.py` & `excel-models-0.2.1/excel_models/column_inst/array.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/column_inst/map.py` & `excel-models-0.2.1/excel_models/column_inst/map.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/column_inst/remainder.py` & `excel-models-0.2.1/excel_models/column_inst/remainder.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/columns/_base.py` & `excel-models-0.2.1/excel_models/columns/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/columns/_std.py` & `excel-models-0.2.1/excel_models/columns/_std.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/columns/basic_types.py` & `excel-models-0.2.1/excel_models/columns/basic_types.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/columns/collection_types.py` & `excel-models-0.2.1/excel_models/columns/collection_types.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/columns/multi.py` & `excel-models-0.2.1/excel_models/columns/multi.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/db.py` & `excel-models-0.2.1/excel_models/db.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/models/_base.py` & `excel-models-0.2.1/excel_models/models/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/tables/_base.py` & `excel-models-0.2.1/excel_models/tables/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class BaseExcelTableDefinition(
     BasePropertyDescriptor[TDB],
     AbstractTableDefinition,
 ):
     table_class: typing.Type[TTable]  # assign in subclass
     title_row: int = 1
+    trim_by_title: bool = False
     trim: bool = False
 
     def _add_to_class(self):
         super()._add_to_class()
         self.obj_type.tables.append(self)
 
     def make_table(self, db: TDB, ws: Worksheet) -> TTable:
@@ -40,14 +41,16 @@
         self._f_initialize = f_initialize
         return self
 
     def _get_default(self, db: TDB) -> TTable:
         if self.name in db.wb:
             ws = db.wb[self.name]
             table = self.make_table(db, ws)
+            if self.trim_by_title:
+                table.trim_cols(use_title_row=True)
             if self.trim:
                 table.trim()
             table.find_columns()
         else:
             ws = db.wb.create_sheet(self.name)
             table = self.make_table(db, ws)
             table.init_columns()
```

### Comparing `excel-models-0.2/excel_models/tables/_inst.py` & `excel-models-0.2.1/excel_models/tables/_inst.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,17 +221,32 @@
         while col > 0:
             for cell in self.col(col):
                 if cell.value is not None:
                     return col
             col -= 1
         return col
 
-    def trim_cols(self) -> int:
+    @property
+    def _max_title_col(self) -> int:
+        col = 0
+        for cell in self.row(self.title_row):
+            if cell.value is not None:
+                col = max(col, cell.column)
+        return col
+
+    def trim_cols(
+            self,
+            *,
+            use_title_row: bool = False,
+    ) -> int:
         max_col = self.max_col
-        col = self._max_notnone_col
+        if use_title_row:
+            col = self._max_title_col
+        else:
+            col = self._max_notnone_col
         if col == max_col:
             return col
         self.ws.delete_cols(col + 1, max_col - col)
         return col
 
     @property
     def _max_notnone_row(self) -> int:
```

### Comparing `excel-models-0.2/excel_models/typing.py` & `excel-models-0.2.1/excel_models/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,19 @@
             max_row: int = None,
             data_only: bool = False,
     ) -> typing.Sequence[Cell]:
         raise NotImplementedError  # pragma: no cover
 
     # --- utils ---
 
-    def trim_cols(self) -> int:
+    def trim_cols(
+            self,
+            *,
+            use_title_row: bool = False,
+    ) -> int:
         raise NotImplementedError  # pragma: no cover
 
     def trim_rows(self) -> int:
         raise NotImplementedError  # pragma: no cover
 
     def trim(self) -> tuple[int, int]:
         raise NotImplementedError  # pragma: no cover
```

### Comparing `excel-models-0.2/excel_models/utils/class_collector.py` & `excel-models-0.2.1/excel_models/utils/class_collector.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/utils/descriptors.py` & `excel-models-0.2.1/excel_models/utils/descriptors.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/validators/_base.py` & `excel-models-0.2.1/excel_models/validators/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models/validators/comparisons.py` & `excel-models-0.2.1/excel_models/validators/comparisons.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/excel_models.egg-info/PKG-INFO` & `excel-models-0.2.1/excel_models.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-models
-Version: 0.2
+Version: 0.2.1
 Summary: Model-style Excel File Accessor
 Home-page: https://github.com/MichaelKim0407/excel-models
 Author: Zheng Jin
 Author-email: mkim0407@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `excel-models-0.2/excel_models.egg-info/SOURCES.txt` & `excel-models-0.2.1/excel_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/setup.py` & `excel-models-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_alias.py` & `excel-models-0.2.1/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_caching.py` & `excel-models-0.2.1/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_cell_access.py` & `excel-models-0.2.1/tests/test_cell_access.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_cell_access_many.py` & `excel-models-0.2.1/tests/test_cell_access_many.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_cell_access_raw.py` & `excel-models-0.2.1/tests/test_cell_access_raw.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_custom_column.py` & `excel-models-0.2.1/tests/test_custom_column.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_custom_table.py` & `excel-models-0.2.1/tests/test_custom_table.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_eq.py` & `excel-models-0.2.1/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_model_inheritance.py` & `excel-models-0.2.1/tests/test_model_inheritance.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_new.py` & `excel-models-0.2.1/tests/test_new.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2/tests/test_open_modes.py` & `excel-models-0.2.1/tests/test_open_modes.py`

 * *Files identical despite different names*

