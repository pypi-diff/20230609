# Comparing `tmp/SecuriPy-1.1.2.tar.gz` & `tmp/SecuriPy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.1.2.tar", last modified: Fri Jun  9 07:21:50 2023, max compression
+gzip compressed data, was "SecuriPy-1.1.4.tar", last modified: Fri Jun  9 07:23:30 2023, max compression
```

## Comparing `SecuriPy-1.1.2.tar` & `SecuriPy-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:21:50.858379 SecuriPy-1.1.2/
--rw-rw-rw-   0        0        0     3617 2023-06-09 07:21:50.857378 SecuriPy-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 07:21:50.855388 SecuriPy-1.1.2/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3617 2023-06-09 07:21:50.000000 SecuriPy-1.1.2/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-06-09 07:21:50.000000 SecuriPy-1.1.2/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 07:21:50.000000 SecuriPy-1.1.2/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 07:21:50.000000 SecuriPy-1.1.2/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6857 2023-06-03 17:21:28.000000 SecuriPy-1.1.2/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 07:21:50.859390 SecuriPy-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-06-09 07:21:43.000000 SecuriPy-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:23:30.550588 SecuriPy-1.1.4/
+-rw-rw-rw-   0        0        0     3617 2023-06-09 07:23:30.538928 SecuriPy-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 07:23:30.535931 SecuriPy-1.1.4/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3617 2023-06-09 07:23:30.000000 SecuriPy-1.1.4/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-06-09 07:23:30.000000 SecuriPy-1.1.4/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:23:30.000000 SecuriPy-1.1.4/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 07:23:30.000000 SecuriPy-1.1.4/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6857 2023-06-03 17:21:28.000000 SecuriPy-1.1.4/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:23:30.550588 SecuriPy-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-06-09 07:23:06.000000 SecuriPy-1.1.4/setup.py
```

### Comparing `SecuriPy-1.1.2/PKG-INFO` & `SecuriPy-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.1.2
+Version: 1.1.4
 Summary: Encrypter and Decrypter of all types of human-readable file formats Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.1.2/README.md` & `SecuriPy-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.1.2/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.1.4/SecuriPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.1.2
+Version: 1.1.4
 Summary: Encrypter and Decrypter of all types of human-readable file formats Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.1.2/SecuriPy.py` & `SecuriPy-1.1.4/SecuriPy.py`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.1.2/setup.py` & `SecuriPy-1.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.1.2",
+    version="1.1.4",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of all types of human-readable file formats Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

