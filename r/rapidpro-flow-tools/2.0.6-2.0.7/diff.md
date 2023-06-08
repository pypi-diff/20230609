# Comparing `tmp/rapidpro_flow_tools-2.0.6.tar.gz` & `tmp/rapidpro_flow_tools-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-2.0.6.tar", last modified: Thu Jun  8 23:20:18 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-2.0.7.tar", last modified: Thu Jun  8 23:24:04 2023, max compression
```

## Comparing `rapidpro_flow_tools-2.0.6.tar` & `rapidpro_flow_tools-2.0.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.207959 rapidpro_flow_tools-2.0.6/
--rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.6/LICENSE
--rw-rw-rw-   0        0        0      289 2023-06-08 23:20:18.207959 rapidpro_flow_tools-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.6/README.md
--rw-rw-rw-   0        0        0      111 2023-06-08 23:20:18.214493 rapidpro_flow_tools-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      401 2023-06-08 23:20:10.000000 rapidpro_flow_tools-2.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.054590 rapidpro_flow_tools-2.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.080587 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/
--rw-rw-rw-   0        0        0        0 2023-06-08 23:14:31.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/__init__.py
--rw-rw-rw-   0        0        0     1849 2023-06-08 11:11:36.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/flow_converter.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.103591 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/logger/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/logger/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.105590 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.113949 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4419 2023-06-08 11:37:50.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-06-08 11:16:47.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15982 2023-06-08 11:20:14.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     2170 2023-06-08 11:37:26.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.133949 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      932 2023-06-08 21:43:07.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      620 2023-06-08 21:41:58.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6120 2023-06-08 21:42:50.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3608 2023-06-08 21:44:30.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5106 2023-06-08 21:45:10.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3110 2023-06-08 21:46:04.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2122 2023-06-08 21:46:40.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4744 2023-06-08 21:47:09.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.148950 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     8434 2023-06-08 11:39:21.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      952 2023-06-08 11:39:45.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      122 2023-06-08 12:03:50.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    28243 2023-06-08 12:05:35.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5437 2023-06-08 12:05:47.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1076 2023-06-08 12:06:00.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.162952 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1441 2023-06-08 21:52:03.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17206 2023-06-08 21:53:32.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    40755 2023-06-08 21:56:00.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    15088 2023-06-08 21:57:47.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.169964 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3495 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.173959 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.186963 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/
--rw-rw-rw-   0        0        0        0 2023-06-08 23:19:57.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/__init__.py
--rw-rw-rw-   0        0        0    13287 2023-06-08 12:14:45.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/actions.py
--rw-rw-rw-   0        0        0     1024 2023-06-08 21:26:56.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/common.py
--rw-rw-rw-   0        0        0    11011 2023-06-08 21:27:16.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/containers.py
--rw-rw-rw-   0        0        0      112 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/exceptions.py
--rw-rw-rw-   0        0        0    20909 2023-06-08 21:27:46.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/nodes.py
--rw-rw-rw-   0        0        0    18813 2023-06-08 21:28:12.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/routers.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.197962 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      562 2023-06-08 21:34:59.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3533 2023-06-08 21:35:13.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4625 2023-06-08 21:35:26.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1344 2023-06-08 21:35:46.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6388 2023-06-08 21:35:59.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.100591 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0      289 2023-06-08 23:20:17.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3446 2023-06-08 23:20:18.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:20:17.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-08 23:20:17.000000 rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 23:20:18.206967 rapidpro_flow_tools-2.0.6/tests/
--rw-rw-rw-   0        0        0     2194 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.6/tests/test_template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.119842 rapidpro_flow_tools-2.0.7/
+-rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0      289 2023-06-08 23:24:04.120845 rapidpro_flow_tools-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-2.0.7/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-08 23:24:04.127845 rapidpro_flow_tools-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-06-08 23:23:54.000000 rapidpro_flow_tools-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:03.997756 rapidpro_flow_tools-2.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.020754 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-08 23:14:31.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1849 2023-06-08 11:11:36.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.037284 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/logger/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/logger/__init__.py
+-rw-rw-rw-   0        0        0     2426 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.038314 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.046311 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4419 2023-06-08 11:37:50.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-06-08 11:16:47.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15982 2023-06-08 11:20:14.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     2170 2023-06-08 11:37:26.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.062309 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      932 2023-06-08 21:43:07.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      620 2023-06-08 21:41:58.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6120 2023-06-08 21:42:50.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3608 2023-06-08 21:44:30.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5106 2023-06-08 21:45:10.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3110 2023-06-08 21:46:04.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2122 2023-06-08 21:46:40.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4744 2023-06-08 21:47:09.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.074324 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     8434 2023-06-08 11:39:21.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      952 2023-06-08 11:39:45.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      122 2023-06-08 12:03:50.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    28243 2023-06-08 12:05:35.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5437 2023-06-08 12:05:47.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1076 2023-06-08 12:06:00.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.085324 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1441 2023-06-08 21:52:03.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17206 2023-06-08 21:53:32.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    40755 2023-06-08 21:56:00.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    15088 2023-06-08 21:57:47.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.090845 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3147 2023-06-08 23:22:46.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.092844 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.103845 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/
+-rw-rw-rw-   0        0        0        0 2023-06-08 23:19:57.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/__init__.py
+-rw-rw-rw-   0        0        0    13287 2023-06-08 12:14:45.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/actions.py
+-rw-rw-rw-   0        0        0     1024 2023-06-08 21:26:56.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/common.py
+-rw-rw-rw-   0        0        0    11011 2023-06-08 21:27:16.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/containers.py
+-rw-rw-rw-   0        0        0      112 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/exceptions.py
+-rw-rw-rw-   0        0        0    20909 2023-06-08 21:27:46.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/nodes.py
+-rw-rw-rw-   0        0        0    18813 2023-06-08 21:28:12.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/routers.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.112844 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-06-08 21:34:59.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3533 2023-06-08 21:35:13.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4625 2023-06-08 21:35:26.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1344 2023-06-08 21:35:46.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6388 2023-06-08 21:35:59.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.034753 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-06-08 23:24:03.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3446 2023-06-08 23:24:03.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 23:24:03.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-08 23:24:03.000000 rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 23:24:04.118843 rapidpro_flow_tools-2.0.7/tests/
+-rw-rw-rw-   0        0        0     2194 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-06-08 11:04:15.000000 rapidpro_flow_tools-2.0.7/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-2.0.6/LICENSE` & `rapidpro_flow_tools-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/README.md` & `rapidpro_flow_tools-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/flow_converter.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/flow_converter.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/logger/logger.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/cellparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/rowparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/sheetparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/models.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/flowparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 import tablib
 from googleapiclient.discovery import build
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 import os
 
