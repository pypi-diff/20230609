# Comparing `tmp/sscws-2.3.15.tar.gz` & `tmp/sscws-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscws-2.3.15.tar", last modified: Fri Jun  9 13:32:05 2023, max compression
+gzip compressed data, was "dist/sscws-2.3.8.tar", last modified: Wed Jul 14 09:30:23 2021, max compression
```

## Comparing `sscws-2.3.15.tar` & `sscws-2.3.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwx---   0 btharris   (503) btharris   (503)        0 2023-06-09 13:32:05.000000 sscws-2.3.15/
-drwxrwx---   0 btharris   (503) btharris   (503)        0 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws/
--rwxrwx---   0 btharris   (503) btharris   (503)     2674 2023-06-09 13:06:54.000000 sscws-2.3.15/sscws/__init__.py
--rwxrwx---   0 btharris   (503) btharris   (503)    18051 2023-06-09 13:18:05.000000 sscws-2.3.15/sscws/__main__.py
--rw-rw----   0 btharris   (503) btharris   (503)    12112 2022-05-13 12:54:13.000000 sscws-2.3.15/sscws/bfieldmodels.py
--rw-rw----   0 btharris   (503) btharris   (503)    37799 2023-04-13 17:16:02.000000 sscws-2.3.15/sscws/conjunctions.py
--rw-rw----   0 btharris   (503) btharris   (503)     8410 2022-05-13 12:54:13.000000 sscws-2.3.15/sscws/coordinates.py
--rw-rw----   0 btharris   (503) btharris   (503)    30897 2023-04-13 14:24:01.000000 sscws-2.3.15/sscws/filteroptions.py
--rw-rw----   0 btharris   (503) btharris   (503)    11731 2023-05-23 11:45:01.000000 sscws-2.3.15/sscws/formatoptions.py
--rw-rw----   0 btharris   (503) btharris   (503)     2978 2023-04-13 17:10:49.000000 sscws-2.3.15/sscws/mapping.py
--rw-rw----   0 btharris   (503) btharris   (503)    35223 2023-04-13 14:33:56.000000 sscws-2.3.15/sscws/outputoptions.py
--rw-rw----   0 btharris   (503) btharris   (503)     5736 2023-04-13 17:15:25.000000 sscws-2.3.15/sscws/regions.py
--rwxrwx---   0 btharris   (503) btharris   (503)    19686 2023-04-13 18:08:31.000000 sscws-2.3.15/sscws/request.py
--rw-rw----   0 btharris   (503) btharris   (503)    23528 2023-04-13 18:17:54.000000 sscws-2.3.15/sscws/result.py
--rwxrwx---   0 btharris   (503) btharris   (503)    32895 2023-06-09 13:22:09.000000 sscws-2.3.15/sscws/sscws.py
--rw-rw----   0 btharris   (503) btharris   (503)     7056 2023-04-13 17:22:12.000000 sscws-2.3.15/sscws/timeinterval.py
--rw-rw----   0 btharris   (503) btharris   (503)     7307 2023-04-13 17:16:59.000000 sscws-2.3.15/sscws/tracing.py
-drwxrwx---   0 btharris   (503) btharris   (503)        0 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws.egg-info/
--rw-rw----   0 btharris   (503) btharris   (503)     5258 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws.egg-info/PKG-INFO
--rw-rw----   0 btharris   (503) btharris   (503)      453 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws.egg-info/SOURCES.txt
--rw-rw----   0 btharris   (503) btharris   (503)        1 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws.egg-info/dependency_links.txt
--rw-rw----   0 btharris   (503) btharris   (503)       78 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws.egg-info/requires.txt
--rw-rw----   0 btharris   (503) btharris   (503)        6 2023-06-09 13:32:05.000000 sscws-2.3.15/sscws.egg-info/top_level.txt
--rw-rw----   0 btharris   (503) btharris   (503)     3462 2022-10-07 11:09:55.000000 sscws-2.3.15/README.md
--rw-rw----   0 btharris   (503) btharris   (503)     1948 2023-06-09 13:07:11.000000 sscws-2.3.15/setup.py
--rw-rw----   0 btharris   (503) btharris   (503)     5258 2023-06-09 13:32:05.000000 sscws-2.3.15/PKG-INFO
--rw-rw----   0 btharris   (503) btharris   (503)       38 2023-06-09 13:32:05.000000 sscws-2.3.15/setup.cfg
+drwxrwx---   0 btharris   (503) btharris   (503)        0 2021-07-14 09:30:23.000000 sscws-2.3.8/
+drwxrwx---   0 btharris   (503) btharris   (503)        0 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws/
+-rwxrwx---   0 btharris   (503) btharris   (503)     2578 2021-07-13 14:09:55.000000 sscws-2.3.8/sscws/__init__.py
+-rwxrwx---   0 btharris   (503) btharris   (503)    17710 2021-04-20 17:31:59.000000 sscws-2.3.8/sscws/__main__.py
+-rw-rw----   0 btharris   (503) btharris   (503)    12112 2021-03-01 16:34:11.000000 sscws-2.3.8/sscws/bfieldmodels.py
+-rw-rw----   0 btharris   (503) btharris   (503)    37732 2021-03-01 17:03:29.000000 sscws-2.3.8/sscws/conjunctions.py
+-rw-rw----   0 btharris   (503) btharris   (503)     8410 2021-03-01 17:13:57.000000 sscws-2.3.8/sscws/coordinates.py
+-rw-rw----   0 btharris   (503) btharris   (503)    30863 2021-03-01 17:19:08.000000 sscws-2.3.8/sscws/filteroptions.py
+-rw-rw----   0 btharris   (503) btharris   (503)    11731 2021-03-01 17:21:15.000000 sscws-2.3.8/sscws/formatoptions.py
+-rw-rw----   0 btharris   (503) btharris   (503)     2978 2020-10-14 18:51:18.000000 sscws-2.3.8/sscws/mapping.py
+-rw-rw----   0 btharris   (503) btharris   (503)    35189 2021-03-01 17:29:01.000000 sscws-2.3.8/sscws/outputoptions.py
+-rw-rw----   0 btharris   (503) btharris   (503)     5702 2021-03-26 09:40:39.000000 sscws-2.3.8/sscws/regions.py
+-rwxrwx---   0 btharris   (503) btharris   (503)    19709 2021-03-01 17:49:53.000000 sscws-2.3.8/sscws/request.py
+-rw-rw----   0 btharris   (503) btharris   (503)    22230 2021-03-25 18:50:41.000000 sscws-2.3.8/sscws/result.py
+-rwxrwx---   0 btharris   (503) btharris   (503)    29901 2021-07-12 17:00:10.000000 sscws-2.3.8/sscws/sscws.py
+-rw-rw----   0 btharris   (503) btharris   (503)     7041 2021-03-29 11:36:13.000000 sscws-2.3.8/sscws/timeinterval.py
+-rw-rw----   0 btharris   (503) btharris   (503)     7273 2021-03-01 17:41:24.000000 sscws-2.3.8/sscws/tracing.py
+drwxrwx---   0 btharris   (503) btharris   (503)        0 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws.egg-info/
+-rw-rw----   0 btharris   (503) btharris   (503)     4516 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws.egg-info/PKG-INFO
+-rw-rw----   0 btharris   (503) btharris   (503)      453 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws.egg-info/SOURCES.txt
+-rw-rw----   0 btharris   (503) btharris   (503)        1 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws.egg-info/dependency_links.txt
+-rw-rw----   0 btharris   (503) btharris   (503)       78 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws.egg-info/requires.txt
+-rw-rw----   0 btharris   (503) btharris   (503)        6 2021-07-14 09:30:23.000000 sscws-2.3.8/sscws.egg-info/top_level.txt
+-rw-rw----   0 btharris   (503) btharris   (503)     2838 2021-05-10 12:04:52.000000 sscws-2.3.8/README.md
+-rw-rw----   0 btharris   (503) btharris   (503)     1934 2021-07-13 14:09:41.000000 sscws-2.3.8/setup.py
+-rw-rw----   0 btharris   (503) btharris   (503)     4516 2021-07-14 09:30:23.000000 sscws-2.3.8/PKG-INFO
+-rw-rw----   0 btharris   (503) btharris   (503)       38 2021-07-14 09:30:23.000000 sscws-2.3.8/setup.cfg
```

### Comparing `sscws-2.3.15/sscws/__init__.py` & `sscws-2.3.8/sscws/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2020-2023 United States Government as represented by
+# Copyright (c) 2020-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Package for accessing the NASA's Satellite Situation Center (SSC) web
 services https://sscweb.gsfc.nasa.gov/WebServices/REST/.
 
