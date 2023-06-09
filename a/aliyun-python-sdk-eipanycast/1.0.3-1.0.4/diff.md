# Comparing `tmp/aliyun-python-sdk-eipanycast-1.0.3.tar.gz` & `tmp/aliyun-python-sdk-eipanycast-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eipanycast-1.0.3.tar", last modified: Fri Apr  7 10:49:28 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eipanycast-1.0.4.tar", last modified: Fri Jun  9 04:50:47 2023, max compression
```

## Comparing `aliyun-python-sdk-eipanycast-1.0.3.tar` & `aliyun-python-sdk-eipanycast-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1572 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1301 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/
--rw-r--r--   0 root         (0) root         (0)     2746 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     1693 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 10:49:28.000000 aliyun-python-sdk-eipanycast-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2487 2023-04-07 10:49:27.000000 aliyun-python-sdk-eipanycast-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/setup.py
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/LICENSE` & `aliyun-python-sdk-eipanycast-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/PKG-INFO` & `aliyun-python-sdk-eipanycast-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eipanycast
-Version: 1.0.3
+Version: 1.0.4
 Summary: The eipanycast module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eipanycast
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/README.rst` & `aliyun-python-sdk-eipanycast-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO` & `aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eipanycast
-Version: 1.0.3
+Version: 1.0.4
 Summary: The eipanycast module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eipanycast
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt` & `aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,13 +13,16 @@
 aliyunsdkeipanycast/request/__init__.py
 aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py
 aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py
 aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py
 aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py
 aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py
 aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py
+aliyunsdkeipanycast/request/v20200309/ListTagResourcesRequest.py
 aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py
 aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py
 aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py
+aliyunsdkeipanycast/request/v20200309/TagResourcesRequest.py
 aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py
+aliyunsdkeipanycast/request/v20200309/UntagResourcesRequest.py
 aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py
 aliyunsdkeipanycast/request/v20200309/__init__.py
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/endpoint.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class AllocateAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AllocateAnycastEipAddress','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AllocateAnycastEipAddress')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class AssociateAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AssociateAnycastEipAddress','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AssociateAnycastEipAddress')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class DescribeAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastEipAddress','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastEipAddress')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class DescribeAnycastPopLocationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastPopLocations','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastPopLocations')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class DescribeAnycastServerRegionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastServerRegions','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastServerRegions')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ListAnycastEipAddressesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ListAnycastEipAddresses','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ListAnycastEipAddresses')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ModifyAnycastEipAddressAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressAttribute','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressAttribute')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ModifyAnycastEipAddressSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressSpec','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressSpec')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ReleaseAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ReleaseAnycastEipAddress','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ReleaseAnycastEipAddress')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class UnassociateAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UnassociateAnycastEipAddress','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UnassociateAnycastEipAddress')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py` & `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class UpdateAnycastEipAddressAssociationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UpdateAnycastEipAddressAssociations','eipanycast')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UpdateAnycastEipAddressAssociations')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.3/setup.py` & `aliyun-python-sdk-eipanycast-1.0.4/setup.py`

 * *Files identical despite different names*

