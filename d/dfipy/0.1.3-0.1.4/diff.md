# Comparing `tmp/dfipy-0.1.3.tar.gz` & `tmp/dfipy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-0.1.3.tar", max compression
+gzip compressed data, was "dfipy-0.1.4.tar", max compression
```

## Comparing `dfipy-0.1.3.tar` & `dfipy-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      557 2023-06-05 12:24:24.510120 dfipy-0.1.3/LICENCE
--rw-r--r--   0        0        0     1741 2023-06-05 12:24:24.510120 dfipy-0.1.3/README.md
--rw-r--r--   0        0        0      194 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/__init__.py
--rw-r--r--   0        0        0    16364 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/analysis.py
--rw-r--r--   0        0        0     4631 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/connection.py
--rw-r--r--   0        0        0    25259 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/getters.py
--rw-r--r--   0        0        0     1537 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/logging.py
--rw-r--r--   0        0        0    15871 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/show.py
--rw-r--r--   0        0        0     5566 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/stream.py
--rw-r--r--   0        0        0     1994 2023-06-05 12:24:25.394132 dfipy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 dfipy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      568 2023-06-09 11:22:46.249829 dfipy-0.1.4/LICENCE
+-rw-r--r--   0        0        0     1753 2023-06-09 11:22:46.249829 dfipy-0.1.4/README.md
+-rw-r--r--   0        0        0      194 2023-06-09 11:22:46.249829 dfipy-0.1.4/dfi/__init__.py
+-rw-r--r--   0        0        0    16347 2023-06-09 11:22:46.249829 dfipy-0.1.4/dfi/analysis.py
+-rw-r--r--   0        0        0     4631 2023-06-09 11:22:46.249829 dfipy-0.1.4/dfi/connection.py
+-rw-r--r--   0        0        0    26566 2023-06-09 11:22:46.249829 dfipy-0.1.4/dfi/getters.py
+-rw-r--r--   0        0        0    14461 2023-06-09 11:22:46.249829 dfipy-0.1.4/dfi/show.py
+-rw-r--r--   0        0        0     5548 2023-06-09 11:22:46.249829 dfipy-0.1.4/dfi/stream.py
+-rw-r--r--   0        0        0     1970 2023-06-09 11:22:47.273846 dfipy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 dfipy-0.1.4/PKG-INFO
```

### Comparing `dfipy-0.1.3/LICENCE` & `dfipy-0.1.4/LICENCE`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 generalsystem.com
+Copyright 2023 General System Group Limited
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dfipy-0.1.3/README.md` & `dfipy-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 
 - [DfiPyDocs](https://gitlab.com/excession/software/dfi/public-examples/DfiPyDocs)
   
 - [DfiPyExamples](https://gitlab.com/excession/software/dfi/public-examples/DfiPyExamples)
 
 ## Licence
 
-- Copyright (c) 2023, generalsystem.com
+- Copyright (c) 2023, General System Group Limited.
 
 - DFIPy is provided as it is and copyrighted under [Apache2 License](LICENCE).
 
 - DFIPy is currently released on public pypi in beta, strictly for testing and evaluation purposes.
```

### Comparing `dfipy-0.1.3/dfi/analysis.py` & `dfipy-0.1.4/dfi/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Class with DFI analytic methods, leveraging on the python api wrappers to gain analytical informations.
 Composition of the class DFIConnection.
 """
 
+import logging
 from datetime import datetime, timedelta
 from functools import partial
 from typing import List, Optional, Tuple
 
 import branca  # pylint: disable=import-error
 import geopandas as gpd
 import h3.api.numpy_int as h3
@@ -14,17 +15,16 @@
 import pandas as pd
 from shapely.geometry import Polygon
 from shapely.wkt import loads
 from tqdm import tqdm
 
 from dfi.connection import DFIConnect
 from dfi.getters import DFIGet
-from dfi.logging import setup_logger
 
-logger = setup_logger(__file__)
+logger = logging.getLogger(__name__)
 
 # TODO: rename pings to records everywhere (records are used in colocated_records and pings
 # everywhere else).
 # TODO: remanme history to historical_records?
 # TODO: remove ipython from the list of requirements, as not needed for the
 # library, and can causes conflicts with colab.
```

### Comparing `dfipy-0.1.3/dfi/connection.py` & `dfipy-0.1.4/dfi/connection.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.3/dfi/getters.py` & `dfipy-0.1.4/dfi/getters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Class with DFI getters, srappers of the DFI python API.
 Composition of the class DFIConnection.
 """
 
 import json
