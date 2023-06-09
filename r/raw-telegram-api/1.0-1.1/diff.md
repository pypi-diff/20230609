# Comparing `tmp/raw-telegram-api-1.0.tar.gz` & `tmp/raw-telegram-api-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raw-telegram-api-1.0.tar", last modified: Fri Jun  9 12:44:58 2023, max compression
+gzip compressed data, was "raw-telegram-api-1.1.tar", last modified: Fri Jun  9 13:00:26 2023, max compression
```

## Comparing `raw-telegram-api-1.0.tar` & `raw-telegram-api-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 12:44:58.422229 raw-telegram-api-1.0/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)     1073 2023-06-09 12:38:58.000000 raw-telegram-api-1.0/LICENSE
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 12:44:58.422229 raw-telegram-api-1.0/PKG-INFO
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      249 2023-06-09 12:39:19.000000 raw-telegram-api-1.0/README.md
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      592 2023-06-09 12:44:11.000000 raw-telegram-api-1.0/pyproject.toml
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 12:44:58.410230 raw-telegram-api-1.0/raw-telegram/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       20 2023-06-09 12:22:03.000000 raw-telegram-api-1.0/raw-telegram/__init__.py
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      462 2023-06-09 12:31:30.000000 raw-telegram-api-1.0/raw-telegram/api.py
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 12:44:58.418229 raw-telegram-api-1.0/raw_telegram_api.egg-info/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 12:44:58.000000 raw-telegram-api-1.0/raw_telegram_api.egg-info/PKG-INFO
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      246 2023-06-09 12:44:58.000000 raw-telegram-api-1.0/raw_telegram_api.egg-info/SOURCES.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)        1 2023-06-09 12:44:58.000000 raw-telegram-api-1.0/raw_telegram_api.egg-info/dependency_links.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       13 2023-06-09 12:44:58.000000 raw-telegram-api-1.0/raw_telegram_api.egg-info/top_level.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       38 2023-06-09 12:44:58.422229 raw-telegram-api-1.0/setup.cfg
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      242 2023-06-09 12:21:26.000000 raw-telegram-api-1.0/setup.py
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:00:26.262230 raw-telegram-api-1.1/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)     1073 2023-06-09 12:38:58.000000 raw-telegram-api-1.1/LICENSE
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 13:00:26.258230 raw-telegram-api-1.1/PKG-INFO
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      249 2023-06-09 12:54:44.000000 raw-telegram-api-1.1/README.md
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      592 2023-06-09 12:59:38.000000 raw-telegram-api-1.1/pyproject.toml
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:00:26.254229 raw-telegram-api-1.1/raw_telegram/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       20 2023-06-09 12:22:03.000000 raw-telegram-api-1.1/raw_telegram/__init__.py
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      462 2023-06-09 12:31:30.000000 raw-telegram-api-1.1/raw_telegram/api.py
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:00:26.258230 raw-telegram-api-1.1/raw_telegram_api.egg-info/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/PKG-INFO
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      246 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/SOURCES.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)        1 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/dependency_links.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       13 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/top_level.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       38 2023-06-09 13:00:26.262230 raw-telegram-api-1.1/setup.cfg
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      242 2023-06-09 12:59:30.000000 raw-telegram-api-1.1/setup.py
```

### Comparing `raw-telegram-api-1.0/LICENSE` & `raw-telegram-api-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raw-telegram-api-1.0/PKG-INFO` & `raw-telegram-api-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raw-telegram-api
-Version: 1.0
+Version: 1.1
 Summary: Raw Telegram API
 Author: mishpro
 Author-email: mishpro <root@venusbiser.ru>
 Project-URL: Homepage, https://github.com/mishpro-programm/raw-telegram-api
 Project-URL: Bug Tracker, https://github.com/mishpro-programm/raw-telegram-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,12 +13,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # raw-telegram-api
 Raw Telegram API for Python 3\
 #Example
 ```python
-from raw-telegram.api import APIClient
+from raw_telegram.api import APIClient
 token = "<paste your token here>"
 api = APIClient(token)
 api.send_method("sendMessage", {'chat_id': 5102762920, 'text': 'Hello world!'})
 ```
```

### Comparing `raw-telegram-api-1.0/pyproject.toml` & `raw-telegram-api-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raw-telegram-api"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="mishpro", email="root@venusbiser.ru" },
 ]
 description = "Raw Telegram API"
 readme = "README.md"
 requires-python = ">3"
 classifiers = [
```

### Comparing `raw-telegram-api-1.0/raw_telegram_api.egg-info/PKG-INFO` & `raw-telegram-api-1.1/raw_telegram_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raw-telegram-api
-Version: 1.0
+Version: 1.1
 Summary: Raw Telegram API
 Author: mishpro
 Author-email: mishpro <root@venusbiser.ru>
 Project-URL: Homepage, https://github.com/mishpro-programm/raw-telegram-api
 Project-URL: Bug Tracker, https://github.com/mishpro-programm/raw-telegram-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,12 +13,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # raw-telegram-api
 Raw Telegram API for Python 3\
 #Example
 ```python
-from raw-telegram.api import APIClient
+from raw_telegram.api import APIClient
 token = "<paste your token here>"
 api = APIClient(token)
 api.send_method("sendMessage", {'chat_id': 5102762920, 'text': 'Hello world!'})
 ```
```

