# Comparing `tmp/myelectricaldatapy-2.1.0.tar.gz` & `tmp/myelectricaldatapy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.1.0.tar", last modified: Thu Jun  8 06:35:48 2023, max compression
+gzip compressed data, was "myelectricaldatapy-2.1.1.tar", last modified: Fri Jun  9 06:58:13 2023, max compression
```

## Comparing `myelectricaldatapy-2.1.0.tar` & `myelectricaldatapy-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:35:48.179151 myelectricaldatapy-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-08 06:35:48.179151 myelectricaldatapy-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:35:48.175151 myelectricaldatapy-2.1.0/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:35:48.179151 myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-08 06:35:48.000000 myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 06:35:48.000000 myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:35:48.000000 myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 06:35:48.000000 myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 06:35:48.000000 myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 06:35:48.179151 myelectricaldatapy-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-08 06:35:46.000000 myelectricaldatapy-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:35:48.179151 myelectricaldatapy-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    52825 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-08 06:35:39.000000 myelectricaldatapy-2.1.0/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:58:13.587933 myelectricaldatapy-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-09 06:58:13.587933 myelectricaldatapy-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:58:13.583932 myelectricaldatapy-2.1.1/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:58:13.583932 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-09 06:58:13.000000 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-09 06:58:13.000000 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:58:13.000000 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:58:13.000000 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 06:58:13.000000 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 06:58:13.000000 myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-09 06:58:04.000000 myelectricaldatapy-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:58:13.587933 myelectricaldatapy-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:58:13.587933 myelectricaldatapy-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52825 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-09 06:57:53.000000 myelectricaldatapy-2.1.1/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.0/LICENSE` & `myelectricaldatapy-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/PKG-INFO` & `myelectricaldatapy-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.0
+Version: 2.1.1
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
-Author-email: cyr-ius@ipocus.net
+Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
+Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Home Automation
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myelectricaldatapy
 
 Fetch date Enedis Linky from myelectricaldata.fr (enedisgateway.tech)
```

### Comparing `myelectricaldatapy-2.1.0/README.md` & `myelectricaldatapy-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.1.1/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.1.1/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.1.1/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.1.1/myelectricaldatapy/mypdl.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.0
+Version: 2.1.1
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
-Author-email: cyr-ius@ipocus.net
+Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
+Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Home Automation
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myelectricaldatapy
 
 Fetch date Enedis Linky from myelectricaldata.fr (enedisgateway.tech)
```

### Comparing `myelectricaldatapy-2.1.0/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.1.1/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 myelectricaldatapy/const.py
 myelectricaldatapy/exceptions.py
 myelectricaldatapy/myelectricaldata.py
 myelectricaldatapy/mypdl.py
 myelectricaldatapy.egg-info/PKG-INFO
 myelectricaldatapy.egg-info/SOURCES.txt
 myelectricaldatapy.egg-info/dependency_links.txt
+myelectricaldatapy.egg-info/not-zip-safe
 myelectricaldatapy.egg-info/requires.txt
 myelectricaldatapy.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/consts.py
 tests/test_analytics.py
 tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.0/setup.py` & `myelectricaldatapy-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="2.1.0",
+    version="replace_by_workflow",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-2.1.0/tests/conftest.py` & `myelectricaldatapy-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/tests/consts.py` & `myelectricaldatapy-2.1.1/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/tests/test_analytics.py` & `myelectricaldatapy-2.1.1/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.0/tests/test_load_data.py` & `myelectricaldatapy-2.1.1/tests/test_load_data.py`

 * *Files identical despite different names*