+import logging
 from datetime import datetime
 from typing import List, Optional
 
 import pandas as pd
 import requests
 from requests.exceptions import ConnectionError as RequestsConnectionError
 from tqdm import tqdm
 
 from dfi import stream
 from dfi.connection import DFIConnect
-from dfi.logging import setup_logger
 
-logger = setup_logger(__file__)
+logger = logging.getLogger(__name__)
 
 
 # TODO: rename uid to device_id and uid to list_device_ids?
 
 # TODO (Robert): count() & entities() - these functions only take as parameters, start_time and end_time,
 # there’s no argument for polygon or vertices or bbox.  There are polygon_count() and polygon_entities()
 # which appear to be the same but can add a polygon filter.
@@ -90,22 +90,23 @@
 
     def api_version(self) -> str:
         """
         Version of the Data Flow Index.
         """
         my_url = f"{self.dfi_conn.base_url}/version"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.get(
+
+        with requests.get(
             url=my_url,
             headers=my_headers,
-            stream=True,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, {})
-        return response.text
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, {})
+            return response.text
 
     def count(self, start_time: Optional[datetime] = None, end_time: Optional[datetime] = None) -> int:
         """
         Returns the number of records stored in the DFI engine with an optional time constraint.
 
         Parameters
         ----------
@@ -125,23 +126,24 @@
         my_params = {"instance": self.dfi_conn.qualified_instance_name}
         if start_time is not None:
             my_params["startTime"] = start_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         if end_time is not None:
             my_params["endTime"] = end_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         my_url = f"{self.dfi_conn.base_url}/count"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.get(
+
+        with requests.get(
             url=my_url,
             headers=my_headers,
-            stream=True,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params)
-        return stream.receive_count(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params)
+            return stream.receive_count(response, self.dfi_conn.progress_bar)
 
     def entities(self, start_time: Optional[datetime] = None, end_time: Optional[datetime] = None) -> int:
         """
         Returns the number of entities stored in the DFI engine with an optional time constraint.
 
         Parameters
         ----------