-Copyright &copy; 2020-2023 United States Government as represented by the
+Copyright &copy; 2020-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 
 Notes
 -----
 <ul>
   <li>Due to rate limiting implemented by the SSC web services, an
@@ -51,15 +51,15 @@
   <li>The core functionality is implemented in the `sscws.sscws`
       sub-module.  New users should start by viewing the `sscws.sscws`
       sub-module.</li>
 </ul>
 """
 
 
-__version__ = "2.3.15"
+__version__ = "2.3.8"
 
 
 #
 # Limit on the number of times an HTTP request which returns a
 # 429 or 503 status with a Retry-After header will be retried.
 #
 RETRY_LIMIT = 100
@@ -77,14 +77,7 @@
 # XHTML schema namespace
 #
 XHTML_NS = 'http://www.w3.org/1999/xhtml'
 #
 # Namespace for use in xml.etree.ElementTree.find*
 #
 ET_XHTML_NS = '{' + XHTML_NS + '}'
-#
-# All namespaces found in responses.
-#
-NAMESPACES = {
-    'ssc': NS,
-    'xhtml': XHTML_NS
-}
```

### Comparing `sscws-2.3.15/sscws/__main__.py` & `sscws-2.3.8/sscws/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,36 +20,36 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Example Satellite Situation Center (SSC) web services client.
 https://sscweb.gsfc.nasa.gov/WebServices/REST/.
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
 import sys
 import getopt
 import json
 import xml.etree.ElementTree as ET
 import logging
 import logging.config
-from typing import List
+from typing import Dict, List
 import urllib3
 
 #import matplotlib as mpl
 #from mpl_toolkits.mplot3d import Axes3D  # pylint: disable=unused-import
 try:
     import matplotlib.pyplot as plt
     PLT_AVAILABLE = True
@@ -76,15 +76,15 @@
 from sscws.timeinterval import TimeInterval
 from sscws.tracing import BFieldTraceDirection, TraceType
 
 
 logging.basicConfig()
 LOGGING_CONFIG_FILE = 'logging_config.json'
 try:
-    with open(LOGGING_CONFIG_FILE, 'r', encoding='utf-8') as fd:
+    with open(LOGGING_CONFIG_FILE, 'r') as fd:
         logging.config.dictConfig(json.load(fd))
 except BaseException as exc:    # pylint: disable=broad-except
     if not isinstance(exc, FileNotFoundError):
         print('Logging configuration failed')
         print('Exception: ', exc)
         print('Ignoring failure')
         print()
@@ -107,15 +107,15 @@
     name
         name of this program
 
     Returns
     -------
     None
     """
-    print(f'USAGE: {name} [-e url][-d][-c cacerts][-h]')
+    print('USAGE: {name} [-e url][-d][-c cacerts][-h]'.format(name=name))
     print('WHERE: url = SSC web service endpoint URL')
     print('       -d disables TLS server certificate validation')
     print('       cacerts = CA certificate filename')
 
 
 # pylint: disable=too-many-locals,too-many-branches,too-many-statements
 def example(
@@ -161,60 +161,57 @@
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         elif opt in ('-h', '--help'):
             print_usage(argv[0])
             sys.exit()
 
     ssc = SscWs(endpoint=endpoint, ca_certs=ca_certs,
                 disable_ssl_certificate_validation=
-                disable_ssl_certificate_validation, user_agent='Example')
+                disable_ssl_certificate_validation)
 
     result = ssc.get_observatories()
     if result['HttpStatus'] == 200:
         print('SSC Observatories:')
         for observatory in result['Observatory']:
 
-            print((f"{observatory['Id']:15s} {observatory['Name']:20.20s} "
-                   f"{observatory['StartTime'].isoformat():25s}"))
+            print('{:15s} {:20.20s} {:25s}'.format(\
+                observatory['Id'], observatory['Name'],\
+                observatory['StartTime'].isoformat()))
     else:
         print('ssc.get_observatories failed with status = ',
               result['HttpStatus'])
         if 'ErrorMessage' in result:
             print('ErrorMessage = ', result['ErrorMessage'])
             print('ErrorDescription = ', result['ErrorDescription'])
         else:
             print('HttpText = ', result['ErrorText'])
 
-
     result = ssc.get_ground_stations()
     if result['HttpStatus'] == 200:
         print('SSC Ground Stations:')
         for ground_station in result['GroundStation']:
 
             location = ground_station['Location']
 
-            print((f"{ground_station['Id']:5s} {ground_station['Name']:20.20s} "
-                   f"{location['Latitude']:7.2f} {location['Longitude']:7.2f}"))
+            print('{:5s} {:20.20s} {:7.2f} {:7.2f}'.format(\
+                  ground_station['Id'], ground_station['Name'],\
+                  location['Latitude'], location['Longitude']))
     else:
         print('ssc.get_ground_stations failed with status = ',
               result['HttpStatus'])
 
-    obs_id = 'iss'
-    example_interval = ssc.get_example_time_interval(obs_id)
-    print('example_interval = ', example_interval)
-
     # A simple request.
     result = ssc.get_locations(['iss'],
                                ['2020-01-01T00:00:00Z',
                                 '2020-01-01T01:00:00Z'])
     #print(result)
     if result['HttpStatus'] == 200:
 
         if PLT_AVAILABLE:
             figure = plt.figure()
-            axis = figure.add_subplot(projection='3d')
+            axis = figure.gca(projection='3d')
             data = result['Data'][0]
             coords = data['Coordinates'][0]
             title = data['Id'] + ' Orbit (' + \
                 coords['CoordinateSystem'].value.upper() + ')'
             axis.plot(coords['X'], coords['Y'], coords['Z'], label=title)
             axis.legend()
             plt.show()
@@ -307,34 +304,30 @@
         None, None,
         RegionOptions(True, True, True, True),
         ValueOptions(True, True, True, True),
         DistanceFromOptions(True, True, True, True),
         b_field_trace_options
         )
     loc_filter = LocationFilter(0, 100000, True, True)
-    # pylint: disable=unused-variable
-    loc_filter_options = \
-        LocationFilterOptions(True, loc_filter, loc_filter, loc_filter,
-                              loc_filter, loc_filter, loc_filter,
-                              loc_filter)
-    # pylint: enable=unused-variable
+    loc_filter_options = LocationFilterOptions(True, loc_filter,
+                                               loc_filter, loc_filter,
+                                               loc_filter, loc_filter,
+                                               loc_filter, loc_filter)
 
     hemisphere_region = HemisphereRegions(True, True)
     trace_regions = MappedRegionFilterOptions(hemisphere_region,
                                               hemisphere_region,
                                               hemisphere_region,
                                               hemisphere_region,
                                               hemisphere_region,
                                               True)
     srfo = SpaceRegionsFilterOptions(True, True, True, True, True, True,
                                      True, True, True, True, True)
 
-    # pylint: disable=unused-variable
     rfo = RegionFilterOptions(srfo, trace_regions, trace_regions)
-    # pylint: enable=unused-variable
 
     #format_options = CdfFormatOptions()
     format_options = None
 
     loc_request = DataRequest('swarma b-trace locator request.',
                               TimeInterval('2020-01-01T00:00:00Z',
                                            '2020-01-01T00:10:00Z'),
@@ -378,34 +371,30 @@
         None, None,
         RegionOptions(True, True, True, True),
         ValueOptions(True, True, True, True),
         DistanceFromOptions(True, True, True, True),
         b_field_trace_options
         )
     loc_filter = LocationFilter(0, 100000, True, True)
