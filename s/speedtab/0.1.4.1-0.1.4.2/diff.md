# Comparing `tmp/speedtab-0.1.4.1.tar.gz` & `tmp/speedtab-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.4.1.tar", max compression
+gzip compressed data, was "speedtab-0.1.4.2.tar", max compression
```

## Comparing `speedtab-0.1.4.1.tar` & `speedtab-0.1.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-06-02 10:10:18.360384 speedtab-0.1.4.1/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.4.1/speedtab/__init__.py
--rw-r--r--   0        0        0    49953 2023-05-24 14:57:04.407916 speedtab-0.1.4.1/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4.1/speedtab/enums.py
--rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.4.1/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-06-02 10:11:19.248435 speedtab-0.1.4.1/setup.py
--rw-r--r--   0        0        0      808 2023-06-02 10:11:19.248435 speedtab-0.1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-06-09 12:08:08.609798 speedtab-0.1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.4.2/speedtab/__init__.py
+-rw-r--r--   0        0        0    49953 2023-05-24 14:57:04.407916 speedtab-0.1.4.2/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4.2/speedtab/enums.py
+-rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.4.2/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-06-09 12:08:17.357980 speedtab-0.1.4.2/setup.py
+-rw-r--r--   0        0        0      808 2023-06-09 12:08:17.357980 speedtab-0.1.4.2/PKG-INFO
```

### Comparing `speedtab-0.1.4.1/pyproject.toml` & `speedtab-0.1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.4.1"
+version = "0.1.4.2"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.4.1/speedtab/client.py` & `speedtab-0.1.4.2/speedtab/client.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.1/speedtab/enums.py` & `speedtab-0.1.4.2/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.1/speedtab/formats.py` & `speedtab-0.1.4.2/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.1/setup.py` & `speedtab-0.1.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.4.1',
+    'version': '0.1.4.2',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.4.1/PKG-INFO` & `speedtab-0.1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

