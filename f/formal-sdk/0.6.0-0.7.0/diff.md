# Comparing `tmp/formal-sdk-0.6.0.tar.gz` & `tmp/formal-sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-0.6.0.tar", last modified: Thu Jun  8 14:08:31 2023, max compression
+gzip compressed data, was "formal-sdk-0.7.0.tar", last modified: Thu Jun  8 22:38:18 2023, max compression
```

## Comparing `formal-sdk-0.6.0.tar` & `formal-sdk-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.496161 formal-sdk-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.496161 formal-sdk-0.6.0/src/formal_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/src/formal_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/src/formal_sdk/datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:38:18.168105 formal-sdk-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-08 22:38:18.168105 formal-sdk-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:38:18.168105 formal-sdk-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:38:18.164105 formal-sdk-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:38:18.164105 formal-sdk-0.7.0/src/formal_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/src/formal_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/src/formal_sdk/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-08 22:38:00.000000 formal-sdk-0.7.0/src/formal_sdk/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:38:18.164105 formal-sdk-0.7.0/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-08 22:38:18.000000 formal-sdk-0.7.0/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-08 22:38:18.000000 formal-sdk-0.7.0/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:38:18.000000 formal-sdk-0.7.0/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:38:18.000000 formal-sdk-0.7.0/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 22:38:18.000000 formal-sdk-0.7.0/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-0.6.0/LICENSE` & `formal-sdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.6.0/PKG-INFO` & `formal-sdk-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 0.6.0
+Version: 0.7.0
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,25 +46,29 @@
 
 ```python
 import os
 import formal_sdk
 
 if __name__ == '__main__':
 
-    dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
-    nativeRoleId = "abc"
-    nativeRoleSecret = "nativeSecret"
+    dataStoreId = ""
+    nativeRoleId = ""
+    nativeRoleSecret = ""
     useAsDefault = True
     apiKey = os.environ.get('TEST_API_KEY')
     
     newClient = formal_sdk.Client(apiKey)
     # Create Native Role
     createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
     
     # Get Native Role    
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
     print(f'NativeRoleId: {previousRole.nativeRoleId}')
     print(f'NativeRoleSecret: {previousRole.nativeRoleSecret}')
     print(f'UseAsDefault: {previousRole.useAsDefault}')
+
+    # Get sidecar tls certificate and private key
+    sidecarId = ""
+    certificate, privateKey, fullSecret = newClient.SidecarClient.GetTLSCertificate(sidecarId)
 ```
```

### Comparing `formal-sdk-0.6.0/README.md` & `formal-sdk-0.7.0/src/example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-# Formal Admin Python SDK
-
-
-This is the Python SDK for the Formal Admin API.
-
-
-
-## Installing
-    pip install formal-sdk
-
-## Example Use
-
-Create and Get a Native Role
-
-```python
 import os
 import formal_sdk
 
 if __name__ == '__main__':
 
-    dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
-    nativeRoleId = "abc"
-    nativeRoleSecret = "nativeSecret"
+    dataStoreId = ""
+    nativeRoleId = ""
+    nativeRoleSecret = ""
     useAsDefault = True
     apiKey = os.environ.get('TEST_API_KEY')
-    
+
     newClient = formal_sdk.Client(apiKey)
     # Create Native Role
     createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
-    
-    # Get Native Role    
+
+    # Get Native Role
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
     print(f'NativeRoleId: {previousRole.nativeRoleId}')
     print(f'NativeRoleSecret: {previousRole.nativeRoleSecret}')
     print(f'UseAsDefault: {previousRole.useAsDefault}')
-```
+
+    # Get sidecar tls cert by id
+    sidecarId = ""
+    certificate, privateKey, fullSecret = newClient.SidecarClient.GetTLSCertificate(sidecarId)
```

### Comparing `formal-sdk-0.6.0/pyproject.toml` & `formal-sdk-0.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-sdk"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal SDK"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-sdk-0.6.0/src/example.py` & `formal-sdk-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,42 @@
+# Formal Admin Python SDK
+
+
+This is the Python SDK for the Formal Admin API.
+
+
+
+## Installing
+    pip install formal-sdk
+
+## Example Use
+
+Create and Get a Native Role
+
+```python
 import os
 import formal_sdk
 
 if __name__ == '__main__':
 
-    dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
-    nativeRoleId = "abc"
-    nativeRoleSecret = "nativeSecret"
+    dataStoreId = ""
+    nativeRoleId = ""
+    nativeRoleSecret = ""
     useAsDefault = True
-    apiKey = os.environ.get('r629SJ3yWVYk07vhB1gXdb8jQoHA5D4e')
-
+    apiKey = os.environ.get('TEST_API_KEY')
+    
     newClient = formal_sdk.Client(apiKey)
     # Create Native Role
-    # createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
-
-    # Get Native Role
+    createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
+    
+    # Get Native Role    
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
     print(f'NativeRoleId: {previousRole.nativeRoleId}')
     print(f'NativeRoleSecret: {previousRole.nativeRoleSecret}')
-    print(f'UseAsDefault: {previousRole.useAsDefault}')
+    print(f'UseAsDefault: {previousRole.useAsDefault}')
+
+    # Get sidecar tls certificate and private key
+    sidecarId = ""
+    certificate, privateKey, fullSecret = newClient.SidecarClient.GetTLSCertificate(sidecarId)
+```
```

### Comparing `formal-sdk-0.6.0/src/formal_sdk/datastore.py` & `formal-sdk-0.7.0/src/formal_sdk/datastore.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.6.0/src/formal_sdk.egg-info/PKG-INFO` & `formal-sdk-0.7.0/src/formal_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 0.6.0
+Version: 0.7.0
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,25 +46,29 @@
 
 ```python
 import os
 import formal_sdk
 
 if __name__ == '__main__':
 
-    dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
-    nativeRoleId = "abc"
-    nativeRoleSecret = "nativeSecret"
+    dataStoreId = ""
+    nativeRoleId = ""
+    nativeRoleSecret = ""
     useAsDefault = True
     apiKey = os.environ.get('TEST_API_KEY')
     
     newClient = formal_sdk.Client(apiKey)
     # Create Native Role
     createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
     
     # Get Native Role    
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
     print(f'NativeRoleId: {previousRole.nativeRoleId}')
     print(f'NativeRoleSecret: {previousRole.nativeRoleSecret}')
     print(f'UseAsDefault: {previousRole.useAsDefault}')
+
+    # Get sidecar tls certificate and private key
+    sidecarId = ""
+    certificate, privateKey, fullSecret = newClient.SidecarClient.GetTLSCertificate(sidecarId)
 ```
```

