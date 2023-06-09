# Comparing `tmp/aliyun-python-sdk-resourcecenter-1.0.2.tar.gz` & `tmp/aliyun-python-sdk-resourcecenter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-resourcecenter-1.0.2.tar", last modified: Fri Jun  2 01:54:16 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-resourcecenter-1.0.3.tar", last modified: Fri Jun  9 06:15:13 2023, max compression
```

## Comparing `aliyun-python-sdk-resourcecenter-1.0.2.tar` & `aliyun-python-sdk-resourcecenter-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1779 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/DisableMultiAccountResourceCenterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/DisableResourceCenterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/EnableMultiAccountResourceCenterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/EnableResourceCenterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceCenterServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetResourceCenterServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetResourceConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetResourceCountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountResourceGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListResourceTypesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2660 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/SearchMultiAccountResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2696 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/SearchResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-02 01:54:16.000000 aliyun-python-sdk-resourcecenter-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2507 2023-06-02 01:54:15.000000 aliyun-python-sdk-resourcecenter-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/DisableMultiAccountResourceCenterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/DisableResourceCenterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/EnableMultiAccountResourceCenterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/EnableResourceCenterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceCenterServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetResourceCenterServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetResourceConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetResourceCountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountResourceGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListResourceTypesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/SearchMultiAccountResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/SearchResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-09 06:15:13.000000 aliyun-python-sdk-resourcecenter-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-06-09 06:15:12.000000 aliyun-python-sdk-resourcecenter-1.0.3/setup.py
```

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/LICENSE` & `aliyun-python-sdk-resourcecenter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/PKG-INFO` & `aliyun-python-sdk-resourcecenter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-resourcecenter
-Version: 1.0.2
+Version: 1.0.3
 Summary: The resourcecenter module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-resourcecenter
```

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/README.rst` & `aliyun-python-sdk-resourcecenter-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/PKG-INFO` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-resourcecenter
-Version: 1.0.2
+Version: 1.0.3
 Summary: The resourcecenter module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-resourcecenter
```

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyun_python_sdk_resourcecenter.egg-info/SOURCES.txt` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyun_python_sdk_resourcecenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/DisableMultiAccountResourceCenterRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/DisableMultiAccountResourceCenterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/DisableResourceCenterRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/DisableResourceCenterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/EnableMultiAccountResourceCenterRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/EnableMultiAccountResourceCenterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/EnableResourceCenterRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/EnableResourceCenterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceCenterServiceStatusRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceCenterServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceConfigurationRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetMultiAccountResourceConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetResourceCenterServiceStatusRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetResourceCenterServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetResourceConfigurationRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetResourceConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/GetResourceCountsRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/GetResourceCountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountResourceGroupsRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountResourceGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagKeysRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagValuesRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListMultiAccountTagValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListResourceTypesRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListResourceTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListTagKeysRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/ListTagValuesRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/ListTagValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/SearchMultiAccountResourcesRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/SearchMultiAccountResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/aliyunsdkresourcecenter/request/v20221201/SearchResourcesRequest.py` & `aliyun-python-sdk-resourcecenter-1.0.3/aliyunsdkresourcecenter/request/v20221201/SearchResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcecenter-1.0.2/setup.py` & `aliyun-python-sdk-resourcecenter-1.0.3/setup.py`

 * *Files identical despite different names*

