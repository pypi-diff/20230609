# Comparing `tmp/fosslight_android-4.1.13.tar.gz` & `tmp/fosslight_android-4.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_android-4.1.13.tar", last modified: Mon Feb 27 01:15:28 2023, max compression
+gzip compressed data, was "fosslight_android-4.1.14.tar", last modified: Fri Jun  9 04:37:40 2023, max compression
```

## Comparing `fosslight_android-4.1.13.tar` & `fosslight_android-4.1.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-27 01:15:28.900860 fosslight_android-4.1.13/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      183 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1856 2023-02-27 01:15:28.896860 fosslight_android-4.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1009 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      201 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-27 01:15:28.900860 fosslight_android-4.1.13/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     1493 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-27 01:15:28.896860 fosslight_android-4.1.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-27 01:15:28.896860 fosslight_android-4.1.13/src/fosslight_android/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6398 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/_binary_db_controller.py
--rw-r--r--   0 runner    (1001) docker     (116)     6477 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/_common.py
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/_help.py
--rw-r--r--   0 runner    (1001) docker     (116)     3264 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/_src_analysis.py
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     2385 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/_write_excel.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    33528 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/android_binary_analysis.py
--rw-r--r--   0 runner    (1001) docker     (116)    12153 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/check_notice_file.py
--rw-r--r--   0 runner    (1001) docker     (116)     5177 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/check_package_file.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-27 01:15:28.896860 fosslight_android-4.1.13/src/fosslight_android/resources/
--rw-r--r--   0 runner    (1001) docker     (116)   146753 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/resources/aosp_repository.json
--rw-r--r--   0 runner    (1001) docker     (116)      953 2023-02-27 01:15:21.000000 fosslight_android-4.1.13/src/fosslight_android/resources/module_license.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-27 01:15:28.896860 fosslight_android-4.1.13/src/fosslight_android.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1856 2023-02-27 01:15:28.000000 fosslight_android-4.1.13/src/fosslight_android.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      821 2023-02-27 01:15:28.000000 fosslight_android-4.1.13/src/fosslight_android.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-27 01:15:28.000000 fosslight_android-4.1.13/src/fosslight_android.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       86 2023-02-27 01:15:28.000000 fosslight_android-4.1.13/src/fosslight_android.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      201 2023-02-27 01:15:28.000000 fosslight_android-4.1.13/src/fosslight_android.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2023-02-27 01:15:28.000000 fosslight_android-4.1.13/src/fosslight_android.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/src/fosslight_android/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/_binary_db_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/_src_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/_write_excel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33528 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/android_binary_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/check_notice_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/check_package_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/src/fosslight_android/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   146753 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/resources/aosp_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 04:37:26.000000 fosslight_android-4.1.14/src/fosslight_android/resources/module_license.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:37:40.003108 fosslight_android-4.1.14/src/fosslight_android.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 04:37:39.000000 fosslight_android-4.1.14/src/fosslight_android.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-09 04:37:39.000000 fosslight_android-4.1.14/src/fosslight_android.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:37:39.000000 fosslight_android-4.1.14/src/fosslight_android.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 04:37:39.000000 fosslight_android-4.1.14/src/fosslight_android.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-09 04:37:39.000000 fosslight_android-4.1.14/src/fosslight_android.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 04:37:39.000000 fosslight_android-4.1.14/src/fosslight_android.egg-info/top_level.txt
```

### Comparing `fosslight_android-4.1.13/LICENSE` & `fosslight_android-4.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/PKG-INFO` & `fosslight_android-4.1.14/src/fosslight_android.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fosslight_android
-Version: 4.1.13
+Name: fosslight-android
+Version: 4.1.14
 Summary: FOSSLight Android Scanner
 Home-page: https://github.com/fosslight/fosslight_android_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_android_scanner
 Description: <!--
         # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

### Comparing `fosslight_android-4.1.13/README.md` & `fosslight_android-4.1.14/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/setup.py` & `fosslight_android-4.1.14/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 
 if __name__ == "__main__":
     setup(
         name='fosslight_android',
-        version='4.1.13',
+        version='4.1.14',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Android Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_android-4.1.13/src/fosslight_android/_binary_db_controller.py` & `fosslight_android-4.1.14/src/fosslight_android/_binary_db_controller.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/_common.py` & `fosslight_android-4.1.14/src/fosslight_android/_common.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/_help.py` & `fosslight_android-4.1.14/src/fosslight_android/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/_src_analysis.py` & `fosslight_android-4.1.14/src/fosslight_android/_src_analysis.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/_util.py` & `fosslight_android-4.1.14/src/fosslight_android/_util.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/_write_excel.py` & `fosslight_android-4.1.14/src/fosslight_android/_write_excel.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/android_binary_analysis.py` & `fosslight_android-4.1.14/src/fosslight_android/android_binary_analysis.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/check_notice_file.py` & `fosslight_android-4.1.14/src/fosslight_android/check_notice_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import logging
 import os
 from bs4 import BeautifulSoup
 from ._util import read_file, write_txt_file
 from ._common import NOTICE_FILE_NAME
 from fosslight_util.constant import LOGGER_NAME
 import re
+import gzip
+import shutil
 
 logger = logging.getLogger(LOGGER_NAME)
 CANNOT_FIND_MSG = "CANNOT_FIND_NOTICE_HTML"
 
 
 def run_notice_html_checklist(binary_file, check_type, notice_file):
     notice_file_list = {}  # File list in NOTICE.html
@@ -69,19 +71,32 @@
                     break
 
     return notice_found
 
 
 def find_files_by_extension(path):
     extensions = ['.html', '.xml']
+    GZ_EXTENSION = '.gz'
     files = []
+    try:
+        gz_files = [os.path.join(path, f) for f in os.listdir(path) if f.endswith(GZ_EXTENSION)]
+        for gz_file in gz_files:
+            unzip_file = gz_file.replace('.gz', '')
+            if not os.path.isfile(unzip_file):
+                with gzip.open(gz_file, 'rb') as f_in:
+                    with open(unzip_file, 'wb') as f_out:
+                        shutil.copyfileobj(f_in, f_out)
+    except Exception as error:
+        logger.info(f"Fail unzip gz file:{error}")
+
     for extension in extensions:
         files = [os.path.join(path, f) for f in os.listdir(path) if f.endswith(extension)]
         if len(files) > 0:
             break
+
     return files
 
 
 def read_notice_file(notice_file_path, notice_html_file):
     final_notice_file = {}
     # NOTICE.html need to be skipped the errors related to decode
     encodings = ["latin-1", "utf-8", "utf-16"]
```

### Comparing `fosslight_android-4.1.13/src/fosslight_android/check_package_file.py` & `fosslight_android-4.1.14/src/fosslight_android/check_package_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/resources/aosp_repository.json` & `fosslight_android-4.1.14/src/fosslight_android/resources/aosp_repository.json`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android/resources/module_license.json` & `fosslight_android-4.1.14/src/fosslight_android/resources/module_license.json`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.13/src/fosslight_android.egg-info/PKG-INFO` & `fosslight_android-4.1.14/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fosslight-android
-Version: 4.1.13
+Name: fosslight_android
+Version: 4.1.14
 Summary: FOSSLight Android Scanner
 Home-page: https://github.com/fosslight/fosslight_android_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_android_scanner
 Description: <!--
         # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

### Comparing `fosslight_android-4.1.13/src/fosslight_android.egg-info/SOURCES.txt` & `fosslight_android-4.1.14/src/fosslight_android.egg-info/SOURCES.txt`

 * *Files identical despite different names*