-class GoogleSheetReader:
 
-    # If modifying these scopes, delete the file token.json.
+class GoogleSheetReader:
     SCOPES = ['https://www.googleapis.com/auth/spreadsheets.readonly']
 
-    def __init__(self, spreadsheet_id):
+    def __init__(self, spreadsheet_id, credentials_file=None, token_file=None):
         '''
         Args:
-            spreadsheet_id: You can extract it from the spreadsheed URL, like this
-            https://docs.google.com/spreadsheets/d/[spreadsheet_id]/edit
+            spreadsheet_id: You can extract it from the spreadsheet URL, like this:
+                            https://docs.google.com/spreadsheets/d/[spreadsheet_id]/edit
+            credentials_file: Dictionary representing the contents of the 'credentials.json' file (default: None)
+            token_file: Dictionary representing the contents of the 'token.json' file (default: None)
         '''
-
-        # Authentication code nabbed from
-        # https://developers.google.com/sheets/api/quickstart/python
         creds = None
-        # The file token.json stores the user's access and refresh tokens, and is
-        # created automatically when the authorization flow completes for the first
-        # time.
-        if os.path.exists('token.json'):
-            creds = Credentials.from_authorized_user_file('token.json', GoogleSheetReader.SCOPES)
-        # If there are no (valid) credentials available, let the user log in.
+
+        if token_file is not None:
+            creds = Credentials.from_authorized_user_info(token_file, GoogleSheetReader.SCOPES)
+
         if not creds or not creds.valid:
             if creds and creds.expired and creds.refresh_token:
                 creds.refresh(Request())
             else:
-                # TODO: Provide instructions how to obtain this file and get access
-                flow = InstalledAppFlow.from_client_secrets_file(
-                    'credentials.json', GoogleSheetReader.SCOPES)
+                flow = InstalledAppFlow.from_client_config(credentials_file, GoogleSheetReader.SCOPES)
                 creds = flow.run_local_server(port=0)
-            # Save the credentials for the next run
+
             with open('token.json', 'w') as token:
                 token.write(creds.to_json())
+
         service = build('sheets', 'v4', credentials=creds)
 
+
         # Call the Sheets API
         sheet_metadata = service.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
         sheets = sheet_metadata.get('sheets', '')
         titles = []
+
         for sheet in sheets:
             title = sheet.get("properties", {}).get("title", "Sheet1")
             titles.append(title)
 
-        result = service.spreadsheets().values().batchGet(
-                spreadsheetId=spreadsheet_id, ranges=titles).execute()
+        result = service.spreadsheets().values().batchGet(spreadsheetId=spreadsheet_id, ranges=titles).execute()
 
         self.main_sheet = None
         self.sheets = {}
+
         for sheet in result.get('valueRanges', []):
             name = sheet.get('range', '').split('!')[0]
             if name.startswith("'") and name.endswith("'"):
                 name = name[1:-1]
             content = sheet.get('values', [])
             if name == 'content_index':
                 self.main_sheet = self._table_from_content(content)
@@ -76,8 +73,8 @@
             table.append(row + ([''] * (n_headers - len(row))))
         return table
 
     def get_main_sheet(self):
         return self.main_sheet
 
     def get_sheet(self, name):
-        return self.sheets[name]
+        return self.sheets[name]
```

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/actions.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/common.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/common.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/containers.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/nodes.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/models/routers.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/models/routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/src/rapidpro_flow_tools.egg-info/SOURCES.txt` & `rapidpro_flow_tools-2.0.7/src/rapidpro_flow_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/tests/test_contentindexparser.py` & `rapidpro_flow_tools-2.0.7/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/tests/test_flowparser.py` & `rapidpro_flow_tools-2.0.7/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-2.0.7/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-2.0.6/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-2.0.7/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

