# Comparing `tmp/mindsight_people_control_api-0.1.2.tar.gz` & `tmp/mindsight_people_control_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsight_people_control_api-0.1.2.tar", max compression
+gzip compressed data, was "mindsight_people_control_api-0.1.3.tar", max compression
```

## Comparing `mindsight_people_control_api-0.1.2.tar` & `mindsight_people_control_api-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,23 @@
--rw-r--r--   0        0        0      614 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/helpers/__init__.py
--rw-r--r--   0        0        0     6434 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/helpers/base_requests.py
--rw-r--r--   0        0        0      392 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/helpers/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/__init__.py
--rw-r--r--   0        0        0     3813 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/area_records.py
--rw-r--r--   0        0        0     6692 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/areas.py
--rw-r--r--   0        0        0     8857 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/employees.py
--rw-r--r--   0        0        0     7658 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/users.py
--rw-r--r--   0        0        0      690 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/settings.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/utils/__init__.py
--rw-r--r--   0        0        0      308 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/mindsight_people_control_api/utils/aux_functions.py
--rw-r--r--   0        0        0      391 2023-06-08 16:51:55.754569 mindsight_people_control_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1342 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/README.md
+-rw-r--r--   0        0        0      407 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/helpers/__init__.py
+-rw-r--r--   0        0        0     5225 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/helpers/base_requests.py
+-rw-r--r--   0        0        0      392 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/helpers/exceptions.py
+-rw-r--r--   0        0        0     1869 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/helpers/models.py
+-rw-r--r--   0        0        0      783 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/__init__.py
+-rw-r--r--   0        0        0     4566 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/area_records.py
+-rw-r--r--   0        0        0     7415 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/areas.py
+-rw-r--r--   0        0        0     5513 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/employee_areas.py
+-rw-r--r--   0        0        0     5591 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/employee_managers.py
+-rw-r--r--   0        0        0     5623 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/employee_positions.py
+-rw-r--r--   0        0        0     4896 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/employee_records.py
+-rw-r--r--   0        0        0    12367 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/employees.py
+-rw-r--r--   0        0        0     4721 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/parent_areas.py
+-rw-r--r--   0        0        0     7060 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/positions.py
+-rw-r--r--   0        0        0     7654 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/users.py
+-rw-r--r--   0        0        0      843 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/settings.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/utils/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/mindsight_people_control_api/utils/aux_functions.py
+-rw-r--r--   0        0        0      542 2023-06-09 00:40:05.630109 mindsight_people_control_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.3/PKG-INFO
```

### Comparing `mindsight_people_control_api-0.1.2/mindsight_people_control_api/helpers/base_requests.py` & `mindsight_people_control_api-0.1.3/mindsight_people_control_api/helpers/base_requests.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,60 +5,20 @@
 import requests
 
 from mindsight_people_control_api.helpers.exceptions import BadRequestException
 from mindsight_people_control_api.settings import API_TOKEN, TIMEOUT
 from mindsight_people_control_api.utils.aux_functions import generate_url
 
 
-class ApiPaginationResponse:
-    """Class to work with paginated responses"""
-
-    results: list = []
-
-    def __init__(
-        self,
-        count: int,
-        previous: str = None,
-        results: list = None,
-        headers: dict = None,
-        **kwargs,
-    ) -> None:
-        self.count = count
-        self.next = kwargs.get("next")
-        self.previous = previous
-        self.results.extend(results if results else [])
-        self.__headers = headers
-
-    def get_all(self):
-        """Get all pages of data"""
-        if self.next:
-            response = requests.get(
-                url=self.next, headers=self.__headers, timeout=TIMEOUT
-            )
-
-            response.raise_for_status()
-            response_data = response.json()
-
-            self.results.extend(response_data["results"])
-            self.count = response_data["count"]
-            self.next = response_data["next"]
-            self.previous = response_data["previous"]
-
-            if self.next:
-                self.get_all()
-
-        return self
-
-
 class BaseRequests:
     """Aux class to communicate with mindsight api"""
 
     def __init__(self):
         self.__token = API_TOKEN
