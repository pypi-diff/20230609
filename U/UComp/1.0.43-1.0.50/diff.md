# Comparing `tmp/UComp-1.0.43.tar.gz` & `tmp/UComp-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.43.tar", last modified: Fri Jun  9 15:28:10 2023, max compression
+gzip compressed data, was "UComp-1.0.50.tar", last modified: Fri Jun  9 15:39:44 2023, max compression
```

## Comparing `UComp-1.0.43.tar` & `UComp-1.0.50.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:28:10.352693 UComp-1.0.43/
--rw-rw-rw-   0        0        0      356 2023-06-09 15:08:24.000000 UComp-1.0.43/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-09 15:28:10.352693 UComp-1.0.43/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.43/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 15:28:10.346171 UComp-1.0.43/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.43/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.43/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    10831 2023-06-09 15:21:08.000000 UComp-1.0.43/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11596 2023-06-09 12:22:16.000000 UComp-1.0.43/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.43/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.43/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24258 2023-06-09 15:20:10.000000 UComp-1.0.43/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      121 2023-06-09 12:24:40.000000 UComp-1.0.43/UComp/__init__.py
--rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.43/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.43/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.43/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.43/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    30026 2023-06-09 15:27:28.000000 UComp-1.0.43/UComp/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:28:10.352693 UComp-1.0.43/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-09 15:28:09.000000 UComp-1.0.43/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-09 15:28:09.000000 UComp-1.0.43/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:28:09.000000 UComp-1.0.43/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-09 15:28:09.000000 UComp-1.0.43/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 15:28:09.000000 UComp-1.0.43/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 15:28:10.352693 UComp-1.0.43/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-09 15:28:01.000000 UComp-1.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:39:44.202726 UComp-1.0.50/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.50/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-06-09 15:39:44.202726 UComp-1.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.50/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:39:44.187104 UComp-1.0.50/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.50/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.50/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    10831 2023-06-09 15:21:08.000000 UComp-1.0.50/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11596 2023-06-09 12:22:16.000000 UComp-1.0.50/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.50/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.50/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24258 2023-06-09 15:20:10.000000 UComp-1.0.50/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.50/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.50/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.50/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.50/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.50/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    30026 2023-06-09 15:27:28.000000 UComp-1.0.50/UComp/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:39:44.202726 UComp-1.0.50/UComp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-06-09 15:39:44.000000 UComp-1.0.50/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-09 15:39:44.000000 UComp-1.0.50/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:39:44.000000 UComp-1.0.50/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-09 15:39:44.000000 UComp-1.0.50/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 15:39:44.000000 UComp-1.0.50/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:39:44.218343 UComp-1.0.50/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-09 15:39:22.000000 UComp-1.0.50/setup.py
```

### Comparing `UComp-1.0.43/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.50/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/ETSmodule.py` & `UComp-1.0.50/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/PTSmodule.py` & `UComp-1.0.50/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.50/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/UCmodule.py` & `UComp-1.0.50/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/airpas.bin` & `UComp-1.0.50/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/gdp.bin` & `UComp-1.0.50/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/ipi.bin` & `UComp-1.0.50/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/libopenblas.dll` & `UComp-1.0.50/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/UComp/tools.py` & `UComp-1.0.50/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.43/setup.py` & `UComp-1.0.50/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.43',
+    version='1.0.50',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