@@ -161,23 +163,24 @@
         my_params = {"instance": self.dfi_conn.qualified_instance_name}
         if start_time is not None:
             my_params["startTime"] = start_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         if end_time is not None:
             my_params["endTime"] = end_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         my_url = f"{self.dfi_conn.base_url}/entities"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.get(
+
+        with requests.get(
             my_url,
             headers=my_headers,
-            stream=True,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params)
-        return stream.receive_entities(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params)
+            return stream.receive_entities(response, self.dfi_conn.progress_bar)
 
     def entity_count(self, uid: str, start_time: Optional[datetime] = None, end_time: Optional[datetime] = None) -> int:
         """
         Count the records for a given uid, with the optional time interval constraint.
 
         Parameters
         ----------
@@ -199,23 +202,24 @@
         my_params = {"instance": self.dfi_conn.qualified_instance_name}
         if start_time is not None:
             my_params["startTime"] = start_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         if end_time is not None:
             my_params["endTime"] = end_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         my_url = f"{self.dfi_conn.base_url}/entities/{uid}/count"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.get(
+
+        with requests.get(
             my_url,
             headers=my_headers,
-            stream=True,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params)
-        return stream.receive_count(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params)
+            return stream.receive_count(response, self.dfi_conn.progress_bar)
 
     def polygon_count(
         self,
         polygon: Optional[str] = None,
         vertices: Optional[List[List[float]]] = None,
         include_list: Optional[List[any]] = None,
         start_time: Optional[datetime] = None,
@@ -268,24 +272,25 @@
             return
         if polygon is not None:
             my_payload["name"] = polygon
         if vertices is not None:
             my_payload["vertices"] = vertices
         my_url = f"{self.dfi_conn.base_url}/polygon/count"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.post(
+
+        with requests.post(
             my_url,
             headers=my_headers,
-            stream=True,
             json=my_payload,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params)
-        return stream.receive_count(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params)
+            return stream.receive_count(response, self.dfi_conn.progress_bar)
 
     def polygon_entities(
         self,
         polygon: str = None,
         vertices: List[List[float]] = None,
         include_list: List[any] = None,
         start_time: datetime = None,
@@ -338,24 +343,25 @@
             return
         if polygon is not None:
             my_payload["name"] = polygon
         if vertices is not None:
             my_payload["vertices"] = vertices
         my_url = f"{self.dfi_conn.base_url}/polygon/entities"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.post(
+
+        with requests.post(
             my_url,
             headers=my_headers,
-            stream=True,
             json=my_payload,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params, my_payload)
-        return stream.receive_entities(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params, my_payload)
+            return stream.receive_entities(response, self.dfi_conn.progress_bar)
 
     def polygon_history(
         self,
         polygon: str = None,
         vertices: List[List[float]] = None,
         include_list: List[any] = None,
         start_time: Optional[datetime] = None,
@@ -414,24 +420,26 @@
             logger.warning("You cannot specify both Polygon and Vertices. Pick one")
             return
         if polygon is not None:
             my_payload["name"] = polygon
         if vertices is not None:
             my_payload["vertices"] = vertices
         my_url = f"{self.dfi_conn.base_url}/polygon/history"
-        response = requests.post(
+
+        with requests.post(
             my_url,
             headers=self.dfi_conn.streaming_headers,
-            stream=True,
             json=my_payload,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, self.dfi_conn.streaming_headers, my_params, my_payload)
-        data = stream.receive_history(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, self.dfi_conn.streaming_headers, my_params, my_payload)
+            data = stream.receive_history(response, self.dfi_conn.progress_bar)
+
         data_formatted = []
         for item in data:
             if parse_payload_as_json:
                 try:
                     payload = json.loads(item["payload"])
                 except Exception as err:
                     payload = {}
@@ -492,23 +500,25 @@
         my_params = {"instance": self.dfi_conn.qualified_instance_name}
         if start_time is not None:
             my_params["startTime"] = start_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         if end_time is not None:
             my_params["endTime"] = end_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         my_url = f"{self.dfi_conn.base_url}/entities/{uid}/history"
         my_headers = self.dfi_conn.streaming_headers
-        response = requests.get(
+
+        with requests.get(
             my_url,
             headers=my_headers,
-            stream=True,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params)
-        data = stream.receive_history(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params)
+            data = stream.receive_history(response, self.dfi_conn.progress_bar)
+
         logger.debug("Uid: %s \nHistory length: %i", uid, len(data))
         data_formatted = []
         for item in data:
             if parse_payload_as_json:
                 try:
                     payload = json.loads(item["payload"])
                 except Exception as err:
@@ -593,31 +603,67 @@
         my_payload = {
             "vertices": polygon_vertices,
             "startTime": min_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ"),
             "endTime": max_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ"),
         }
         my_headers = self.dfi_conn.streaming_headers
         my_params = {"instance": f"{self.dfi_conn.namespace}.{self.dfi_conn.instance_name}"}
-        response = requests.post(
+
+        with requests.post(
             my_url,
             json=my_payload,
             headers=my_headers,
-            stream=True,
             params=my_params,
             timeout=self.dfi_conn.query_timeout,
-        )
-        self._check_response(response, my_url, my_headers, my_params, my_payload)
-        data = stream.receive_history(response, self.dfi_conn.progress_bar)
+            stream=True,
+        ) as response:
+            self._check_response(response, my_url, my_headers, my_params, my_payload)
+            data = stream.receive_history(response, self.dfi_conn.progress_bar)
+
         if data is None:
             logger.warning("Query Error. Vertices: %s", str(polygon_vertices))
             data = []
         data = [
             {
                 "hex_id": hex_id,
                 "entity_id": x["id"],
                 "timestamp": datetime.strptime(x["time"], "%Y-%m-%dT%H:%M:%S.%fZ"),
                 "longitude": x["coordinate"][0],
                 "latitude": x["coordinate"][1],
             }
             for x in data
         ]
         return data
+
+    def retrieve_saved_polygon(self, polygon_name: str) -> List[List[float]]:
+        """
+        Get the list of a polygon saved in the polygon database from its name.
+
+        Parameters
+        ----------
+        polygon_name: str
+            Name of the polygon the user wants to retrieve from database.
+
+        Return
+        -------
+            List of the polygon coordinates.
+        """
+        # TODO: check if it is (lat, lon) or (lon, lat) and add to the docstring.
+        # It should be lon, lat. Make sure this is the convention we want the user to be
+        # exposed to.
+        url = self.dfi_conn.base_url + "/polygons/" + polygon_name
+        headers = self.dfi_conn.synchronous_headers
+
+        response = requests.get(
+            url,
+            headers=headers,
+            timeout=self.dfi_conn.query_timeout,
+        )
+        self._check_response(response, url, headers, params={})
+        vertices = response.json().get("vertices")
+
+        if vertices is not None:
+            return vertices
+
+        msg = f"Polygon vertices can not be retrieved from the json response: {response.json()}"
+        logger.error(msg)
+        raise IOError(msg)
```

### Comparing `dfipy-0.1.3/dfi/show.py` & `dfipy-0.1.4/dfi/show.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Class with methods to show DFI results.
 Composition of the class DFIConnection.
 """
 
 import json
+import logging
 from typing import List, Optional
 
 import pandas as pd
 import pydeck as pdk
 import pyperclip
-import requests
 from IPython.display import IFrame  # pylint: disable=import-error
 
 from dfi.connection import DFIConnect
-from dfi.logging import setup_logger
+from dfi.getters import DFIGet
+
+logger = logging.getLogger(__name__)
 
-logger = setup_logger(__file__)
 
 # TODO: find a way to avoid importing IPython and removing
 # ipython from requirements.
 # TODO: why not using KeplerGl as industry standard? Passing polygons via copy paste
 # is not ideal, or via passing html code is not ideal. Kepler has the methods to draw
 # map out of the box. A lightweigth alternative to kepler is https://leafmap.org/
 # also having the draw polygon option out of the box.
@@ -40,70 +41,46 @@
     """
     Visualisation methods to build use case on top of the queries from DFI.
     Not part of the DFI API wrapper, but handy to have it embedded there for demo and functionalities.
     """
 
     def __init__(self, dfi_conn: DFIConnect) -> None:
         self.dfi_conn: DFIConnect = dfi_conn
+        self.dfi_get: DFIGet = DFIGet(self.dfi_conn)
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.dfi_conn!r}){self.__dict__}"
 
     def __str__(self):
         return f"""DFI Python API: instance of {self.__class__.__name__} composed with {self.dfi_conn!r}"""
 
