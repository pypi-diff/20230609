# Comparing `tmp/pyNekobin-2.4.tar.gz` & `tmp/pyNekobin-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNekobin-2.4.tar", last modified: Fri Jun  9 09:54:19 2023, max compression
+gzip compressed data, was "pyNekobin-2.5.tar", last modified: Fri Jun  9 10:42:33 2023, max compression
```

## Comparing `pyNekobin-2.4.tar` & `pyNekobin-2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:54:19.742181 pyNekobin-2.4/
--rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.4/LICENSE
--rw-rw-rw-   0        0        0     3965 2023-06-09 09:54:19.740181 pyNekobin-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3081 2023-06-09 09:53:29.000000 pyNekobin-2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:54:19.674166 pyNekobin-2.4/nekobin/
--rw-rw-rw-   0        0        0       50 2023-06-09 09:50:49.000000 pyNekobin-2.4/nekobin/__init__.py
--rw-rw-rw-   0        0        0     4356 2023-06-09 09:53:05.000000 pyNekobin-2.4/nekobin/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:54:19.738181 pyNekobin-2.4/pyNekobin.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-06-09 09:54:19.000000 pyNekobin-2.4/pyNekobin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-09 09:54:19.000000 pyNekobin-2.4/pyNekobin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:54:19.000000 pyNekobin-2.4/pyNekobin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 09:54:19.000000 pyNekobin-2.4/pyNekobin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 09:54:19.000000 pyNekobin-2.4/pyNekobin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 09:54:19.743183 pyNekobin-2.4/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-06-09 05:23:14.000000 pyNekobin-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 10:42:33.702330 pyNekobin-2.5/
+-rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.5/LICENSE
+-rw-rw-rw-   0        0        0     3965 2023-06-09 10:42:33.700325 pyNekobin-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3081 2023-06-09 10:04:54.000000 pyNekobin-2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 10:42:33.637317 pyNekobin-2.5/nekobin/
+-rw-rw-rw-   0        0        0       52 2023-06-09 10:20:25.000000 pyNekobin-2.5/nekobin/__init__.py
+-rw-rw-rw-   0        0        0     4355 2023-06-09 10:21:13.000000 pyNekobin-2.5/nekobin/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 10:42:33.698339 pyNekobin-2.5/pyNekobin.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 10:42:33.702330 pyNekobin-2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1639 2023-06-09 10:21:50.000000 pyNekobin-2.5/setup.py
```

### Comparing `pyNekobin-2.4/LICENSE` & `pyNekobin-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.4/PKG-INFO` & `pyNekobin-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.4
+Version: 2.5
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.4
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.5
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyNekobin - A Wrapper for Nekobin API
 
 This is a Python package that provides a simple wrapper around the [Nekobin](https://nekobin.com/) API, allowing you to easily paste and retrieve text snippets from the popular pastebin service.
 
-<img src="https://img.shields.io/pypi/l/pyNekobin.svg" alt="MIT LICENSE"> <img src="https://img.shields.io/pypi/pyversions/pynekobin.svg" alt="Supported Oython Versions">
+<img src="https://img.shields.io/pypi/l/pyNekobin.svg" alt="MIT LICENSE"> <img src="https://img.shields.io/pypi/pyversions/pynekobin.svg" alt="Supported Python Versions">
 <img src="https://img.shields.io/pypi/v/pynekobin.svg" alt="PyPy Version">
 <img src="https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968" alt="Code Quality">
 
 ## Installation
 
 You can install the package from [pypy](https://pypi.org/project/pyNekobin/) using pip:
```

### Comparing `pyNekobin-2.4/README.md` & `pyNekobin-2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyNekobin - A Wrapper for Nekobin API
 
 This is a Python package that provides a simple wrapper around the [Nekobin](https://nekobin.com/) API, allowing you to easily paste and retrieve text snippets from the popular pastebin service.
 
-<img src="https://img.shields.io/pypi/l/pyNekobin.svg" alt="MIT LICENSE"> <img src="https://img.shields.io/pypi/pyversions/pynekobin.svg" alt="Supported Oython Versions">
+<img src="https://img.shields.io/pypi/l/pyNekobin.svg" alt="MIT LICENSE"> <img src="https://img.shields.io/pypi/pyversions/pynekobin.svg" alt="Supported Python Versions">
 <img src="https://img.shields.io/pypi/v/pynekobin.svg" alt="PyPy Version">
 <img src="https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968" alt="Code Quality">
 
 ## Installation
 
 You can install the package from [pypy](https://pypi.org/project/pyNekobin/) using pip:
```

### Comparing `pyNekobin-2.4/nekobin/main.py` & `pyNekobin-2.5/nekobin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+# pylint:disable=C0103, C0114, C0301, R0903, W0718
+
+
 import re
 import json
 import httpx
-import asyncio
 
 
 class Objectify:
     """
     A utility class that converts a dictionary into an object.
     """
+
     def __init__(self, entries):
         """
         Initializes the Objectify instance with the given dictionary entries.
 
         Args:
             entries (dict): A dictionary containing the entries to be added as attributes to the object.
         """
@@ -20,19 +23,19 @@
         self.content: str = None
         self.message: str = None
         self.error: Exception = None
 
         self.__dict__.update(entries)
 
 
-
 class Nekobin:
     """
-    A wrapper class for the nekobin.com API.
+A wrapper class for the nekobin.com API.
     """
+
     def __init__(self, **kw):
         """
         Initializes the Nekobin instance with the given arguments.
 
         Args:
             **kw: Any keyword arguments that http.AsyncClient may take, such as headers, timeout, or proxy.
         """
@@ -73,22 +76,21 @@
                 "ok": True,
                 "url": f"https://nekobin.com/{r['result']['key']}",
                 "message": "Successfully pasted text in Nekobin"
             }
 
             return Objectify(x)
 
-        else:
-            x = {
-                "ok": False,
-                "message": "Nekobin did not fulfill the request",
-                "error": Exception("Response is not 200")
-            }
+        x = {
+            "ok": False,
+            "message": "Nekobin did not fulfill the request",
+            "error": Exception("Response is not 200")
+        }
 
-            return Objectify(x)
+        return Objectify(x)
 
     async def read(self, url: str, **kw):
         """
         Reads the text from the nekobin.com API for the given URL and returns an Objectify instance.
 
         Args:
             url (str): The URL of the nekobin.com document to read.
@@ -96,15 +98,14 @@
 
         Returns:
             Objectify: An Objectify instance representing the result of the read operation.
         """
         if not url.startswith("http"):
             url = "https://" + url
 
-
         pattern = r"^(http|https):\/\/nekobin\.com\/[a-z.]{5,20}$"
 
         if not re.match(pattern, url):
             x = {
                 "ok": False,
                 "message": "URL is not valid. Example Url: https://nekobin.com/abcdefghi",
                 "error": Exception("URL is not Valid")
@@ -136,8 +137,8 @@
         except Exception:
             x = {
                 "ok": False,
                 "message": "Nekobin did not fulfill the request",
                 "error": Exception("Document not retrieved")
             }
 
-            return Objectify(x)
+            return Objectify(x)
```

### Comparing `pyNekobin-2.4/pyNekobin.egg-info/PKG-INFO` & `pyNekobin-2.5/pyNekobin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.4
+Version: 2.5
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.4
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.5
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyNekobin - A Wrapper for Nekobin API
 
 This is a Python package that provides a simple wrapper around the [Nekobin](https://nekobin.com/) API, allowing you to easily paste and retrieve text snippets from the popular pastebin service.
 
-<img src="https://img.shields.io/pypi/l/pyNekobin.svg" alt="MIT LICENSE"> <img src="https://img.shields.io/pypi/pyversions/pynekobin.svg" alt="Supported Oython Versions">
+<img src="https://img.shields.io/pypi/l/pyNekobin.svg" alt="MIT LICENSE"> <img src="https://img.shields.io/pypi/pyversions/pynekobin.svg" alt="Supported Python Versions">
 <img src="https://img.shields.io/pypi/v/pynekobin.svg" alt="PyPy Version">
 <img src="https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968" alt="Code Quality">
 
 ## Installation
 
 You can install the package from [pypy](https://pypi.org/project/pyNekobin/) using pip:
```

### Comparing `pyNekobin-2.4/setup.py` & `pyNekobin-2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Nusab19 
+# Copyright (c) 2023 Nusab19
 
 import os
 from setuptools import setup, find_packages
 
 # Version
 from nekobin import __version__ as v
 
@@ -11,43 +11,40 @@
 
 
 if os.path.isfile("README.md"):
     with open(("README.md"), encoding="utf-8") as readme:
         big_description = readme.read()
 
 else:
-    big_description = "pyNekobin - Paste Text into Nekobin with Python"
-
-
-
+    big_description = "PyNekobin - Paste Text into Nekobin with Python"
 
 
 setup(name="pyNekobin",
       version=v,
       description="Paste codes to Nekobin.com with python",
       url="https://github.com/Nusab19/pyNekobin",
       author="Nusab Taha",
       author_email="nusabtaha33@gmail.com",
       license="MIT",
       packages=find_packages(),
       download_url=f"https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-{v}",
       keywords=["Nekobin", "pyNekobin", "Paste Code", "Paste Bin"],
       long_description=big_description,
       long_description_content_type="text/markdown",
-      
+
       package_data={"pyNekobin": ["data/*.json"]},
       include_package_data=True,
-      
+
       install_requires=["httpx>=0.23.0"],
-      python_requires = ">=3.6",
+      python_requires=">=3.6",
       classifiers=[
           "Development Status :: 5 - Production/Stable",
           "Intended Audience :: Developers",
           "Topic :: Education",
           "License :: OSI Approved :: MIT License",
           "Programming Language :: Python :: 3.6",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
       ],
-)
+      )
```

