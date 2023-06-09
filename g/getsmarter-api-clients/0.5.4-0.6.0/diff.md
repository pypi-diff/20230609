# Comparing `tmp/getsmarter-api-clients-0.5.4.tar.gz` & `tmp/getsmarter-api-clients-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsmarter-api-clients-0.5.4.tar", last modified: Tue May  9 15:19:44 2023, max compression
+gzip compressed data, was "getsmarter-api-clients-0.6.0.tar", last modified: Fri Jun  9 14:52:35 2023, max compression
```

## Comparing `getsmarter-api-clients-0.5.4.tar` & `getsmarter-api-clients-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6307 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/getsmarter_api_clients/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9862 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients/geag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6307 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-09 15:19:44.625422 getsmarter-api-clients-0.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.068590 getsmarter-api-clients-0.6.0/getsmarter_api_clients/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients/geag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/setup.py
```

### Comparing `getsmarter-api-clients-0.5.4/CHANGELOG.rst` & `getsmarter-api-clients-0.6.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,21 @@
    
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
+* Nothing unreleased
 
-*
+[0.6.0]
+~~~~~~~
+* Adds optional arg to create_enterprise_allocation() to either raise (current/default behavior),
+  or not raise and fall through to returning the response. This will allow callers
+  to do things with the response payload in error conditions.
 
 [0.5.4]
 ~~~~~~~
 * Add `org_id`` as an optional enterprise allocation param
 
 [0.5.3]
 ~~~~~~~
```

### Comparing `getsmarter-api-clients-0.5.4/LICENSE.txt` & `getsmarter-api-clients-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.4/PKG-INFO` & `getsmarter-api-clients-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.5.4
+Version: 0.6.0
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -166,16 +166,21 @@
    
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
+* Nothing unreleased
 
-*
+[0.6.0]
+~~~~~~~
+* Adds optional arg to create_enterprise_allocation() to either raise (current/default behavior),
+  or not raise and fall through to returning the response. This will allow callers
+  to do things with the response payload in error conditions.
 
 [0.5.4]
 ~~~~~~~
 * Add `org_id`` as an optional enterprise allocation param
 
 [0.5.3]
 ~~~~~~~
```

### Comparing `getsmarter-api-clients-0.5.4/README.rst` & `getsmarter-api-clients-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.4/getsmarter_api_clients/geag.py` & `getsmarter-api-clients-0.6.0/getsmarter_api_clients/geag.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,16 @@
         state=None,
         state_code=None,
         country=None,
         country_code=None,
         mobile_phone=None,
         work_experience=None,
         education_highest_level=None,
-        org_id=None
+        org_id=None,
+        should_raise=True,
     ):
         """
         Create an enterprise_allocation (enrollment) through GEAG.
 
         :Parameters:
           - `payment_reference (str)`: Reference used by enterprise partner
             when payment is made to GetSmarter
@@ -265,9 +266,10 @@
         except HTTPError:
             message = (
               f'Enterprise allocation failed to be created for order {payment_reference} '
               f'with reasons: {response.text}, '
               f'with payload: {payload}'
             )
             logger.error(message)
-            raise
+            if should_raise:
+                raise
         return response
```

### Comparing `getsmarter-api-clients-0.5.4/getsmarter_api_clients/oauth.py` & `getsmarter-api-clients-0.6.0/getsmarter_api_clients/oauth.py`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/PKG-INFO` & `getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.5.4
+Version: 0.6.0
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -166,16 +166,21 @@
    
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
+* Nothing unreleased
 
-*
+[0.6.0]
+~~~~~~~
+* Adds optional arg to create_enterprise_allocation() to either raise (current/default behavior),
+  or not raise and fall through to returning the response. This will allow callers
+  to do things with the response payload in error conditions.
 
 [0.5.4]
 ~~~~~~~
 * Add `org_id`` as an optional enterprise allocation param
 
 [0.5.3]
 ~~~~~~~
```

### Comparing `getsmarter-api-clients-0.5.4/requirements/constraints.txt` & `getsmarter-api-clients-0.6.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.4/setup.py` & `getsmarter-api-clients-0.6.0/setup.py`

 * *Files identical despite different names*

