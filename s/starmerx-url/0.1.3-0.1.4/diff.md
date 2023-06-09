# Comparing `tmp/starmerx_url-0.1.3.tar.gz` & `tmp/starmerx_url-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmerx_url-0.1.3.tar", last modified: Fri Jun  9 08:51:09 2023, max compression
+gzip compressed data, was "starmerx_url-0.1.4.tar", last modified: Fri Jun  9 10:00:15 2023, max compression
```

## Comparing `starmerx_url-0.1.3.tar` & `starmerx_url-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 08:51:09.422678 starmerx_url-0.1.3/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.3/LICENSE
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 08:51:09.418678 starmerx_url-0.1.3/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      494 2023-06-09 05:48:32.000000 starmerx_url-0.1.3/README.md
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-06-09 08:51:09.422678 starmerx_url-0.1.3/setup.cfg
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-06-09 08:51:08.000000 starmerx_url-0.1.3/setup.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 08:51:09.418678 starmerx_url-0.1.3/starmerx_url/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.3/starmerx_url/__init__.py
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     2116 2023-06-09 08:50:28.000000 starmerx_url-0.1.3/starmerx_url/verify_url.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 08:51:09.418678 starmerx_url-0.1.3/starmerx_url.egg-info/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/SOURCES.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/dependency_links.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/top_level.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.3/starmerx_url.egg-info/zip-safe
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 10:00:15.233679 starmerx_url-0.1.4/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.4/LICENSE
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 10:00:15.233679 starmerx_url-0.1.4/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      494 2023-06-09 05:48:32.000000 starmerx_url-0.1.4/README.md
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-06-09 10:00:15.233679 starmerx_url-0.1.4/setup.cfg
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-06-09 10:00:07.000000 starmerx_url-0.1.4/setup.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 10:00:15.233679 starmerx_url-0.1.4/starmerx_url/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.4/starmerx_url/__init__.py
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     2252 2023-06-09 09:59:34.000000 starmerx_url-0.1.4/starmerx_url/verify_url.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 10:00:15.233679 starmerx_url-0.1.4/starmerx_url.egg-info/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 10:00:15.000000 starmerx_url-0.1.4/starmerx_url.egg-info/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-06-09 10:00:15.000000 starmerx_url-0.1.4/starmerx_url.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-06-09 10:00:15.000000 starmerx_url-0.1.4/starmerx_url.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-06-09 10:00:15.000000 starmerx_url-0.1.4/starmerx_url.egg-info/top_level.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.4/starmerx_url.egg-info/zip-safe
```

### Comparing `starmerx_url-0.1.3/LICENSE` & `starmerx_url-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerx_url-0.1.3/setup.py` & `starmerx_url-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="starmerx_url",
-    version="0.1.3",
+    version="0.1.4",
     author="yang",
     author_email="yangjuan@starmerx.com",
     description="starmerx verify url",
     license="MIT",
     url="",  # github
     packages=setuptools.find_packages(),
     include_package_data=True,
```

### Comparing `starmerx_url-0.1.3/starmerx_url/verify_url.py` & `starmerx_url-0.1.4/starmerx_url/verify_url.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
     def validate_remote(self, request):
         remote_addr = request.META.get("REMOTE_ADDR", "")
         remote_addr_real = request.META.get("HTTP_X_REAL_IP", "")
         referer = request.META.get("HTTP_REFERER", "")
         reg2 = re.compile(reg2_compile)
         reg1 = re.compile(reg1_compile)
-
+        print(f"remote_addr--{remote_addr}")
+        print(f"remote_addr_real--{remote_addr_real}")
+        print(f"referer--{referer}")
         if referer_host:
             return re.match(reg2, remote_addr) or \
                    re.match(reg1, remote_addr_real) or \
                    remote_addr_real == remote_addr_real_host or \
                    referer_host in referer
 
         return re.match(reg2, remote_addr) or \
```

