# Comparing `tmp/rapidpro_flow_tools-2.0.4.tar.gz` & `tmp/rapidpro_flow_tools-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-2.0.4.tar", last modified: Thu Jun  8 22:09:45 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-2.0.5.tar", last modified: Thu Jun  8 23:15:08 2023, max compression
```

## Comparing `rapidpro_flow_tools-2.0.4.tar` & `rapidpro_flow_tools-2.0.5.tar`

### file list

```diff
@@ -1,17 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.383658 rapidpro_flow_tools-2.0.4/
--rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.4/LICENSE
--rw-rw-rw-   0        0        0      289 2023-06-08 22:09:45.384655 rapidpro_flow_tools-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.4/README.md
--rw-rw-rw-   0        0        0      111 2023-06-08 22:09:45.389666 rapidpro_flow_tools-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      401 2023-06-08 11:26:53.000000 rapidpro_flow_tools-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.283107 rapidpro_flow_tools-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.322111 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0      289 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.382661 rapidpro_flow_tools-2.0.4/tests/
--rw-rw-rw-   0        0        0     2194 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.083281 rapidpro_flow_tools-2.0.5/
+-rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0      289 2023-06-08 23:15:08.084281 rapidpro_flow_tools-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.5/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-08 23:15:08.086286 rapidpro_flow_tools-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-06-08 23:14:34.000000 rapidpro_flow_tools-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:07.941557 rapidpro_flow_tools-2.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:07.965546 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-08 23:14:31.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1849 2023-06-08 11:11:36.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:07.991555 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/logger/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/logger/__init__.py
+-rw-rw-rw-   0        0        0     2426 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:07.993546 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.003552 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4419 2023-06-08 11:37:50.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-06-08 11:16:47.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15982 2023-06-08 11:20:14.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     2170 2023-06-08 11:37:26.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.023555 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      932 2023-06-08 21:43:07.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      620 2023-06-08 21:41:58.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6120 2023-06-08 21:42:50.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3608 2023-06-08 21:44:30.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5106 2023-06-08 21:45:10.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3110 2023-06-08 21:46:04.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2122 2023-06-08 21:46:40.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4744 2023-06-08 21:47:09.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.039281 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     8434 2023-06-08 11:39:21.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      952 2023-06-08 11:39:45.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      122 2023-06-08 12:03:50.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    28243 2023-06-08 12:05:35.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5437 2023-06-08 12:05:47.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1076 2023-06-08 12:06:00.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.053282 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1441 2023-06-08 21:52:03.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17206 2023-06-08 21:53:32.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    40755 2023-06-08 21:56:00.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    15088 2023-06-08 21:57:47.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.059286 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3495 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.064290 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.074287 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-06-08 21:34:59.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3533 2023-06-08 21:35:13.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4625 2023-06-08 21:35:26.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1344 2023-06-08 21:35:46.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6388 2023-06-08 21:35:59.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:07.988561 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-06-08 23:15:07.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3085 2023-06-08 23:15:07.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 23:15:07.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-08 23:15:07.000000 rapidpro_flow_tools-2.0.5/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 23:15:08.082284 rapidpro_flow_tools-2.0.5/tests/
+-rw-rw-rw-   0        0        0     2194 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.5/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-2.0.4/LICENSE` & `rapidpro_flow_tools-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.4/README.md` & `rapidpro_flow_tools-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.4/tests/test_contentindexparser.py` & `rapidpro_flow_tools-2.0.5/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.4/tests/test_flowparser.py` & `rapidpro_flow_tools-2.0.5/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.4/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-2.0.5/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.4/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-2.0.5/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

