# Comparing `tmp/alibabacloud_resourcecenter20221201_py2-1.0.1.tar.gz` & `tmp/alibabacloud_resourcecenter20221201_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcecenter20221201_py2-1.0.1.tar", last modified: Wed Mar  8 03:43:43 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcecenter20221201_py2-1.0.2.tar", last modified: Fri Jun  9 11:33:31 2023, max compression
```

## Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1.tar` & `alibabacloud_resourcecenter20221201_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2538 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1066 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1149 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20281 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201/client.py
--rw-r--r--   0 root         (0) root         (0)    83759 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2538 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-08 03:43:43.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2958 2023-03-08 03:43:42.000000 alibabacloud_resourcecenter20221201_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22496 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201/client.py
+-rw-r--r--   0 root         (0) root         (0)   108194 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 11:33:31.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-06-09 11:33:30.000000 alibabacloud_resourcecenter20221201_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/LICENSE` & `alibabacloud_resourcecenter20221201_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/PKG-INFO` & `alibabacloud_resourcecenter20221201_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcecenter20221201_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud ResourceCenter (20221201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/README-CN.md` & `alibabacloud_resourcecenter20221201_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/README.md` & `alibabacloud_resourcecenter20221201_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201/client.py` & `alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,24 @@
         )
 
     def disable_resource_center(self):
         runtime = util_models.RuntimeOptions()
         return self.disable_resource_center_with_options(runtime)
 
     def enable_multi_account_resource_center_with_options(self, runtime):
+        """
+        If you have created a resource directory for your enterprise, you can enable the cross-account resource search feature by using the management account of the resource directory or a delegated administrator account of Resource Center to view the resources of members in the resource directory. For more information about a resource directory, see [Resource Directory overview](~~200506~~).
+        
+
+        @param request: EnableMultiAccountResourceCenterRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: EnableMultiAccountResourceCenterResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='EnableMultiAccountResourceCenter',
             version='2022-12-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -89,14 +99,20 @@
         )
         return TeaCore.from_map(
             resource_center_20221201_models.EnableMultiAccountResourceCenterResponse(),
             self.call_api(params, req, runtime)
         )
 
     def enable_multi_account_resource_center(self):
+        """
+        If you have created a resource directory for your enterprise, you can enable the cross-account resource search feature by using the management account of the resource directory or a delegated administrator account of Resource Center to view the resources of members in the resource directory. For more information about a resource directory, see [Resource Directory overview](~~200506~~).
+        
+
+        @return: EnableMultiAccountResourceCenterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_multi_account_resource_center_with_options(runtime)
 
     def enable_resource_center_with_options(self, runtime):
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='EnableResourceCenter',
@@ -224,14 +240,44 @@
             self.call_api(params, req, runtime)
         )
 
     def get_resource_configuration(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_resource_configuration_with_options(request, runtime)
 
+    def get_resource_counts_with_options(self, request, runtime):
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
+    def get_resource_counts(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_resource_counts_with_options(request, runtime)
+
     def list_multi_account_resource_groups_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
```

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/PKG-INFO` & `alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcecenter20221201-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud ResourceCenter (20221201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/alibabacloud_resourcecenter20221201_py2.egg-info/SOURCES.txt` & `alibabacloud_resourcecenter20221201_py2-1.0.2/alibabacloud_resourcecenter20221201_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcecenter20221201_py2-1.0.1/setup.py` & `alibabacloud_resourcecenter20221201_py2-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcecenter20221201_py2.
 
-Created on 08/03/2023
+Created on 09/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcecenter20221201"
 NAME = "alibabacloud_resourcecenter20221201_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceCenter (20221201) SDK Library for Python2"
```

