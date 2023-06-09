# Comparing `tmp/scramjet_multi_manager_client-1.0.1.tar.gz` & `tmp/scramjet-multi-manager-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scramjet_multi_manager_client-1.0.1.tar", max compression
+gzip compressed data, was "scramjet-multi-manager-client-1.1.0.tar", last modified: Fri Jun  9 11:37:25 2023, max compression
```

## Comparing `scramjet_multi_manager_client-1.0.1.tar` & `scramjet-multi-manager-client-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0     1100 2023-01-10 13:40:17.586693 scramjet_multi_manager_client-1.0.1/README.md
--rw-r--r--   0        0        0        0 2022-09-22 12:31:28.000000 scramjet_multi_manager_client-1.0.1/multi_manager_client/__init__.py
--rw-r--r--   0        0        0     1343 2023-01-10 13:40:31.110627 scramjet_multi_manager_client-1.0.1/multi_manager_client/multi_manager_client.py
--rw-r--r--   0        0        0      405 2023-01-10 13:39:43.426862 scramjet_multi_manager_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 scramjet_multi_manager_client-1.0.1/setup.py
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 scramjet_multi_manager_client-1.0.1/PKG-INFO
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:37:25.368700 scramjet-multi-manager-client-1.1.0/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1374 2023-06-09 11:37:25.368700 scramjet-multi-manager-client-1.1.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1085 2023-04-25 21:18:30.000000 scramjet-multi-manager-client-1.1.0/README.md
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:37:25.368700 scramjet-multi-manager-client-1.1.0/multi_manager_client/
+-rw-rw-r--   0 bob       (1000) bob       (1000)        0 2023-04-25 19:55:28.000000 scramjet-multi-manager-client-1.1.0/multi_manager_client/__init__.py
+-rw-rw-r--   0 bob       (1000) bob       (1000)      915 2023-04-28 10:00:38.000000 scramjet-multi-manager-client-1.1.0/multi_manager_client/multi_manager_client.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:37:25.368700 scramjet-multi-manager-client-1.1.0/scramjet_multi_manager_client.egg-info/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1374 2023-06-09 11:37:25.000000 scramjet-multi-manager-client-1.1.0/scramjet_multi_manager_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)      360 2023-06-09 11:37:25.000000 scramjet-multi-manager-client-1.1.0/scramjet_multi_manager_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2023-06-09 11:37:25.000000 scramjet-multi-manager-client-1.1.0/scramjet_multi_manager_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       76 2023-06-09 11:37:25.000000 scramjet-multi-manager-client-1.1.0/scramjet_multi_manager_client.egg-info/requires.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       21 2023-06-09 11:37:25.000000 scramjet-multi-manager-client-1.1.0/scramjet_multi_manager_client.egg-info/top_level.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       38 2023-06-09 11:37:25.368700 scramjet-multi-manager-client-1.1.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)      847 2023-06-09 11:37:00.000000 scramjet-multi-manager-client-1.1.0/setup.py
```

### Comparing `scramjet_multi_manager_client-1.0.1/README.md` & `scramjet-multi-manager-client-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 
 ## Usage:
 > ❗NOTE: You need to provide your middleware [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-the-environment) if you are not hosting STH locally.
 
 ```python
 import asyncio
-import json
 from multi_manager_client.multi_manager_client import MultiManagerClient
-from client_utils.client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
 #TODO
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                   ****** Scramjet Multi Manager client ******
                           [GitHub_license] [Discord]
 ## About: This package provides a **Multi manager client** which manages
 **manager** clients. ## Usage: > âNOTE: You need to provide your middleware
 [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-
 the-environment) if you are not hosting STH locally. ```python import asyncio
-import json from multi_manager_client.multi_manager_client import
-MultiManagerClient from client_utils.client_utils import ClientUtils # your
-middleware token token = '' # set the token ClientUtils.setDefaultHeaders(
-{'Authorization': f'Bearer {token}'}) # middleware url api_base ='https://
-api.scramjet.cloud/api/v1' #TODO ```
+from multi_manager_client.multi_manager_client import MultiManagerClient from
+client_utils.base_client import BaseClient # your middleware token token = '' #
+set the token BaseClient.setDefaultHeaders({'Authorization': f'Bearer
+{token}'}) # middleware url api_base ='https://api.scramjet.cloud/api/v1' #TODO
+```
```

### Comparing `scramjet_multi_manager_client-1.0.1/PKG-INFO` & `scramjet-multi-manager-client-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 Metadata-Version: 2.1
 Name: scramjet-multi-manager-client
-Version: 1.0.1
-Summary: 
+Version: 1.1.0
+Home-page: https://github.com/scramjetorg/api-client-python/tree/main/multi_manager_client
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
 
 <h1 align="center"><strong>Scramjet Multi Manager client</strong></h1>
 
 <p align="center">
     <a href="https://github.com/scramjetorg/transform-hub/blob/HEAD/LICENSE"><img src="https://img.shields.io/github/license/scramjetorg/transform-hub?color=green&style=plastic" alt="GitHub license" /></a>
     <a href="https://scr.je/join-community-mg1"><img alt="Discord" src="https://img.shields.io/discord/925384545342201896?label=discord&style=plastic"></a>
@@ -26,23 +20,21 @@
 
 
 ## Usage:
 > ❗NOTE: You need to provide your middleware [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-the-environment) if you are not hosting STH locally.
 
 ```python
 import asyncio
-import json
 from multi_manager_client.multi_manager_client import MultiManagerClient
-from client_utils.client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
 #TODO
 ```
-
```

#### html2text {}

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 2.1 Name: scramjet-multi-manager-client Version: 1.0.1
-Summary: Author: Scramjet Author-email: open-source@scramjet.org Requires-
-Python: >=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: scramjet-client-utils (>=1.0.1,<2.0.0) Requires-Dist: scramjet-manager-
-client (>=1.0.1,<2.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: scramjet-multi-manager-client Version: 1.1.0 Home-
+page: https://github.com/scramjetorg/api-client-python/tree/main/
+multi_manager_client Author: Scramjet Author-email: open-source@scramjet.org
+Requires-Python: >=3.9,<4.0 Description-Content-Type: text/markdown
                   ****** Scramjet Multi Manager client ******
                           [GitHub_license] [Discord]
 ## About: This package provides a **Multi manager client** which manages
 **manager** clients. ## Usage: > âNOTE: You need to provide your middleware
 [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-
 the-environment) if you are not hosting STH locally. ```python import asyncio
-import json from multi_manager_client.multi_manager_client import
-MultiManagerClient from client_utils.client_utils import ClientUtils # your
-middleware token token = '' # set the token ClientUtils.setDefaultHeaders(
-{'Authorization': f'Bearer {token}'}) # middleware url api_base ='https://
-api.scramjet.cloud/api/v1' #TODO ```
+from multi_manager_client.multi_manager_client import MultiManagerClient from
+client_utils.base_client import BaseClient # your middleware token token = '' #
+set the token BaseClient.setDefaultHeaders({'Authorization': f'Bearer
+{token}'}) # middleware url api_base ='https://api.scramjet.cloud/api/v1' #TODO
+```
```

