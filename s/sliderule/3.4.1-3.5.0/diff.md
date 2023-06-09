# Comparing `tmp/sliderule-3.4.1.tar.gz` & `tmp/sliderule-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.4.1.tar", last modified: Thu Jun  1 15:18:13 2023, max compression
+gzip compressed data, was "sliderule-3.5.0.tar", last modified: Fri Jun  9 17:43:39 2023, max compression
```

## Comparing `sliderule-3.4.1.tar` & `sliderule-3.5.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.337535 sliderule-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-01 15:17:57.000000 sliderule-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-01 15:17:57.000000 sliderule-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-01 15:18:13.337535 sliderule-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-01 15:17:57.000000 sliderule-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-01 15:17:57.000000 sliderule-3.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 15:18:13.337535 sliderule-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-01 15:17:57.000000 sliderule-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.333534 sliderule-3.4.1/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29288 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    34861 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    45777 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-01 15:17:57.000000 sliderule-3.4.1/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.333534 sliderule-3.4.1/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-01 15:18:13.000000 sliderule-3.4.1/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 15:18:13.337535 sliderule-3.4.1/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_3dep_DEM_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-06-01 15:17:57.000000 sliderule-3.4.1/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-01 15:17:57.000000 sliderule-3.4.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-09 17:43:27.000000 sliderule-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-09 17:43:27.000000 sliderule-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-09 17:43:39.936906 sliderule-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-09 17:43:27.000000 sliderule-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-09 17:43:27.000000 sliderule-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 17:43:39.936906 sliderule-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-09 17:43:27.000000 sliderule-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30629 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17363 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34802 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45769 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/swot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_3dep_DEM_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6260 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-09 17:43:27.000000 sliderule-3.5.0/version.txt
```

### Comparing `sliderule-3.4.1/LICENSE` & `sliderule-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/PKG-INFO` & `sliderule-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.4.1
+Version: 3.5.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.4.1/README.md` & `sliderule-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/setup.py` & `sliderule-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/sliderule/earthdata.py` & `sliderule-3.5.0/sliderule/earthdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,25 +51,27 @@
 
 # default maximum number of resources to process in one request
 DEFAULT_MAX_REQUESTED_RESOURCES = 300
 max_requested_resources = DEFAULT_MAX_REQUESTED_RESOURCES
 
 # best effort match of datasets to providers and versions for earthdata
 DATASETS = {
-    "ATL03":                                    {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "collections": [] },
-    "ATL06":                                    {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "collections": []},
-    "ATL08":                                    {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "collections": []},
-    "GEDI01_B":                                 {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "collections": []},
-    "GEDI02_A":                                 {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "collections": []},
-    "GEDI02_B":                                 {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "collections": []},
-    "GEDI_L3_LandSurface_Metrics_V2_1952":      {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "collections": []},
-    "GEDI_L4A_AGB_Density_V2_1_2056":           {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "collections": []},
-    "GEDI_L4B_Gridded_Biomass_2017":            {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "collections": []},
-    "HLS":                                      {"provider": "LPCLOUD",     "version": None,   "api": "stac",  "collections": ["HLSS30.v2.0", "HLSL30.v2.0"]},
-    "Digital Elevation Model (DEM) 1 meter":    {"provider": "USGS",        "version": None,   "api": "tnm",   "collections": []}
+    "ATL03":                                               {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "formats": [".h5"],    "collections": [] },
+    "ATL06":                                               {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "ATL08":                                               {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "GEDI01_B":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "GEDI02_A":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "GEDI02_B":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".tiff"],  "collections": []},
+    "GEDI_L3_LandSurface_Metrics_V2_1952":                 {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "GEDI_L4A_AGB_Density_V2_1_2056":                      {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "GEDI_L4B_Gridded_Biomass_2017":                       {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".tiff"],  "collections": []},
+    "HLS":                                                 {"provider": "LPCLOUD",     "version": None,   "api": "stac",  "formats": [".tiff"],  "collections": ["HLSS30.v2.0", "HLSL30.v2.0"]},
+    "Digital Elevation Model (DEM) 1 meter":               {"provider": "USGS",        "version": None,   "api": "tnm",   "formats": [".tiff"],  "collections": []},
+    "SWOT_SIMULATED_L2_KARIN_SSH_ECCO_LLC4320_CALVAL_V1":  {"provider": "POCLOUD",     "version": None,   "api": "cmr",   "formats": [".nc"],    "collections": ["C2147947806-POCLOUD"]},
+    "SWOT_SIMULATED_L2_KARIN_SSH_GLORYS_CALVAL_V1":        {"provider": "POCLOUD",     "version": None,   "api": "cmr",   "formats": [".nc"],    "collections": ["C2152046451-POCLOUD"]}
 }
 
 # upper limit on resources returned from CMR query per request
 CMR_PAGE_SIZE = 2000
 
 # upper limit on resources returned from STAC query per request
 STAC_PAGE_SIZE = 100
@@ -89,15 +91,15 @@
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
 # The above copyright notice and this permission notice shall be included
 # in all copies or substantial portions of the Software.
 
-def __cmr_filter_urls(search_results):
+def __cmr_filter_urls(search_results, data_formats):
     """Select only the desired data files from CMR response."""
     if 'feed' not in search_results or 'entry' not in search_results['feed']:
         return []
     entries = [e['links']
                for e in search_results['feed']['entry']
                if 'links' in e]
     # Flatten "entries" to a simple list of links
@@ -121,15 +123,15 @@
             # non-datapool links, we should be able to do this in a non-hack way
             continue
         filename = link['href'].split('/')[-1]
         if filename in unique_filenames:
             # Exclude links with duplicate filenames (they would overwrite)
             continue
         unique_filenames.add(filename)
-        if ".h5" in link['href'][-3:]:
+        if any([extension in link['href'] for extension in data_formats]):
             resource = link['href'].split("/")[-1]
             urls.append(resource)
     # return filtered urls
     return urls
 
 def __cmr_granule_metadata(search_results):
     """Get the metadata for CMR returned granules"""
@@ -181,15 +183,16 @@
     kwargs.setdefault('polygon',None)
     kwargs.setdefault('name_filter',None)
     kwargs.setdefault('return_metadata',False)
     # build params
     params = '&short_name={0}'.format(short_name)
     if version != None:
         params += '&version={0}'.format(version)
-    params += '&temporal[]={0},{1}'.format(time_start, time_end)
+    if time_start != None and time_end != None:
+        params += '&temporal[]={0},{1}'.format(time_start, time_end)
     if kwargs['polygon']:
         params += '&polygon={0}'.format(kwargs['polygon'])
     if kwargs['name_filter']:
         params += '&options[producer_granule_id][pattern]=true'
         params += '&producer_granule_id[]=' + kwargs['name_filter']
     CMR_URL = 'https://cmr.earthdata.nasa.gov'
     cmr_query_url = ('{0}/search/granules.json?provider={1}'
@@ -213,15 +216,15 @@
         response = urllib.request.urlopen(req, context=ctx)
         if not cmr_scroll_id:
             # Python 2 and 3 have different case for the http headers
             headers = {k.lower(): v for k, v in dict(response.info()).items()}
             cmr_scroll_id = headers['cmr-scroll-id']
         search_page = response.read()
         search_page = json.loads(search_page.decode('utf-8'))
-        url_scroll_results = __cmr_filter_urls(search_page)
+        url_scroll_results = __cmr_filter_urls(search_page, DATASETS[short_name]["formats"])
         if not url_scroll_results:
             break
         urls += url_scroll_results
         # query for granule metadata and polygons
         if kwargs['return_metadata']:
             metadata_results = __cmr_granule_metadata(search_page)
         else:
@@ -236,14 +239,16 @@
 ###############################################################################
 
 #
 # Perform a CMR Search Request
 #
 def __cmr_search(provider, short_name, version, polygons, time_start, time_end, return_metadata, name_filter):
 
+    global max_requested_resources
+
     # initialize return value
     resources = {} # [<url>] = <polygon>
 
     # iterate through each polygon (or none if none supplied)
     for polygon in polygons:
         urls = []
         metadata = sliderule.emptyframe()
@@ -290,14 +295,20 @@
         for i,url, in enumerate(urls):
             resources[url] = metadata.iloc[i]
 
     # build return lists
     url_list = list(resources.keys())
     meta_list = list(resources.values())
 
+    # Check Resources are Under Limit
+    if(len(url_list) > max_requested_resources):
+        raise sliderule.FatalError('Exceeded maximum requested resources: {} (current max is {})\nConsider using earthdata.set_max_resources to set a higher limit.'.format(len(url_list), max_requested_resources))
+    else:
+        logger.info("Identified %d resources to process", len(url_list))
+
     if return_metadata:
         return (url_list,meta_list)
     else:
         return url_list
 
 #
 # Build a GeoJSON Response from STAC Query Response
@@ -567,15 +578,17 @@
     provider = __get_provider(short_name)
 
     # check collections
     if collections == None:
         collections = DATASETS[short_name]["collections"]
 
     # create list of polygons
-    polygons = __format_polygons(polygon)
+    polygons = None
+    if polygon:
+        polygons = __format_polygons(polygon)
 
     # perform query
     geojson = __stac_search(provider, short_name, collections, polygons, time_start, time_end)
 
     # return
     if as_str:
         return json.dumps(geojson)
```

### Comparing `sliderule-3.4.1/sliderule/gedi.py` & `sliderule-3.5.0/sliderule/gedi.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ###############################################################################
 # LOCAL FUNCTIONS
 ###############################################################################
 
 #
 # Flatten Batches
 #
-def __flattenbatches(rsps, rectype, batch_column, parm, keep_id):
+def __flattenbatches(rsps, rectype, batch_column, parm, keep_id, as_numpy_array):
 
     # Latch Start Time
     tstart_flatten = time.perf_counter()
 
     # Check for Output Options
     if "output" in parm:
         gdf = sliderule.procoutputfile(parm)
@@ -89,15 +89,14 @@
                 if rsp["num_samples"] <= 0:
                     continue
                 # Get field names and set
                 sample = rsp["samples"][0]
                 field_names = list(sample.keys())
                 field_names.remove("__rectype")
                 field_set = rsp['key']
-                as_numpy_array = False
                 if rsp["num_samples"] > 1:
                     as_numpy_array = True
                 # On first time, build empty dictionary for field set associated with raster
                 if field_set not in field_dictionary:
                     field_dictionary[field_set] = {'shot_number': []}
                     for field in field_names:
                         field_dictionary[field_set][field_set + "." + field] = []
@@ -187,33 +186,27 @@
 
     # Make CMR Request
     if kwargs['return_metadata']:
         resources,metadata = earthdata.cmr(short_name=dataset, **kwargs)
     else:
         resources = earthdata.cmr(short_name=dataset, **kwargs)
 
-    # Check Resources are Under Limit
-    if(len(resources) > earthdata.max_requested_resources):
-        raise sliderule.FatalError('Exceeded maximum requested granules: {} (current max is {})\nConsider using icesat2.set_max_resources to set a higher limit.'.format(len(resources), earthdata.max_requested_resources))
-    else:
-        logger.info("Identified %d resources to process", len(resources))
-
     # Update Profile
     profiles[__query_resources.__name__] = time.perf_counter() - tstart
 
     # Return Resources
     if kwargs['return_metadata']:
         return (resources,metadata)
     else:
         return resources
 
 #
 #  Perform Processing Request
 #
-def __processing_request(parm, asset, callbacks, resources, keep_id, dataset, api, rec, profile):
+def __processing_request(parm, asset, callbacks, resources, keep_id, as_numpy_array, dataset, api, rec, profile):
     try:
         tstart = time.perf_counter()
 
         # Get List of Resources from CMR (if not supplied)
         if resources == None:
             resources = __query_resources(parm, dataset)
 
@@ -224,15 +217,15 @@
             "parms": parm
         }
 
         # Make API Processing Request
         rsps = sliderule.source(api, rqst, stream=True, callbacks=callbacks)
 
         # Flatten Responses
-        gdf = __flattenbatches(rsps, rec, 'footprint', parm, keep_id)
+        gdf = __flattenbatches(rsps, rec, 'footprint', parm, keep_id, as_numpy_array)
 
         # Return Response
         profiles[profile] = time.perf_counter() - tstart
         return gdf
 
     # Handle Runtime Errors
     except RuntimeError as e:
@@ -242,31 +235,25 @@
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
 #
-def init (url=sliderule.service_url, verbose=False, max_resources=earthdata.DEFAULT_MAX_REQUESTED_RESOURCES, loglevel=logging.CRITICAL, organization=sliderule.service_org, desired_nodes=None, time_to_live=60, bypass_dns=False):
+def init (url=sliderule.service_url, verbose=False, loglevel=logging.CRITICAL, organization=sliderule.service_org, desired_nodes=None, time_to_live=60, bypass_dns=False):
     '''
     Initializes the Python client for use with SlideRule and should be called before other GEDI API calls.
     This function is a wrapper for the `sliderule.init(...) function </web/rtds/api_reference/sliderule.html#init>`_.
 
-    Parameters
-    ----------
-        max_resources:  int
-                        maximum number of H5 granules to process in the request
-
     Examples
     --------
         >>> from sliderule import gedi
         >>> gedi.init()
     '''
     sliderule.init(url, verbose, loglevel, organization, desired_nodes, time_to_live, bypass_dns, plugins=['gedi'])
-    earthdata.set_max_resources(max_resources) # set maximum number of resources allowed per request
 
 #
 #  GEDI L4A
 #
 def gedi04a (parm, resource, asset=DEFAULT_L4A_ASSET):
     '''
     Performs GEDI L4A subsetting of elevation footprints
@@ -286,15 +273,15 @@
         gridded footrpints
     '''
     return gedi04ap(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel GEDI04A
 #
-def gedi04ap(parm, asset=DEFAULT_L4A_ASSET, callbacks={}, resources=None, keep_id=False):
+def gedi04ap(parm, asset=DEFAULT_L4A_ASSET, callbacks={}, resources=None, keep_id=False, as_numpy_array=False):
     '''
     Performs subsetting in parallel on GEDI data and returns elevation footprints.  This function expects that the **parm** argument
     includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
     then any polygon or resource filtering options supplied in **parm** are ignored.
 
     Parameters
     ----------
@@ -304,14 +291,16 @@
                         data source asset
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
+        as_numpy_array: bool
+                        whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
     GeoDataFrame
         geolocated footprints
 
     Examples
@@ -324,15 +313,15 @@
         ...            {"lon":-105.82971551223244, "lat": 40.164048017973755},
         ...            {"lon":-105.82971551223244, "lat": 39.81983728534918} ]
         >>> parms = { "poly": region }
         >>> resources = ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5"]
         >>> asset = "ornldaac-s3"
         >>> rsps = gedi.gedi04ap(parms, asset=asset, resources=resources)
     '''
-    return __processing_request(parm, asset, callbacks, resources, keep_id, 'GEDI_L4A_AGB_Density_V2_1_2056', 'gedi04ap', 'gedi04arec', gedi04ap.__name__)
+    return __processing_request(parm, asset, callbacks, resources, keep_id, as_numpy_array, 'GEDI_L4A_AGB_Density_V2_1_2056', 'gedi04ap', 'gedi04arec', gedi04ap.__name__)
 
 #
 #  GEDI L2A
 #
 def gedi02a (parm, resource, asset=DEFAULT_L2A_ASSET):
     '''
     Performs GEDI L2A subsetting of elevation footprints
@@ -352,15 +341,15 @@
         gridded footrpints
     '''
     return gedi02ap(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel GEDI02A
 #
-def gedi02ap(parm, asset=DEFAULT_L2A_ASSET, callbacks={}, resources=None, keep_id=False):
+def gedi02ap(parm, asset=DEFAULT_L2A_ASSET, callbacks={}, resources=None, keep_id=False, as_numpy_array=False):
     '''
     Performs subsetting in parallel on GEDI data and returns geolocated footprints.  This function expects that the **parm** argument
     includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
     then any polygon or resource filtering options supplied in **parm** are ignored.
 
     Parameters
     ----------
@@ -370,14 +359,16 @@
                         data source asset
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
+        as_numpy_array: bool
+                        whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
     GeoDataFrame
         geolocated footprints
 
     Examples
@@ -390,15 +381,15 @@
         ...            {"lon":-105.82971551223244, "lat": 40.164048017973755},
         ...            {"lon":-105.82971551223244, "lat": 39.81983728534918} ]
         >>> parms = { "poly": region }
         >>> resources = ["GEDI02_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5"]
         >>> asset = "gedi-local"
         >>> rsps = gedi.gedi02ap(parms, asset=asset, resources=resources)
     '''
-    return __processing_request(parm, asset, callbacks, resources, keep_id, 'GEDI02_A', 'gedi02ap', 'gedi02arec', gedi02ap.__name__)
+    return __processing_request(parm, asset, callbacks, resources, keep_id, as_numpy_array, 'GEDI02_A', 'gedi02ap', 'gedi02arec', gedi02ap.__name__)
 
 #
 #  GEDI L1B
 #
 def gedi01b (parm, resource, asset=DEFAULT_L1B_ASSET):
     '''
     Performs GEDI L1B subsetting of elevation waveforms
@@ -418,15 +409,15 @@
         gridded footrpints
     '''
     return gedi01bp(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel GEDI01B
 #
-def gedi01bp(parm, asset=DEFAULT_L1B_ASSET, callbacks={}, resources=None, keep_id=False):
+def gedi01bp(parm, asset=DEFAULT_L1B_ASSET, callbacks={}, resources=None, keep_id=False, as_numpy_array=False):
     '''
     Performs subsetting in parallel on GEDI data and returns geolocated footprints.  This function expects that the **parm** argument
     includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
     then any polygon or resource filtering options supplied in **parm** are ignored.
 
     Parameters
     ----------
@@ -436,14 +427,16 @@
                         data source asset
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
+        as_numpy_array: bool
+                        whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
     GeoDataFrame
         geolocated footprints
 
     Examples
@@ -456,8 +449,8 @@
         ...            {"lon":-105.82971551223244, "lat": 40.164048017973755},
         ...            {"lon":-105.82971551223244, "lat": 39.81983728534918} ]
         >>> parms = { "poly": region }
         >>> resources = ["GEDI01_B_2019229131935_O03846_02_T03642_02_002_02_V002.h5"]
         >>> asset = "gedi-local"
         >>> rsps = gedi.gedi01bp(parms, asset=asset, resources=resources)
     '''
-    return __processing_request(parm, asset, callbacks, resources, keep_id, 'GEDI01_B', 'gedi01bp', 'gedi01brec', gedi01bp.__name__)
+    return __processing_request(parm, asset, callbacks, resources, keep_id, as_numpy_array, 'GEDI01_B', 'gedi01bp', 'gedi01brec', gedi01bp.__name__)
```

### Comparing `sliderule-3.4.1/sliderule/h5.py` & `sliderule-3.5.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/sliderule/icesat2.py` & `sliderule-3.5.0/sliderule/icesat2.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     # unknown spot
     return 0
 
 #
 # Flatten Batches
 #
-def __flattenbatches(rsps, rectype, batch_column, parm, keep_id):
+def __flattenbatches(rsps, rectype, batch_column, parm, keep_id, as_numpy_array):
 
     # Latch Start Time
     tstart_flatten = time.perf_counter()
 
     # Check for Output Options
     if "output" in parm:
         gdf = sliderule.procoutputfile(parm)
@@ -178,15 +178,14 @@
                 if rsp["num_samples"] <= 0:
                     continue
                 # Get field names and set
                 sample = rsp["samples"][0]
                 field_names = list(sample.keys())
                 field_names.remove("__rectype")
                 field_set = rsp['key']
-                as_numpy_array = False
                 if rsp["num_samples"] > 1:
                     as_numpy_array = True
                 # On first time, build empty dictionary for field set associated with raster
                 if field_set not in field_dictionary:
                     field_dictionary[field_set] = {'extent_id': []}
                     for field in field_names:
                         field_dictionary[field_set][field_set + "." + field] = []
@@ -308,20 +307,14 @@
 
     # Make CMR Request
     if kwargs['return_metadata']:
         resources,metadata = earthdata.cmr(short_name='ATL03', version=version, **kwargs)
     else:
         resources = earthdata.cmr(short_name='ATL03', version=version, **kwargs)
 
-    # Check Resources are Under Limit
-    if(len(resources) > earthdata.max_requested_resources):
-        raise sliderule.FatalError('Exceeded maximum requested granules: {} (current max is {})\nConsider using cmr.set_max_resources to set a higher limit.'.format(len(resources), earthdata.max_requested_resources))
-    else:
-        logger.info("Identified %d resources to process", len(resources))
-
     # Update Profile
     profiles[__query_resources.__name__] = time.perf_counter() - tstart
 
     # Return Resources
     if kwargs['return_metadata']:
         return (resources,metadata)
     else:
@@ -375,15 +368,15 @@
         geolocated elevations (see `Elevations </web/rtd/user_guide/ICESat-2.html#elevations>`_)
     '''
     return atl06p(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel ATL06
 #
-def atl06p(parm, asset=DEFAULT_ASSET, version=DEFAULT_ICESAT2_SDP_VERSION, callbacks={}, resources=None, keep_id=False):
+def atl06p(parm, asset=DEFAULT_ASSET, version=DEFAULT_ICESAT2_SDP_VERSION, callbacks={}, resources=None, keep_id=False, as_numpy_array=False):
     '''
     Performs ATL06-SR processing in parallel on ATL03 data and returns geolocated elevations.  This function expects that the **parm** argument
     includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
     then any polygon or resource filtering options supplied in **parm** are ignored.
 
     Warnings
     --------
@@ -402,14 +395,16 @@
                         the version of the ATL03 data to use for processing
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
+        as_numpy_array: bool
+                        whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
     GeoDataFrame
         geolocated elevations (see `Elevations </web/rtd/user_guide/ICESat-2.html#elevations>`_)
 
     Examples
@@ -450,15 +445,15 @@
             "parms": parm
         }
 
         # Make API Processing Request
         rsps = sliderule.source("atl06p", rqst, stream=True, callbacks=callbacks)
 
         # Flatten Responses
-        gdf = __flattenbatches(rsps, 'atl06rec', 'elevation', parm, keep_id)
+        gdf = __flattenbatches(rsps, 'atl06rec', 'elevation', parm, keep_id, as_numpy_array)
 
         # Return Response
         profiles[atl06p.__name__] = time.perf_counter() - tstart
         return gdf
 
     # Handle Runtime Errors
     except RuntimeError as e:
@@ -695,15 +690,15 @@
         geolocated vegatation statistics
     '''
     return atl08p(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel ATL08
 #
-def atl08p(parm, asset=DEFAULT_ASSET, version=DEFAULT_ICESAT2_SDP_VERSION, callbacks={}, resources=None, keep_id=False):
+def atl08p(parm, asset=DEFAULT_ASSET, version=DEFAULT_ICESAT2_SDP_VERSION, callbacks={}, resources=None, keep_id=False, as_numpy_array=False):
     '''
     Performs ATL08-PhoREAL processing in parallel on ATL03 and ATL08 data and returns geolocated vegatation statistics.  This function expects that the **parm** argument
     includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
     then any polygon or resource filtering options supplied in **parm** are ignored.
 
     Warnings
     --------
@@ -722,14 +717,16 @@
                         the version of the ATL03 data to use for processing
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
+        as_numpy_array: bool
+                        whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
     GeoDataFrame
         geolocated vegetation statistics
     '''
     try:
@@ -746,15 +743,15 @@
             "parms": parm
         }
 
         # Make API Processing Request
         rsps = sliderule.source("atl08p", rqst, stream=True, callbacks=callbacks)
 
         # Flatten Responses
-        gdf = __flattenbatches(rsps, 'atl08rec', 'vegetation', parm, keep_id)
+        gdf = __flattenbatches(rsps, 'atl08rec', 'vegetation', parm, keep_id, as_numpy_array)
 
         # Return Response
         profiles[atl08p.__name__] = time.perf_counter() - tstart
         return gdf
 
     # Handle Runtime Errors
     except RuntimeError as e:
```

### Comparing `sliderule-3.4.1/sliderule/io.py` & `sliderule-3.5.0/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/sliderule/ipxapi.py` & `sliderule-3.5.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/sliderule/ipysliderule.py` & `sliderule-3.5.0/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/sliderule/raster.py` & `sliderule-3.5.0/sliderule/raster.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/sliderule/sliderule.py` & `sliderule-3.5.0/sliderule/sliderule.py`

 * *Files 0% similar despite different names*

```diff
@@ -881,22 +881,22 @@
                 host = "https://ps." + service_url + "/api/desired_org_num_nodes/" + service_org + "/" + str(requested_nodes) + "/"
                 rsps = session.put(host, headers=headers, timeout=request_timeout)
             rsps_body = rsps.json()
             rsps.raise_for_status()
         except requests.exceptions.HTTPError as e:
             logger.info('{}'.format(e))
             logger.error('Provisioning system update request error => {}'.format(rsps_body["error_msg"]))
-    
+
     # Get number of nodes currently registered
     try:
         rsps = source("status", parm={"service":"sliderule"}, path="/discovery", silence=True)
         available_servers = rsps["nodes"]
     except FatalError:
         available_servers = 0
-    
+
     return available_servers, requested_nodes
 
 #
 # scaleout
 #
 def scaleout(desired_nodes, time_to_live, bypass_dns):
     '''
```

### Comparing `sliderule-3.4.1/sliderule.egg-info/PKG-INFO` & `sliderule-3.5.0/sliderule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.4.1
+Version: 3.5.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.4.1/sliderule.egg-info/SOURCES.txt` & `sliderule-3.5.0/sliderule.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 sliderule/h5.py
 sliderule/icesat2.py
 sliderule/io.py
 sliderule/ipxapi.py
 sliderule/ipysliderule.py
 sliderule/raster.py
 sliderule/sliderule.py
+sliderule/swot.py
 sliderule/version.py
 sliderule.egg-info/PKG-INFO
 sliderule.egg-info/SOURCES.txt
 sliderule.egg-info/dependency_links.txt
 sliderule.egg-info/requires.txt
 sliderule.egg-info/top_level.txt
 utils/big_query.py
```

### Comparing `sliderule-3.4.1/utils/big_query.py` & `sliderule-3.5.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/build_3dep_DEM_geojson.py` & `sliderule-3.5.0/utils/build_3dep_DEM_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.5.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.5.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.5.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/extract_h5_dataset.py` & `sliderule-3.5.0/utils/extract_h5_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 # Uses the icesat2.h5p api to read a dataset from an H5 file and write the contents to a file
 #
 
 import sys
-from sliderule import icesat2
+from sliderule import h5
 from utils import parse_command_line, initialize_client
 
 ###############################################################################
 # MAIN
 ###############################################################################
 
 if __name__ == '__main__':
@@ -24,15 +24,15 @@
     parms, cfg = initialize_client(sys.argv)
 
     # parse configuration parameters
     parse_command_line(sys.argv, local)
 
     # Read Dataset #
     datasets = [ {"dataset": local["dataset"], "col": local["col"], "startrow": local["startrow"], "numrows": local["numrows"]} ]
-    rawdata = icesat2.h5p(datasets, cfg["resource"], cfg["asset"])
+    rawdata = h5.h5p(datasets, cfg["resource"], cfg["asset"])
     print(rawdata)
 
     # Write Dataset to File #
     filename = local["dataset"][local["dataset"].rfind("/")+1:]
     f = open(filename + ".bin", 'w+b')
     f.write(bytearray(rawdata[local["dataset"]]))
     f.close()
```

### Comparing `sliderule-3.4.1/utils/icepyx_region.py` & `sliderule-3.5.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/lpdaac_download.py` & `sliderule-3.5.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/monitor.py` & `sliderule-3.5.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/query_cmr.py` & `sliderule-3.5.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/query_elevations.py` & `sliderule-3.5.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/query_metrics.py` & `sliderule-3.5.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/query_photons.py` & `sliderule-3.5.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/query_stac.py` & `sliderule-3.5.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/query_version.py` & `sliderule-3.5.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/region_of_interest.py` & `sliderule-3.5.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/results_to_s3.py` & `sliderule-3.5.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/stac.py` & `sliderule-3.5.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/stream_events.py` & `sliderule-3.5.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/tail_events.py` & `sliderule-3.5.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.4.1/utils/utils.py` & `sliderule-3.5.0/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     global tstart
 
     # Set Script Defaults
     cfg = {
         "domain":                   'localhost',
         "organization":             None,
         "asset":                    'atlas-local',
-        "region":                   'examples/grandmesa.geojson',
+        "region":                   None,
         "resource":                 'ATL03_20181017222812_02950102_005_01.h5',
         "raster":                   True,
         "atl08_class":              [],
         "yapc.score":               0,
         "yapc.knn":                 0,
         "yapc.min_knn":             5,
         "yapc.win_h":               6.0,
```