-    # pylint: disable=unused-variable
-    loc_filter_options = \
-        LocationFilterOptions(True, loc_filter, loc_filter, loc_filter,
-                              loc_filter, loc_filter, loc_filter,
-                              loc_filter)
-    # pylint: enable=unused-variable
+    loc_filter_options = LocationFilterOptions(True, loc_filter,
+                                               loc_filter, loc_filter,
+                                               loc_filter, loc_filter,
+                                               loc_filter, loc_filter)
 
     hemisphere_region = HemisphereRegions(True, True)
     trace_regions = MappedRegionFilterOptions(hemisphere_region,
                                               hemisphere_region,
                                               hemisphere_region,
                                               hemisphere_region,
                                               hemisphere_region,
                                               True)
     srfo = SpaceRegionsFilterOptions(True, True, True, True, True, True,
                                      True, True, True, True, True)
 
-    # pylint: disable=unused-variable
     rfo = RegionFilterOptions(srfo, trace_regions, trace_regions)
-    # pylint: enable=unused-variable
 
     #format_options = CdfFormatOptions()
     format_options = None
 
     loc_request = DataRequest('Example locator request.',
                               TimeInterval('2020-10-02T00:00:00Z',
                                            '2020-10-02T01:00:00Z'),
@@ -422,17 +411,15 @@
     Create an example QueryRequest.
 
     Returns
     -------
     ET
         ElementTree representation of an example QueryRequest.
     """
-    # pylint: disable=unused-variable
     b_field_model = BFieldModel(external=Tsyganenko89cBFieldModel())
-    # pylint: enable=unused-variable
 
     sats = [
         Satellite('themisa', BFieldTraceDirection.SAME_HEMISPHERE),
         Satellite('themisb', BFieldTraceDirection.SAME_HEMISPHERE),
         Satellite('themisc', BFieldTraceDirection.SAME_HEMISPHERE),
         Satellite('themisd', BFieldTraceDirection.SAME_HEMISPHERE),
         Satellite('themise', BFieldTraceDirection.SAME_HEMISPHERE)
```

### Comparing `sscws-2.3.15/sscws/bfieldmodels.py` & `sscws-2.3.8/sscws/bfieldmodels.py`

 * *Files identical despite different names*

### Comparing `sscws-2.3.15/sscws/conjunctions.py` & `sscws-2.3.8/sscws/conjunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,32 +20,29 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to represent conjunction related classes from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
-# pylint: disable=duplicate-code
-# pylint: disable=too-many-lines
-
 import xml.etree.ElementTree as ET
 from enum import Enum
 from abc import ABCMeta
 from typing import List
 
 from sscws.coordinates import CoordinateSystem, CoordinateSystemType, \
     SurfaceGeographicCoordinates
```

### Comparing `sscws-2.3.15/sscws/coordinates.py` & `sscws-2.3.8/sscws/coordinates.py`

 * *Files identical despite different names*

### Comparing `sscws-2.3.15/sscws/filteroptions.py` & `sscws-2.3.8/sscws/filteroptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to related to filter options from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
-# pylint: disable=too-many-lines
-
 import xml.etree.ElementTree as ET
 
 from sscws.outputoptions import LocationFilter
 
 
 
 class RegionFilterOptions:
```

### Comparing `sscws-2.3.15/sscws/formatoptions.py` & `sscws-2.3.8/sscws/formatoptions.py`

 * *Files identical despite different names*

### Comparing `sscws-2.3.15/sscws/mapping.py` & `sscws-2.3.8/sscws/mapping.py`

 * *Files identical despite different names*

### Comparing `sscws-2.3.15/sscws/outputoptions.py` & `sscws-2.3.8/sscws/outputoptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to represent output options from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
-# pylint: disable=too-many-lines
-
 import xml.etree.ElementTree as ET
 from typing import List
 
 from sscws.coordinates import CoordinateSystem, CoordinateComponent
 from sscws.regions import Hemisphere
```

### Comparing `sscws-2.3.15/sscws/regions.py` & `sscws-2.3.8/sscws/regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2020 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to represent region classes from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2020 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
-# pylint: disable=duplicate-code
-
 import xml.etree.ElementTree as ET
 from enum import Enum
 
 
 class FootpointRegion(Enum):
     """
     Enumerations representing the FootpointRegion defined
```

### Comparing `sscws-2.3.15/sscws/request.py` & `sscws-2.3.8/sscws/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to represent the Request and its
 sub-classes from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
 import xml.etree.ElementTree as ET
 from typing import List
-from abc import ABCMeta
+from abc import ABCMeta, abstractmethod
 
-from sscws import NS
+from sscws import NS, ET_NS
 from sscws.bfieldmodels import BFieldModel
 from sscws.conjunctions import Condition, ConditionOperator, \
     ExecuteOptions, GroundStationCondition, LeadSatelliteCondition, \
     RegionCondition, ResultOptions, SatelliteCondition
 from sscws.filteroptions import LocationFilterOptions, RegionFilterOptions
 from sscws.formatoptions import FormatOptions
 from sscws.outputoptions import OutputOptions
```

### Comparing `sscws-2.3.15/sscws/result.py` & `sscws-2.3.8/sscws/result.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,39 +20,39 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to represent the Result class and its
 sub-classes from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
 import xml.etree.ElementTree as ET
 from datetime import datetime
 from typing import Any, Callable, Dict, List
 from abc import ABCMeta, abstractmethod
 from enum import Enum
 import dateutil.parser
 import numpy as np
 
-from sscws import NAMESPACES as NS
+from sscws import ET_NS
 from sscws.coordinates import CoordinateSystem
 from sscws.regions import FootpointRegion, Hemisphere, SpaceRegion
 
 
 class ResultStatusCode(Enum):
     """
     Enumerations representing the ResultStatusCode defined
@@ -271,22 +271,20 @@
         ValueError
             If the given xml is not a valid XML representation of a
             DataResult.
         """
 
         return {
             'StatusCode': ResultStatusCode(\
-                 result_element.find('ssc:StatusCode', namespaces=NS).text),
+                 result_element.find(ET_NS + 'StatusCode').text),
             'StatusSubCode': ResultStatusSubCode(\
-                 result_element.find('ssc:StatusSubCode', namespaces=NS).text)
+                 result_element.find(ET_NS + 'StatusSubCode').text)
         }
 
 
-    # pylint: disable=too-many-locals
-    # pylint: disable=too-many-branches
     @staticmethod
     def get_data_result(
             data_result_element: ET
         ) -> Dict:
         """
         Produces a Dict representation of a DataResult from the given
         xml representation of a DataResult.
@@ -309,40 +307,39 @@
         ValueError
             If the given xml is not a valid XML representation of a
             DataResult.
         """
 
         result = Result.get_status(data_result_element)
 
-        data_elements = data_result_element.findall('ssc:Data', namespaces=NS)
+        data_elements = data_result_element.findall(ET_NS + 'Data')
         if data_elements is not None:
             data_len = len(data_elements)
         else:
             data_len = 0
         result['Data'] = np.empty(data_len, dtype=object)
 
         for data_i, data_element in enumerate(data_elements):
 
             result['Data'][data_i] = {
-                'Id': data_element.find('ssc:Id', namespaces=NS).text,
+                'Id': data_element.find(ET_NS + 'Id').text,
             }
