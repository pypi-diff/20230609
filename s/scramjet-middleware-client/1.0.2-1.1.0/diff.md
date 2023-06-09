# Comparing `tmp/scramjet_middleware_client-1.0.2.tar.gz` & `tmp/scramjet-middleware-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scramjet_middleware_client-1.0.2.tar", max compression
+gzip compressed data, was "scramjet-middleware-client-1.1.0.tar", last modified: Fri Jun  9 11:34:13 2023, max compression
```

## Comparing `scramjet_middleware_client-1.0.2.tar` & `scramjet-middleware-client-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0     1246 2023-01-10 13:29:37.730113 scramjet_middleware_client-1.0.2/README.md
--rw-r--r--   0        0        0        0 2022-09-22 12:31:28.000000 scramjet_middleware_client-1.0.2/middleware_client/__init__.py
--rw-r--r--   0        0        0      630 2023-01-10 13:49:33.884038 scramjet_middleware_client-1.0.2/middleware_client/middleware_client.py
--rw-r--r--   0        0        0      400 2023-01-10 13:50:42.923717 scramjet_middleware_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 scramjet_middleware_client-1.0.2/setup.py
--rw-r--r--   0        0        0     1762 1970-01-01 00:00:00.000000 scramjet_middleware_client-1.0.2/PKG-INFO
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:34:13.212370 scramjet-middleware-client-1.1.0/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1471 2023-06-09 11:34:13.212370 scramjet-middleware-client-1.1.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1188 2023-04-25 21:03:21.000000 scramjet-middleware-client-1.1.0/README.md
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:34:13.212370 scramjet-middleware-client-1.1.0/middleware_client/
+-rw-rw-r--   0 bob       (1000) bob       (1000)        0 2023-04-25 19:55:28.000000 scramjet-middleware-client-1.1.0/middleware_client/__init__.py
+-rw-rw-r--   0 bob       (1000) bob       (1000)      648 2023-06-09 05:45:44.000000 scramjet-middleware-client-1.1.0/middleware_client/middleware_client.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:34:13.212370 scramjet-middleware-client-1.1.0/scramjet_middleware_client.egg-info/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1471 2023-06-09 11:34:13.000000 scramjet-middleware-client-1.1.0/scramjet_middleware_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)      336 2023-06-09 11:34:13.000000 scramjet-middleware-client-1.1.0/scramjet_middleware_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2023-06-09 11:34:13.000000 scramjet-middleware-client-1.1.0/scramjet_middleware_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       60 2023-06-09 11:34:13.000000 scramjet-middleware-client-1.1.0/scramjet_middleware_client.egg-info/requires.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       18 2023-06-09 11:34:13.000000 scramjet-middleware-client-1.1.0/scramjet_middleware_client.egg-info/top_level.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       38 2023-06-09 11:34:13.212370 scramjet-middleware-client-1.1.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)      823 2023-06-09 11:33:57.000000 scramjet-middleware-client-1.1.0/setup.py
```

### Comparing `scramjet_middleware_client-1.0.2/README.md` & `scramjet-middleware-client-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 
 
 ## Usage:
 > ❗NOTE: You need to provide your middleware [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-the-environment) if you are not hosting STH locally.
 
 ```python
 import asyncio
-import json
 from middleware_client.middleware_client import MiddlewareClient
-from client_utils.client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
 middleware = MiddlewareClient(api_base)
 res = asyncio.run(middleware.get_managers())
-# convert response to json
-managers = json.loads(res)
+print(res)
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
                    ****** Scramjet Middleware client ******
                           [GitHub_license] [Discord]
 ## About: This package provides a **Middleware client** to let you connect with
 your Scramjet Cloud Platform account. ## Usage: > âNOTE: You need to provide
 your middleware [access token](https://docs.scramjet.org/platform/quick-
 start#step-1-set-up-the-environment) if you are not hosting STH locally.
-```python import asyncio import json from middleware_client.middleware_client
-import MiddlewareClient from client_utils.client_utils import ClientUtils #
-your middleware token token = '' # set the token ClientUtils.setDefaultHeaders(
+```python import asyncio from middleware_client.middleware_client import
+MiddlewareClient from client_utils.base_client import BaseClient # your
+middleware token token = '' # set the token BaseClient.setDefaultHeaders(
 {'Authorization': f'Bearer {token}'}) # middleware url api_base ='https://
 api.scramjet.cloud/api/v1' middleware = MiddlewareClient(api_base) res =
-asyncio.run(middleware.get_managers()) # convert response to json managers =
-json.loads(res) ```
+asyncio.run(middleware.get_managers()) print(res) ```
```

