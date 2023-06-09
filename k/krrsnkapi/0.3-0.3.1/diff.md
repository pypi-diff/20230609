# Comparing `tmp/krrsnkapi-0.3.tar.gz` & `tmp/krrsnkapi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.3.tar", last modified: Wed Jun  7 17:33:32 2023, max compression
+gzip compressed data, was "krrsnkapi-0.3.1.tar", last modified: Fri Jun  9 18:02:15 2023, max compression
```

## Comparing `krrsnkapi-0.3.tar` & `krrsnkapi-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:33:32.722921 krrsnkapi-0.3/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      617 2023-06-07 17:33:32.722921 krrsnkapi-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 17:33:32.707920 krrsnkapi-0.3/krrsnkapi/
--rw-rw-rw-   0        0        0       35 2023-04-13 13:20:12.000000 krrsnkapi-0.3/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-06-07 17:23:47.000000 krrsnkapi-0.3/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:33:32.719921 krrsnkapi-0.3/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-07 17:33:31.000000 krrsnkapi-0.3/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-06-07 17:33:32.000000 krrsnkapi-0.3/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:33:31.000000 krrsnkapi-0.3/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 17:33:31.000000 krrsnkapi-0.3/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-07 17:33:32.000000 krrsnkapi-0.3/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-07 17:33:32.724922 krrsnkapi-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-06-07 17:24:34.000000 krrsnkapi-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:02:15.337585 krrsnkapi-0.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      619 2023-06-09 18:02:15.338585 krrsnkapi-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 18:02:15.319584 krrsnkapi-0.3.1/krrsnkapi/
+-rw-rw-rw-   0        0        0       47 2023-06-09 18:01:47.000000 krrsnkapi-0.3.1/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-06-07 17:23:47.000000 krrsnkapi-0.3.1/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:02:15.335585 krrsnkapi-0.3.1/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-06-09 18:02:12.000000 krrsnkapi-0.3.1/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-06-09 18:02:13.000000 krrsnkapi-0.3.1/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 18:02:12.000000 krrsnkapi-0.3.1/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 18:02:12.000000 krrsnkapi-0.3.1/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 18:02:12.000000 krrsnkapi-0.3.1/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-09 18:02:15.340585 krrsnkapi-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-06-09 18:01:12.000000 krrsnkapi-0.3.1/setup.py
```

### Comparing `krrsnkapi-0.3/LICENSE.txt` & `krrsnkapi-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.3/PKG-INFO` & `krrsnkapi-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.3
+Version: 0.3.1
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
 Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.3.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
```

### Comparing `krrsnkapi-0.3/README.md` & `krrsnkapi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.3/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.3.1/krrsnkapi/krrsnkapi.py`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.3/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-0.3.1/krrsnkapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.3
+Version: 0.3.1
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
 Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.3.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
```

### Comparing `krrsnkapi-0.3/setup.py` & `krrsnkapi-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # ver = input("version: ")
 
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = "0.3",      # Start with a small number and increase it with every change you make
+  version = "0.3.1",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kararasenok-gd/krrsnkapi',   # Provide either the link to your github or to your website
   download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.3.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
```