-            coords_elements = data_element.findall('ssc:Coordinates',
-                                                   namespaces=NS)
+            coords_elements = data_element.findall(ET_NS + 'Coordinates')
 
             if coords_elements is not None:
                 coords_len = len(coords_elements)
             else:
                 coords_len = 0
             result['Data'][data_i]['Coordinates'] =\
                 np.empty(coords_len, dtype=object)
 
             for coords_i, coords_element in enumerate(coords_elements):
 
                 coord_system = coords_element.find(\
-                            'ssc:CoordinateSystem', namespaces=NS).text
+                            ET_NS + 'CoordinateSystem').text
 
                 result['Data'][data_i]['Coordinates'][coords_i] = {
                     'CoordinateSystem': CoordinateSystem(coord_system)
                 }
 
                 for name in ['X', 'Y', 'Z', 'Latitude', 'Longitude',
                              'LocalTime']:
@@ -350,32 +347,32 @@
                         Result._get_data(coords_element, name, float)
 
             result['Data'][data_i]['Time'] = \
                 Result._get_data(data_element, 'Time', datetime)
 
 
             b_trace_data_elements = data_element.findall(\
-                   'ssc:BTraceData', namespaces=NS)
+                   ET_NS + 'BTraceData')
             if b_trace_data_elements is not None:
                 b_trace_data_len = len(b_trace_data_elements)
             else:
                 b_trace_data_len = 0
 
             result['Data'][data_i]['BTraceData'] = \
                 np.empty(b_trace_data_len, dtype=object)
 
             for b_trace_data_i, b_trace_data in \
                 enumerate(b_trace_data_elements):
 
                 result['Data'][data_i]['BTraceData'][b_trace_data_i] = {
                     'CoordinateSystem': CoordinateSystem(\
                         b_trace_data.find(\
-                            'ssc:CoordinateSystem', namespaces=NS).text),
+                            ET_NS + 'CoordinateSystem').text),
                     'Hemisphere': Hemisphere(b_trace_data.find(\
-                            'ssc:Hemisphere', namespaces=NS).text),
+                            ET_NS + 'Hemisphere').text),
                 }
                 for name in ['Latitude', 'Longitude', 'ArcLength']:
                     result['Data'][data_i]['BTraceData'][b_trace_data_i][name] = \
                         Result._get_data(b_trace_data, name, float)
 
 
             for name in ['RadialLength', 'MagneticStrength',
@@ -398,16 +395,14 @@
                          'NorthBTracedFootpointRegions',
                          'SouthBTracedFootpointRegions']:
                 result['Data'][data_i][name] = \
                     Result._get_data(data_element, name,
                                      FootpointRegion)
 
         return result
-    # pylint: enable=too-many-locals
-    # pylint: enable=too-many-branches
 
 
     @staticmethod
     def _get_data(
             data_element: ET,
             name: str,
             value_type: Callable[[str], Any],
@@ -428,15 +423,15 @@
 
         Returns
         -------
         np.ndarray
             np.ndarray representation of the specified values from
             data_element.
         """
-        data_elements = data_element.findall('ssc:' + name, namespaces=NS)
+        data_elements = data_element.findall(ET_NS + name)
         if data_elements is not None:
             size = len(data_elements)
         else:
             size = 0
         values = np.empty(size, dtype=value_type)
         for index, value in enumerate(data_elements):
             if value_type is datetime:
@@ -475,41 +470,37 @@
             FileResult.
         """
 
         result = Result.get_status(file_result_element)
         result['Files'] = []
 
         for file_description in file_result_element.findall(\
-                'ssc:Files', namespaces=NS):
+                ET_NS + 'Files'):
             result['Files'].append({
-                'Name': file_description.find('ssc:Name', namespaces=NS).text,
-                'MimeType': file_description.find('ssc:MimeType',
-                                                  namespaces=NS).text,
-                'Length': int(file_description.find('ssc:Length',
-                                                    namespaces=NS).text),
+                'Name': file_description.find(ET_NS + 'Name').text,
+                'MimeType': file_description.find(ET_NS + 'MimeType').text,
+                'Length': int(file_description.find(ET_NS + 'Length').text),
                 'LastModified': dateutil.parser.parse(\
-                    file_description.find('ssc:LastModified',
-                                          namespaces=NS).text)
+                    file_description.find(ET_NS + 'LastModified').text)
             })
         return result
 
 
     @staticmethod
     def __get_conjunction_description(
             description: ET
         ) -> Dict:
 
         conjunction = {}
 
-        location = description.find('ssc:Location', namespaces=NS)
+        location = description.find(ET_NS + 'Location')
         if location is not None:
             conjunction['Location'] = Result.__get_location(location)
 
-        trace_description = description.find('ssc:TraceDescription',
-                                             namespaces=NS)
+        trace_description = description.find(ET_NS + 'TraceDescription')
         if trace_description is not None:
             conjunction['TraceDescription'] = \
                 Result.__get_trace_description(trace_description)
 
         return conjunction
 
 
@@ -539,27 +530,22 @@
         """
 
         loc_type = location.get(\
                        '{http://www.w3.org/2001/XMLSchema-instance}type')
 
         if loc_type == 'RadiusGeographicCoordinates':
             location = {
-                'Latitude': float(location.find('ssc:Latitude',
-                                                namespaces=NS).text),
-                'Longitude': float(location.find('ssc:Longitude',
-                                                 namespaces=NS).text),
-                'Radius': float(location.find('ssc:Radius',
-                                              namespaces=NS).text)
+                'Latitude': float(location.find(ET_NS + 'Latitude').text),
+                'Longitude': float(location.find(ET_NS + 'Longitude').text),
+                'Radius': float(location.find(ET_NS + 'Radius').text)
             }
         elif loc_type == 'SurfaceGeographicCoordinates':
             location = {
-                'Latitude': float(location.find('ssc:Latitude',
-                                                namespaces=NS).text),
-                'Longitude': float(location.find('ssc:Longitude',
-                                                 namespaces=NS).text),
+                'Latitude': float(location.find(ET_NS + 'Latitude').text),
+                'Longitude': float(location.find(ET_NS + 'Longitude').text),
             }
         else:
             raise ValueError('Unrecongized Location xsi:type = ' + loc_type)
 
         return location
 
 
@@ -581,20 +567,19 @@
         Dict
             Dict representation of the given TraceDescription element's
             value.
         """
 
         return {
             'Location': Result.__get_location(\
-                trace_element.find('ssc:Location', namespaces=NS)),
+                trace_element.find(ET_NS + 'Location')),
             'ArcLength': float(trace_element.find(\
-                                   'ssc:ArcLength', namespaces=NS).text),
+                                   ET_NS + 'ArcLength').text),
             'Target': Result.__get_target(\
-                                 trace_element.find('ssc:Target',
-                                                    namespaces=NS))
+                                 trace_element.find(ET_NS + 'Target'))
         }
 
 
     @staticmethod
     def __get_target(
             target: ET
         ) -> Dict:
@@ -620,31 +605,27 @@
         """
 
         target_type = target.get(\
                           '{http://www.w3.org/2001/XMLSchema-instance}type')
 
         if target_type == 'GroundStationTarget':
             target = {
-                'GroundStation': target.find('ssc:GroundStation',
-                                             namespaces=NS).text
+                'GroundStation': target.find(ET_NS + 'GroundStation').text
             }
         elif target_type == 'SatelliteTarget':
             target = {
-                'LeadSatellite': target.find('ssc:LeadSatellite',
-                                             namespaces=NS).text,
-                'Distance': float(target.find('ssc:Distance',
-                                              namespaces=NS).text),
+                'LeadSatellite': target.find(ET_NS + 'LeadSatellite').text,
+                'Distance': float(target.find(ET_NS + 'Distance').text),
             }
         else:
             raise ValueError('Unrecongized Target xsi:type = ' +
                              target_type)
         return target
 
 
-    # pylint: disable=too-many-locals
     @staticmethod
     def get_query_result(
             query_result_element: ET
         ) -> Dict:  # pylint: disable=too-many-locals
         """
         Produces a Dict representation of a QueryDataResult from the given
         xml representation of a QueryDataResult.
