# Comparing `tmp/conlay-1.0.2.tar.gz` & `tmp/conlay-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlay-1.0.2.tar", last modified: Fri Jun  9 13:32:09 2023, max compression
+gzip compressed data, was "conlay-1.0.3.tar", last modified: Fri Jun  9 13:46:02 2023, max compression
```

## Comparing `conlay-1.0.2.tar` & `conlay-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:32:09.146850 conlay-1.0.2/
--rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1555 2023-06-09 13:32:09.145350 conlay-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2023-06-09 13:25:18.000000 conlay-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 13:32:09.140849 conlay-1.0.2/conlay.egg-info/
--rw-rw-rw-   0        0        0     1555 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-09 13:32:09.000000 conlay-1.0.2/conlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 13:32:09.146850 conlay-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-06-09 13:31:46.000000 conlay-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:32:09.142850 conlay-1.0.2/src/
--rw-rw-rw-   0        0        0       19 2023-06-09 13:30:45.000000 conlay-1.0.2/src/__init__.py
--rw-rw-rw-   0        0        0    11531 2023-06-09 11:38:45.000000 conlay-1.0.2/src/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:46:02.779812 conlay-1.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1555 2023-06-09 13:46:02.778312 conlay-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2023-06-09 13:25:18.000000 conlay-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 13:46:02.770311 conlay-1.0.3/conlay/
+-rw-rw-rw-   0        0        0       19 2023-06-09 13:30:45.000000 conlay-1.0.3/conlay/__init__.py
+-rw-rw-rw-   0        0        0    11531 2023-06-09 11:38:45.000000 conlay-1.0.3/conlay/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:46:02.776812 conlay-1.0.3/conlay.egg-info/
+-rw-rw-rw-   0        0        0     1555 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 13:46:02.780312 conlay-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-06-09 13:44:29.000000 conlay-1.0.3/setup.py
```

### Comparing `conlay-1.0.2/LICENSE` & `conlay-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conlay-1.0.2/PKG-INFO` & `conlay-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conlay
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python library for creating nice layouts in the console environment
 Home-page: https://github.com/Salliii/conlay
 Author: Salliii
 Keywords: python,library,console,layout
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conlay Version: 1.0.2 Summary: A python library for
+Metadata-Version: 2.1 Name: conlay Version: 1.0.3 Summary: A python library for
 creating nice layouts in the console environment Home-page: https://github.com/
 Salliii/conlay Author: Salliii Keywords: python,library,console,layout
 Description-Content-Type: text/markdown License-File: LICENSE Conlay - Console
 Layout ======================= [![PyPi version][shields-pypi_version]][url-
 pypi_version] [![Github Issues][shields-issues]][url-issues] [![Github License]
 [shields-license]][url-license] Create visually pleasing console layouts with
 this easy-to-use Python library.
```

### Comparing `conlay-1.0.2/README.md` & `conlay-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `conlay-1.0.2/conlay.egg-info/PKG-INFO` & `conlay-1.0.3/conlay.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conlay
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python library for creating nice layouts in the console environment
 Home-page: https://github.com/Salliii/conlay
 Author: Salliii
 Keywords: python,library,console,layout
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conlay Version: 1.0.2 Summary: A python library for
+Metadata-Version: 2.1 Name: conlay Version: 1.0.3 Summary: A python library for
 creating nice layouts in the console environment Home-page: https://github.com/
 Salliii/conlay Author: Salliii Keywords: python,library,console,layout
 Description-Content-Type: text/markdown License-File: LICENSE Conlay - Console
 Layout ======================= [![PyPi version][shields-pypi_version]][url-
 pypi_version] [![Github Issues][shields-issues]][url-issues] [![Github License]
 [shields-license]][url-license] Create visually pleasing console layouts with
 this easy-to-use Python library.
```

### Comparing `conlay-1.0.2/setup.py` & `conlay-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 with open("README.md", "r", encoding="utf-8") as readme:
     DESC_LONG = readme.read()
 
 
 setuptools.setup(
     name="conlay",
```

### Comparing `conlay-1.0.2/src/main.py` & `conlay-1.0.3/conlay/main.py`

 * *Files identical despite different names*