-        self.__headers = None
+        self.headers = None
         self.base_path = "/"
 
     def __authorization_header(self) -> dict:
         return {
             "Authorization": f"Token {self.__token}",
             "Content-Type": "application/json",
         }
@@ -96,76 +56,73 @@
         data: Any = None,
         json: Any = None,
     ):
         if not headers:
             headers = {}
 
         request_url = generate_url(base_path=self.base_path, path=path)
-        self.__headers = {**self.__authorization_header(), **headers}
+        self.headers = {**self.__authorization_header(), **headers}
 
         response = None
         method = method.lower()
 
         if method == "get":
             response = requests.get(
                 url=request_url,
-                headers=self.__headers,
+                headers=self.headers,
                 params=parameters,
                 data=data,
                 timeout=TIMEOUT,
             )
 
         elif method == "post":
             response = requests.post(
                 url=request_url,
-                headers=self.__headers,
+                headers=self.headers,
                 params=parameters,
                 data=data,
                 json=json,
                 timeout=TIMEOUT,
             )
 
         elif method == "put":
             response = requests.put(
                 url=request_url,
-                headers=self.__headers,
+                headers=self.headers,
                 params=parameters,
                 data=data,
                 json=json,
                 timeout=TIMEOUT,
             )
 
         elif method == "patch":
             response = requests.patch(
                 url=request_url,
-                headers=self.__headers,
+                headers=self.headers,
                 params=parameters,
                 data=data,
                 json=json,
                 timeout=TIMEOUT,
             )
 
         elif method == "delete":
             response = requests.delete(
                 url=request_url,
-                headers=self.__headers,
+                headers=self.headers,
                 params=parameters,
                 data=data,
                 json=json,
                 timeout=TIMEOUT,
             )
 
         # Check response
         self.__check_response(response)
 
         response_json = response.json()
 
