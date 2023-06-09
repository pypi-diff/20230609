# Comparing `tmp/BingImageCreator-0.4.1.tar.gz` & `tmp/BingImageCreator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.4.1.tar", last modified: Fri Jun  2 16:45:55 2023, max compression
+gzip compressed data, was "BingImageCreator-0.4.2.tar", last modified: Fri Jun  9 09:46:30 2023, max compression
```

## Comparing `BingImageCreator-0.4.1.tar` & `BingImageCreator-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:46:30.273857 BingImageCreator-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-09 09:46:09.000000 BingImageCreator-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 09:46:30.273857 BingImageCreator-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-09 09:46:09.000000 BingImageCreator-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 09:46:30.273857 BingImageCreator-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 09:46:09.000000 BingImageCreator-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:46:30.273857 BingImageCreator-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:46:30.273857 BingImageCreator-0.4.2/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 09:46:30.000000 BingImageCreator-0.4.2/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 09:46:30.000000 BingImageCreator-0.4.2/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:46:30.000000 BingImageCreator-0.4.2/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 09:46:30.000000 BingImageCreator-0.4.2/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 09:46:30.000000 BingImageCreator-0.4.2/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 09:46:09.000000 BingImageCreator-0.4.2/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:46:30.273857 BingImageCreator-0.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 09:46:09.000000 BingImageCreator-0.4.2/test/test_example.py
```

### Comparing `BingImageCreator-0.4.1/LICENSE` & `BingImageCreator-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.4.1/PKG-INFO` & `BingImageCreator-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.4.1
+Version: 0.4.2
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.4.1/README.md` & `BingImageCreator-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.4.1/setup.py` & `BingImageCreator-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.4.1",
+    version="0.4.2",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.4.1/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.4.2/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.4.1
+Version: 0.4.2
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.4.1/src/BingImageCreator.py` & `BingImageCreator-0.4.2/src/BingImageCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,20 @@
     with open(f"{debug_file}", "a", encoding="utf-8") as f:
         f.write(str(text_var))
 
 
 class ImageGen:
     """
     Image generation by Microsoft Bing
-    Parameters:3
+    Parameters:
         auth_cookie: str
+    Optional Parameters:
+        debug_file: str
+        quiet: bool
+        all_cookies: List[Dict]
     """
 
     def __init__(
         self,
         auth_cookie: str,
         debug_file: Union[str, None] = None,
         quiet: bool = False,
@@ -180,14 +184,18 @@
         if not normal_image_links:
             raise Exception(error_no_images)
         return normal_image_links
 
     def save_images(self, links: list, output_dir: str, file_name: str = None) -> None:
         """
         Saves images to output directory
+        Parameters:
+            links: list[str]
+            output_dir: str
+            file_name: str
         """
         if self.debug_file:
             self.debug(download_message)
         if not self.quiet:
             print(download_message)
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
@@ -214,14 +222,19 @@
             ) from url_exception
 
 
 class ImageGenAsync:
     """
     Image generation by Microsoft Bing
     Parameters:
+        auth_cookie: str
+    Optional Parameters:
+        debug_file: str
+        quiet: bool
+        all_cookies: list[dict]
     """
 
     def __init__(
         self,
         auth_cookie: str = None,
         debug_file: Union[str, None] = None,
         quiet: bool = False,
```

### Comparing `BingImageCreator-0.4.1/test/test_example.py` & `BingImageCreator-0.4.2/test/test_example.py`

 * *Files identical despite different names*

