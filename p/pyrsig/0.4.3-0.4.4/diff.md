# Comparing `tmp/pyrsig-0.4.3.tar.gz` & `tmp/pyrsig-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.4.3.tar", last modified: Wed Jun  7 12:44:27 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.4.4.tar", last modified: Fri Jun  9 15:49:01 2023, max compression
```

## Comparing `pyrsig-0.4.3.tar` & `pyrsig-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.3/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-07 12:44:27.000000 pyrsig-0.4.3/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.3/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-07 12:44:27.000000 pyrsig-0.4.3/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.3/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.3/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3182 2023-06-07 12:10:43.000000 pyrsig-0.4.3/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.3/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2774 2023-06-07 12:09:56.000000 pyrsig-0.4.3/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.3/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.3/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)    48873 2023-06-07 12:29:16.000000 pyrsig-0.4.3/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-07 12:44:27.000000 pyrsig-0.4.3/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.3/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.4/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-09 15:49:01.000000 pyrsig-0.4.4/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.4/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.4/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.4/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3182 2023-06-07 12:10:43.000000 pyrsig-0.4.4/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.4/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3129 2023-06-08 20:39:38.000000 pyrsig-0.4.4/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.4/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.4/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    50427 2023-06-08 20:40:23.000000 pyrsig-0.4.4/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-09 15:49:01.000000 pyrsig-0.4.4/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.4/README.md
```

### Comparing `pyrsig-0.4.3/setup.py` & `pyrsig-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.3/PKG-INFO` & `pyrsig-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.3/LICENSE` & `pyrsig-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.3/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.4.4/pyrsig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.3/pyrsig/tests/test_api.py` & `pyrsig-0.4.4/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.3/pyrsig/tests/test_ioapi.py` & `pyrsig-0.4.4/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.3/pyrsig/tests/test_dataframes.py` & `pyrsig-0.4.4/pyrsig/tests/test_dataframes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+def test_pandora():
+    from .. import RsigApi
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as td:
+        rsigapi = RsigApi(
+            bdate='2023-03-01', bbox=(-80, 30, -60, 50), workdir=td
+        )
+        ds = rsigapi.to_dataframe(
+            'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide'
+        )
+        print(ds.shape)
+
+
 def test_viirsnoaa():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
             bdate='2022-03-01', bbox=(-85, 30, -70, 45), workdir=td
```

### Comparing `pyrsig-0.4.3/pyrsig/tests/test_coards.py` & `pyrsig-0.4.4/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.3/pyrsig/tests/test_gui.py` & `pyrsig-0.4.4/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.3/pyrsig/__init__.py` & `pyrsig-0.4.4/pyrsig/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['RsigApi', 'RsigGui', 'open_ioapi']
-__version__ = '0.4.3'
+__version__ = '0.4.4'
 
 import pandas as pd
 
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
@@ -62,14 +62,16 @@
     A=50., T0=290, P0=1000e2, REGRID_AGGREGATE='None'
 )
 
 for key in _def_grid_kw:
     for pk, pv in _shared_grid_kw.items():
         _def_grid_kw[key].setdefault(pk, pv)
 
