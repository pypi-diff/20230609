# Comparing `tmp/sonic-uia2-client-0.0.4.tar.gz` & `tmp/sonic-uia2-client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonic-uia2-client-0.0.4.tar", last modified: Thu Jun  8 07:39:08 2023, max compression
+gzip compressed data, was "sonic-uia2-client-0.0.5.tar", last modified: Fri Jun  9 12:23:06 2023, max compression
```

## Comparing `sonic-uia2-client-0.0.4.tar` & `sonic-uia2-client-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.473238 sonic-uia2-client-0.0.4/client/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/client/android_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/client/uia_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.473238 sonic-uia2-client-0.0.4/common/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/resp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/sonic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/tests/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/uia2/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/uia2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/uia2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/client/android_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/client/uia_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/resp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/sonic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/tests/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/uia2/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/uia2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/uia2/driver.py
```

### Comparing `sonic-uia2-client-0.0.4/LICENSE` & `sonic-uia2-client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/PKG-INFO` & `sonic-uia2-client-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.4/README.md` & `sonic-uia2-client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/client/android_element.py` & `sonic-uia2-client-0.0.5/client/android_element.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/client/uia_client.py` & `sonic-uia2-client-0.0.5/client/uia_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/common/http_client.py` & `sonic-uia2-client-0.0.5/common/http_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/common/logger.py` & `sonic-uia2-client-0.0.5/common/logger.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/common/models.py` & `sonic-uia2-client-0.0.5/common/models.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/common/resp_handler.py` & `sonic-uia2-client-0.0.5/common/resp_handler.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/setup.py` & `sonic-uia2-client-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 4
+PATCH = 5
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 setup(
     name="sonic-uia2-client",
     version=VERSION,
     author="SonicCloudOrg",
     author_email="soniccloudorg@163.com",
```

### Comparing `sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/PKG-INFO` & `sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.4/tests/test_driver.py` & `sonic-uia2-client-0.0.5/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.4/uia2/driver.py` & `sonic-uia2-client-0.0.5/uia2/driver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from client.uia_client import UiaClient
-from common.models import PasteboardType
+from common.models import PasteboardType, AndroidSelector
 from common.resp_handler import RespHandler
 
 
 # Android Driver with uia client.
 class AndroidDriver(object):
 
     def __init__(self, url, cap=None, session_id=None, timeout=RespHandler.DEFAULT_REQUEST_TIMEOUT):
@@ -42,18 +42,18 @@
 
     def get_page_source(self):
         return self._client.page_source()
 
     def set_default_find_element_interval(self, retry: int, interval: int):
         self._client.set_default_find_element_interval(retry, interval)
 
-    def find_element(self, selector: str, value: str, retry: int = None, interval: int = None):
-        return self._client.find_element(selector, value, retry, interval)
+    def find_element(self, selector: AndroidSelector, value: str, retry: int = None, interval: int = None):
+        return self._client.find_element(selector.value, value, retry, interval)
 
-    def find_element_list(self, selector: str, value: str, retry: int = None, interval: int = None):
-        return self._client.find_element_list(selector, value, retry, interval)
+    def find_element_list(self, selector: AndroidSelector, value: str, retry: int = None, interval: int = None):
+        return self._client.find_element_list(selector.value, value, retry, interval)
 
     def screenshot(self):
         return self._client.screenshot()
 
     def set_appium_settings(self, settings: dict):
         self._client.set_appium_settings(settings)
```

