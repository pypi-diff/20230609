# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.0.9.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.0.9.tar", last modified: Tue Sep  6 03:42:26 2022, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.2.tar", last modified: Fri Jun  9 03:25:37 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.0.9.tar` & `alibabacloud_btripopen20220520_py2-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      421 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   102966 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)   734601 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2022-09-06 03:42:26.000000 alibabacloud_btripopen20220520_py2-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223086 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2001831 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.0.9/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.0.9/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.0.9
+Version: 1.1.2
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.0.9/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.0.9/README.md` & `alibabacloud_btripopen20220520_py2-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.0.9/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.0.9
+Version: 1.1.2
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.0.9/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 06/09/2022
+Created on 09/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

