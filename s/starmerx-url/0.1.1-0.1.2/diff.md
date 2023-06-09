# Comparing `tmp/starmerx_url-0.1.1.tar.gz` & `tmp/starmerx_url-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmerx_url-0.1.1.tar", last modified: Thu Nov 10 06:39:38 2022, max compression
+gzip compressed data, was "starmerx_url-0.1.2.tar", last modified: Fri Jun  9 05:49:22 2023, max compression
```

## Comparing `starmerx_url-0.1.1.tar` & `starmerx_url-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2022-11-10 06:39:38.942736 starmerx_url-0.1.1/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.1/LICENSE
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2022-11-10 06:39:38.942736 starmerx_url-0.1.1/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      257 2022-11-10 06:36:37.000000 starmerx_url-0.1.1/README.md
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       59 2022-11-10 06:39:38.942736 starmerx_url-0.1.1/setup.cfg
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2022-11-10 06:39:15.000000 starmerx_url-0.1.1/setup.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2022-11-10 06:39:38.942736 starmerx_url-0.1.1/starmerx_url/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.1/starmerx_url/__init__.py
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     1905 2022-11-10 06:36:37.000000 starmerx_url-0.1.1/starmerx_url/verify_url.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2022-11-10 06:39:38.942736 starmerx_url-0.1.1/starmerx_url.egg-info/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2022-11-10 06:39:38.000000 starmerx_url-0.1.1/starmerx_url.egg-info/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      263 2022-11-10 06:39:38.000000 starmerx_url-0.1.1/starmerx_url.egg-info/SOURCES.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-11-10 06:39:38.000000 starmerx_url-0.1.1/starmerx_url.egg-info/dependency_links.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2022-11-10 06:39:38.000000 starmerx_url-0.1.1/starmerx_url.egg-info/top_level.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-11-10 06:39:38.000000 starmerx_url-0.1.1/starmerx_url.egg-info/zip-safe
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 05:49:22.418235 starmerx_url-0.1.2/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.2/LICENSE
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 05:49:22.418235 starmerx_url-0.1.2/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      494 2023-06-09 05:48:32.000000 starmerx_url-0.1.2/README.md
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-06-09 05:49:22.418235 starmerx_url-0.1.2/setup.cfg
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-06-09 05:49:19.000000 starmerx_url-0.1.2/setup.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 05:49:22.414235 starmerx_url-0.1.2/starmerx_url/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.2/starmerx_url/__init__.py
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     1905 2023-06-09 05:47:47.000000 starmerx_url-0.1.2/starmerx_url/verify_url.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 05:49:22.414235 starmerx_url-0.1.2/starmerx_url.egg-info/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/top_level.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.2/starmerx_url.egg-info/zip-safe
```

### Comparing `starmerx_url-0.1.1/LICENSE` & `starmerx_url-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerx_url-0.1.1/setup.py` & `starmerx_url-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="starmerx_url",
-    version="0.1.1",
+    version="0.1.2",
     author="yang",
     author_email="yangjuan@starmerx.com",
     description="starmerx verify url",
     license="MIT",
     url="",  # github
     packages=setuptools.find_packages(),
     include_package_data=True,
```

### Comparing `starmerx_url-0.1.1/starmerx_url/verify_url.py` & `starmerx_url-0.1.2/starmerx_url/verify_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 white_url_list = list()
 
 reg1_compile = r"192\.168\.\d{1,3}.\d{1,3}"
 reg2_compile = r"192\.168\.1.\d{1,3}"
 remote_addr_real_host = ""
 referer_host = "."
 
-if hasattr(settings, "WHIIT_URL_LIST"):
-    white_url_list = settings.WHIIT_URL_LIST
+if hasattr(settings, "WHITE_URL_LIST"):
+    white_url_list = settings.WHITE_URL_LIST
 
 if hasattr(settings, "COMPILE_REG1"):
     reg1_compile = settings.COMPILE_REG1
 
 if hasattr(settings, "COMPILE_REG2"):
     reg2_compile = settings.COMPILE_REG2
```

