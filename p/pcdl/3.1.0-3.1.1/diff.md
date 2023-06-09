# Comparing `tmp/pcdl-3.1.0.tar.gz` & `tmp/pcdl-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdl-3.1.0.tar", last modified: Fri Jun  9 08:19:36 2023, max compression
+gzip compressed data, was "pcdl-3.1.1.tar", last modified: Fri Jun  9 08:26:59 2023, max compression
```

## Comparing `pcdl-3.1.0.tar` & `pcdl-3.1.1.tar`

### file list

```diff
@@ -1,22 +1,189 @@
-drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:19:36.514130 pcdl-3.1.0/
--rw-rw-r--   0 bue       (1000) bue       (1000)     1523 2023-06-09 03:35:20.000000 pcdl-3.1.0/LICENSE
--rw-rw-r--   0 bue       (1000) bue       (1000)    11305 2023-06-09 08:19:36.514130 pcdl-3.1.0/PKG-INFO
--rw-rw-r--   0 bue       (1000) bue       (1000)     8438 2023-06-09 05:59:46.000000 pcdl-3.1.0/README.md
-drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:19:36.514130 pcdl-3.1.0/pcdl/
--rw-rw-r--   0 bue       (1000) bue       (1000)      242 2023-06-09 05:29:32.000000 pcdl-3.1.0/pcdl/__init__.py
--rw-rw-r--   0 bue       (1000) bue       (1000)     3952 2023-06-09 03:35:21.000000 pcdl-3.1.0/pcdl/pdplt.py
--rw-rw-r--   0 bue       (1000) bue       (1000)    51788 2023-06-09 03:35:21.000000 pcdl-3.1.0/pcdl/pyMCDS.py
--rw-rw-r--   0 bue       (1000) bue       (1000)    18951 2023-06-09 03:35:21.000000 pcdl-3.1.0/pcdl/pyMCDSts.py
-drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:19:36.514130 pcdl-3.1.0/pcdl.egg-info/
--rw-rw-r--   0 bue       (1000) bue       (1000)    11305 2023-06-09 08:19:36.000000 pcdl-3.1.0/pcdl.egg-info/PKG-INFO
--rw-rw-r--   0 bue       (1000) bue       (1000)      347 2023-06-09 08:19:36.000000 pcdl-3.1.0/pcdl.egg-info/SOURCES.txt
--rw-rw-r--   0 bue       (1000) bue       (1000)        1 2023-06-09 08:19:36.000000 pcdl-3.1.0/pcdl.egg-info/dependency_links.txt
--rw-rw-r--   0 bue       (1000) bue       (1000)       30 2023-06-09 08:19:36.000000 pcdl-3.1.0/pcdl.egg-info/requires.txt
--rw-rw-r--   0 bue       (1000) bue       (1000)        5 2023-06-09 08:19:36.000000 pcdl-3.1.0/pcdl.egg-info/top_level.txt
--rw-rw-r--   0 bue       (1000) bue       (1000)     4350 2023-06-09 08:18:59.000000 pcdl-3.1.0/pyproject.toml
--rw-rw-r--   0 bue       (1000) bue       (1000)       38 2023-06-09 08:19:36.514130 pcdl-3.1.0/setup.cfg
-drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:19:36.514130 pcdl-3.1.0/test/
--rw-rw-r--   0 bue       (1000) bue       (1000)    12490 2023-06-09 06:35:11.000000 pcdl-3.1.0/test/test_snapshot_2d.py
--rw-rw-r--   0 bue       (1000) bue       (1000)    13190 2023-06-09 06:36:22.000000 pcdl-3.1.0/test/test_snapshot_3d.py
--rw-rw-r--   0 bue       (1000) bue       (1000)     8016 2023-06-09 06:37:22.000000 pcdl-3.1.0/test/test_snapshot_3d_microenvfalse.py
--rw-rw-r--   0 bue       (1000) bue       (1000)     4159 2023-06-09 06:38:29.000000 pcdl-3.1.0/test/test_timeseries.py
+drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:26:59.459508 pcdl-3.1.1/
+-rw-rw-r--   0 bue       (1000) bue       (1000)     1523 2023-06-09 03:35:20.000000 pcdl-3.1.1/LICENSE
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11305 2023-06-09 08:26:59.459508 pcdl-3.1.1/PKG-INFO
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8438 2023-06-09 05:59:46.000000 pcdl-3.1.1/README.md
+drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:26:59.387507 pcdl-3.1.1/pcdl/
+-rw-rw-r--   0 bue       (1000) bue       (1000)      242 2023-06-09 05:29:32.000000 pcdl-3.1.1/pcdl/__init__.py
+drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:26:59.459508 pcdl-3.1.1/pcdl/data_timeseries_2d/
+-rw-rw-r--   0 bue       (1000) bue       (1000)      568 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/ALL_CITATIONS.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    13208 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/PhysiCell_settings.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)   313850 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/final.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8239 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/final.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6597 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/final_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    17815 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/final_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   685801 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/final_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/final_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)   254328 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8243 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5223 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5223 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   554761 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     3896 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial_mesh0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/initial_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)      725 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/legend.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8271 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000000.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5223 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000000_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5223 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000000_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   554761 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000000_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000000_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8272 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000001.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5277 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000001_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    10443 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000001_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   560377 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000001_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000001_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8273 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000002.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5319 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000002_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    10669 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000002_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   564745 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000002_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000002_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8273 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000003.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5379 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000003_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    10877 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000003_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   570985 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000003_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000003_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8273 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000004.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5415 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000004_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11006 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000004_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   574729 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000004_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000004_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8273 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000005.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5445 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000005_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11118 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000005_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   577849 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000005_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000005_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8273 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000006.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5487 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000006_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11322 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000006_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   582217 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000006_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000006_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8273 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000007.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5529 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000007_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11561 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000007_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   586585 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000007_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000007_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000008.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5607 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000008_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11949 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000008_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   594697 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000008_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000008_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000009.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5673 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000009_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    12262 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000009_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   601561 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000009_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000009_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000010.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5733 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000010_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    12613 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000010_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   607801 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000010_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000010_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000011.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5805 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000011_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    13003 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000011_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   615289 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000011_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000011_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000012.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5841 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000012_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    13228 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000012_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   619033 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000012_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000012_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000013.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5899 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000013_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    13468 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000013_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   624649 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000013_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000013_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000014.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     5983 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000014_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    13994 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000014_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   632137 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000014_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000014_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000015.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6004 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000015_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    14046 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000015_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   634009 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000015_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000015_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8274 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000016.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6069 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000016_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    14441 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000016_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   639625 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000016_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000016_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000017.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6105 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000017_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    14602 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000017_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   642745 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000017_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000017_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000018.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6197 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000018_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    15119 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000018_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   650857 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000018_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000018_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000019.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6256 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000019_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    15489 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000019_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   655849 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000019_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000019_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000020.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6319 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000020_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    15921 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000020_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   661465 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000020_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000020_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000021.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6369 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000021_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    16246 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000021_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   665833 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000021_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000021_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000022.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6419 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000022_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    16633 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000022_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   670201 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000022_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000022_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000023.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6483 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000023_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    16918 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000023_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   675817 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000023_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000023_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8275 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000024.xml
+-rw-rw-r--   0 bue       (1000) bue       (1000)     6597 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000024_attached_cells_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)    17808 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000024_cell_neighbor_graph.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)   685801 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000024_cells.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4887 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/output00000024_microenvironment0.mat
+-rw-rw-r--   0 bue       (1000) bue       (1000)   254328 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000000.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   257071 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000001.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   259013 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000002.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   261847 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000003.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   263541 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000004.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   264942 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000005.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   266956 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000006.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   268880 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000007.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   272540 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000008.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   275696 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000009.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   278516 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000010.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   281847 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000011.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   283560 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000012.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   286112 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000013.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   289482 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000014.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   290340 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000015.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   292888 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000016.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   294281 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000017.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   298014 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000018.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   300295 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000019.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   302842 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000020.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   304767 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000021.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   306732 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000022.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   309307 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000023.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)   313853 2023-06-09 03:35:20.000000 pcdl-3.1.1/pcdl/data_timeseries_2d/snapshot00000024.svg
+-rw-rw-r--   0 bue       (1000) bue       (1000)     3952 2023-06-09 03:35:21.000000 pcdl-3.1.1/pcdl/pdplt.py
+-rw-rw-r--   0 bue       (1000) bue       (1000)    51788 2023-06-09 03:35:21.000000 pcdl-3.1.1/pcdl/pyMCDS.py
+-rw-rw-r--   0 bue       (1000) bue       (1000)    18951 2023-06-09 03:35:21.000000 pcdl-3.1.1/pcdl/pyMCDSts.py
+drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:26:59.387507 pcdl-3.1.1/pcdl.egg-info/
+-rw-rw-r--   0 bue       (1000) bue       (1000)    11305 2023-06-09 08:26:59.000000 pcdl-3.1.1/pcdl.egg-info/PKG-INFO
+-rw-rw-r--   0 bue       (1000) bue       (1000)     9188 2023-06-09 08:26:59.000000 pcdl-3.1.1/pcdl.egg-info/SOURCES.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)        1 2023-06-09 08:26:59.000000 pcdl-3.1.1/pcdl.egg-info/dependency_links.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)       30 2023-06-09 08:26:59.000000 pcdl-3.1.1/pcdl.egg-info/requires.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)        5 2023-06-09 08:26:59.000000 pcdl-3.1.1/pcdl.egg-info/top_level.txt
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4344 2023-06-09 08:25:55.000000 pcdl-3.1.1/pyproject.toml
+-rw-rw-r--   0 bue       (1000) bue       (1000)       38 2023-06-09 08:26:59.459508 pcdl-3.1.1/setup.cfg
+drwxrwxr-x   0 bue       (1000) bue       (1000)        0 2023-06-09 08:26:59.459508 pcdl-3.1.1/test/
+-rw-rw-r--   0 bue       (1000) bue       (1000)    12490 2023-06-09 06:35:11.000000 pcdl-3.1.1/test/test_snapshot_2d.py
+-rw-rw-r--   0 bue       (1000) bue       (1000)    13190 2023-06-09 06:36:22.000000 pcdl-3.1.1/test/test_snapshot_3d.py
+-rw-rw-r--   0 bue       (1000) bue       (1000)     8016 2023-06-09 06:37:22.000000 pcdl-3.1.1/test/test_snapshot_3d_microenvfalse.py
+-rw-rw-r--   0 bue       (1000) bue       (1000)     4159 2023-06-09 06:38:29.000000 pcdl-3.1.1/test/test_timeseries.py
```

### Comparing `pcdl-3.1.0/LICENSE` & `pcdl-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/PKG-INFO` & `pcdl-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdl
-Version: 3.1.0
+Version: 3.1.1
 Summary: physicell data loader (pcdl) provides a platform independent, python3 based, pip installable interface to load output, generated with the PhysiCell agent based modeling framework, into python3.
 Author-email: Elmar Bucher <epbucher@iu.edu>
 Maintainer-email: Elmar Bucher <epbucher@iu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, PhysiCell-Tools
         All rights reserved.
