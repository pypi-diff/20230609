# Comparing `tmp/scramjet_manager_client-1.0.1.tar.gz` & `tmp/scramjet-manager-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scramjet_manager_client-1.0.1.tar", max compression
+gzip compressed data, was "scramjet-manager-client-1.1.0.tar", last modified: Fri Jun  9 11:35:42 2023, max compression
```

## Comparing `scramjet_manager_client-1.0.1.tar` & `scramjet-manager-client-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0     1356 2023-01-10 13:35:41.864091 scramjet_manager_client-1.0.1/README.md
--rw-r--r--   0        0        0        0 2022-09-22 12:14:06.000000 scramjet_manager_client-1.0.1/manager_client/__init__.py
--rw-r--r--   0        0        0     1250 2023-01-10 13:33:27.244809 scramjet_manager_client-1.0.1/manager_client/manager_client.py
--rw-r--r--   0        0        0      390 2023-01-10 13:33:37.164754 scramjet_manager_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2065 1970-01-01 00:00:00.000000 scramjet_manager_client-1.0.1/setup.py
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 scramjet_manager_client-1.0.1/PKG-INFO
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:35:42.478759 scramjet-manager-client-1.1.0/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1579 2023-06-09 11:35:42.478759 scramjet-manager-client-1.1.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1302 2023-04-26 06:20:09.000000 scramjet-manager-client-1.1.0/README.md
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:35:42.478759 scramjet-manager-client-1.1.0/manager_client/
+-rw-rw-r--   0 bob       (1000) bob       (1000)        0 2023-04-25 19:55:28.000000 scramjet-manager-client-1.1.0/manager_client/__init__.py
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1641 2023-04-28 10:00:38.000000 scramjet-manager-client-1.1.0/manager_client/manager_client.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:35:42.478759 scramjet-manager-client-1.1.0/scramjet_manager_client.egg-info/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1579 2023-06-09 11:35:42.000000 scramjet-manager-client-1.1.0/scramjet_manager_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)      312 2023-06-09 11:35:42.000000 scramjet-manager-client-1.1.0/scramjet_manager_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2023-06-09 11:35:42.000000 scramjet-manager-client-1.1.0/scramjet_manager_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       56 2023-06-09 11:35:42.000000 scramjet-manager-client-1.1.0/scramjet_manager_client.egg-info/requires.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       15 2023-06-09 11:35:42.000000 scramjet-manager-client-1.1.0/scramjet_manager_client.egg-info/top_level.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       38 2023-06-09 11:35:42.478759 scramjet-manager-client-1.1.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)      809 2023-06-09 11:35:24.000000 scramjet-manager-client-1.1.0/setup.py
```

### Comparing `scramjet_manager_client-1.0.1/README.md` & `scramjet-manager-client-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 
 ## Usage:
 
 > ❗NOTE: You need to provide your middleware [access token](https://docs.scramjet.org/platform/quick-start#step-1-set-up-the-environment) if you are not hosting STH locally.
 
 ```python
 import asyncio
-import json
 from manager_client.manager_client import ManagerClient
-from client_utils.client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
 # url = {middlewareURL}/space/{manager_id}/api/v1
 manager = ManagerClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-manager/api/v1')
+
 res = asyncio.run(manager.get_hosts())
-# convert response to json
-hosts = json.loads(res)
+print(res)
 ```
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
                      ****** Scramjet Manager client ******
                           [GitHub_license] [Discord]
 ## About: This package provides a **Manager client** which manages [Transform
 Hub](https://github.com/scramjetorg/transform-hub) clients. ## Usage: >
 âNOTE: You need to provide your middleware [access token](https://
 docs.scramjet.org/platform/quick-start#step-1-set-up-the-environment) if you
-are not hosting STH locally. ```python import asyncio import json from
+are not hosting STH locally. ```python import asyncio from
 manager_client.manager_client import ManagerClient from
-client_utils.client_utils import ClientUtils # your middleware token token = ''
-# set the token ClientUtils.setDefaultHeaders({'Authorization': f'Bearer
+client_utils.base_client import BaseClient # your middleware token token = '' #
+set the token BaseClient.setDefaultHeaders({'Authorization': f'Bearer
 {token}'}) # middleware url api_base ='https://api.scramjet.cloud/api/v1' # url
 = {middlewareURL}/space/{manager_id}/api/v1 manager = ManagerClient(f'
 {api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-manager/api/v1') res
-= asyncio.run(manager.get_hosts()) # convert response to json hosts =
-json.loads(res) ```
+= asyncio.run(manager.get_hosts()) print(res) ```
```

