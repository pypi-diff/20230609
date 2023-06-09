# Comparing `tmp/pyNekobin-2.2.tar.gz` & `tmp/pyNekobin-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNekobin-2.2.tar", last modified: Fri Jun  9 06:36:19 2023, max compression
+gzip compressed data, was "pyNekobin-2.3.tar", last modified: Fri Jun  9 06:39:52 2023, max compression
```

## Comparing `pyNekobin-2.2.tar` & `pyNekobin-2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:36:19.766717 pyNekobin-2.2/
--rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.2/LICENSE
--rw-rw-rw-   0        0        0     3655 2023-06-09 06:36:19.764716 pyNekobin-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2769 2023-06-09 06:27:06.000000 pyNekobin-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:36:19.745712 pyNekobin-2.2/nekobin/
--rw-rw-rw-   0        0        0       50 2023-06-09 06:28:34.000000 pyNekobin-2.2/nekobin/__init__.py
--rw-rw-rw-   0        0        0     4339 2023-06-09 06:25:11.000000 pyNekobin-2.2/nekobin/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:36:19.763733 pyNekobin-2.2/pyNekobin.egg-info/
--rw-rw-rw-   0        0        0     3655 2023-06-09 06:36:19.000000 pyNekobin-2.2/pyNekobin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-09 06:36:19.000000 pyNekobin-2.2/pyNekobin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:36:19.000000 pyNekobin-2.2/pyNekobin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 06:36:19.000000 pyNekobin-2.2/pyNekobin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 06:36:19.000000 pyNekobin-2.2/pyNekobin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 06:36:19.766717 pyNekobin-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-06-09 05:23:14.000000 pyNekobin-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:39:52.805411 pyNekobin-2.3/
+-rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.3/LICENSE
+-rw-rw-rw-   0        0        0     3707 2023-06-09 06:39:52.794408 pyNekobin-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2821 2023-06-09 06:38:17.000000 pyNekobin-2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:39:52.774387 pyNekobin-2.3/nekobin/
+-rw-rw-rw-   0        0        0       50 2023-06-09 06:39:13.000000 pyNekobin-2.3/nekobin/__init__.py
+-rw-rw-rw-   0        0        0     4339 2023-06-09 06:25:11.000000 pyNekobin-2.3/nekobin/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:39:52.792408 pyNekobin-2.3/pyNekobin.egg-info/
+-rw-rw-rw-   0        0        0     3707 2023-06-09 06:39:52.000000 pyNekobin-2.3/pyNekobin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-09 06:39:52.000000 pyNekobin-2.3/pyNekobin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:39:52.000000 pyNekobin-2.3/pyNekobin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 06:39:52.000000 pyNekobin-2.3/pyNekobin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 06:39:52.000000 pyNekobin-2.3/pyNekobin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:39:52.805411 pyNekobin-2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-06-09 05:23:14.000000 pyNekobin-2.3/setup.py
```

### Comparing `pyNekobin-2.2/LICENSE` & `pyNekobin-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.2/PKG-INFO` & `pyNekobin-2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.2
+Version: 2.3
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.2
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.3
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -25,18 +25,18 @@
 
 # pyNekobin - A Wrapper for Nekobin API
 
 This is a Python package that provides a simple wrapper around the [Nekobin](https://nekobin.com/) API, allowing you to easily paste and retrieve text snippets from the popular pastebin service.
 
 ## Installation
 
-You can install the package using pip:
+You can install the package from [pypy](https://pypi.org/project/pyNekobin/) using pip:
 
 ```
-pip install pynekobin
+pip install -U pynekobin
 ```
 
 ## Usage
 
 This package is asynchronous and uses httpx under the hood to make HTTP requests. So, you need to use the `await` keyword with each method call.
 First, import the `Nekobin` class and the `asyncio` library:
```

### Comparing `pyNekobin-2.2/README.md` & `pyNekobin-2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 # pyNekobin - A Wrapper for Nekobin API
 
 This is a Python package that provides a simple wrapper around the [Nekobin](https://nekobin.com/) API, allowing you to easily paste and retrieve text snippets from the popular pastebin service.
 
 ## Installation
 
-You can install the package using pip:
+You can install the package from [pypy](https://pypi.org/project/pyNekobin/) using pip:
 
 ```
-pip install pynekobin
+pip install -U pynekobin
 ```
 
 ## Usage
 
 This package is asynchronous and uses httpx under the hood to make HTTP requests. So, you need to use the `await` keyword with each method call.
 First, import the `Nekobin` class and the `asyncio` library:
```

### Comparing `pyNekobin-2.2/nekobin/main.py` & `pyNekobin-2.3/nekobin/main.py`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.2/pyNekobin.egg-info/PKG-INFO` & `pyNekobin-2.3/pyNekobin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.2
+Version: 2.3
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.2
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.3
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -25,18 +25,18 @@
 
 # pyNekobin - A Wrapper for Nekobin API
 
 This is a Python package that provides a simple wrapper around the [Nekobin](https://nekobin.com/) API, allowing you to easily paste and retrieve text snippets from the popular pastebin service.
 
 ## Installation
 
-You can install the package using pip:
+You can install the package from [pypy](https://pypi.org/project/pyNekobin/) using pip:
 
 ```
-pip install pynekobin
+pip install -U pynekobin
 ```
 
 ## Usage
 
 This package is asynchronous and uses httpx under the hood to make HTTP requests. So, you need to use the `await` keyword with each method call.
 First, import the `Nekobin` class and the `asyncio` library:
```

### Comparing `pyNekobin-2.2/setup.py` & `pyNekobin-2.3/setup.py`

 * *Files identical despite different names*

