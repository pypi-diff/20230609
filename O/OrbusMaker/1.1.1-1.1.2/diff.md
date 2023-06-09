# Comparing `tmp/OrbusMaker-1.1.1.tar.gz` & `tmp/OrbusMaker-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OrbusMaker-1.1.1.tar", last modified: Fri Jun  9 16:01:30 2023, max compression
+gzip compressed data, was "OrbusMaker-1.1.2.tar", last modified: Fri Jun  9 16:11:04 2023, max compression
```

## Comparing `OrbusMaker-1.1.1.tar` & `OrbusMaker-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-09 16:01:30.760923 OrbusMaker-1.1.1/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 04:29:39.000000 OrbusMaker-1.1.1/LICENSE
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-09 16:01:30.760923 OrbusMaker-1.1.1/OrbusMaker.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      919 2023-06-09 16:01:30.000000 OrbusMaker-1.1.1/OrbusMaker.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      199 2023-06-09 16:01:30.000000 OrbusMaker-1.1.1/OrbusMaker.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-09 16:01:30.000000 OrbusMaker-1.1.1/OrbusMaker.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       61 2023-06-09 16:01:30.000000 OrbusMaker-1.1.1/OrbusMaker.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        6 2023-06-09 16:01:30.000000 OrbusMaker-1.1.1/OrbusMaker.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      919 2023-06-09 16:01:30.760923 OrbusMaker-1.1.1/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      469 2023-06-09 15:53:11.000000 OrbusMaker-1.1.1/README.md
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-09 16:01:30.760923 OrbusMaker-1.1.1/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      855 2023-06-09 16:01:16.000000 OrbusMaker-1.1.1/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-09 16:11:04.479759 OrbusMaker-1.1.2/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 04:29:39.000000 OrbusMaker-1.1.2/LICENSE
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-09 16:11:04.479759 OrbusMaker-1.1.2/OrbusMaker.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      929 2023-06-09 16:11:04.000000 OrbusMaker-1.1.2/OrbusMaker.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      199 2023-06-09 16:11:04.000000 OrbusMaker-1.1.2/OrbusMaker.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-09 16:11:04.000000 OrbusMaker-1.1.2/OrbusMaker.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       61 2023-06-09 16:11:04.000000 OrbusMaker-1.1.2/OrbusMaker.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        6 2023-06-09 16:11:04.000000 OrbusMaker-1.1.2/OrbusMaker.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      929 2023-06-09 16:11:04.479759 OrbusMaker-1.1.2/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      479 2023-06-09 16:09:50.000000 OrbusMaker-1.1.2/README.md
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-09 16:11:04.479759 OrbusMaker-1.1.2/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      855 2023-06-09 16:10:41.000000 OrbusMaker-1.1.2/setup.py
```

### Comparing `OrbusMaker-1.1.1/LICENSE` & `OrbusMaker-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OrbusMaker-1.1.1/OrbusMaker.egg-info/PKG-INFO` & `OrbusMaker-1.1.2/OrbusMaker.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OrbusMaker
-Version: 1.1.1
+Version: 1.1.2
 Summary: An app skeleton creator, using CLI interface
 Home-page: https://github.com/Orbus-Company/OrbusMaker
 Author: Wilovy09
 Author-email: orbuscompany@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # Orbus
 
 Orbus es un creador de proyectos.
 
 Puedes instalarlo con:
 
 ```bash
-pip install Orbus
+pip install OrbusMaker
 ```
 
 Para invocarlo hace falta usar el comando:
 
 ```bash
 python -m orbus create-flet-app
 
@@ -32,12 +32,12 @@
 # >> 
 ```
 
 Esto generara una carpeta donde estemos ubicados.
 
 
 Links:
-- [Pypi](https://pypi.org/project/Orbus/)
+- [Pypi](https://pypi.org/project/OrbusMaker/)
 - [Github](https://github.com/Orbus-Company/OrbusMaker)
 
 Actualizaciones:
 - [ ] Soporte a distintos lenguajes/frameworks
```

### Comparing `OrbusMaker-1.1.1/PKG-INFO` & `OrbusMaker-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OrbusMaker
-Version: 1.1.1
+Version: 1.1.2
 Summary: An app skeleton creator, using CLI interface
 Home-page: https://github.com/Orbus-Company/OrbusMaker
 Author: Wilovy09
 Author-email: orbuscompany@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # Orbus
 
 Orbus es un creador de proyectos.
 
 Puedes instalarlo con:
 
 ```bash
-pip install Orbus
+pip install OrbusMaker
 ```
 
 Para invocarlo hace falta usar el comando:
 
 ```bash
 python -m orbus create-flet-app
 
@@ -32,12 +32,12 @@
 # >> 
 ```
 
 Esto generara una carpeta donde estemos ubicados.
 
 
 Links:
-- [Pypi](https://pypi.org/project/Orbus/)
+- [Pypi](https://pypi.org/project/OrbusMaker/)
 - [Github](https://github.com/Orbus-Company/OrbusMaker)
 
 Actualizaciones:
 - [ ] Soporte a distintos lenguajes/frameworks
```

### Comparing `OrbusMaker-1.1.1/setup.py` & `OrbusMaker-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as ld:
     long_description = ld.read()
 
 setup(
     name="OrbusMaker",
-    version="1.1.1",
+    version="1.1.2",
     author="Wilovy09",
     author_email="orbuscompany@gmail.com",
     description="An app skeleton creator, using CLI interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Orbus-Company/OrbusMaker",
     python_requires=">3.10",
```

