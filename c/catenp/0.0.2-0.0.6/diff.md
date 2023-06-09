# Comparing `tmp/catenp-0.0.2.tar.gz` & `tmp/catenp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catenp-0.0.2.tar", last modified: Fri Jun  9 13:50:33 2023, max compression
+gzip compressed data, was "catenp-0.0.6.tar", last modified: Fri Jun  9 13:50:16 2023, max compression
```

## Comparing `catenp-0.0.2.tar` & `catenp-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:50:33.535896 catenp-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1173 2023-06-09 13:50:33.531305 catenp-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-09 11:05:06.000000 catenp-0.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:50:33.448246 catenp-0.0.2/catenp/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-06-09 09:37:10.000000 catenp-0.0.2/catenp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10052 2023-06-09 09:37:58.000000 catenp-0.0.2/catenp/catenumpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:50:33.519536 catenp-0.0.2/catenp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1173 2023-06-09 13:50:33.000000 catenp-0.0.2/catenp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      213 2023-06-09 13:50:33.000000 catenp-0.0.2/catenp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:50:33.000000 catenp-0.0.2/catenp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 13:50:33.000000 catenp-0.0.2/catenp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-09 13:50:33.000000 catenp-0.0.2/catenp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-09 13:50:26.000000 catenp-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:50:33.538220 catenp-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:50:16.517399 catenp-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-06-09 13:50:16.512562 catenp-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-09 11:05:06.000000 catenp-0.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:50:16.424805 catenp-0.0.6/catenp/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-09 09:37:10.000000 catenp-0.0.6/catenp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10052 2023-06-09 09:37:58.000000 catenp-0.0.6/catenp/catenumpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:50:16.499312 catenp-0.0.6/catenp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-06-09 13:50:16.000000 catenp-0.0.6/catenp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-09 13:50:16.000000 catenp-0.0.6/catenp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:50:16.000000 catenp-0.0.6/catenp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 13:50:16.000000 catenp-0.0.6/catenp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-09 13:50:16.000000 catenp-0.0.6/catenp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-09 13:50:10.000000 catenp-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:50:16.520477 catenp-0.0.6/setup.cfg
```

### Comparing `catenp-0.0.2/PKG-INFO` & `catenp-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catenp
-Version: 0.0.2
+Version: 0.0.6
 Summary: Python client for extracting data from CATE archives to numpy arrays
 Author-email: Motion Signal Technologies <info@motionsignaltechnologies.com>
 Project-URL: Homepage, https://github.com/motionsignaltechnologies/cate-numpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `catenp-0.0.2/README.rst` & `catenp-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `catenp-0.0.2/catenp/__init__.py` & `catenp-0.0.6/catenp/__init__.py`

 * *Files identical despite different names*

### Comparing `catenp-0.0.2/catenp/catenumpy.py` & `catenp-0.0.6/catenp/catenumpy.py`

 * *Files identical despite different names*

### Comparing `catenp-0.0.2/catenp.egg-info/PKG-INFO` & `catenp-0.0.6/catenp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catenp
-Version: 0.0.2
+Version: 0.0.6
 Summary: Python client for extracting data from CATE archives to numpy arrays
 Author-email: Motion Signal Technologies <info@motionsignaltechnologies.com>
 Project-URL: Homepage, https://github.com/motionsignaltechnologies/cate-numpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `catenp-0.0.2/pyproject.toml` & `catenp-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "catenp"
-version = "0.0.2"
+version = "0.0.6"
 authors = [
   { name="Motion Signal Technologies", email="info@motionsignaltechnologies.com" },
 ]
 description = "Python client for extracting data from CATE archives to numpy arrays"
 readme = "README.rst"
 requires-python = ">=3.10"
 classifiers = [
```

