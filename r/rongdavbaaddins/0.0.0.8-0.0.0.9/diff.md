# Comparing `tmp/rongdavbaaddins-0.0.0.8.tar.gz` & `tmp/rongdavbaaddins-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.0.8.tar", last modified: Thu Jun  8 02:52:59 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.0.9.tar", last modified: Thu Jun  8 09:58:32 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.0.8.tar` & `rongdavbaaddins-0.0.0.9.tar`

### file list

```diff
@@ -1,63 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.375619 rongdavbaaddins-0.0.0.8/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-06-08 02:52:59.376606 rongdavbaaddins-0.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.190605 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.205613 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0   107702 2023-06-07 08:07:55.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.213601 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0      999 2023-06-07 09:28:00.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      372 2023-06-08 01:57:56.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/minusFunction.pyd
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.263605 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/
--rw-rw-rw-   0        0        0    90160 2023-06-08 02:07:36.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/__init__.py
--rw-rw-rw-   0        0        0    30117 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_common.py
--rw-rw-rw-   0        0        0    15475 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_compat.py
--rw-rw-rw-   0        0        0    19253 2023-06-08 02:39:18.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psaix.py
--rw-rw-rw-   0        0        0    32729 2023-06-08 02:40:14.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psbsd.py
--rw-rw-rw-   0        0        0    89211 2023-06-08 02:49:21.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pslinux.py
--rw-rw-rw-   0        0        0    16851 2023-06-08 02:40:14.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psosx.py
--rw-rw-rw-   0        0        0     8477 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psposix.py
--rw-rw-rw-   0        0        0    26246 2023-06-08 02:40:14.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pssunos.py
--rw-rw-rw-   0        0        0    78336 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psutil_windows.pyd
--rw-rw-rw-   0        0        0    38545 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pswindows.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.353603 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/
--rw-rw-rw-   0        0        0    61064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/__init__.py
--rw-rw-rw-   0        0        0      308 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/__main__.py
--rw-rw-rw-   0        0        0    11554 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/runner.py
--rw-rw-rw-   0        0        0     4630 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_aix.py
--rw-rw-rw-   0        0        0    21638 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_bsd.py
--rw-rw-rw-   0        0        0    21458 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_connections.py
--rw-rw-rw-   0        0        0    28501 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_contracts.py
--rw-rw-rw-   0        0        0    97598 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_linux.py
--rw-rw-rw-   0        0        0    15520 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_memleaks.py
--rw-rw-rw-   0        0        0    35604 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_misc.py
--rw-rw-rw-   0        0        0     6791 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_osx.py
--rw-rw-rw-   0        0        0    17487 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_posix.py
--rw-rw-rw-   0        0        0    64702 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_process.py
--rw-rw-rw-   0        0        0     1379 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_sunos.py
--rw-rw-rw-   0        0        0    36812 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_system.py
--rw-rw-rw-   0        0        0    15064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_testutils.py
--rw-rw-rw-   0        0        0    12576 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_unicode.py
--rw-rw-rw-   0        0        0    36065 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_windows.py
--rw-rw-rw-   0        0        0   125952 2023-06-08 02:52:28.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/rongdaVbaAddins.pyd
--rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-06-07 09:28:00.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    27804 2023-06-07 02:50:03.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.371604 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1950 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-08 02:52:59.378607 rongdavbaaddins-0.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-06-08 02:52:44.000000 rongdavbaaddins-0.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.436972 rongdavbaaddins-0.0.0.9/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      409 2023-06-08 09:58:32.437970 rongdavbaaddins-0.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.409973 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.416937 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   107844 2023-06-08 09:52:04.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.423936 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      384 2023-06-08 09:57:48.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   140800 2023-06-08 09:56:35.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/rongdaVbaAddins.pyd
+-rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27804 2023-06-08 09:52:05.000000 rongdavbaaddins-0.0.0.9/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-08 09:58:32.433936 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 09:58:32.000000 rongdavbaaddins-0.0.0.9/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-08 09:58:32.438977 rongdavbaaddins-0.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-06-08 09:58:30.000000 rongdavbaaddins-0.0.0.9/setup.py
```

### Comparing `rongdavbaaddins-0.0.0.8/LICENSE.txt` & `rongdavbaaddins-0.0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py` & `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/Vbalogpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import traceback
 
 try:
     from Vbalog import FunctionLog
     from minusFunction import minusFunction
-except
+except:
     try:
         from .Vbalog import FunctionLog
         from .minusFunction import minusFunction
     except:
         traceback.print_exc()
 import sys, datetime
 if __name__ == "__main__":
```

### Comparing `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.0.0.9/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.8/setup.py` & `rongdavbaaddins-0.0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.8"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.9"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

