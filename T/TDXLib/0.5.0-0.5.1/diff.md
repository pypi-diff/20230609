# Comparing `tmp/TDXLib-0.5.0.tar.gz` & `tmp/TDXLib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDXLib-0.5.0.tar", last modified: Tue Jun  6 19:19:28 2023, max compression
+gzip compressed data, was "TDXLib-0.5.1.tar", last modified: Fri Jun  9 19:03:38 2023, max compression
```

## Comparing `TDXLib-0.5.0.tar` & `TDXLib-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.824928 TDXLib-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 19:19:17.000000 TDXLib-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 19:19:17.000000 TDXLib-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-06 19:19:28.824928 TDXLib-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-06-06 19:19:17.000000 TDXLib-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.820928 TDXLib-0.5.0/TDXLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 19:19:17.000000 TDXLib-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:19:28.824928 TDXLib-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-06 19:19:17.000000 TDXLib-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.820928 TDXLib-0.5.0/tdxlib/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    54083 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_asset_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    46059 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_ticket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.820928 TDXLib-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-06 19:19:17.000000 TDXLib-0.5.0/test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-06 19:19:17.000000 TDXLib-0.5.0/test/test_tdx_ticket_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.802640 TDXLib-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 19:03:21.000000 TDXLib-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 19:03:21.000000 TDXLib-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-09 19:03:38.802640 TDXLib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-06-09 19:03:21.000000 TDXLib-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.798640 TDXLib-0.5.1/TDXLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 19:03:21.000000 TDXLib-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:03:38.802640 TDXLib-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-09 19:03:21.000000 TDXLib-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.802640 TDXLib-0.5.1/tdxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54083 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_asset_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46059 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_ticket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.802640 TDXLib-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-09 19:03:21.000000 TDXLib-0.5.1/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-09 19:03:21.000000 TDXLib-0.5.1/test/test_tdx_ticket_integration.py
```

### Comparing `TDXLib-0.5.0/LICENSE` & `TDXLib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/PKG-INFO` & `TDXLib-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDXLib
-Version: 0.5.0
+Version: 0.5.1
 Summary: a python library for interacting with the TeamDynamix Web API
 Home-page: https://github.com/cedarville-university/tdxlib
 Author: Nat Biggs, Stephen Gaines, Josiah Lansford
 Author-email: tdxlib@cedarville.edu
 License: GNU General Public License v3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `TDXLib-0.5.0/README.md` & `TDXLib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/TDXLib.egg-info/PKG-INFO` & `TDXLib-0.5.1/TDXLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDXLib
-Version: 0.5.0
+Version: 0.5.1
 Summary: a python library for interacting with the TeamDynamix Web API
 Home-page: https://github.com/cedarville-university/tdxlib
 Author: Nat Biggs, Stephen Gaines, Josiah Lansford
 Author-email: tdxlib@cedarville.edu
 License: GNU General Public License v3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `TDXLib-0.5.0/setup.py` & `TDXLib-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", 'r', encoding='utf-8"') as fh:
     outer_long_description = fh.read()
 
 setup(
     name='TDXLib',
     description='a python library for interacting with the TeamDynamix Web API',
-    version='0.5.0',
+    version='0.5.1',
     author='Nat Biggs, Stephen Gaines, Josiah Lansford',
     author_email='tdxlib@cedarville.edu',
     packages=['tdxlib'],
     url='https://github.com/cedarville-university/tdxlib',
     license='GNU General Public License v3.0',
     long_description_content_type='text/markdown',
     long_description=outer_long_description,
```

### Comparing `TDXLib-0.5.0/tdxlib/tdx_asset_integration.py` & `TDXLib-0.5.1/tdxlib/tdx_asset_integration.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/tdxlib/tdx_config.py` & `TDXLib-0.5.1/tdxlib/tdx_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,21 @@
             self.auth_type = self.get_value('authType')
         if not self.auth_type or self.auth_type == 'password':
             self.username = self.get_value('username')
             self.password = self.get_value('password')
         self.ticket_app_id = self.get_value('ticket_app_id')
         if not self.ticket_app_id:
             self.ticket_app_id = self.get_value('ticketAppId')
-        self.asset_app_id = self.get_value('asset_app_id')
         if not self.ticket_app_id:
-            self.ticket_app_id = self.get_value('assetAppId')
+            self.ticket_app_id = self.get_value('ticketappid')
+        self.asset_app_id = self.get_value('asset_app_id')
+        if not self.asset_app_id:
+            self.asset_app_id = self.get_value('assetAppId')
+        if not self.asset_app_id:
+            self.asset_app_id = self.get_value('assetappid')
         self.caching = self.get_value('caching', bool)
         self.timezone = self.get_value('timezone')
         self.full_host = self.get_value('full_host')
 
     def setup_from_attributes(self):
         if not self.timezone:
             self.timezone = 'Z'
```

### Comparing `TDXLib-0.5.0/tdxlib/tdx_constants.py` & `TDXLib-0.5.1/tdxlib/tdx_constants.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/tdxlib/tdx_integration.py` & `TDXLib-0.5.1/tdxlib/tdx_integration.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/tdxlib/tdx_ticket.py` & `TDXLib-0.5.1/tdxlib/tdx_ticket.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/tdxlib/tdx_ticket_integration.py` & `TDXLib-0.5.1/tdxlib/tdx_ticket_integration.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/tdxlib/tdx_utils.py` & `TDXLib-0.5.1/tdxlib/tdx_utils.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/test/test_setup.py` & `TDXLib-0.5.1/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.0/test/test_tdx_ticket_integration.py` & `TDXLib-0.5.1/test/test_tdx_ticket_integration.py`

 * *Files identical despite different names*