-    @staticmethod
-    def _check_response(response: requests.Response, url: str, headers: dict):
-        """Log the response of a request with the given parameters. Raise an error if status code is not 20x."""
-        # prevent from showing the user token to terminal and logs
-        headers = headers.copy()
-        headers["X-API-TOKEN"] = "Bearer XXX"
-
-        msg = f"""Response status code {response.status_code}.
-Query URL: {url},
-HEADER: {json.dumps(headers, sort_keys=True, indent=4)},
-Text: {json.dumps(json.loads(response.text), sort_keys=True, indent=4)}
-"""
-        if int(response.status_code / 10) != 20:
-            logger.error(msg)
-            raise ConnectionError(msg)
-        else:
-            logger.debug(msg)
-
     def heatmap(
         self,
-        query_polygons: List[str] = None,
+        query_polygons: List[str] = None,  # TODO: maybe calling this polygon_names could help.
         vertices: List[List[float]] = None,
         df_history: pd.DataFrame = None,
         df_hexagons: pd.DataFrame = None,
         df_colocs: pd.DataFrame = None,
         view_state=None,
         color_gradient: bool = True,
     ) -> pdk.Deck:
         """
         Helper method to create a heatmap from the components of a range of queries.
         """
         layers = []
 
         if query_polygons is not None:
             for query_polygon in query_polygons:
-                my_url = self.dfi_conn.base_url + "/polygons/" + query_polygon
-                my_headers = self.dfi_conn.synchronous_headers
-                response = requests.get(
-                    my_url,
-                    headers=my_headers,
-                    timeout=self.dfi_conn.query_timeout,
-                )
-                self._check_response(response, my_url, my_headers)
+                list_vertices = self.dfi_get.retrieve_saved_polygon(query_polygon)
+                geojson_poly = _create_geojson_from_coordinates(list_vertices)
 
