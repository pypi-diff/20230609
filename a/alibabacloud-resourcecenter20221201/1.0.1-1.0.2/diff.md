# Comparing `tmp/alibabacloud_resourcecenter20221201-1.0.1.tar.gz` & `tmp/alibabacloud_resourcecenter20221201-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcecenter20221201-1.0.1.tar", last modified: Wed Mar  8 03:44:28 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcecenter20221201-1.0.2.tar", last modified: Fri Jun  9 11:34:14 2023, max compression
```

## Comparing `alibabacloud_resourcecenter20221201-1.0.1.tar` & `alibabacloud_resourcecenter20221201-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 03:44:28.000000 alibabacloud_resourcecenter20221201-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-08 03:44:28.000000 alibabacloud_resourcecenter20221201-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 03:44:28.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49225 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201/client.py
--rw-r--r--   0 root         (0) root         (0)    83059 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 03:44:28.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-08 03:44:28.000000 alibabacloud_resourcecenter20221201-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2023-03-08 03:44:27.000000 alibabacloud_resourcecenter20221201-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54335 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201/client.py
+-rw-r--r--   0 root         (0) root         (0)   107440 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-06-09 11:34:14.000000 alibabacloud_resourcecenter20221201-1.0.2/setup.py
```

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/LICENSE` & `alibabacloud_resourcecenter20221201-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/PKG-INFO` & `alibabacloud_resourcecenter20221201-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcecenter20221201
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud ResourceCenter (20221201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/README-CN.md` & `alibabacloud_resourcecenter20221201-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/README.md` & `alibabacloud_resourcecenter20221201-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201/client.py` & `alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,21 @@
         runtime = util_models.RuntimeOptions()
         return await self.disable_resource_center_with_options_async(runtime)
 
     def enable_multi_account_resource_center_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_center_20221201_models.EnableMultiAccountResourceCenterResponse:
+        """
+        If you have created a resource directory for your enterprise, you can enable the cross-account resource search feature by using the management account of the resource directory or a delegated administrator account of Resource Center to view the resources of members in the resource directory. For more information about a resource directory, see [Resource Directory overview](~~200506~~).
+        
+        @param request: EnableMultiAccountResourceCenterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableMultiAccountResourceCenterResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='EnableMultiAccountResourceCenter',
             version='2022-12-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -162,14 +169,21 @@
             self.call_api(params, req, runtime)
         )
 
     async def enable_multi_account_resource_center_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_center_20221201_models.EnableMultiAccountResourceCenterResponse:
+        """
+        If you have created a resource directory for your enterprise, you can enable the cross-account resource search feature by using the management account of the resource directory or a delegated administrator account of Resource Center to view the resources of members in the resource directory. For more information about a resource directory, see [Resource Directory overview](~~200506~~).
+        
+        @param request: EnableMultiAccountResourceCenterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableMultiAccountResourceCenterResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='EnableMultiAccountResourceCenter',
             version='2022-12-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -180,18 +194,28 @@
         )
         return TeaCore.from_map(
             resource_center_20221201_models.EnableMultiAccountResourceCenterResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_multi_account_resource_center(self) -> resource_center_20221201_models.EnableMultiAccountResourceCenterResponse:
+        """
+        If you have created a resource directory for your enterprise, you can enable the cross-account resource search feature by using the management account of the resource directory or a delegated administrator account of Resource Center to view the resources of members in the resource directory. For more information about a resource directory, see [Resource Directory overview](~~200506~~).
+        
+        @return: EnableMultiAccountResourceCenterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_multi_account_resource_center_with_options(runtime)
 
     async def enable_multi_account_resource_center_async(self) -> resource_center_20221201_models.EnableMultiAccountResourceCenterResponse:
+        """
+        If you have created a resource directory for your enterprise, you can enable the cross-account resource search feature by using the management account of the resource directory or a delegated administrator account of Resource Center to view the resources of members in the resource directory. For more information about a resource directory, see [Resource Directory overview](~~200506~~).
+        
+        @return: EnableMultiAccountResourceCenterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_multi_account_resource_center_with_options_async(runtime)
 
     def enable_resource_center_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_center_20221201_models.EnableResourceCenterResponse:
@@ -497,14 +521,88 @@
     async def get_resource_configuration_async(
         self,
         request: resource_center_20221201_models.GetResourceConfigurationRequest,
     ) -> resource_center_20221201_models.GetResourceConfigurationResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_resource_configuration_with_options_async(request, runtime)
 
+    def get_resource_counts_with_options(
+        self,
+        request: resource_center_20221201_models.GetResourceCountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> resource_center_20221201_models.GetResourceCountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.group_by_key):
+            query['GroupByKey'] = request.group_by_key
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetResourceCounts',
+            version='2022-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            resource_center_20221201_models.GetResourceCountsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_resource_counts_with_options_async(
+        self,
+        request: resource_center_20221201_models.GetResourceCountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> resource_center_20221201_models.GetResourceCountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.group_by_key):
+            query['GroupByKey'] = request.group_by_key
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetResourceCounts',
+            version='2022-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            resource_center_20221201_models.GetResourceCountsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_resource_counts(
+        self,
+        request: resource_center_20221201_models.GetResourceCountsRequest,
+    ) -> resource_center_20221201_models.GetResourceCountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_resource_counts_with_options(request, runtime)
+
+    async def get_resource_counts_async(
+        self,
+        request: resource_center_20221201_models.GetResourceCountsRequest,
+    ) -> resource_center_20221201_models.GetResourceCountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_resource_counts_with_options_async(request, runtime)
+
     def list_multi_account_resource_groups_with_options(
         self,
         request: resource_center_20221201_models.ListMultiAccountResourceGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_center_20221201_models.ListMultiAccountResourceGroupsResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/alibabacloud_resourcecenter20221201.egg-info/PKG-INFO` & `alibabacloud_resourcecenter20221201-1.0.2/alibabacloud_resourcecenter20221201.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcecenter20221201
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud ResourceCenter (20221201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcecenter20221201-1.0.1/setup.py` & `alibabacloud_resourcecenter20221201-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcecenter20221201.
 
-Created on 08/03/2023
+Created on 09/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcecenter20221201"
 NAME = "alibabacloud_resourcecenter20221201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceCenter (20221201) SDK Library for Python"
```

