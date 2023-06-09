# Comparing `tmp/quickstart-vdk-0.2.893910391.dev11244.tar.gz` & `tmp/quickstart-vdk-0.2.894599572.dev11255.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.893910391.dev11244.tar", last modified: Thu Jun  8 13:25:58 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.894599572.dev11255.tar", last modified: Fri Jun  9 04:23:20 2023, max compression
```

## Comparing `quickstart-vdk-0.2.893910391.dev11244.tar` & `quickstart-vdk-0.2.894599572.dev11255.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:25:58.561204 quickstart-vdk-0.2.893910391.dev11244/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-08 13:25:58.557204 quickstart-vdk-0.2.893910391.dev11244/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-08 13:25:37.000000 quickstart-vdk-0.2.893910391.dev11244/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:25:58.557204 quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-08 13:25:58.000000 quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-08 13:25:58.000000 quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:25:58.000000 quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-08 13:25:58.000000 quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-08 13:25:58.000000 quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 13:25:58.561204 quickstart-vdk-0.2.893910391.dev11244/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-08 13:25:48.000000 quickstart-vdk-0.2.893910391.dev11244/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:25:58.557204 quickstart-vdk-0.2.893910391.dev11244/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-08 13:25:37.000000 quickstart-vdk-0.2.893910391.dev11244/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:23:20.665229 quickstart-vdk-0.2.894599572.dev11255/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-09 04:23:20.665229 quickstart-vdk-0.2.894599572.dev11255/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-09 04:20:21.000000 quickstart-vdk-0.2.894599572.dev11255/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:23:20.661229 quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-09 04:23:20.000000 quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-09 04:23:20.000000 quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:23:20.000000 quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-09 04:23:20.000000 quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 04:23:20.000000 quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 04:23:20.665229 quickstart-vdk-0.2.894599572.dev11255/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-09 04:23:10.000000 quickstart-vdk-0.2.894599572.dev11255/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:23:20.661229 quickstart-vdk-0.2.894599572.dev11255/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-09 04:20:21.000000 quickstart-vdk-0.2.894599572.dev11255/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.893910391.dev11244/PKG-INFO` & `quickstart-vdk-0.2.894599572.dev11255/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.893910391.dev11244
+Version: 0.2.894599572.dev11255
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.893910391.dev11244/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.894599572.dev11255/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.893910391.dev11244
+Version: 0.2.894599572.dev11255
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.893910391.dev11244/setup.py` & `quickstart-vdk-0.2.894599572.dev11255/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.893910391.dev11244"
+__version__ = "0.2.894599572.dev11255"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

