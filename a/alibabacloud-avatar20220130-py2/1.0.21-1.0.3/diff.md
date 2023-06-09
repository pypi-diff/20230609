# Comparing `tmp/alibabacloud_avatar20220130_py2-1.0.21.tar.gz` & `tmp/alibabacloud_avatar20220130_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_avatar20220130_py2-1.0.21.tar", last modified: Thu Jun  8 03:50:37 2023, max compression
+gzip compressed data, was "dist/alibabacloud_avatar20220130_py2-1.0.3.tar", last modified: Thu Jul 28 03:49:33 2022, max compression
```

## Comparing `alibabacloud_avatar20220130_py2-1.0.21.tar` & `alibabacloud_avatar20220130_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/
--rw-r--r--   0 root         (0) root         (0)      467 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2491 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27296 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130/client.py
--rw-r--r--   0 root         (0) root         (0)   144945 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2491 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2023-06-08 03:50:37.000000 alibabacloud_avatar20220130_py2-1.0.21/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      139 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7719 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/client.py
+-rw-r--r--   0 root         (0) root         (0)    35687 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.21/LICENSE` & `alibabacloud_avatar20220130_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-1.0.21/PKG-INFO` & `alibabacloud_avatar20220130_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_avatar20220130_py2
-Version: 1.0.21
+Version: 1.0.3
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.21/README-CN.md` & `alibabacloud_avatar20220130_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-1.0.21/README.md` & `alibabacloud_avatar20220130_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-1.0.21/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO` & `alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-avatar20220130-py2
-Version: 1.0.21
+Version: 1.0.3
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.21/setup.py` & `alibabacloud_avatar20220130_py2-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_avatar20220130_py2.
 
-Created on 08/06/2023
+Created on 28/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_avatar20220130"
 NAME = "alibabacloud_avatar20220130_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud avatar (20220130) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