-                geojson = _create_geojson_from_coordinates(response.json()["vertices"])
                 # return geoJSON
                 geojson_pdk = pdk.Layer(
                     "GeoJsonLayer",
-                    geojson,
+                    geojson_poly,
                     opacity=0.2,
                     stroked=True,
                     filled=True,
                     extruded=False,
                     wireframe=True,
                     get_elevation="0",
                     get_fill_color="[255, 255, 0]",
@@ -271,31 +248,21 @@
                 get_line_color=[255, 0, 0],
                 coverage=1,
             )
             layers.append(pdk_df_history)
 
         if query_polygons is not None:
             for query_polygon in query_polygons:
-                my_url = self.dfi_conn.base_url + "/polygons/" + query_polygon
-                my_headers = self.dfi_conn.synchronous_headers
-
-                # TODO: this should be part of the getters method, as it is not reponsibility of
-                # the DFIShow class to submit requests.
-                response = requests.get(
-                    my_url,
-                    headers=my_headers,
-                    timeout=self.dfi_conn.query_timeout,
-                )
-                self._check_response(response, my_url, my_headers)
+                list_vertices = self.dfi_get.retrieve_saved_polygon(query_polygon)
+                geojson_poly = _create_geojson_from_coordinates(list_vertices)
 
-                geojson = _create_geojson_from_coordinates(response.json()["vertices"])
                 # return geoJSON
                 geojson_pdk = pdk.Layer(
                     "GeoJsonLayer",
-                    geojson,
+                    geojson_poly,
                     opacity=0.2,
                     stroked=True,
                     filled=True,
                     extruded=False,
                     wireframe=True,
                     get_elevation="0",
                     get_fill_color="[255, 255, 0]",
```

### Comparing `dfipy-0.1.3/dfi/stream.py` & `dfipy-0.1.4/dfi/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Auxiliary methods for streamed data.
 """
 
 import json
+import logging
 from time import sleep
 from typing import List
 
 import requests
 import sseclient  # pylint: disable=import-error
 from tqdm import tqdm
 
-from dfi.logging import setup_logger
-
-logger = setup_logger(__file__)
+logger = logging.getLogger(__name__)
 
 
 # TODO: the need of split this function in 3 different ones shows some problem in the API.
 # Refactor into one, possibly with one decorator with the progress bar on its own.
 # TODO: the 0.1 second sleep is masking the "real" speed and should be avoided.
 
 # TODO (Robert): stream.receive_entities() - the progress bar updates fairly infrequently due
```

### Comparing `dfipy-0.1.3/pyproject.toml` & `dfipy-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,27 +60,26 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "0.1.3"
+version = "0.1.4"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@excession.co>",
   "Sebastiano Ferraris <sebastiano.ferraris@excession.co>",
 ]
 readme = "README.md"
 include = ["LICENCE"]
 packages = [{ include = "dfi" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-coloredlogs = "^15.0.1"
 h3 = "^3.7.6"
 pandas = "^2.0.1"
 pydeck = "^0.8.0"
 requests = "^2.30.0"
 shapely = "^2.0.1"
 sseclient-py = "^1.7.2"
 tqdm = "^4.65.0"
```

### Comparing `dfipy-0.1.3/PKG-INFO` & `dfipy-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: DFI api python wrapper
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@excession.co
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: branca (>=0.6.0,<0.7.0)
-Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: geopandas (>=0.13.0,<0.14.0)
 Requires-Dist: h3 (>=3.7.6,<4.0.0)
 Requires-Dist: ipython (==7.31.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
@@ -50,13 +49,13 @@
 
 - [DfiPyDocs](https://gitlab.com/excession/software/dfi/public-examples/DfiPyDocs)
   
 - [DfiPyExamples](https://gitlab.com/excession/software/dfi/public-examples/DfiPyExamples)
 
 ## Licence
 
-- Copyright (c) 2023, generalsystem.com
+- Copyright (c) 2023, General System Group Limited.
 
 - DFIPy is provided as it is and copyrighted under [Apache2 License](LICENCE).
 
 - DFIPy is currently released on public pypi in beta, strictly for testing and evaluation purposes.
```

