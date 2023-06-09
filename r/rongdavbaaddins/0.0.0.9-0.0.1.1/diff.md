# Comparing `tmp/rongdavbaaddins-0.0.0.9.tar.gz` & `tmp/rongdavbaaddins-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.0.9.tar", last modified: Thu Jun  8 09:58:32 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.1.1.tar", last modified: Fri Jun  9 03:54:23 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.0.9.tar` & `rongdavbaaddins-0.0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.436972 rongdavbaaddins-0.0.0.9/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-06-08 09:58:32.437970 rongdavbaaddins-0.0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.409973 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.416937 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0   107844 2023-06-08 09:52:04.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.423936 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      384 2023-06-08 09:57:48.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/minusFunction.pyd
--rw-rw-rw-   0        0        0   140800 2023-06-08 09:56:35.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/rongdaVbaAddins.pyd
--rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    27804 2023-06-08 09:52:05.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.433936 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-08 09:58:32.438977 rongdavbaaddins-0.0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-06-08 09:58:30.000000 rongdavbaaddins-0.0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.966097 rongdavbaaddins-0.0.1.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      409 2023-06-09 03:54:23.966097 rongdavbaaddins-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.923140 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.937095 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   107928 2023-06-09 03:53:46.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.944092 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      384 2023-06-08 09:57:48.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   141824 2023-06-09 03:53:51.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/rongdaVbaAddins.pyd
+-rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27804 2023-06-09 03:47:56.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.962091 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-09 03:54:23.968091 rongdavbaaddins-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-06-09 03:54:21.000000 rongdavbaaddins-0.0.1.1/setup.py
```

### Comparing `rongdavbaaddins-0.0.0.9/LICENSE.txt` & `rongdavbaaddins-0.0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py` & `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.9/setup.py` & `rongdavbaaddins-0.0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.9"
+PATCH = 1
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