@@ -667,62 +648,61 @@
         ValueError
             If the given xml is not a valid XML representation of a
             QueryResult.
         """
 
         result = Result.get_status(query_result_element)
         conjunction_elements = query_result_element.findall(\
-                                   'ssc:Conjunction', namespaces=NS)
+                                   ET_NS + 'Conjunction')
         if conjunction_elements is not None:
             conjunction_len = len(conjunction_elements)
         else:
             conjunction_len = 0
 
         result['Conjunction'] = np.empty(conjunction_len, dtype=object)
 
         for conjunction_i, conjunction in enumerate(conjunction_elements):
 
             time_interval = conjunction.find(\
-                                'ssc:TimeInterval', namespaces=NS)
+                                ET_NS + 'TimeInterval')
             start = dateutil.parser.parse(\
-                        time_interval.find('ssc:Start', namespaces=NS).text)
+                        time_interval.find(ET_NS + 'Start').text)
             end = dateutil.parser.parse(\
-                      time_interval.find('ssc:End', namespaces=NS).text)
+                      time_interval.find(ET_NS + 'End').text)
             sat_description_elements = \
-                conjunction.findall('ssc:SatelliteDescription', namespaces=NS)
+                conjunction.findall(ET_NS + 'SatelliteDescription')
             if sat_description_elements is not None:
                 sat_description_len = len(sat_description_elements)
             else:
                 sat_description_len = 0
             sat_descriptions = np.empty(sat_description_len, dtype=object)
             for sat_description_i, sat_description in \
                 enumerate(sat_description_elements):
 
                 description_elements = \
-                    sat_description.findall('ssc:Description', namespaces=NS)
+                    sat_description.findall(ET_NS + 'Description')
                 if description_elements is not None:
                     description_len = len(description_elements)
                 else:
                     description_len = 0
                 descriptions = np.empty(description_len, dtype=object)
                 for description_i, description in \
                     enumerate(description_elements):
 
                     descriptions[description_i] = \
                         Result.__get_conjunction_description(description)
 
                 sat_descriptions[sat_description_i] = {
                     'Satellite': sat_description.find(\
-                        'ssc:Satellite', namespaces=NS).text,
+                        ET_NS + 'Satellite').text,
                     'Description': descriptions
                 }
 
             result['Conjunction'][conjunction_i] = {
                 'TimeInterval': {
                     'Start': start,
                     'End': end
                 },
                 'SatelliteDescription': sat_descriptions
             }
 
         return result
-    # pylint: enable=too-many-locals
```

### Comparing `sscws-2.3.15/sscws/sscws.py` & `sscws-2.3.8/sscws/sscws.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,36 +20,35 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module for accessing the Satellite Situation Center (SSC) web services
 https://sscweb.gsfc.nasa.gov/WebServices/REST/.
 """
 
 import platform
-from datetime import timedelta
 import xml.etree.ElementTree as ET
 from xml.etree.ElementTree import ParseError
 import time
 import logging
-from typing import Dict, List, Union
+from typing import Dict, List, Tuple, Union
 import requests
 import dateutil.parser
 
-from sscws import __version__, RETRY_LIMIT, NAMESPACES as NS
+from sscws import __version__, RETRY_LIMIT, ET_NS, ET_XHTML_NS
 from sscws.coordinates import CoordinateSystem, CoordinateComponent
 from sscws.outputoptions import CoordinateOptions, OutputOptions
 from sscws.request import DataRequest, QueryRequest, SatelliteSpecification
 from sscws.result import Result
 from sscws.timeinterval import TimeInterval
 
 #try:
@@ -68,30 +67,28 @@
     ----------
     endpoint
         URL of the SSC web service.  If None, the default is
         'https://sscweb.gsfc.nasa.gov/WS/sscr/2/'.
     timeout
         Number of seconds to wait for a response from the server.
     proxy
-        HTTP proxy information.  For example,<pre>
+        HTTP proxy information.  For example,
         proxies = {
           'http': 'http://10.10.1.10:3128',
           'https': 'http://10.10.1.10:1080',
-        }</pre>
+        }
         Proxy information can also be set with environment variables.
-        For example,<pre>
+        For example,
         $ export HTTP_PROXY="http://10.10.1.10:3128"
-        $ export HTTPS_PROXY="http://10.10.1.10:1080"</pre>
+        $ export HTTPS_PROXY="http://10.10.1.10:1080"
     ca_certs
         Path to certificate authority (CA) certificates that will
         override the default bundle.
     disable_ssl_certificate_validation
         Flag indicating whether to validate the SSL certificate.
-    user_agent
-        A value that is appended to the HTTP User-Agent values.
 
     Notes
     -----
     The logger used by this class has the class' name (SscWs).  By default,
     it is configured with a NullHandler.  Users of this class may configure
     the logger to aid in diagnosing problems.
 
@@ -107,16 +104,15 @@
     # pylint: disable=too-many-arguments
     def __init__(
             self,
             endpoint=None,
             timeout=None,
             proxy=None,
             ca_certs=None,
-            disable_ssl_certificate_validation=False,
-            user_agent=None):
+            disable_ssl_certificate_validation=False):
 
         self.logger = logging.getLogger(type(self).__name__)
         self.logger.addHandler(logging.NullHandler())
 
         self.retry_after_time = None
 
         self.logger.debug('endpoint = %s', endpoint)
@@ -124,22 +120,17 @@
         self.logger.debug('disable_ssl_certificate_validation = %s',
                           disable_ssl_certificate_validation)
 
         if endpoint is None:
             self._endpoint = 'https://sscweb.gsfc.nasa.gov/WS/sscr/2/'
         else:
             self._endpoint = endpoint
-
         self._user_agent = 'sscws/' + __version__ + ' (' + \
             platform.python_implementation() + ' ' \
             + platform.python_version() + '; '+ platform.platform() + ')'
-
-        if user_agent is not None:
-            self._user_agent += ' (' + user_agent + ')'
-
         self._request_headers = {
             'Content-Type' : 'application/xml',
             'Accept' : 'application/xml',
             'User-Agent' : self._user_agent
         }
         self._session = requests.Session()
         #self._session.max_redirects = 0
@@ -152,25 +143,14 @@
             self._session.verify = False
 
         if proxy is not None:
             self._proxy = proxy
 
         self._timeout = timeout
 
-        self._cache = {
-            'Observatories': {
-                'ETag': None,
-                'Value': None
-            },
-            'GroundStations': {
-                'Last-Modified': None,
-                'Value': None
-            }
-        }
-
     # pylint: enable=too-many-arguments
 
 
     def __str__(self) -> str:
         """
         Produces a string representation of this object.
 
@@ -222,63 +202,40 @@
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         """
         url = self._endpoint + 'observatories'
 
         self.logger.debug('request url = %s', url)
 
-        headers = None
-        if self._cache['Observatories']['ETag'] is not None:
-            headers = {
-                'If-None-Match': self._cache['Observatories']['ETag']
-            }
-
-        response = self._session.get(url, timeout=self._timeout,
-                                     headers=headers)
-
-        if response.status_code == 304:
-            return self._cache['Observatories']['Value']
+        response = self._session.get(url, timeout=self._timeout)
 
         status = self.__get_status(response)
         if response.status_code != 200:
             return status
 
         observatory_response = ET.fromstring(response.text)
 
         result = {
             'Observatory': []
         }
 
-        for observatory in observatory_response.findall('ssc:Observatory',
-                                                        namespaces=NS):
+        for observatory in observatory_response.findall(ET_NS + 'Observatory'):
+
             result['Observatory'].append({
-                'Id': observatory.find('ssc:Id', namespaces=NS).text,
-                'Name': observatory.find('ssc:Name', namespaces=NS).text,
-                'Resolution': int(observatory.find('ssc:Resolution',
-                                                   namespaces=NS).text),
+                'Id': observatory.find(ET_NS + 'Id').text,
+                'Name': observatory.find(ET_NS + 'Name').text,
+                'Resolution': int(observatory.find(ET_NS + 'Resolution').text),
                 'StartTime': dateutil.parser.parse(observatory.find(\
-                    'ssc:StartTime', namespaces=NS).text),
+                    ET_NS + 'StartTime').text),
                 'EndTime': dateutil.parser.parse(observatory.find(\
-                    'ssc:EndTime', namespaces=NS).text),
-                'ResourceId': observatory.find('ssc:ResourceId',
-                                               namespaces=NS).text
+                    ET_NS + 'EndTime').text),
+                'ResourceId': observatory.find(ET_NS + 'ResourceId').text
             })
 
         result.update(status)
