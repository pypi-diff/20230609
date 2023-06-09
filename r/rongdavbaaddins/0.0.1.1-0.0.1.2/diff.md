# Comparing `tmp/rongdavbaaddins-0.0.1.1.tar.gz` & `tmp/rongdavbaaddins-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.1.1.tar", last modified: Fri Jun  9 03:54:23 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.1.2.tar", last modified: Fri Jun  9 06:42:20 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.1.1.tar` & `rongdavbaaddins-0.0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.966097 rongdavbaaddins-0.0.1.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-06-09 03:54:23.966097 rongdavbaaddins-0.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.923140 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.937095 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0   107928 2023-06-09 03:53:46.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.944092 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      384 2023-06-08 09:57:48.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/minusFunction.pyd
--rw-rw-rw-   0        0        0   141824 2023-06-09 03:53:51.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/rongdaVbaAddins.pyd
--rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    27804 2023-06-09 03:47:56.000000 rongdavbaaddins-0.0.1.1/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-06-09 03:54:23.962091 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 03:54:23.000000 rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-09 03:54:23.968091 rongdavbaaddins-0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-06-09 03:54:21.000000 rongdavbaaddins-0.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:42:20.307159 rongdavbaaddins-0.0.1.2/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      409 2023-06-09 06:42:20.307159 rongdavbaaddins-0.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:42:20.259158 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-09 06:42:20.275159 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   107778 2023-06-09 06:10:47.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-09 06:42:20.285113 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   141824 2023-06-09 06:40:27.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/rongdaVbaAddins.pyd
+-rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27804 2023-06-09 06:10:47.000000 rongdavbaaddins-0.0.1.2/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-09 06:42:20.303160 rongdavbaaddins-0.0.1.2/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-09 06:42:20.000000 rongdavbaaddins-0.0.1.2/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-09 06:42:20.000000 rongdavbaaddins-0.0.1.2/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:42:20.000000 rongdavbaaddins-0.0.1.2/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 06:42:20.000000 rongdavbaaddins-0.0.1.2/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-09 06:42:20.309156 rongdavbaaddins-0.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-06-09 06:11:07.000000 rongdavbaaddins-0.0.1.2/setup.py
```

### Comparing `rongdavbaaddins-0.0.1.1/LICENSE.txt` & `rongdavbaaddins-0.0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py` & `rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.1.2/rongdaVbaAddins/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.1/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.0.1.2/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.1/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.1.2/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.1/setup.py` & `rongdavbaaddins-0.0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 1
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.2"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

