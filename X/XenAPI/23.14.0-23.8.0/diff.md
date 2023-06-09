# Comparing `tmp/XenAPI-23.14.0.tar.gz` & `tmp/XenAPI-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XenAPI-23.14.0.tar", last modified: Fri Jun  9 13:04:37 2023, max compression
+gzip compressed data, was "XenAPI-23.8.0.tar", last modified: Wed Mar  8 14:57:18 2023, max compression
```

## Comparing `XenAPI-23.14.0.tar` & `XenAPI-23.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:04:37.603822 XenAPI-23.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-09 13:03:53.000000 XenAPI-23.14.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-09 13:04:37.603822 XenAPI-23.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-09 13:03:53.000000 XenAPI-23.14.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:04:37.603822 XenAPI-23.14.0/XenAPI/
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-09 13:03:53.000000 XenAPI-23.14.0/XenAPI/XenAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 13:03:53.000000 XenAPI-23.14.0/XenAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:04:37.603822 XenAPI-23.14.0/XenAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-09 13:04:37.000000 XenAPI-23.14.0/XenAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-09 13:04:37.000000 XenAPI-23.14.0/XenAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:04:37.000000 XenAPI-23.14.0/XenAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 13:04:37.000000 XenAPI-23.14.0/XenAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-09 13:03:53.000000 XenAPI-23.14.0/XenAPIPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-09 13:03:53.000000 XenAPI-23.14.0/echo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-06-09 13:03:53.000000 XenAPI-23.14.0/exportimport.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-09 13:03:53.000000 XenAPI-23.14.0/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 13:03:53.000000 XenAPI-23.14.0/lvhd-api-test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-09 13:03:53.000000 XenAPI-23.14.0/mini-xenrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-09 13:03:53.000000 XenAPI-23.14.0/monitor-unwanted-domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-09 13:03:53.000000 XenAPI-23.14.0/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 13:03:53.000000 XenAPI-23.14.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     6386 2023-06-09 13:03:53.000000 XenAPI-23.14.0/renameif.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-09 13:04:37.603822 XenAPI-23.14.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-09 13:03:53.000000 XenAPI-23.14.0/shell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4710 2023-06-09 13:03:53.000000 XenAPI-23.14.0/xva.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:57:18.712777 XenAPI-23.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-08 14:56:48.000000 XenAPI-23.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-08 14:57:18.712777 XenAPI-23.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-08 14:56:48.000000 XenAPI-23.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:57:18.708777 XenAPI-23.8.0/XenAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-03-08 14:56:48.000000 XenAPI-23.8.0/XenAPI/XenAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 14:56:48.000000 XenAPI-23.8.0/XenAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:57:18.712777 XenAPI-23.8.0/XenAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-08 14:57:18.000000 XenAPI-23.8.0/XenAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-08 14:57:18.000000 XenAPI-23.8.0/XenAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 14:57:18.000000 XenAPI-23.8.0/XenAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 14:57:18.000000 XenAPI-23.8.0/XenAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-08 14:56:48.000000 XenAPI-23.8.0/XenAPIPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-08 14:56:48.000000 XenAPI-23.8.0/echo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-03-08 14:56:48.000000 XenAPI-23.8.0/exportimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-08 14:56:48.000000 XenAPI-23.8.0/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-08 14:56:48.000000 XenAPI-23.8.0/lvhd-api-test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-03-08 14:56:48.000000 XenAPI-23.8.0/mini-xenrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-08 14:56:48.000000 XenAPI-23.8.0/monitor-unwanted-domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-08 14:56:48.000000 XenAPI-23.8.0/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-08 14:56:48.000000 XenAPI-23.8.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6386 2023-03-08 14:56:48.000000 XenAPI-23.8.0/renameif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-08 14:57:18.712777 XenAPI-23.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-08 14:56:48.000000 XenAPI-23.8.0/shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4710 2023-03-08 14:56:48.000000 XenAPI-23.8.0/xva.py
```

### Comparing `XenAPI-23.14.0/PKG-INFO` & `XenAPI-23.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XenAPI
-Version: 23.14.0
+Version: 23.8.0
 Summary: XenAPI SDK, for communication with XenServer.
 Home-page: https://www.citrix.com/community/citrix-developer/citrix-hypervisor-developer/
 Author: Citrix Systems, Inc.
 Author-email: xen-api@lists.xenproject.org
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/xapi-project/xen-api/issues
 Project-URL: Source Code, https://github.com/xapi-project/xen-api
```

### Comparing `XenAPI-23.14.0/README.md` & `XenAPI-23.8.0/README.md`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/XenAPI/XenAPI.py` & `XenAPI-23.8.0/XenAPI/XenAPI.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/XenAPI.egg-info/PKG-INFO` & `XenAPI-23.8.0/XenAPI.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XenAPI
-Version: 23.14.0
+Version: 23.8.0
 Summary: XenAPI SDK, for communication with XenServer.
 Home-page: https://www.citrix.com/community/citrix-developer/citrix-hypervisor-developer/
 Author: Citrix Systems, Inc.
 Author-email: xen-api@lists.xenproject.org
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/xapi-project/xen-api/issues
 Project-URL: Source Code, https://github.com/xapi-project/xen-api
```

### Comparing `XenAPI-23.14.0/XenAPIPlugin.py` & `XenAPI-23.8.0/XenAPIPlugin.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/exportimport.py` & `XenAPI-23.8.0/exportimport.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/inventory.py` & `XenAPI-23.8.0/inventory.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/lvhd-api-test.py` & `XenAPI-23.8.0/lvhd-api-test.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/mini-xenrt.py` & `XenAPI-23.8.0/mini-xenrt.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/monitor-unwanted-domains.py` & `XenAPI-23.8.0/monitor-unwanted-domains.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/provision.py` & `XenAPI-23.8.0/provision.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/renameif.py` & `XenAPI-23.8.0/renameif.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/setup.cfg` & `XenAPI-23.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/shell.py` & `XenAPI-23.8.0/shell.py`

 * *Files identical despite different names*

### Comparing `XenAPI-23.14.0/xva.py` & `XenAPI-23.8.0/xva.py`

 * *Files identical despite different names*

