# Comparing `tmp/PanjSim-1.0.0.tar.gz` & `tmp/PanjSim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PanjSim-1.0.0.tar", last modified: Tue Jun  6 15:22:22 2023, max compression
+gzip compressed data, was "PanjSim-1.0.3.tar", last modified: Fri Jun  9 03:09:49 2023, max compression
```

## Comparing `PanjSim-1.0.0.tar` & `PanjSim-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.695551 PanjSim-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-06 13:41:52.000000 PanjSim-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5206 2023-06-06 15:22:22.693554 PanjSim-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.559549 PanjSim-1.0.0/PanjSim/
--rw-rw-rw-   0        0        0    57337 2023-06-06 01:55:37.000000 PanjSim-1.0.0/PanjSim/Countrys.py
--rw-rw-rw-   0        0        0       40 2023-06-05 03:38:25.000000 PanjSim-1.0.0/PanjSim/__init__.py
--rw-rw-rw-   0        0        0     4967 2023-06-05 03:30:14.000000 PanjSim-1.0.0/PanjSim/_http_client.py
--rw-rw-rw-   0        0        0     2853 2023-06-06 01:26:56.000000 PanjSim-1.0.0/PanjSim/client.py
--rw-rw-rw-   0        0        0     2184 2023-06-04 05:25:38.000000 PanjSim-1.0.0/PanjSim/errors.py
--rw-rw-rw-   0        0        0     4938 2023-06-05 02:45:12.000000 PanjSim-1.0.0/PanjSim/http_client.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.645542 PanjSim-1.0.0/PanjSim/products/
--rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.0/PanjSim/products/__init__.py
--rw-rw-rw-   0        0        0      988 2023-06-06 01:29:31.000000 PanjSim-1.0.0/PanjSim/products/products.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.654553 PanjSim-1.0.0/PanjSim/purchase/
--rw-rw-rw-   0        0        0        0 2023-06-04 02:57:26.000000 PanjSim-1.0.0/PanjSim/purchase/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-06-05 00:44:28.000000 PanjSim-1.0.0/PanjSim/purchase/management.py
--rw-rw-rw-   0        0        0     1757 2023-06-05 04:14:39.000000 PanjSim-1.0.0/PanjSim/purchase/purchase.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.671556 PanjSim-1.0.0/PanjSim/types/
--rw-rw-rw-   0        0        0      124 2023-06-06 01:41:13.000000 PanjSim-1.0.0/PanjSim/types/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-06-06 01:32:51.000000 PanjSim-1.0.0/PanjSim/types/_operators.py
--rw-rw-rw-   0        0        0      335 2023-06-06 01:38:10.000000 PanjSim-1.0.0/PanjSim/types/_order.py
--rw-rw-rw-   0        0        0     7621 2023-06-06 01:38:43.000000 PanjSim-1.0.0/PanjSim/types/_products.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.681540 PanjSim-1.0.0/PanjSim/user/
--rw-rw-rw-   0        0        0        0 2023-06-04 00:41:18.000000 PanjSim-1.0.0/PanjSim/user/__init__.py
--rw-rw-rw-   0        0        0     1309 2023-06-05 02:57:45.000000 PanjSim-1.0.0/PanjSim/user/user.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.687543 PanjSim-1.0.0/PanjSim/vendor/
--rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.0/PanjSim/vendor/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-06-04 04:03:39.000000 PanjSim-1.0.0/PanjSim/vendor/vendor.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:22:22.635538 PanjSim-1.0.0/PanjSim.egg-info/
--rw-rw-rw-   0        0        0     5206 2023-06-06 15:22:22.000000 PanjSim-1.0.0/PanjSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      668 2023-06-06 15:22:22.000000 PanjSim-1.0.0/PanjSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:22:22.000000 PanjSim-1.0.0/PanjSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 15:22:22.000000 PanjSim-1.0.0/PanjSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 15:22:22.000000 PanjSim-1.0.0/PanjSim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3886 2023-06-06 14:52:25.000000 PanjSim-1.0.0/README.md
--rw-rw-rw-   0        0        0       99 2023-06-06 04:27:45.000000 PanjSim-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 15:22:22.696545 PanjSim-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-06-06 15:21:00.000000 PanjSim-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.624508 PanjSim-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-06 13:41:52.000000 PanjSim-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5169 2023-06-09 03:09:49.622503 PanjSim-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.514505 PanjSim-1.0.3/PanjSim/
+-rw-rw-rw-   0        0        0    57337 2023-06-06 01:55:37.000000 PanjSim-1.0.3/PanjSim/Countrys.py
+-rw-rw-rw-   0        0        0       40 2023-06-05 03:38:25.000000 PanjSim-1.0.3/PanjSim/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-06-06 01:26:56.000000 PanjSim-1.0.3/PanjSim/client.py
+-rw-rw-rw-   0        0        0     2472 2023-06-09 02:45:24.000000 PanjSim-1.0.3/PanjSim/errors.py
+-rw-rw-rw-   0        0        0     4938 2023-06-09 02:46:33.000000 PanjSim-1.0.3/PanjSim/http_client.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.572507 PanjSim-1.0.3/PanjSim/products/
+-rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.3/PanjSim/products/__init__.py
+-rw-rw-rw-   0        0        0      988 2023-06-06 01:29:31.000000 PanjSim-1.0.3/PanjSim/products/products.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.582503 PanjSim-1.0.3/PanjSim/purchase/
+-rw-rw-rw-   0        0        0        0 2023-06-04 02:57:26.000000 PanjSim-1.0.3/PanjSim/purchase/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-06-05 00:44:28.000000 PanjSim-1.0.3/PanjSim/purchase/management.py
+-rw-rw-rw-   0        0        0     1757 2023-06-05 04:14:39.000000 PanjSim-1.0.3/PanjSim/purchase/purchase.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.599507 PanjSim-1.0.3/PanjSim/types/
+-rw-rw-rw-   0        0        0      124 2023-06-06 01:41:13.000000 PanjSim-1.0.3/PanjSim/types/__init__.py
+-rw-rw-rw-   0        0        0     1302 2023-06-06 01:32:51.000000 PanjSim-1.0.3/PanjSim/types/_operators.py
+-rw-rw-rw-   0        0        0      335 2023-06-06 01:38:10.000000 PanjSim-1.0.3/PanjSim/types/_order.py
+-rw-rw-rw-   0        0        0     7621 2023-06-06 01:38:43.000000 PanjSim-1.0.3/PanjSim/types/_products.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.608502 PanjSim-1.0.3/PanjSim/user/
+-rw-rw-rw-   0        0        0        0 2023-06-04 00:41:18.000000 PanjSim-1.0.3/PanjSim/user/__init__.py
+-rw-rw-rw-   0        0        0     1309 2023-06-05 02:57:45.000000 PanjSim-1.0.3/PanjSim/user/user.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.617508 PanjSim-1.0.3/PanjSim/vendor/
+-rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.3/PanjSim/vendor/__init__.py
+-rw-rw-rw-   0        0        0     1877 2023-06-04 04:03:39.000000 PanjSim-1.0.3/PanjSim/vendor/vendor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.566511 PanjSim-1.0.3/PanjSim.egg-info/
+-rw-rw-rw-   0        0        0     5169 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3849 2023-06-09 03:08:46.000000 PanjSim-1.0.3/README.md
+-rw-rw-rw-   0        0        0       99 2023-06-06 04:27:45.000000 PanjSim-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:09:49.624508 PanjSim-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2023-06-09 03:08:25.000000 PanjSim-1.0.3/setup.py
```

### Comparing `PanjSim-1.0.0/LICENSE` & `PanjSim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PKG-INFO` & `PanjSim-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PanjSim
-Version: 1.0.0
+Version: 1.0.3
 Summary: A simple Python API for 5sim.net
 Home-page: https://github.com/abbas-bachari/PanjSim
 Author: Abbas Bachari
 Author-email: abbas-bachari@hotmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/abbas-bachari/PanjSim
 Project-URL: Documentation, https://github.com/abbas-bachari/PanjSim
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Abbas Bachari](https://img.shields.io/badge/Abbas%20Bachari-PanjSim-green?style=plastic&logo=codemagic)](https://github.com/abbas-bachari/PanjSim)
+[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.3-green?style=plastic&logo=codemagic)](https://python.org)
 [![python](https://img.shields.io/badge/Python%20-3.7+-green?style=plastic&logo=Python)](https://python.org)
 
 
 
 
 # What is PanjSim ? ([فارسی](https://github.com/abbas-bachari/PanjSim/blob/main/README-fa.md))
 A simple Python API for [5sim.net](https://5sim.net)
@@ -115,15 +115,15 @@
 
 country=usa
 
 
 product=client.Products()
 
 # Receive the name, the price, quantity of all products, available to buy.
-operator=country.operators.virtual23.name
+operator=country.Operator.virtual23
 product.get_products(country=country.name,operator=operator)
 
 
 # Get all product prices
 product.get_prices()
 
 # Get product prices by country
@@ -149,15 +149,15 @@
 
 country=usa
 
 Purchase=client.Purchase()
 
 
 # Buy activation number
-operator=country.operators.virtual23.name
+operator=country.Operator.virtual23
 order=Purchase.buy_activation_number(country=country.name,operator=operator,product='telegram')
 
 # Check order (Get SMS)
 Purchase.check_order(order_id=order['id'])
 
 # Ban order
 Purchase.ban_order(order_id=order['id'])
```

### Comparing `PanjSim-1.0.0/PanjSim/Countrys.py` & `PanjSim-1.0.3/PanjSim/Countrys.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/_http_client.py` & `PanjSim-1.0.3/PanjSim/http_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,103 +19,106 @@
 
    
 
     def _generate_query_string(self, payload: dict[str, Any] = {}) -> str:
         """
         It takes a payload and returns a query string
 
-        :param payload: The payload that you want to convert to a query string
-        :return: A string of the query string
+        + payload: The payload that you want to convert to a query string
+        * return: A string of the query string
         """
 
         
         query_string = '&'.join(f'{k}={v}' for k, v in payload.items() if v)
         
         return query_string
 
-    def _request(self, method: str, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {}) -> requests.Response:
+    def _request(self, method: str, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {},data=None) -> requests.Response:
         """
-        It takes a method, endpoint, payload, and headers, and returns a response
-
-        :param method: The HTTP method to use (GET, POST, PUT, DELETE)
-        :param endpoint: The endpoint you want to hit i.e. /openApi/swap/v2/trade/order
-        :param payload: The data to be sent to the server
-        :param headers: This is a dictionary of headers that will be sent with the request
+        It takes a method, endpoint, payload, and headers, and returns a respons
+        + method: The HTTP method to use (GET, POST, PUT, DELETE)
+        + endpoint: The endpoint you want to hit i.e. /v1/guest/countries
+        + payload:  The data to be sent to the server
+        + headers:  This is a dictionary of headers that will be sent with the request
+        + data:     The data to be sent to the server by post metod
         """
         if headers:
             self.__session.headers.update(headers)
 
         url = f"{self.__BASE_URL}{endpoint}?{self._generate_query_string(payload)}" if payload else f"{self.__BASE_URL}{endpoint}"
         match method:
             case "GET":
                 req = self.__session.get(url)
             case "POST":
-                req = self.__session.post(url)
+                req = self.__session.post(url,data=data)
             case "PUT":
                 req = self.__session.put(url)
             case "DELETE":
                 req = self.__session.delete(url)
             case _:
                 raise InvalidMethodException(f"Invalid method used: {method}")
 
         if req.status_code != 200:
             
             raise ServerError(req.status_code, req.text)
 
         try:
             req_json: dict[str, Any] = req.json()
-        except JSONDecodeError: # i.e. sometimes it return just int status code
-            return req
+        
+        except JSONDecodeError: 
+            raise ErrorJSONDecode(req.status_code,req.text)
+        
         else:
-            
             if isinstance(req_json, dict):
-                if req_json.get("code") is not None and req_json.get("code") != 0:
-                    raise ClientError(req_json.get("code"), req_json.get("msg"))
-            return req
+               return req
+            
+            raise ClientError(req.status_code, req.text)
+            
 
     def get(self, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {}) -> requests.Response:
         """
         It makes a GET request to the given endpoint with the given payload and headers
 
-        :param endpoint: The endpoint you want to hit i.e. /openApi/swap/v2/trade/order
-        :param payload: The data to be sent to the server
-        :param headers: This is a dictionary of headers that will be sent with the request
-        :return: A response object
+        + endpoint: The endpoint you want to hit i.e. /v1/guest/countries
+        + payload: The data to be sent to the server
+        + headers: This is a dictionary of headers that will be sent with the request
+        * return: A response object
         """
 
         return self._request("GET", endpoint, payload, headers)
 
-    def post(self, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {}) -> requests.Response:
+    def post(self, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {},data=None) -> requests.Response:
         """
         It makes a POST request to the given endpoint with the given payload and headers
 
-        :param endpoint: The endpoint you want to hit i.e. /openApi/swap/v2/trade/order
-        :param payload: The data to be sent to the server
-        :param headers: This is a dictionary of headers that will be sent with the request
-        :return: A response object
+        + endpoint: The endpoint you want to hit i.e. /v1/guest/countries
+        + payload: The data to be sent to the server
+        + headers: This is a dictionary of headers that will be sent with the request
+        + data:     The data to be sent to the server by post metod
+        * return: A response object
         """
 
-        return self._request("POST", endpoint, payload, headers)
+        return self._request("POST", endpoint, payload, headers,data=data)
 
     def put(self, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {}) -> requests.Response:
         """
         It makes a PUT request to the given endpoint with the given payload and headers
 
-        :param endpoint: The endpoint you want to hit i.e. /openApi/swap/v2/trade/order
-        :param payload: The data to be sent to the server
-        :param headers: This is a dictionary of headers that will be sent with the request
-        :return: A response object
+        + endpoint: The endpoint you want to hit i.e. /v1/guest/countries
+        + payload: The data to be sent to the server
+        + headers: This is a dictionary of headers that will be sent with the request
+        * return: A response object
         """
 
         return self._request("PUT", endpoint, payload, headers)
 
     def delete(self, endpoint: str, payload: dict[str, Any] = {}, headers: dict[str, Any] = {}) -> requests.Response:
         """
         It makes a DELETE request to the given endpoint with the given payload and headers
 
-        :param endpoint: The endpoint you want to hit i.e. /openApi/swap/v2/trade/order
-        :param payload: The data to be sent to the server
-        :param headers: This is a dictionary of headers that will be sent with the request
-        :return: A response object
+        + endpoint: The endpoint you want to hit i.e. /v1/guest/countries
+        + payload: The data to be sent to the server
+        + headers: This is a dictionary of headers that will be sent with the request
+        * return: A response object
         """
 
         return self._request("DELETE", endpoint, payload, headers)
```

### Comparing `PanjSim-1.0.0/PanjSim/client.py` & `PanjSim-1.0.3/PanjSim/client.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/errors.py` & `PanjSim-1.0.3/PanjSim/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,7 +41,13 @@
         504: "return code means that the API server has submitted a request to the service center but failed to get a response. It should be noted that the 504 return code does not mean that the request failed. It refers to an unknown status. The request may have been executed, or it may have failed. Further confirmation is required."
     }
 
     def __init__(self, error_code: int, error_message: str) -> None:
         self.error_code = error_code
         self.error_message = error_message
         super().__init__(self.error_message if len(self.error_message) > 0 else self.ERROR_CODES.get(self.error_code, "Unknown Error"))
+
+class ErrorJSONDecode(Exception):
+    def __init__(self, error_code: int, error_message: str) -> None:
+        self.error_code = error_code
+        self.error_message = error_message
+        super().__init__(self.error_message if len(self.error_message) > 0 else  "Unknown Error")
```

### Comparing `PanjSim-1.0.0/PanjSim/products/products.py` & `PanjSim-1.0.3/PanjSim/products/products.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/purchase/management.py` & `PanjSim-1.0.3/PanjSim/purchase/management.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/purchase/purchase.py` & `PanjSim-1.0.3/PanjSim/purchase/purchase.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/types/_operators.py` & `PanjSim-1.0.3/PanjSim/types/_operators.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/types/_products.py` & `PanjSim-1.0.3/PanjSim/types/_products.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/user/user.py` & `PanjSim-1.0.3/PanjSim/user/user.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim/vendor/vendor.py` & `PanjSim-1.0.3/PanjSim/vendor/vendor.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.0/PanjSim.egg-info/PKG-INFO` & `PanjSim-1.0.3/PanjSim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PanjSim
-Version: 1.0.0
+Version: 1.0.3
 Summary: A simple Python API for 5sim.net
 Home-page: https://github.com/abbas-bachari/PanjSim
 Author: Abbas Bachari
 Author-email: abbas-bachari@hotmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/abbas-bachari/PanjSim
 Project-URL: Documentation, https://github.com/abbas-bachari/PanjSim
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Abbas Bachari](https://img.shields.io/badge/Abbas%20Bachari-PanjSim-green?style=plastic&logo=codemagic)](https://github.com/abbas-bachari/PanjSim)
+[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.3-green?style=plastic&logo=codemagic)](https://python.org)
 [![python](https://img.shields.io/badge/Python%20-3.7+-green?style=plastic&logo=Python)](https://python.org)
 
 
 
 
 # What is PanjSim ? ([فارسی](https://github.com/abbas-bachari/PanjSim/blob/main/README-fa.md))
 A simple Python API for [5sim.net](https://5sim.net)
@@ -115,15 +115,15 @@
 
 country=usa
 
 
 product=client.Products()
 
 # Receive the name, the price, quantity of all products, available to buy.
-operator=country.operators.virtual23.name
+operator=country.Operator.virtual23
 product.get_products(country=country.name,operator=operator)
 
 
 # Get all product prices
 product.get_prices()
 
 # Get product prices by country
@@ -149,15 +149,15 @@
 
 country=usa
 
 Purchase=client.Purchase()
 
 
 # Buy activation number
-operator=country.operators.virtual23.name
+operator=country.Operator.virtual23
 order=Purchase.buy_activation_number(country=country.name,operator=operator,product='telegram')
 
 # Check order (Get SMS)
 Purchase.check_order(order_id=order['id'])
 
 # Ban order
 Purchase.ban_order(order_id=order['id'])
```

### Comparing `PanjSim-1.0.0/PanjSim.egg-info/SOURCES.txt` & `PanjSim-1.0.3/PanjSim.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 PanjSim/Countrys.py
 PanjSim/__init__.py
-PanjSim/_http_client.py
 PanjSim/client.py
 PanjSim/errors.py
 PanjSim/http_client.py
 PanjSim.egg-info/PKG-INFO
 PanjSim.egg-info/SOURCES.txt
 PanjSim.egg-info/dependency_links.txt
 PanjSim.egg-info/requires.txt
```

### Comparing `PanjSim-1.0.0/README.md` & `PanjSim-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Abbas Bachari](https://img.shields.io/badge/Abbas%20Bachari-PanjSim-green?style=plastic&logo=codemagic)](https://github.com/abbas-bachari/PanjSim)
+[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.3-green?style=plastic&logo=codemagic)](https://python.org)
 [![python](https://img.shields.io/badge/Python%20-3.7+-green?style=plastic&logo=Python)](https://python.org)
 
 
 
 
 # What is PanjSim ? ([فارسی](https://github.com/abbas-bachari/PanjSim/blob/main/README-fa.md))
 A simple Python API for [5sim.net](https://5sim.net)
@@ -89,15 +89,15 @@
 
 country=usa
 
 
 product=client.Products()
 
 # Receive the name, the price, quantity of all products, available to buy.
-operator=country.operators.virtual23.name
+operator=country.Operator.virtual23
 product.get_products(country=country.name,operator=operator)
 
 
 # Get all product prices
 product.get_prices()
 
 # Get product prices by country
@@ -123,15 +123,15 @@
 
 country=usa
 
 Purchase=client.Purchase()
 
 
 # Buy activation number
-operator=country.operators.virtual23.name
+operator=country.Operator.virtual23
 order=Purchase.buy_activation_number(country=country.name,operator=operator,product='telegram')
 
 # Check order (Get SMS)
 Purchase.check_order(order_id=order['id'])
 
 # Ban order
 Purchase.ban_order(order_id=order['id'])
```

### Comparing `PanjSim-1.0.0/setup.py` & `PanjSim-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PanjSim',
-    version='1.0.0',
+    version='1.0.3',
     author='Abbas Bachari',
     author_email='abbas-bachari@hotmail.com',
     description='A simple Python API for 5sim.net',
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
@@ -33,7 +33,8 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         
         
     ],
 )
 
+
```

