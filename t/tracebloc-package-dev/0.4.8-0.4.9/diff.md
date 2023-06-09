# Comparing `tmp/tracebloc_package-dev-0.4.8.tar.gz` & `tmp/tracebloc_package-dev-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.8.tar", last modified: Fri Jun  9 11:22:34 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.9.tar", last modified: Fri Jun  9 11:52:41 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.8.tar` & `tracebloc_package-dev-0.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:22:34.484254 tracebloc_package-dev-0.4.8/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.8/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-09 11:22:34.484340 tracebloc_package-dev-0.4.8/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.8/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-09 11:22:34.484679 tracebloc_package-dev-0.4.8/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-09 11:21:16.000000 tracebloc_package-dev-0.4.8/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:22:34.482883 tracebloc_package-dev-0.4.8/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.8/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.8/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    21521 2023-06-09 09:24:35.000000 tracebloc_package-dev-0.4.8/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    61149 2023-06-09 09:24:35.000000 tracebloc_package-dev-0.4.8/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.8/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    10245 2023-06-09 11:15:51.000000 tracebloc_package-dev-0.4.8/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-09 09:24:35.000000 tracebloc_package-dev-0.4.8/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.8/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 09:24:35.000000 tracebloc_package-dev-0.4.8/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:22:34.484077 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-09 11:22:34.000000 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-09 11:22:34.000000 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-09 11:22:34.000000 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-09 11:22:34.000000 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-09 11:22:34.000000 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-09 11:22:34.000000 tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:52:41.851592 tracebloc_package-dev-0.4.9/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.9/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-09 11:52:41.851713 tracebloc_package-dev-0.4.9/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.9/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-09 11:52:41.856260 tracebloc_package-dev-0.4.9/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-09 11:51:30.000000 tracebloc_package-dev-0.4.9/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:52:41.850265 tracebloc_package-dev-0.4.9/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.9/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.9/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    21521 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    61149 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10234 2023-06-09 11:45:18.000000 tracebloc_package-dev-0.4.9/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.9/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:52:41.851398 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.8/LICENSE.txt` & `tracebloc_package-dev-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/PKG-INFO` & `tracebloc_package-dev-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.4.8
+Version: 0.4.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.8/setup.py` & `tracebloc_package-dev-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.8",
+    version="0.4.9",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,8 +272,8 @@
                 f"Weights upload failed with error {e}",
                 "red",
             )
             print(text, "\n")
             print(
                 "For more information check the docs 'https://docs.tracebloc.io/weights'"
             )
-            return False, []
+            raise
```

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.9/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.4.8
+Version: 0.4.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.8/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

