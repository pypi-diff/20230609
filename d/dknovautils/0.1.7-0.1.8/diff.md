# Comparing `tmp/dknovautils-0.1.7.tar.gz` & `tmp/dknovautils-0.1.8.tar.gz`

## Comparing `dknovautils-0.1.7.tar` & `dknovautils-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 dknovautils-0.1.7/.gitignore
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 dknovautils-0.1.7/LICENSE
--rwxr-xr-x   0        0        0      476 2020-02-02 00:00:00.000000 dknovautils-0.1.7/README.md
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 dknovautils-0.1.7/pyproject.toml
--rwxr-xr-x   0        0        0     1159 2020-02-02 00:00:00.000000 dknovautils-0.1.7/setup.py
--rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 dknovautils-0.1.7/test_a.py
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 dknovautils-0.1.7/test_b01.py
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 dknovautils-0.1.7/test_c.py
--rwxr-xr-x   0        0        0     1181 2020-02-02 00:00:00.000000 dknovautils-0.1.7/upload.sh
--rwxr-xr-x   0        0        0      880 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/PKG-INFO
--rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/SOURCES.txt
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/dependency_links.txt
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/requires.txt
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dknovautils-0.1.7/dknovautils.egg-info/top_level.txt
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/__init__.py
--rwxr-xr-x   0        0        0     2523 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/commons.py
--rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dk_imports.py
--rwxr-xr-x   0        0        0     8679 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dkat.py
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dkfiles.py
--rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/dkipy.py
--rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/example.py
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/myadd.py
--rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 dknovautils-0.1.7/src/dknovautils/mysubtract.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dknovautils-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 dknovautils-0.1.8/.gitignore
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 dknovautils-0.1.8/LICENSE
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 dknovautils-0.1.8/README.md
+-rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 dknovautils-0.1.8/pyproject.toml
+-rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 dknovautils-0.1.8/test_a.py
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 dknovautils-0.1.8/test_b01.py
+-rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 dknovautils-0.1.8/test_c.py
+-rwxr-xr-x   0        0        0     1184 2020-02-02 00:00:00.000000 dknovautils-0.1.8/upload.sh
+-rwxr-xr-x   0        0        0      880 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/PKG-INFO
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/SOURCES.txt
+-rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/dependency_links.txt
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/requires.txt
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/__init__.py
+-rwxr-xr-x   0        0        0     2523 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/commons.py
+-rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dk_imports.py
+-rwxr-xr-x   0        0        0     8679 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dkat.py
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dkfiles.py
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dkipy.py
+-rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/example.py
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/myadd.py
+-rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/mysubtract.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 dknovautils-0.1.8/PKG-INFO
```

### Comparing `dknovautils-0.1.7/.gitignore` & `dknovautils-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.7/LICENSE` & `dknovautils-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.7/pyproject.toml` & `dknovautils-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "dknovautils"
-version = '0.1.7'
+version = '0.1.8'
 authors = [
   { name="dknova", email="dikisite@outlook.com" },
 ]
 description = "A small example package"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `dknovautils-0.1.7/test_a.py` & `dknovautils-0.1.8/test_a.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.7/upload.sh` & `dknovautils-0.1.8/upload.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-AppVer="0.1.7"
+AppVer="0.1.8"
+
+# sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./setup.py
 
-sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./setup.py
 sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./src/dknovautils/dk_imports.py
 sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./src/dknovautils/dkat.py
 
 sed -i "s/^version =.*/version = '$AppVer'/" ./pyproject.toml
 
 rm ./dist/*
```

### Comparing `dknovautils-0.1.7/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.8/dknovautils.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.7/src/dknovautils/commons.py` & `dknovautils-0.1.8/src/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.7/src/dknovautils/dk_imports.py` & `dknovautils-0.1.8/src/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.7/src/dknovautils/dkat.py` & `dknovautils-0.1.8/src/dknovautils/dkat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from typing import Any
 import dknovautils
 from dknovautils.commons import *
 
 
-DkAppVer = '0.1.7'
+DkAppVer = '0.1.8'
 
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
```

### Comparing `dknovautils-0.1.7/src/dknovautils/dkipy.py` & `dknovautils-0.1.8/src/dknovautils/dkipy.py`

 * *Files identical despite different names*