+# Used to shorten pandora names for 80 character PEP
+_trvca = 'tropospheric_vertical_column_amount'
 
 _keys = (
     'airnow.pm25', 'airnow.pm10', 'airnow.ozone', 'airnow.no', 'airnow.no2',
     'airnow.nox', 'airnow.so2', 'airnow.co', 'airnow.temperature',
     'airnow.pressure', 'airnow.rh', 'airnow2.pm25', 'airnow2.ozone',
     'airnow2.no2', 'airnow2.so2', 'airnow2.co',
     'aqs.pm25', 'aqs.pm25_daily_average', 'aqs.pm25_daily_filter', 'aqs.pm10',
@@ -84,15 +86,38 @@
     'metar.temperature', 'metar.dewpoint', 'metar.relativeHumidity',
     'metar.windDir', 'metar.windSpeed', 'metar.windGustSpeed', 'metar.wind',
     'metar.altimeter', 'metar.minTemp24Hour', 'metar.maxTemp24Hour',
     'metar.precip1Hour', 'metar.precip3Hour', 'metar.precip6Hour',
     'metar.precip24Hour', 'metar.pressChange3Hour', 'metar.snowCover'
     'nesdis.pm25', 'nesdis.co', 'nesdis.co2', 'nesdis.ch4', 'nesdis.n2o',
     'nesdis.nh3', 'nesdis.nox', 'nesdis.so2', 'nesdis.tnmhc',
-    'pandora.ozone', 'purpleair.pm25_corrected',
+    'pandora.ozone'
+    f'pandora.L2_rfuh5p1_8.formaldehyde_{_trvca}',
+    f'pandora.L2_rfuh5p1_8.formaldehyde_{_trvca}_uncertainty',
+    'pandora.L2_rfus5p1_8.direct_formaldehyde_air_mass_factor',
+    'pandora.L2_rfus5p1_8.direct_formaldehyde_air_mass_factor_uncertainty',
+    'pandora.L2_rfus5p1_8.formaldehyde_total_vertical_column_amount',
+    'pandora.L2_rfus5p1_8.formaldehyde_vertical_column_amount_uncertainty'
+    f'pandora.L2_rnvh3p1_8.water_vapor_{_trvca}',
+    f'pandora.L2_rnvh3p1_8.water_vapor_{_trvca}_uncertainty',
+    'pandora.L2_rnvs3p1_8.nitrogen_dioxide_vertical_column_amount',
+    'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide',
+    'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide_uncertainty',
+    'pandora.L2_rnvs3p1_8.direct_nitrogen_dioxide_air_mass_factor',
+    'pandora.L2_rnvs3p1_8.direct_nitrogen_dioxide_air_mass_factor_uncertainty',
+    'pandora.L2_rout2p1_8.ozone_vertical_column_amount',
+    'pandora.L2_rout2p1_8.direct_ozone_air_mass_factor',
+    'pandora.L2_rout2p1_8.ozone_air_mass_factor_uncertainty',
+    'pandora.L2_rsus1p1_8.sulfur_dioxide_vertical_column_amount',
+    'pandora.L2_rsus1p1_8.direct_sulfur_dioxide_air_mass_factor',
+    'pandora.L2_rsus1p1_8.sulfur_dioxide_air_mass_factor_uncertainty',
+    'pandora.L2_rnvssp1_8.nitrogen_dioxide_vertical_column_amount',
+    'pandora.L2_rnvssp1_8.direct_nitrogen_dioxide_air_mass_factor',
+    'pandora.L2_rnvssp1_8.direct_nitrogen_dioxide_air_mass_factor_uncertainty',
+    'purpleair.pm25_corrected',
     'purpleair.pm25_corrected_hourly', 'purpleair.pm25_corrected_daily',
     'purpleair.pm25_corrected_monthly', 'purpleair.pm25_corrected_yearly',
     'tempo.proxy_l2.no2.vertical_column_total',
     'tempo.proxy_l2.no2.vertical_column_total_uncertainty',
     'tempo.proxy_l2.no2.vertical_column_troposphere',
     'tempo.proxy_l2.no2.vertical_column_stratosphere',
     'tempo.proxy_l2.no2.amf_total',
@@ -875,16 +900,16 @@
         return self._capabilities
 
     def keys(self, offline=True):
         """
         Arguments
         ---------
         offline : bool
-            If True, uses small cached set of coverages.
-            If False, finds all coverages from capabilities.
+            If True, uses small cached set of tested coverages.
+            If False, finds all coverages from capabilities service.
 
         """
         if offline:
             keys = tuple(_keys)
         else:
             keys = []
             for line in self.capabilities().text.split('\n'):
@@ -969,15 +994,18 @@
         tropomi_kw = self.tropomi_kw
         viirsnoaa_kw = self.viirsnoaa_kw
         if compress is None:
             compress = self.compress
 
         wlon, slat, elon, nlat = bbox
 
-        if grid and request == 'GetCoverage':
+        # If already gridded, do not use grid keywords
+        nogridkw = any([key.startswith(pre) for pre in _noregrid_prefixes])
+
+        if (grid and not nogridkw) and request == 'GetCoverage':
             gridstr = self._build_grid(grid_kw)
         else:
             gridstr = ''
 
         if key.startswith('viirsnoaa'):
             viirsnoaastr = '&MINIMUM_QUALITY={minimum_quality}'.format(
                 **viirsnoaa_kw
@@ -1181,22 +1209,18 @@
             Results from download
 
         """
         import gzip
         import shutil
         import os
 
-        # If already gridded, do not use grid keywords
-        nogridkw = any([key.startswith(pre) for pre in _noregrid_prefixes])
-        grid = nogridkw is False
-
         # always use compression for network speed.
         outpath = self.get_file(
             'netcdf-ioapi', key=key, bdate=bdate, edate=edate, bbox=bbox,
-            grid=grid, compress=1, verbose=verbose
+            grid=True, compress=1, verbose=verbose
         )
         # Uncompress the netcdf file. If encoding is available, apply it
         if not self.overwrite and os.path.exists(outpath[:-3]):
             print('Using cached:', outpath[:-3])
         else:
             with gzip.open(outpath, 'rb') as f_in:
                 with open(outpath[:-3], 'wb') as f_out:
@@ -1214,15 +1238,15 @@
                         tvar.encoding.pop('_FillValue', '')
 
                 tmpf.to_netcdf(outpath[:-3], format='NETCDF4_CLASSIC')
 
         if withmeta:
             metapath = self.get_file(
                 'netcdf-ioapi', key=key, bdate=bdate, edate=edate, bbox=bbox,
-                grid=grid, compress=1, request='GetMetadata', verbose=verbose
+                grid=True, compress=1, request='GetMetadata', verbose=verbose
             )
         else:
             metapath = None
 
         f = open_ioapi(outpath[:-3], metapath=metapath)
         if removegz:
             os.remove(outpath)
```

### Comparing `pyrsig-0.4.3/README.md` & `pyrsig-0.4.4/README.md`

 * *Files identical despite different names*

