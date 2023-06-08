# Comparing `tmp/rapidpro_flow_tools-2.0.3.tar.gz` & `tmp/rapidpro_flow_tools-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-2.0.3.tar", last modified: Tue May 30 18:14:56 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-2.0.4.tar", last modified: Thu Jun  8 22:09:45 2023, max compression
```

## Comparing `rapidpro_flow_tools-2.0.3.tar` & `rapidpro_flow_tools-2.0.4.tar`

### file list

```diff
@@ -1,85 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.412505 rapidpro_flow_tools-2.0.3/
--rw-rw-rw-   0        0        0      242 2023-05-30 18:14:56.413501 rapidpro_flow_tools-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/README.md
--rw-rw-rw-   0        0        0      115 2023-05-30 18:14:56.419570 rapidpro_flow_tools-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-05-30 18:14:28.000000 rapidpro_flow_tools-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.274309 rapidpro_flow_tools-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.290005 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/__init__.py
--rw-rw-rw-   0        0        0     1851 2023-05-30 17:56:29.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/flow_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.307544 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.314544 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1883 2023-05-24 04:48:55.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.331607 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.345166 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7156 2023-05-24 04:49:46.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      952 2023-05-24 03:59:15.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      122 2023-05-24 03:59:21.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26861 2023-05-24 04:52:23.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5262 2023-05-24 03:59:53.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1076 2023-05-24 04:00:05.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.355862 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.371397 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3149 2023-05-30 18:14:20.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.373397 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.381395 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/
--rw-rw-rw-   0        0        0        0 2023-05-24 04:27:06.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/__init__.py
--rw-rw-rw-   0        0        0    11748 2023-05-24 04:30:12.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/actions.py
--rw-rw-rw-   0        0        0     1024 2023-05-24 04:30:28.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/common.py
--rw-rw-rw-   0        0        0    11011 2023-05-24 04:30:44.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/containers.py
--rw-rw-rw-   0        0        0    20909 2023-05-24 04:31:04.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/nodes.py
--rw-rw-rw-   0        0        0    18813 2023-05-24 04:53:20.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/models/routers.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.394933 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.405514 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.305548 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0      242 2023-05-30 18:14:56.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3604 2023-05-30 18:14:56.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:14:56.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-30 18:14:56.000000 rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 18:14:56.411503 rapidpro_flow_tools-2.0.3/tests/
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.3/tests/test_template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.383658 rapidpro_flow_tools-2.0.4/
+-rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0      289 2023-06-08 22:09:45.384655 rapidpro_flow_tools-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.4/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-08 22:09:45.389666 rapidpro_flow_tools-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-06-08 11:26:53.000000 rapidpro_flow_tools-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.283107 rapidpro_flow_tools-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.322111 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 22:09:45.000000 rapidpro_flow_tools-2.0.4/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 22:09:45.382661 rapidpro_flow_tools-2.0.4/tests/
+-rw-rw-rw-   0        0        0     2194 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.4/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-2.0.3/README.md` & `rapidpro_flow_tools-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_contentindexparser.py` & `rapidpro_flow_tools-2.0.4/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_flowparser.py` & `rapidpro_flow_tools-2.0.4/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-2.0.4/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.3/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-2.0.4/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

