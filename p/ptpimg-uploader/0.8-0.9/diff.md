# Comparing `tmp/ptpimg_uploader-0.8.tar.gz` & `tmp/ptpimg_uploader-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptpimg_uploader-0.8.tar", last modified: Tue Jun  7 06:18:23 2022, max compression
+gzip compressed data, was "ptpimg_uploader-0.9.tar", last modified: Fri Jun  9 19:54:57 2023, max compression
```

## Comparing `ptpimg_uploader-0.8.tar` & `ptpimg_uploader-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 06:18:23.045431 ptpimg_uploader-0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-06-07 06:18:08.000000 ptpimg_uploader-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-06-07 06:18:23.045431 ptpimg_uploader-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-06-07 06:18:08.000000 ptpimg_uploader-0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 06:18:23.045431 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-06-07 06:18:22.000000 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-06-07 06:18:23.000000 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 06:18:22.000000 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-07 06:18:22.000000 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-07 06:18:22.000000 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 06:18:22.000000 ptpimg_uploader-0.8/ptpimg_uploader.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     6794 2022-06-07 06:18:08.000000 ptpimg_uploader-0.8/ptpimg_uploader.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 06:18:23.045431 ptpimg_uploader-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-06-07 06:18:08.000000 ptpimg_uploader-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:57.335986 ptpimg_uploader-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-09 19:54:47.000000 ptpimg_uploader-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-09 19:54:57.335986 ptpimg_uploader-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-09 19:54:47.000000 ptpimg_uploader-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:57.335986 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-09 19:54:57.000000 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 19:54:57.000000 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:54:57.000000 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 19:54:57.000000 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 19:54:57.000000 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 19:54:57.000000 ptpimg_uploader-0.9/ptpimg_uploader.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6820 2023-06-09 19:54:47.000000 ptpimg_uploader-0.9/ptpimg_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:54:57.335986 ptpimg_uploader-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 19:54:47.000000 ptpimg_uploader-0.9/setup.py
```

### Comparing `ptpimg_uploader-0.8/LICENSE` & `ptpimg_uploader-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ptpimg_uploader-0.8/PKG-INFO` & `ptpimg_uploader-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ptpimg_uploader
-Version: 0.8
+Version: 0.9
 Summary: PTPImg uploader, handles local files and URLs, from the commandline
 Home-page: https://github.com/theirix/ptpimg-uploader
 Author: theirix
 Author-email: theirix@gmail.com
 License: BSD
 Keywords: image uploader
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Requires-Python: >=3.3
 License-File: LICENSE
 
 ===============
 ptpimg_uploader
@@ -128,9 +127,7 @@
 * mjpieters - a great refactoring and Python packaging
 * lukacoufyl - fixing image upload order
 
 .. |Build Status| image:: https://github.com/theirix/ptpimg-uploader/workflows/Upload%20Python%20Package/badge.svg
    :target: https://github.com/theirix/ptpimg-uploader/actions
 .. |PyPI version| image:: https://img.shields.io/pypi/v/ptpimg-uploader.svg
    :target: https://pypi.python.org/pypi/ptpimg-uploader
-
-
```

### Comparing `ptpimg_uploader-0.8/README.rst` & `ptpimg_uploader-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ptpimg_uploader-0.8/ptpimg_uploader.egg-info/PKG-INFO` & `ptpimg_uploader-0.9/ptpimg_uploader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ptpimg-uploader
-Version: 0.8
+Version: 0.9
 Summary: PTPImg uploader, handles local files and URLs, from the commandline
 Home-page: https://github.com/theirix/ptpimg-uploader
 Author: theirix
 Author-email: theirix@gmail.com
 License: BSD
 Keywords: image uploader
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Requires-Python: >=3.3
 License-File: LICENSE
 
 ===============
 ptpimg_uploader
@@ -128,9 +127,7 @@
 * mjpieters - a great refactoring and Python packaging
 * lukacoufyl - fixing image upload order
 
 .. |Build Status| image:: https://github.com/theirix/ptpimg-uploader/workflows/Upload%20Python%20Package/badge.svg
    :target: https://github.com/theirix/ptpimg-uploader/actions
 .. |PyPI version| image:: https://img.shields.io/pypi/v/ptpimg-uploader.svg
    :target: https://pypi.python.org/pypi/ptpimg-uploader
-
-
```

### Comparing `ptpimg_uploader-0.8/ptpimg_uploader.py` & `ptpimg_uploader-0.9/ptpimg_uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         help='Output links in BBCode format (with [img] tags)')
     parser.add_argument(
         '--nobell', action='store_true', default=False,
         help='Do not bell in a terminal on completion')
 
     args = parser.parse_args()
     images = args.images
-    if args.clip:
+    if pyperclip is not None and args.clip:
         images.append(pyperclip.paste())
 
     if not args.api_key:
         parser.error('Please specify an API key')
     try:
         image_urls = upload(args.api_key, images)
         if args.bbcode:
```

### Comparing `ptpimg_uploader-0.8/setup.py` & `ptpimg_uploader-0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.rst') as desc:
     long_description = desc.read()
 
 setup(
     name="ptpimg_uploader",
-    version="0.8",
+    version="0.9",
     author="theirix",
     author_email="theirix@gmail.com",
     description=(
         "PTPImg uploader, handles local files and URLs, from the commandline"),
     long_description=long_description,
     license="BSD",
     keywords="image uploader",
```