```

### Comparing `pcdl-3.1.0/README.md` & `pcdl-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/pcdl/pdplt.py` & `pcdl-3.1.1/pcdl/pdplt.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/pcdl/pyMCDS.py` & `pcdl-3.1.1/pcdl/pyMCDS.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/pcdl/pyMCDSts.py` & `pcdl-3.1.1/pcdl/pyMCDSts.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/pcdl.egg-info/PKG-INFO` & `pcdl-3.1.1/pcdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdl
-Version: 3.1.0
+Version: 3.1.1
 Summary: physicell data loader (pcdl) provides a platform independent, python3 based, pip installable interface to load output, generated with the PhysiCell agent based modeling framework, into python3.
 Author-email: Elmar Bucher <epbucher@iu.edu>
 Maintainer-email: Elmar Bucher <epbucher@iu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, PhysiCell-Tools
         All rights reserved.
```

### Comparing `pcdl-3.1.0/pyproject.toml` & `pcdl-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [project]
 # name of the project
 # pip install pcdl
 # import pcdl
 name = "pcdl"  # Required
 
 # version
-version = "3.1.0" # Required
+version = "3.1.1" # Required
 
 # tag
 description = "physicell data loader (pcdl) provides a platform independent, python3 based, pip installable interface to load output, generated with the PhysiCell agent based modeling framework, into python3."  # Optional
 readme = "README.md" # Optional
 
 # python version
 requires-python = ">=3.6"  # >=3.6, <4