### Comparing `scramjet_middleware_client-1.0.2/PKG-INFO` & `scramjet-middleware-client-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 Metadata-Version: 2.1
 Name: scramjet-middleware-client
-Version: 1.0.2
-Summary: 
+Version: 1.1.0
+Home-page: https://github.com/scramjetorg/api-client-python/tree/main/middleware_client
 Author: Scramjet
 Author-email: open-source@scramjet.org
 Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: scramjet-client-utils (>=1.0.1,<2.0.0)
-Requires-Dist: scramjet-manager-client (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center"><strong>Scramjet Middleware client</strong></h1>
 
 <p align="center">
     <a href="https://github.com/scramjetorg/transform-hub/blob/HEAD/LICENSE"><img src="https://img.shields.io/github/license/scramjetorg/transform-hub?color=green&style=plastic" alt="GitHub license" /></a>
     <a href="https://scr.je/join-community-mg1"><img alt="Discord" src="https://img.shields.io/discord/925384545342201896?label=discord&style=plastic"></a>
@@ -26,26 +20,23 @@
 
 
 ## Usage:
 > ❗NOTE: You need to provide your middleware [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-the-environment) if you are not hosting STH locally.
 
 ```python
 import asyncio
-import json
 from middleware_client.middleware_client import MiddlewareClient
-from client_utils.client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
 middleware = MiddlewareClient(api_base)
 res = asyncio.run(middleware.get_managers())
-# convert response to json
-managers = json.loads(res)
+print(res)
 ```
-
```

#### html2text {}

```diff
@@ -1,20 +1,16 @@
-Metadata-Version: 2.1 Name: scramjet-middleware-client Version: 1.0.2 Summary:
-Author: Scramjet Author-email: open-source@scramjet.org Requires-Python:
->=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: scramjet-client-utils (>=1.0.1,<2.0.0) Requires-Dist: scramjet-manager-
-client (>=1.0.1,<2.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: scramjet-middleware-client Version: 1.1.0 Home-
+page: https://github.com/scramjetorg/api-client-python/tree/main/
+middleware_client Author: Scramjet Author-email: open-source@scramjet.org
+Requires-Python: >=3.9,<4.0 Description-Content-Type: text/markdown
                    ****** Scramjet Middleware client ******
                           [GitHub_license] [Discord]
 ## About: This package provides a **Middleware client** to let you connect with
 your Scramjet Cloud Platform account. ## Usage: > âNOTE: You need to provide
 your middleware [access token](https://docs.scramjet.org/platform/quick-
 start#step-1-set-up-the-environment) if you are not hosting STH locally.
-```python import asyncio import json from middleware_client.middleware_client
-import MiddlewareClient from client_utils.client_utils import ClientUtils #
-your middleware token token = '' # set the token ClientUtils.setDefaultHeaders(
+```python import asyncio from middleware_client.middleware_client import
+MiddlewareClient from client_utils.base_client import BaseClient # your
+middleware token token = '' # set the token BaseClient.setDefaultHeaders(
 {'Authorization': f'Bearer {token}'}) # middleware url api_base ='https://
 api.scramjet.cloud/api/v1' middleware = MiddlewareClient(api_base) res =
-asyncio.run(middleware.get_managers()) # convert response to json managers =
-json.loads(res) ```
+asyncio.run(middleware.get_managers()) print(res) ```
```

