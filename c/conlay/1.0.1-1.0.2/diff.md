# Comparing `tmp/conlay-1.0.1.tar.gz` & `tmp/conlay-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlay-1.0.1.tar", last modified: Fri Jun  9 12:13:33 2023, max compression
+gzip compressed data, was "conlay-1.0.2.tar", last modified: Fri Jun  9 13:32:09 2023, max compression
```

## Comparing `conlay-1.0.1.tar` & `conlay-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:13:33.870569 conlay-1.0.1/
--rw-rw-rw-   0        0        0      298 2023-06-09 12:13:33.869570 conlay-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-06-09 11:38:45.000000 conlay-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 12:13:33.864568 conlay-1.0.1/conlay.egg-info/
--rw-rw-rw-   0        0        0      298 2023-06-09 12:13:33.000000 conlay-1.0.1/conlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-09 12:13:33.000000 conlay-1.0.1/conlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:13:33.000000 conlay-1.0.1/conlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-09 12:13:33.000000 conlay-1.0.1/conlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 12:13:33.870569 conlay-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-06-09 12:13:30.000000 conlay-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:13:33.867069 conlay-1.0.1/src/
--rw-rw-rw-   0        0        0       93 2023-06-09 11:38:45.000000 conlay-1.0.1/src/__init__.py
--rw-rw-rw-   0        0        0    11531 2023-06-09 11:38:45.000000 conlay-1.0.1/src/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:32:09.146850 conlay-1.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1555 2023-06-09 13:32:09.145350 conlay-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2023-06-09 13:25:18.000000 conlay-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 13:32:09.140849 conlay-1.0.2/conlay.egg-info/
+-rw-rw-rw-   0        0        0     1555 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 13:32:09.146850 conlay-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-06-09 13:31:46.000000 conlay-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:32:09.142850 conlay-1.0.2/src/
+-rw-rw-rw-   0        0        0       19 2023-06-09 13:30:45.000000 conlay-1.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0    11531 2023-06-09 11:38:45.000000 conlay-1.0.2/src/main.py
```

### Comparing `conlay-1.0.1/setup.py` & `conlay-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 
 with open("README.md", "r", encoding="utf-8") as readme:
     DESC_LONG = readme.read()
 
 
 setuptools.setup(
     name="conlay",
```

### Comparing `conlay-1.0.1/src/main.py` & `conlay-1.0.2/src/main.py`

 * *Files identical despite different names*