-
-        if 'ETag' in response.headers:
-            etag = response.headers['ETag']
-            # workaround old apache bugs that are still causing problems
-            etag = etag.replace('-gzip', '')
-            self._cache['Observatories']['ETag'] = etag
-            self._cache['Observatories']['Value'] = result
-        else:
-            self._cache['Observatories']['ETag'] = None
-            self._cache['Observatories']['Value'] = None
-
         return result
 
 
     def get_ground_stations(
             self
         ) -> Dict:
         """
@@ -301,91 +258,46 @@
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         """
         url = self._endpoint + 'groundStations'
 
         self.logger.debug('request url = %s', url)
 
-        headers = None
-        if self._cache['GroundStations']['Last-Modified'] is not None:
-            headers = {
-                'If-Modified-Since': self._cache['GroundStations']['Last-Modified']
-            }
-
-        response = self._session.get(url, timeout=self._timeout,
-                                     headers=headers)
-
-        if response.status_code == 304:
-            return self._cache['GroundStations']['Value']
+        response = self._session.get(url, timeout=self._timeout)
 
         status = self.__get_status(response)
         if response.status_code != 200:
             return status
 
         ground_station_response = ET.fromstring(response.text)
 
         result = {
             'GroundStation': []
         }
 
         for ground_station in ground_station_response.findall(\
-                'ssc:GroundStation', namespaces=NS):
+                ET_NS + 'GroundStation'):
 
-            location = ground_station.find('ssc:Location', namespaces=NS)
-            latitude = float(location.find('ssc:Latitude', namespaces=NS).text)
-            longitude = float(location.find('ssc:Longitude',
-                                            namespaces=NS).text)
+            location = ground_station.find(ET_NS + 'Location')
+            latitude = float(location.find(ET_NS + 'Latitude').text)
+            longitude = float(location.find(ET_NS + 'Longitude').text)
 
             result['GroundStation'].append({
-                'Id': ground_station.find('ssc:Id', namespaces=NS).text,
-                'Name': ground_station.find('ssc:Name', namespaces=NS).text,
+                'Id': ground_station.find(ET_NS + 'Id').text,
+                'Name': ground_station.find(ET_NS + 'Name').text,
                 'Location': {
                     'Latitude': latitude,
                     'Longitude': longitude
                 }
             })
 
         result.update(status)
-
-        if 'Last-Modified' in response.headers:
-            self._cache['GroundStations']['Last-Modified'] = response.headers['Last-Modified']
-            self._cache['GroundStations']['Value'] = result
-        else:
-            self._cache['GroundStations']['Last-Modified'] = None
-            self._cache['GroundStations']['Value'] = None
-
         return result
 
 
-    def get_example_time_interval(
-            self,
-            observatory: str
-        ) -> TimeInterval:
-        """
-        Gets a small example time interval for the specified observatory.
-
-        Parameters:
-        -----------
-        observatory
-            Specifies the observatory.
-
-        Returns
-        -------
-        TimeInterval
-            A small example time interval for the specified observatory.
-        """
-
-        for obs in self.get_observatories()['Observatory']:
-            if obs['Id'] == observatory:
-                end = obs['EndTime']
-                return TimeInterval(end - timedelta(hours=2), end)
-
-        return None
-
-
     def get_locations(
             self,
             param1: Union[List[str], DataRequest],
             time_range: Union[List[str], TimeInterval] = None,
             coords: List[CoordinateSystem] = None
         ) -> Dict:
         """
@@ -400,15 +312,15 @@
             A locations DataRequest or a list of observatory identifier
             (returned by get_observatories).
         time_range
             A TimeInterval or two element array of ISO 8601 string
             values of the start and stop time of requested data.  The
             datetime values should have a UTC timezone.  If the values
             have no timezone, it will be set to UTC.  A datetime with
-            a non-UTC timezone, will have its value adjusted to UTC and
+            a non-UTC timezone, will have its value adjusted to UTC and 
             the returned data may not have the expected range.
         coords
             Array of CoordinateSystem values that location information
             is to be in.  If None, default is CoordinateSystem.GSE.
         Returns
         -------
         Dict
@@ -417,15 +329,15 @@
             with the addition of the following key/values:<br>
             - HttpStatus: with the value of the HTTP status code.
               Successful == 200.<br>
             When HttpStatus != 200:<br>
             - HttpText: containing a string representation of the HTTP
               entity body.<br>
             When HttpText is a standard SSC WS error entity body the
-            following key/values (convenience to avoid parsing
+            following key/values (convenience to avoid parsing 
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         Raises
         ------
         ValueError
             If param1 is not a DataRequest and time_range is missing or
@@ -549,29 +461,29 @@
             with the addition of the following key/values:<br>
             - HttpStatus: with the value of the HTTP status code.
               Successful == 200.<br>
             When HttpStatus != 200:<br>
             - HttpText: containing a string representation of the HTTP
               entity body.<br>
             When HttpText is a standard SSC WS error entity body the
-            following key/values (convenience to avoid parsing
+            following key/values (convenience to avoid parsing 
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         """
         url = self._endpoint + 'locations'
 
         self.logger.debug('__get_locations: POST request url = %s', url)
 
         xml_data_request = request.xml_element()
 
         #self.logger.debug('request XML = %s',
         #                  ET.tostring(xml_data_request))
 
-        for retries in range(RETRY_LIMIT): # pylint: disable=unused-variable
+        for retries in range(RETRY_LIMIT):
 
             response = self._session.post(url,
                                           data=ET.tostring(xml_data_request),
                                           timeout=self._timeout)
             if response.status_code == 429 or \
                response.status_code == 503 and \
                'Retry-After' in response.headers:
@@ -607,35 +519,35 @@
 
         Returns
         -------
         Dict
             Dict containing the following:<br>
             - HttpStatus: the HTTP status code<br>
             additionally, when HttpStatus != 200<br>
-            - ErrorText: a string representation of the entire entity
+            - ErrorText: a string representation of the entire entity 
               body<br>
             - ErrorMessage: SSC WS ErrorMessage (when available)<br>
             - ErrorDescription: SSC WS ErrorDescription (when available)
         """
         http_result = {
             'HttpStatus': response.status_code
         }
 
         if response.status_code != 200:
 
             http_result['ErrorText'] = response.text
             try:
                 error_element = ET.fromstring(response.text)
                 http_result['ErrorMessage'] = error_element.findall(\
-                    './/xhtml:p[@class="ErrorMessage"]/xhtml:b',
-                    namespaces=NS)[0].tail
+                    './/' + ET_XHTML_NS + 'p[@class="ErrorMessage"]/' +
+                    ET_XHTML_NS + 'b')[0].tail
                 http_result['ErrorDescription'] = error_element.findall(\
-                    './/xhtml:p[@class="ErrorDescription"]/' +
-                    'xhtml:b', namespaces=NS)[0].tail
-            except ParseError:
+                    './/' + ET_XHTML_NS + 'p[@class="ErrorDescription"]/' +
+                    ET_XHTML_NS + 'b')[0].tail
+            except:
                 pass  # ErrorText is the best we can do
 
         return http_result
 
 
     def __get_result(
             self,
@@ -651,32 +563,32 @@
 
         Returns
         -------
         Dict
             Dict representation of a Result as described in
             <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>
             with the addition of an HttpStatus key with the value of the
-            HTTP status code.  When HttpStatus != 200, a key named
+            HTTP status code.  When HttpStatus != 200, a key named 
             HttpText will contain a string representation of the entity
             body.  And if the HttpText is a standard SSC WS error
             entity body, then keys named ErrorMessage and ErrorDescription
             will contain the values from the SSC WS error entity body
             (saving the caller the trouble of parsing HttpText).
         """
 
         status = self.__get_status(response)
         if response.status_code != 200:
             return status
 
         element = ET.fromstring(response.text)
 