-        if response_json.get("count") and response_json.get("next"):
-            return ApiPaginationResponse(**response_json, headers=self.__headers)
-
         return response_json
 
     def get(
         self,
         path: str,
         headers: dict = None,
         parameters: dict = None,
```

### Comparing `mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/area_records.py` & `mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/parent_areas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,129 @@
 """This module provide methods to work with areas records entity"""
+from datetime import datetime
 
-from mindsight_people_control_api.helpers.base_requests import (
+from mindsight_people_control_api.helpers.models import (
+    ApiEndpoint,
     ApiPaginationResponse,
-    BaseRequests,
 )
-from mindsight_people_control_api.settings import API_ENDPOINT_AREAS_RECORDS, PAGE_SIZE
+from mindsight_people_control_api.settings import (
+    API_ENDPOINT_AREAS,
+    API_ENDPOINT_PARENT_AREAS,
+    DATETIME_FORMAT,
+)
+from mindsight_people_control_api.utils.aux_functions import generate_url
 
 
-class AreaRecords:
+class ParentAreas(ApiEndpoint):
     """This class abstract the areas records endpoint methods
-    Reference: https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Registros-de-area
+    Reference: https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Areas-pai
     """
 
-    base_requests = BaseRequests()
-
     def __init__(self) -> None:
-        self.base_requests.base_path = API_ENDPOINT_AREAS_RECORDS
-        self.page_size = PAGE_SIZE
+        super().__init__(API_ENDPOINT_PARENT_AREAS)
 
-    def get_list_area_records(
+    def get_list_parent_areas(
         self,
-        area: str = None,
-        code: str = None,
-        created__gt: str = None,
-        created__lt: str = None,
-        modified__gt: str = None,
-        modified__lt: str = None,
+        area_id: int = None,
+        created__gt: datetime = None,
+        created__lt: datetime = None,
+        modified__gt: datetime = None,
+        modified__lt: datetime = None,
         search: str = None,
     ) -> ApiPaginationResponse:
         """Get areas data
         Reference:
-            https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Registros-de-area/operation/listAreaRecords
+            https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Areas-pai/operation/listParentAreas
 
         Args:
-            area (str, Optional): Area name
-            code (str, Optional): Code of area
-            created__gt (str, Optional): Datetime to apply filter ">=" on created dates.
+            area_id (int, Optional): Area id
+            created__gt (datetime, Optional): Datetime to apply filter ">=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            created__lt (str, Optional): Datetime to apply filter "<=" on created dates.
+            created__lt (datetime, Optional): Datetime to apply filter "<=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            modified__gt (str, Optional): Datetime to apply filter ">=" on modified dates.
+            modified__gt (datetime, Optional): Datetime to apply filter ">=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            modified__lt (str, Optional): Datetime to apply filter "<=" on modified dates.
+            modified__lt (datetime, Optional): Datetime to apply filter "<=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
             search: search
         """
 
         path = ""
         parameters = {
-            "area": area,
-            "code": code,
-            "created__gt": created__gt,
-            "created__lt": created__lt,
-            "modified__gt": modified__gt,
-            "modified__lt": modified__lt,
+            "area": (
+                generate_url(base_path=API_ENDPOINT_AREAS, path=f"/{area_id}")
+                if area_id
+                else None
+            ),
+            "created__gt": created__gt.strftime(DATETIME_FORMAT)
+            if created__gt
+            else None,
+            "created__lt": created__lt.strftime(DATETIME_FORMAT)
+            if created__lt
+            else None,
+            "modified__gt": modified__gt.strftime(DATETIME_FORMAT)
+            if modified__gt
+            else None,
+            "modified__lt": modified__lt.strftime(DATETIME_FORMAT)
+            if modified__lt
+            else None,
             "search": search,
             "page_size": self.page_size,
         }
-        return self.base_requests.get(path=path, parameters=parameters)
+        return ApiPaginationResponse(
+            **self._base_requests.get(path=path, parameters=parameters),
+            headers=self._base_requests.headers,
+        )
 
-    def get_retrieve_area_record(
+    def get_retrieve_parent_area(
         self,
         _id: int,
-        area: str = None,
-        code: str = None,
-        created__gt: str = None,
-        created__lt: str = None,
-        modified__gt: str = None,
-        modified__lt: str = None,
+        area_id: int = None,
+        created__gt: datetime = None,
+        created__lt: datetime = None,
+        modified__gt: datetime = None,
+        modified__lt: datetime = None,
         search: str = None,
     ) -> dict:
-        """Get retrieve area
+        """Get retrieve parent area record
         Reference:
-            https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Registros-de-area/operation/retrieveAreaRecord
+            https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Areas-pai/operation/retrieveParentArea
 
         Args:
-            _id (int, Mandatory): A unique integer value identifying this record of area.
-            area (str, Optional): Area name
-            code (str, Optional): Code of area
+            _id (int, Mandatory): A unique integer value identifying parent area record.
+            area_id (str, Optional): Area id
             created__gt (str, Optional): Datetime to apply filter ">=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
             created__lt (str, Optional): Datetime to apply filter "<=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
             modified__gt (str, Optional): Datetime to apply filter ">=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
             modified__lt (str, Optional): Datetime to apply filter "<=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
             search (str, Optional): search
         """
         path = f"/{_id}"
 
         parameters = {
-            "area": area,
-            "code": code,
-            "created__gt": created__gt,
-            "created__lt": created__lt,
-            "modified__gt": modified__gt,
-            "modified__lt": modified__lt,
+            "area": (
+                generate_url(base_path=API_ENDPOINT_AREAS, path=area_id)
+                if area_id
+                else None
+            ),
+            "created__gt": created__gt.strftime(DATETIME_FORMAT)
+            if created__gt
+            else None,
+            "created__lt": created__lt.strftime(DATETIME_FORMAT)
+            if created__lt
+            else None,
+            "modified__gt": modified__gt.strftime(DATETIME_FORMAT)
+            if modified__gt
+            else None,
+            "modified__lt": modified__lt.strftime(DATETIME_FORMAT)
+            if modified__lt
+            else None,
             "search": search,
         }
-        return self.base_requests.get(
+        return self._base_requests.get(
             path=path,
             parameters=parameters,
         )
```

### Comparing `mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/areas.py` & `mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/areas.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,121 +1,137 @@
 """This module provide methods to work with areas entity"""
 
-from datetime import date
+from datetime import date, datetime
 
-from mindsight_people_control_api.helpers.base_requests import (
+from mindsight_people_control_api.helpers.models import (
+    ApiEndpoint,
     ApiPaginationResponse,
-    BaseRequests,
 )
 from mindsight_people_control_api.settings import (
     API_ENDPOINT_AREAS,
     DATE_FORMAT,
-    PAGE_SIZE,
+    DATETIME_FORMAT,
 )
 
 
-class Areas:
+class Areas(ApiEndpoint):
     """This class abstract the areas endpoint methods
     Reference: https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Areas
     """
 
-    base_requests = BaseRequests()
-
     def __init__(self) -> None:
-        self.base_requests.base_path = API_ENDPOINT_AREAS
-        self.page_size = PAGE_SIZE
+        super().__init__(API_ENDPOINT_AREAS)
 
     def get_list_areas(
         self,
         name: str = None,
         code: str = None,
-        created__gt: str = None,
-        created__lt: str = None,
-        modified__gt: str = None,
-        modified__lt: str = None,
+        created__gt: datetime = None,
+        created__lt: datetime = None,
+        modified__gt: datetime = None,
+        modified__lt: datetime = None,
         active: str = None,
         search: str = None,
     ) -> ApiPaginationResponse:
         """Get areas data
         Reference: https://controle.mindsight.com.br/stone/api/v1/docs/#operation/listAreas
 
         Args:
             name (str, Optional): area_name
             code (str, Optional): Code of area
-            created__gt (str, Optional): Datetime to apply filter ">=" on created dates.
+            created__gt (datetime, Optional): Datetime to apply filter ">=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            created__lt (str, Optional): Datetime to apply filter "<=" on created dates.
+            created__lt (datetime, Optional): Datetime to apply filter "<=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            modified__gt (str, Optional): Datetime to apply filter ">=" on modified dates.
+            modified__gt (datetime, Optional): Datetime to apply filter ">=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            modified__lt (str, Optional): Datetime to apply filter "<=" on modified dates.
+            modified__lt (datetime, Optional): Datetime to apply filter "<=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
             active (str, Optional): is_active: Flag to get areas by status
             search: search
             }
         """
 
         path = ""
         parameters = {
             "name": name,
             "code": code,
-            "created__gt": created__gt,
-            "created__lt": created__lt,
-            "modified__gt": modified__gt,
-            "modified__lt": modified__lt,
+            "created__gt": created__gt.strftime(DATETIME_FORMAT)
+            if created__gt
+            else None,
+            "created__lt": created__lt.strftime(DATETIME_FORMAT)
+            if created__lt
+            else None,
+            "modified__gt": modified__gt.strftime(DATETIME_FORMAT)
+            if modified__gt
+            else None,
+            "modified__lt": modified__lt.strftime(DATETIME_FORMAT)
+            if modified__lt
+            else None,
             "active": active,
             "search": search,
             "page_size": self.page_size,
         }
-        return self.base_requests.get(path=path, parameters=parameters)
+        return ApiPaginationResponse(
+            **self._base_requests.get(path=path, parameters=parameters),
+            headers=self._base_requests.headers,
+        )
 
     def get_retrieve_area(
         self,
         _id: int,
         name: str = None,
         code: str = None,
-        created__gt: str = None,
-        created__lt: str = None,
-        modified__gt: str = None,
-        modified__lt: str = None,
+        created__gt: datetime = None,
+        created__lt: datetime = None,
+        modified__gt: datetime = None,
+        modified__lt: datetime = None,
         active: str = None,
         search: str = None,
     ) -> dict:
         """Get retrieve area
         Reference:
             https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Areas/operation/retrieveArea
 
         Args:
             _id (int, Mandatory): Id of area to retrieve
             name (str, Optional): Name of area
             code (str, Optional): Code of area
-            created__gt (str, Optional): Datetime to apply filter ">=" on created dates.
+            created__gt (datetime, Optional): Datetime to apply filter ">=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            created__lt (str, Optional): Datetime to apply filter "<=" on created dates.
+            created__lt (datetime, Optional): Datetime to apply filter "<=" on created dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            modified__gt (str, Optional): Datetime to apply filter ">=" on modified dates.
+            modified__gt (datetime, Optional): Datetime to apply filter ">=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
-            modified__lt (str, Optional): Datetime to apply filter "<=" on modified dates.
+            modified__lt (datetime, Optional): Datetime to apply filter "<=" on modified dates.
                 Format "%Y-%m-%d %H:%M:%S"
             active (str, Optional): is_active: Flag to get areas by status
             search (str, Optional): search
         """
         path = f"/{_id}"
 
         parameters = {
             "name": name,
             "code": code,
-            "created__gt": created__gt,
-            "created__lt": created__lt,
-            "modified__gt": modified__gt,
-            "modified__lt": modified__lt,
+            "created__gt": created__gt.strftime(DATETIME_FORMAT)
+            if created__gt
+            else None,
+            "created__lt": created__lt.strftime(DATETIME_FORMAT)
+            if created__lt
+            else None,
+            "modified__gt": modified__gt.strftime(DATETIME_FORMAT)
+            if modified__gt
+            else None,
+            "modified__lt": modified__lt.strftime(DATETIME_FORMAT)
+            if modified__lt
+            else None,
             "active": active,
             "search": search,
         }
-        return self.base_requests.get(
+        return self._base_requests.get(
             path=path,
             parameters=parameters,
         )
 
     def post_create_area(
         self,
         code: str,
@@ -137,15 +153,15 @@
         data = {
             "code": code,
             "name": name,
             "start_date": start_date.strftime(DATE_FORMAT),
             "parent_area": parent_area,
         }
 
-        return self.base_requests.post(path=path, data=data)
+        return self._base_requests.post(path=path, data=data)
 
     def patch_edit_area(
         self,
         _id: int,
         code: str = None,
         name: str = None,
         start_date: date = None,
@@ -165,15 +181,15 @@
         path = f"/{_id}/edit_area_and_record"
         data = {
             "code": code,
             "name": name,
             "start_date": start_date.strftime(DATE_FORMAT) if start_date else None,
             "end_date": end_date.strftime(DATE_FORMAT) if end_date else None,
         }
-        return self.base_requests.patch(path=path, data=data)
+        return self._base_requests.patch(path=path, data=data)
 
     def patch_edit_parent_area(
         self,
         _id: int,
         parent_id: int,
         start_date: date,
         end_date: date = None,
@@ -190,8 +206,8 @@
         """
         path = f"/{_id}/edit_parent"
         data = {
             "parent_id": parent_id,
             "start_date": start_date.strftime(DATE_FORMAT) if start_date else None,
             "end_date": end_date.strftime(DATE_FORMAT) if start_date else None,
         }
-        return self.base_requests.patch(path=path, data=data)
+        return self._base_requests.patch(path=path, data=data)
```

### Comparing `mindsight_people_control_api-0.1.2/mindsight_people_control_api/scripts/users.py` & `mindsight_people_control_api-0.1.3/mindsight_people_control_api/scripts/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 """This module provide methods to work with users entity"""
 
 from datetime import datetime
 
-from mindsight_people_control_api.helpers.base_requests import (
+from mindsight_people_control_api.helpers.models import (
+    ApiEndpoint,
     ApiPaginationResponse,
-    BaseRequests,
-)
-from mindsight_people_control_api.settings import (
-    API_ENDPOINT_USERS,
-    DATETIME_FORMAT,
-    PAGE_SIZE,
 )
+from mindsight_people_control_api.settings import API_ENDPOINT_USERS, DATETIME_FORMAT
 
 
-class Users:
+class Users(ApiEndpoint):
     """This class abstract the users endpoint methods
     Reference: https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Users
     """
 
-    base_requests = BaseRequests()
-
     def __init__(self) -> None:
-        self.base_requests.base_path = API_ENDPOINT_USERS
-        self.page_size = PAGE_SIZE
+        super().__init__(API_ENDPOINT_USERS)
 
     def get_list_users(
         self,
         search: str = None,
     ) -> ApiPaginationResponse:
         """Get areas data
         Reference:
@@ -37,15 +30,18 @@
         """
 
         path = ""
         parameters = {
             "search": search,
             "page_size": self.page_size,
         }
-        return self.base_requests.get(path=path, parameters=parameters)
+        return ApiPaginationResponse(
+            **self._base_requests.get(path=path, parameters=parameters),
+            headers=self._base_requests.headers,
+        )
 
     def get_retrieve_user(
         self,
         _id: int,
         search: str = None,
     ) -> dict:
         """Get retrieve user
@@ -57,15 +53,15 @@
             search (str, Optional): search
         """
         path = f"/{_id}"
 
         parameters = {
             "search": search,
         }
-        return self.base_requests.get(
+        return self._base_requests.get(
             path=path,
             parameters=parameters,
         )
 
     def post_create_user(
         self,
         username: str,
@@ -105,15 +101,15 @@
             "is_active": is_active,
             "last_login": last_login.strftime(DATETIME_FORMAT) if last_login else None,
             "date_joined": date_joined.strftime(DATETIME_FORMAT)
             if date_joined
             else None,
         }
 
-        return self.base_requests.post(path=path, json=data)
+        return self._base_requests.post(path=path, json=data)
 
     def patch_update_user(
         self,
         _id: int,
         username: str,
         email: str = None,
         first_name: str = None,
@@ -151,15 +147,15 @@
             "is_staff": is_staff,
             "is_active": is_active,
             "last_login": last_login.strftime(DATETIME_FORMAT) if last_login else None,
             "date_joined": date_joined.strftime(DATETIME_FORMAT)
             if date_joined
             else None,
         }
-        return self.base_requests.patch(path=path, data=data)
+        return self._base_requests.patch(path=path, data=data)
 
     def put_full_update_user(
         self,
         _id: int,
         username: str,
         email: str = None,
         first_name: str = None,
@@ -197,15 +193,15 @@
             "is_staff": is_staff,
             "is_active": is_active,
             "last_login": last_login.strftime(DATETIME_FORMAT) if last_login else None,
             "date_joined": date_joined.strftime(DATETIME_FORMAT)
             if date_joined
             else None,
         }
-        return self.base_requests.put(path=path, data=data)
+        return self._base_requests.put(path=path, data=data)
 
     def delete_destroy_user(self, _id: int, search: str = None):
         """Delete user
         Reference:
             https://controle.mindsight.com.br/stone/api/v1/docs/#tag/Users/operation/destroyUser
 
         Args:
@@ -213,8 +209,8 @@
             search (str, Optional): Search term
         """
         path = f"/{_id}"
 
         parameters = {
             "search": search,
         }
-        return self.base_requests.delete(path=path, parameters=parameters)
+        return self._base_requests.delete(path=path, parameters=parameters)
```

### Comparing `mindsight_people_control_api-0.1.2/mindsight_people_control_api/settings.py` & `mindsight_people_control_api-0.1.3/mindsight_people_control_api/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,13 +13,16 @@
 
 # Date formats
 DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 DATE_FORMAT = "%Y-%m-%d"
 
 # Endpoints
 API_ENDPOINT_EMPLOYEES = "/employees"
+API_ENDPOINT_EMPLOYEE_RECORDS = "/employee_records"
 API_ENDPOINT_AREAS = "/areas"
 API_ENDPOINT_AREAS_RECORDS = "/area_records"
+API_ENDPOINT_PARENT_AREAS = "/parent_areas"
 API_ENDPOINT_EMPLOYEE_AREAS = "/employee_areas"
-API_ENDPOINT_EMPLOYEE_MANAGERS = "/employee_manager"
+API_ENDPOINT_EMPLOYEE_POSITIONS = "/employee_positions"
+API_ENDPOINT_EMPLOYEE_MANAGERS = "/employee_managers"
 API_ENDPOINT_USERS = "/users"
 API_ENDPOINT_POSITIONS = "/positions"
```

