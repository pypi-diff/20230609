# Comparing `tmp/dknovautils-0.1.6.tar.gz` & `tmp/dknovautils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.1.6.tar", last modified: Fri May 19 02:09:17 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dknovautils-0.1.6.tar` & `dknovautils-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-19 02:09:17.000000 dknovautils-0.1.6/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-19 02:09:17.000000 dknovautils-0.1.6/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2523 2023-05-12 05:07:32.000000 dknovautils-0.1.6/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8676 2023-05-19 02:09:12.000000 dknovautils-0.1.6/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.6/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1153 2023-05-07 16:31:40.000000 dknovautils-0.1.6/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-19 02:09:12.000000 dknovautils-0.1.6/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      501 2023-05-07 13:41:47.000000 dknovautils-0.1.6/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.6/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.6/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.6/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-19 02:09:17.000000 dknovautils-0.1.6/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.6/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-19 02:09:17.000000 dknovautils-0.1.6/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.6/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-19 02:09:17.000000 dknovautils-0.1.6/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1159 2023-05-19 02:09:12.000000 dknovautils-0.1.6/setup.py
+-rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 dknovautils-0.1.7/.gitignore
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 dknovautils-0.1.7/LICENSE
+-rwxr-xr-x   0        0        0      476 2020-02-02 00:00:00.000000 dknovautils-0.1.7/README.md
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 dknovautils-0.1.7/pyproject.toml
+-rwxr-xr-x   0        0        0     1159 2020-02-02 00:00:00.000000 dknovautils-0.1.7/setup.py
+-rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 dknovautils-0.1.7/test_a.py
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 dknovautils-0.1.7/test_b01.py
+-rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 dknovautils-0.1.7/test_c.py
+-rwxr-xr-x   0        0        0     1181 2020-02-02 00:00:00.000000 dknovautils-0.1.7/upload.sh
+-rwxr-xr-x   0        0        0      880 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/PKG-INFO
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/SOURCES.txt
+-rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/dependency_links.txt
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/requires.txt
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/__init__.py
+-rwxr-xr-x   0        0        0     2523 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/commons.py
+-rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dk_imports.py
+-rwxr-xr-x   0        0        0     8679 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dkat.py
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dkfiles.py
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dkipy.py
+-rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/example.py
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/myadd.py
+-rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/mysubtract.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dknovautils-0.1.7/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dknovautils-0.1.6/dknovautils/commons.py` & `dknovautils-0.1.7/src/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.6/dknovautils/dkat.py` & `dknovautils-0.1.7/src/dknovautils/dkat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from typing import Any
 import dknovautils
 from dknovautils.commons import *
 
 
-DkAppVer = '0.1.6'
+DkAppVer = '0.1.7'
 
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
@@ -176,15 +176,15 @@
         return millisec
 
     _last_epochsecs = 0.0
 
     @classmethod
     def fepochSecs(cls) -> float:
         '''
-         time.monotonic()不是epoch值。fuck
+         time.monotonic()不是epoch值！！F**K
         # return time.monotonic()
 
         '''
         r = time.time()
         if r <= cls._last_epochsecs:
             return cls._last_epochsecs
         else:
```

### Comparing `dknovautils-0.1.6/dknovautils/dkipy.py` & `dknovautils-0.1.7/src/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.6/dknovautils/dk_imports.py` & `dknovautils-0.1.7/src/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.6/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.7/dknovautils.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.6/setup.py` & `dknovautils-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.1.6'
+DkAppVer = '0.1.7'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

