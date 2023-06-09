# Comparing `tmp/imerit-ango-1.1.0.tar.gz` & `tmp/imerit-ango-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imerit-ango-1.1.0.tar", last modified: Fri Jun  9 09:13:30 2023, max compression
+gzip compressed data, was "imerit-ango-1.1.1.tar", last modified: Fri Jun  9 09:14:23 2023, max compression
```

## Comparing `imerit-ango-1.1.0.tar` & `imerit-ango-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:13:30.636623 imerit-ango-1.1.0/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-09 09:13:30.636623 imerit-ango-1.1.0/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.0/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:13:30.636623 imerit-ango-1.1.0/imerit_ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 imerit-ango-1.1.0/imerit_ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:13:30.636623 imerit-ango-1.1.0/imerit_ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 imerit-ango-1.1.0/imerit_ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 imerit-ango-1.1.0/imerit_ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-09 09:11:15.000000 imerit-ango-1.1.0/imerit_ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 imerit-ango-1.1.0/imerit_ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5652 2023-06-09 09:11:54.000000 imerit-ango-1.1.0/imerit_ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-09 09:11:54.000000 imerit-ango-1.1.0/imerit_ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:13:30.636623 imerit-ango-1.1.0/imerit_ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-09 09:13:30.000000 imerit-ango-1.1.0/imerit_ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-09 09:13:30.000000 imerit-ango-1.1.0/imerit_ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-09 09:13:30.000000 imerit-ango-1.1.0/imerit_ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-09 09:13:30.000000 imerit-ango-1.1.0/imerit_ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-09 09:13:30.000000 imerit-ango-1.1.0/imerit_ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-09 09:13:30.636623 imerit-ango-1.1.0/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-09 09:13:29.000000 imerit-ango-1.1.0/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.1/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/imerit_ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 imerit-ango-1.1.1/imerit_ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/imerit_ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 imerit-ango-1.1.1/imerit_ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 imerit-ango-1.1.1/imerit_ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-09 09:11:15.000000 imerit-ango-1.1.1/imerit_ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 imerit-ango-1.1.1/imerit_ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5652 2023-06-09 09:11:54.000000 imerit-ango-1.1.1/imerit_ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-09 09:11:54.000000 imerit-ango-1.1.1/imerit_ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/imerit_ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-09 09:14:22.000000 imerit-ango-1.1.1/setup.py
```

### Comparing `imerit-ango-1.1.0/PKG-INFO` & `imerit-ango-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.0/README.md` & `imerit-ango-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.0/imerit_ango/models/label_category.py` & `imerit-ango-1.1.1/imerit_ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.0/imerit_ango/plugin_logger.py` & `imerit-ango-1.1.1/imerit_ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.0/imerit_ango/plugins.py` & `imerit-ango-1.1.1/imerit_ango/plugins.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.0/imerit_ango/sdk.py` & `imerit-ango-1.1.1/imerit_ango/sdk.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.0/imerit_ango.egg-info/PKG-INFO` & `imerit-ango-1.1.1/imerit_ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.0/setup.py` & `imerit-ango-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="imerit-ango",
-    version="1.1.0",
+    version="1.1.1",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