@@ -108,23 +108,23 @@
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 #package-data = {"data_timeseries_2d"=["*.mat", "*.svg", "*.txt", "*.xml"], "data_timeseries_3d"=["*.mat", "*.svg", "*.txt", "*.xml"]}
-#package-data = {"pcdl"=[
-#    "data_timeseries_2d/*.mat", 
-#    "data_timeseries_2d/*.svg", 
-#    "data_timeseries_2d/*.txt", 
-#    "data_timeseries_2d/*.xml", 
+package-data = {"pcdl"=[
+    "data_timeseries_2d/*.mat", 
+    "data_timeseries_2d/*.svg", 
+    "data_timeseries_2d/*.txt", 
+    "data_timeseries_2d/*.xml", 
 #    "data_timeseries_3d/*.mat", 
 #    "data_timeseries_3d/*.svg", 
 #    "data_timeseries_3d/*.txt", 
 #    "data_timeseries_3d/*.xml",
-#]}
+]}
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pcdl-3.1.0/test/test_snapshot_2d.py` & `pcdl-3.1.1/test/test_snapshot_2d.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/test/test_snapshot_3d.py` & `pcdl-3.1.1/test/test_snapshot_3d.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/test/test_snapshot_3d_microenvfalse.py` & `pcdl-3.1.1/test/test_snapshot_3d_microenvfalse.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.0/test/test_timeseries.py` & `pcdl-3.1.1/test/test_timeseries.py`

 * *Files identical despite different names*

