# Comparing `tmp/curlify2-1.0.3.1.tar.gz` & `tmp/curlify2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlify2-1.0.3.1.tar", max compression
+gzip compressed data, was "curlify2-2.0.0.tar", max compression
```

## Comparing `curlify2-1.0.3.1.tar` & `curlify2-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-06-07 13:17:59.078986 curlify2-1.0.3.1/LICENSE
--rw-r--r--   0        0        0     1175 2023-06-07 13:17:59.079166 curlify2-1.0.3.1/README.md
--rw-r--r--   0        0        0       52 2023-06-07 13:17:59.079287 curlify2-1.0.3.1/curlify2/__init__.py
--rw-r--r--   0        0        0      629 2023-06-07 13:17:59.079375 curlify2-1.0.3.1/curlify2/curlify.py
--rw-r--r--   0        0        0      681 2023-06-08 03:02:38.687418 curlify2-1.0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 curlify2-1.0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-07 13:17:59.078986 curlify2-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1204 2023-06-09 15:16:58.878335 curlify2-2.0.0/README.md
+-rw-r--r--   0        0        0       52 2023-06-09 15:16:58.878749 curlify2-2.0.0/curlify2/__init__.py
+-rw-r--r--   0        0        0     1282 2023-06-09 15:16:58.879216 curlify2-2.0.0/curlify2/curlify.py
+-rw-r--r--   0        0        0      679 2023-06-09 15:16:58.880064 curlify2-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 curlify2-2.0.0/PKG-INFO
```

### Comparing `curlify2-1.0.3.1/LICENSE` & `curlify2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curlify2-1.0.3.1/README.md` & `curlify2-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,33 +16,31 @@
 ```
 
 ## Usage
 
 using **requests** module:
 
 ```python
-import curlify2
+from curlify2 import Curlify
 import requests
 
 URL = "https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f"
 
 request = requests.get(URL)
-curl = curlify2.to_curl(request.request)
-
-print(curl) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
+response = Curlify(request.request)
 
+print(response.to_curl()) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
 ```
 
 using **httpx** module:
 
 ```python
 import curlify2
 import httpx
 
 URL = "https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f"
 
 request = httpx.get(URL)
-curl = curlify2.to_curl(request.request)
-
-print(curl) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
+response = Curlify(request.request)
 
+print(response.to_curl()) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
 ```
```

### Comparing `curlify2-1.0.3.1/pyproject.toml` & `curlify2-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "curlify2"
-version = "1.0.3.1"
+version = "2.0.0"
 description = "Library to convert python requests and httpx object to curl command."
 authors = ["Marcus Pereira <marcus@negros.dev>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/marcuxyz/curlify2"
 homepage = "https://github.com/marcuxyz/curlify2"
@@ -12,14 +12,14 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 requests = "^2.31.0"
 pytest = "^7.3.1"
-responses = "^0.22.0"
 black = ">=21.7b0"
 pytest-httpx = "^0.22.0"
+responses = "^0.23.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `curlify2-1.0.3.1/PKG-INFO` & `curlify2-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curlify2
-Version: 1.0.3.1
+Version: 2.0.0
 Summary: Library to convert python requests and httpx object to curl command.
 Home-page: https://github.com/marcuxyz/curlify2
 License: MIT
 Keywords: python,curl,requests,curlify,httpx,convert to curl
 Author: Marcus Pereira
 Author-email: marcus@negros.dev
 Requires-Python: >=3.7,<4.0
@@ -36,33 +36,31 @@
 ```
 
 ## Usage
 
 using **requests** module:
 
 ```python
-import curlify2
+from curlify2 import Curlify
 import requests
 
 URL = "https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f"
 
 request = requests.get(URL)
-curl = curlify2.to_curl(request.request)
-
-print(curl) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
+response = Curlify(request.request)
 
+print(response.to_curl()) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
 ```
 
 using **httpx** module:
 
 ```python
 import curlify2
 import httpx
 
 URL = "https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f"
 
 request = httpx.get(URL)
-curl = curlify2.to_curl(request.request)
-
-print(curl) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
+response = Curlify(request.request)
 
+print(response.to_curl()) # curl -X GET -H "User-Agent: python-requests/2.24.0" -H "Accept-Encoding: gzip, deflate" -H "Accept: */*" -H "Connection: keep-alive" -d 'None' https://run.mocky.io/v3/b0f4ffd8-6696-4f90-8bab-4a3bcad9ef3f
 ```
```