-        result_element = element.find('ssc:Result', namespaces=NS)
+        result_element = element.find(ET_NS + 'Result')
 
         if result_element is None:
-            result_element = element.find('ssc:QueryResult', namespaces=NS)
+            result_element = element.find(ET_NS + 'QueryResult')
 
         result = Result.get_result(result_element)
         result.update(status)
         return result
 
 
     def get_conjunctions(
@@ -698,15 +610,15 @@
             with the addition of the following key/values:<br>
             - HttpStatus: with the value of the HTTP status code.
               Successful == 200.<br>
             When HttpStatus != 200:<br>
             - HttpText: containing a string representation of the HTTP
               entity body.<br>
             When HttpText is a standard SSC WS error entity body the
-            following key/values (convenience to avoid parsing
+            following key/values (convenience to avoid parsing 
             HttpStatus):<br>
             - ErrorMessage: value from HttpText.<br>
             - ErrorDescription: value from HttpText.<br>
         Raises
         ------
         ValueError
             If query is invalid.
@@ -717,15 +629,15 @@
         self.logger.debug('POST request url = %s', url)
 
         xml_query_request = query.xml_element()
 
         self.logger.debug('request XML = %s',
                           ET.tostring(xml_query_request))
 
-        for retries in range(RETRY_LIMIT):  # pylint: disable=unused-variable
+        for retries in range(RETRY_LIMIT):
 
             response = self._session.post(url,
                                           data=ET.tostring(xml_query_request),
                                           timeout=self._timeout)
             if response.status_code == 429 or \
                response.status_code == 503 and \
                'Retry-After' in response.headers:
@@ -764,19 +676,19 @@
         result
             Dict representation of Result as described
             <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.
         """
         for file in result['Files']:
             print(file['Name'])
 
-    # pylint: disable=too-many-branches
+
     @staticmethod
     def print_locations_result(
             result: Dict
-        ) -> None:
+        ) -> None:    # pylint: disable=too-many-branches
         """
         Prints a Dict representation of a Result.
 
         Parameters
         ----------
         result
             Dict representation of a Result as described
@@ -809,17 +721,18 @@
                               b_trace['Hemisphere'].value,
                               'Magnetic Field-Line Trace Footpoints')
                         print('Time                          ', 'Latitude        ',
                               'Longitude   ', 'Arc Length')
                         for index in range(min(len(data['Time']),
                                                len(b_trace['Latitude']))):
                             print(data['Time'][index],
-                                  (f"{b_trace['Latitude'][index]:15.5f} "
-                                   f"{b_trace['Longitude'][index]:15.5f} "
-                                   f"{b_trace['ArcLength'][index]:15.5f}"))
+                                  '{:15.5f} {:15.5f} {:15.5f}'.format(\
+                                      b_trace['Latitude'][index],
+                                      b_trace['Longitude'][index],
+                                      b_trace['ArcLength'][index]))
 
                 quantities = ['RadialLength', 'MagneticStrength',
                               'NeutralSheetDistance', 'BowShockDistance',
                               'MagnetoPauseDistance', 'DipoleLValue',
                               'DipoleInvariantLatitude', 'SpacecraftRegion',
                               'RadialTracedFootpointRegions',
                               'NorthBTracedFootpointRegions',
@@ -828,36 +741,36 @@
                 for quantity in quantities:
                     SscWs.print_time_series(quantity, data)
 
                 if 'BGseX' in data and data['BGseX'] is not None:
 
                     min_len = min(len(data['Time']), len(data['BGseX']))
                     if min_len > 0:
-                        print(f"{'Time':25s} {'B Strength GSE':^30s}")
-                        print(f"{'':25s} {'X':^9s} {'Y':^9s} {'Z':^9s}")
+                        print('{:25s} {:^30s}'.format('Time', 'B Strength GSE'))
+                        print('{:25s} {:^9s} {:^9s} {:^9s}'.format('', 'X', 'Y', 'Z'))
                         for index in range(min_len):
-                            print((f"{data['Time'][index].isoformat():25s} "
-                                   f"{data['BGseX'][index]:9.6f} "
-                                   f"{data['BGseY'][index]:9.6f} "
-                                   f"{data['BGseZ'][index]:9.6f}"))
+                            print('{:25s} {:9.6f} {:9.6f} {:9.6f}'.format(\
+                                  data['Time'][index].isoformat(),\
+                                  data['BGseX'][index],\
+                                  data['BGseY'][index],\
+                                  data['BGseZ'][index]))
 
                 if 'NorthBTracedFootpointRegion' in data and \
                    'SouthBTracedFootpointRegion' in data:
 
                     min_len = min(len(data['Time']),
                                   len(data['NorthBTracedFootpointRegion']))
                     if min_len > 0:
                         print('                 B-Traced Footpoint Region')
                         print('Time                     ', 'North            ',
                               'South           ')
                         for index in range(min_len):
                             print(data['Time'][index],
                                   data['NorthBTracedFootpointRegion'][index].value,
                                   data['SouthBTracedFootpointRegion'][index].value)
-    # pylint: enable=too-many-branches
 
 
     @staticmethod
     def print_time_series(
             name: str,
             data: Dict
         ) -> None:
@@ -897,21 +810,22 @@
         print('StatusCode:', result['StatusCode'],
               'StatusSubCode:', result['StatusSubCode'])
         #print(result)
 
         for conjunction in result['Conjunction']:
             print(conjunction['TimeInterval']['Start'].isoformat(), 'to',
                   conjunction['TimeInterval']['End'].isoformat())
-            print((f"  {'Satellite':10s} {'Lat':>7s} {'Lon':>7s} "
-                   f"{'Radius':>9s} {'Ground Stations':20s} {'Lat':>7s} "
-                   f"{'Lon':>7s} {'ArcLen':>9s}"))
+            print('  {:10s} {:>7s} {:>7s} {:>9s} {:20s} {:>7s} {:>7s} {:>9s}'.format(\
+                  'Satellite', 'Lat', 'Lon', 'Radius',
+                  'Ground Station', 'Lat', 'Lon', 'ArcLen'))
             for sat in conjunction['SatelliteDescription']:
                 for description in sat['Description']:
                     trace = description['TraceDescription']
-                    print((f"  {sat['Satellite']:10s} "
-                           f"{description['Location']['Latitude']:7.2f} "
-                           f"{description['Location']['Longitude']:7.2f} "
-                           f"{description['Location']['Radius']:9.2f} "
-                           f"{trace['Target']['GroundStation']:20s} "
-                           f"{trace['Location']['Latitude']:7.2f} "
-                           f"{trace['Location']['Longitude']:7.2f} "
-                           f"{trace['ArcLength']:9.2f}"))
+                    print('  {:10s} {:7.2f} {:7.2f} {:9.2f} {:20s} {:7.2f} {:7.2f} {:9.2f}'.format(\
+                          sat['Satellite'],
+                          description['Location']['Latitude'],
+                          description['Location']['Longitude'],
+                          description['Location']['Radius'],
+                          trace['Target']['GroundStation'],
+                          trace['Location']['Latitude'],
+                          trace['Location']['Longitude'],
+                          trace['ArcLength']))
```

### Comparing `sscws-2.3.15/sscws/timeinterval.py` & `sscws-2.3.8/sscws/timeinterval.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2018-2023 United States Government as represented by
+# Copyright (c) 2018-2021 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 
 """
 Module defining a class to represent the TimeInterval class from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2018-2023 United States Government as represented by the
+Copyright &copy; 2018-2021 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
 
 import xml.etree.ElementTree as ET
 from datetime import datetime, timezone
@@ -194,16 +194,16 @@
             datetime_value = dateutil.parser.parse(value)
         else:
             raise ValueError('unrecognized datetime value')
 
         if datetime_value.tzinfo is None or \
            datetime_value.tzinfo.utcoffset(None) is None:
             return datetime_value.replace(tzinfo=timezone.utc)
-
-        return datetime_value.astimezone(timezone.utc)
+        else:
+            return datetime_value.astimezone(timezone.utc)
 
 
     @staticmethod
     def get_datetimes(
             start: Union[datetime, str],
             end: Union[datetime, str]
         ) -> Tuple[datetime, datetime]:
@@ -224,21 +224,21 @@
         Raises
         ------
         ValueError
             If either of the given values is not a valid datetime value.
         """
         try:
             start_datetime = TimeInterval.get_datetime(start)
-        except ValueError as exc:
-            raise ValueError('unrecognized start datetime value') from exc
+        except ValueError:
+            raise ValueError('unrecognized start datetime value')
 
         try:
             end_datetime = TimeInterval.get_datetime(end)
-        except ValueError as exc:
-            raise ValueError('unrecognized end datetime value') from exc
+        except ValueError:
+            raise ValueError('unrecognized end datetime value')
 
         return start_datetime, end_datetime
 
 
     @staticmethod
     def basic_iso_format(value: datetime) -> str:
         """
```

### Comparing `sscws-2.3.15/sscws/tracing.py` & `sscws-2.3.8/sscws/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2013-2023 United States Government as represented by
+# Copyright (c) 2013-2020 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 """
 Module defining classes to represent tracing classes from
 <https://sscweb.gsfc.nasa.gov/WebServices/REST/SSC.xsd>.<br>
 
-Copyright &copy; 2013-2023 United States Government as represented by the
+Copyright &copy; 2013-2020 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 """
 
-# pylint: disable=duplicate-code
-
 import xml.etree.ElementTree as ET
 from enum import Enum
 
 from sscws.regions import HemisphereRegions
 
 
 class BFieldTraceDirection(Enum):
```

### Comparing `sscws-2.3.15/sscws.egg-info/PKG-INFO` & `sscws-2.3.8/sscws.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscws
-Version: 2.3.15
+Version: 2.3.8
 Summary: NASA's Satellite Situation Center Web Service Client Library
 Home-page: https://sscweb.gsfc.nasa.gov/WebServices/REST
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Description: 
         ## Synopsis
@@ -20,32 +20,19 @@
         
         This package contains example code calling most of the available web services.
         To run the included example, do the following
         
             python -m sscws
         
         ---
-        
-        This 
-        ["Getting Started"](https://sscweb.gsfc.nasa.gov/WebServices/REST/py/GetStarted.html) 
-        page contains information to help someone begin using the sscws library to 
-        access information from the 
-        [Satellite Situation Center](https://sscweb.gsfc.nasa.gov/) in a Python program.
-        
-        ---
-        
         Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
         different features of the library:
         1. [Simple Location Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsExample.ipynb))demonstrating a simple 3D plot of orbit information.
         2. [Complex Location Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsBTraceExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsBTraceExample.ipynb)) requesting many values including magnetic field line tracing. This example also demonstrates how to diagnose a problem with an invalid request.
-        3. [Radial Conjunction With Ground Location](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsRadialConjunction.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsRadialConjunction.ipynb)).
-        4. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/).
-        
-        These notebooks are also available on 
-        [Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main).
+        3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/).
         
         ## Motivation
         
         This library hides the HTTP, JSON/XML, and CDF details of the SSC web 
         services. A python developer only has to deal with python objects and 
         methods.
         
@@ -94,15 +81,15 @@
         ## License
         
         This code is licensed under the 
         [NASA Open Source Agreement](https://sscweb.gsfc.nasa.gov/WebServices/NASA_Open_Source_Agreement_1.3.txt) (NOSA).
         
 Keywords: heliophysics,satellites,trajectories,orbits,location,conjunctions,earth magnetic field,ephemeris,space physics,spdf,ssc
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sscws-2.3.15/README.md` & `sscws-2.3.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,19 @@
 
 This package contains example code calling most of the available web services.
 To run the included example, do the following
 
     python -m sscws
 
 ---
-
-This 
-["Getting Started"](https://sscweb.gsfc.nasa.gov/WebServices/REST/py/GetStarted.html) 
-page contains information to help someone begin using the sscws library to 
-access information from the 
-[Satellite Situation Center](https://sscweb.gsfc.nasa.gov/) in a Python program.
-
----
-
 Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
 different features of the library:
 1. [Simple Location Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsExample.ipynb))demonstrating a simple 3D plot of orbit information.
 2. [Complex Location Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsBTraceExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsBTraceExample.ipynb)) requesting many values including magnetic field line tracing. This example also demonstrates how to diagnose a problem with an invalid request.
-3. [Radial Conjunction With Ground Location](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsRadialConjunction.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsRadialConjunction.ipynb)).
-4. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/).
-
-These notebooks are also available on 
-[Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main).
+3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/).
 
 ## Motivation
 
 This library hides the HTTP, JSON/XML, and CDF details of the SSC web 
 services. A python developer only has to deal with python objects and 
 methods.
```

### Comparing `sscws-2.3.15/setup.py` & `sscws-2.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="sscws",
-    version="2.3.15",
+    version="2.3.8",
     description="NASA's Satellite Situation Center Web Service Client Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://sscweb.gsfc.nasa.gov/WebServices/REST",
     author="Bernie Harris",
     author_email="NASA-SPDF-Support@nasa.onmicrosoft.com",
     license="NOSA",
@@ -25,15 +25,15 @@
 #    install_requires=["python-dateutil>=2.8.0", "requests>=2.20", "spacepy>=0.1.6"],
     install_requires=["python-dateutil>=2.8.0", "requests>=2.20", "numpy>=1.19.4"],
     extras_require={
         'plot': ["matplotlib>=3.3.2"],
     },
     keywords=["heliophysics", "satellites", "trajectories", "orbits", "location", "conjunctions", "earth magnetic field", "ephemeris", "space physics", "spdf", "ssc"],
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
 #        "License :: OSI Approved :: NASA Open Source Agreement",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `sscws-2.3.15/PKG-INFO` & `sscws-2.3.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscws
-Version: 2.3.15
+Version: 2.3.8
 Summary: NASA's Satellite Situation Center Web Service Client Library
 Home-page: https://sscweb.gsfc.nasa.gov/WebServices/REST
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Description: 
         ## Synopsis
@@ -20,32 +20,19 @@
         
         This package contains example code calling most of the available web services.
         To run the included example, do the following
         
             python -m sscws
         
         ---
-        
-        This 
-        ["Getting Started"](https://sscweb.gsfc.nasa.gov/WebServices/REST/py/GetStarted.html) 
-        page contains information to help someone begin using the sscws library to 
-        access information from the 
-        [Satellite Situation Center](https://sscweb.gsfc.nasa.gov/) in a Python program.
-        
-        ---
-        
         Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
         different features of the library:
         1. [Simple Location Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsExample.ipynb))demonstrating a simple 3D plot of orbit information.
         2. [Complex Location Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsBTraceExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsBTraceExample.ipynb)) requesting many values including magnetic field line tracing. This example also demonstrates how to diagnose a problem with an invalid request.
-        3. [Radial Conjunction With Ground Location](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsRadialConjunction.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsRadialConjunction.ipynb)).
-        4. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/).
-        
-        These notebooks are also available on 
-        [Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main).
+        3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/).
         
         ## Motivation
         
         This library hides the HTTP, JSON/XML, and CDF details of the SSC web 
         services. A python developer only has to deal with python objects and 
         methods.
         
@@ -94,15 +81,15 @@
         ## License
         
         This code is licensed under the 
         [NASA Open Source Agreement](https://sscweb.gsfc.nasa.gov/WebServices/NASA_Open_Source_Agreement_1.3.txt) (NOSA).
         
 Keywords: heliophysics,satellites,trajectories,orbits,location,conjunctions,earth magnetic field,ephemeris,space physics,spdf,ssc
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

