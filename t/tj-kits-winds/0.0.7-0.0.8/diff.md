# Comparing `tmp/tj_kits_winds-0.0.7.tar.gz` & `tmp/tj_kits_winds-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tj_kits_winds-0.0.7.tar", last modified: Fri Jun  9 05:24:08 2023, max compression
+gzip compressed data, was "tj_kits_winds-0.0.8.tar", last modified: Fri Jun  9 05:40:13 2023, max compression
```

## Comparing `tj_kits_winds-0.0.7.tar` & `tj_kits_winds-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      247 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/PKG-INFO
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)     1364 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.7/README.md
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)       38 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/setup.cfg
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      505 2023-06-09 05:24:02.000000 tj_kits_winds-0.0.7/setup.py
-drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/tests/
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.7/tests/__init__.py
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      986 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.7/tests/test_logger.py
-drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/tj_kits_wind/
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.7/tj_kits_wind/__init__.py
-drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/tj_kits_wind/tj_logger/
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)     4242 2023-06-09 02:29:49.000000 tj_kits_winds-0.0.7/tj_kits_wind/tj_logger/LoggerFactory.py
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      432 2023-06-09 02:30:51.000000 tj_kits_winds-0.0.7/tj_kits_wind/tj_logger/__init__.py
-drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/tj_kits_wind/tj_path/
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      432 2023-06-09 02:30:58.000000 tj_kits_winds-0.0.7/tj_kits_wind/tj_path/__init__.py
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      945 2023-06-09 02:33:49.000000 tj_kits_winds-0.0.7/tj_kits_wind/tj_path/project_root.py
-drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:24:08.117415 tj_kits_winds-0.0.7/tj_kits_winds.egg-info/
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      247 2023-06-09 05:24:08.000000 tj_kits_winds-0.0.7/tj_kits_winds.egg-info/PKG-INFO
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      375 2023-06-09 05:24:08.000000 tj_kits_winds-0.0.7/tj_kits_winds.egg-info/SOURCES.txt
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)        1 2023-06-09 05:24:08.000000 tj_kits_winds-0.0.7/tj_kits_winds.egg-info/dependency_links.txt
--rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)       19 2023-06-09 05:24:08.000000 tj_kits_winds-0.0.7/tj_kits_winds.egg-info/top_level.txt
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      265 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/PKG-INFO
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)     1364 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.8/README.md
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)       38 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/setup.cfg
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      612 2023-06-09 05:40:08.000000 tj_kits_winds-0.0.8/setup.py
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/tests/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.8/tests/__init__.py
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      986 2023-06-09 02:13:45.000000 tj_kits_winds-0.0.8/tests/test_logger.py
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/tj_kits_wind/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      501 2023-06-09 05:39:05.000000 tj_kits_winds-0.0.8/tj_kits_wind/__init__.py
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/tj_kits_wind/tj_logger/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)     4448 2023-06-09 05:34:33.000000 tj_kits_winds-0.0.8/tj_kits_wind/tj_logger/LoggerFactory.py
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      462 2023-06-09 05:34:56.000000 tj_kits_winds-0.0.8/tj_kits_wind/tj_logger/__init__.py
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/tj_kits_wind/tj_path/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      461 2023-06-09 05:35:52.000000 tj_kits_winds-0.0.8/tj_kits_wind/tj_path/__init__.py
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)     1004 2023-06-09 05:35:40.000000 tj_kits_winds-0.0.8/tj_kits_wind/tj_path/project_root.py
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/tj_kits_wind/tj_time/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      450 2023-06-09 05:38:23.000000 tj_kits_winds-0.0.8/tj_kits_wind/tj_time/__init__.py
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      164 2023-06-09 05:38:01.000000 tj_kits_winds-0.0.8/tj_kits_wind/tj_time/tt.py
+drwxr-xr-x   0 tjno-1    (1000) tjno-1    (1000)        0 2023-06-09 05:40:13.116364 tj_kits_winds-0.0.8/tj_kits_winds.egg-info/
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      265 2023-06-09 05:40:13.000000 tj_kits_winds-0.0.8/tj_kits_winds.egg-info/PKG-INFO
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)      471 2023-06-09 05:40:13.000000 tj_kits_winds-0.0.8/tj_kits_winds.egg-info/SOURCES.txt
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)        1 2023-06-09 05:40:13.000000 tj_kits_winds-0.0.8/tj_kits_winds.egg-info/dependency_links.txt
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)       17 2023-06-09 05:40:13.000000 tj_kits_winds-0.0.8/tj_kits_winds.egg-info/requires.txt
+-rw-r--r--   0 tjno-1    (1000) tjno-1    (1000)       19 2023-06-09 05:40:13.000000 tj_kits_winds-0.0.8/tj_kits_winds.egg-info/top_level.txt
```

### Comparing `tj_kits_winds-0.0.7/README.md` & `tj_kits_winds-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tj_kits_winds-0.0.7/tests/test_logger.py` & `tj_kits_winds-0.0.8/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `tj_kits_winds-0.0.7/tj_kits_wind/tj_logger/LoggerFactory.py` & `tj_kits_winds-0.0.8/tj_kits_wind/tj_logger/LoggerFactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 import logging.config
 import os
 import sys
 from typing import AnyStr, Dict, Optional, Literal, Union
 
+__all__ = ['FORMAT_VERY_SHORT', 'FORMAT_SHORT', 'FORMAT_NORMAL', 'FORMAT_WORDY',
+           'LOG_DEBUG', 'LOG_INFO', 'LOG_WARNING', 'LOG_ERROR', 'LOG_CRITICAL',
+           'logger_console', 'logger_auto']
+
 FORMAT_VERY_SHORT = "very_short"
 FORMAT_SHORT = "short"
 FORMAT_NORMAL = "normal"
 FORMAT_WORDY = "wordy"
 LOGGER_FORMAT = Union[FORMAT_VERY_SHORT, FORMAT_SHORT, FORMAT_NORMAL, FORMAT_WORDY]
 
 LOG_DEBUG = "DEBUG"
```

### Comparing `tj_kits_winds-0.0.7/tj_kits_wind/tj_path/project_root.py` & `tj_kits_winds-0.0.8/tj_kits_wind/tj_path/project_root.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+import inspect
+import os
+
+__all__ = ['get_project_root']
+
+
 def get_project_root(project_name: str | None = None, defalut_path: str | None = "/tmp/JustDemo") -> str:
     if not project_name:
         return defalut_path
 
     try:
         frame = inspect.currentframe().f_back
         str_frame = str(frame)
```

