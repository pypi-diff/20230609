# Comparing `tmp/raw-telegram-api-1.1.tar.gz` & `tmp/raw-telegram-api-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raw-telegram-api-1.1.tar", last modified: Fri Jun  9 13:00:26 2023, max compression
+gzip compressed data, was "raw-telegram-api-1.2.tar", last modified: Fri Jun  9 13:28:27 2023, max compression
```

## Comparing `raw-telegram-api-1.1.tar` & `raw-telegram-api-1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:00:26.262230 raw-telegram-api-1.1/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)     1073 2023-06-09 12:38:58.000000 raw-telegram-api-1.1/LICENSE
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 13:00:26.258230 raw-telegram-api-1.1/PKG-INFO
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      249 2023-06-09 12:54:44.000000 raw-telegram-api-1.1/README.md
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      592 2023-06-09 12:59:38.000000 raw-telegram-api-1.1/pyproject.toml
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:00:26.254229 raw-telegram-api-1.1/raw_telegram/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       20 2023-06-09 12:22:03.000000 raw-telegram-api-1.1/raw_telegram/__init__.py
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      462 2023-06-09 12:31:30.000000 raw-telegram-api-1.1/raw_telegram/api.py
-drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:00:26.258230 raw-telegram-api-1.1/raw_telegram_api.egg-info/
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/PKG-INFO
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      246 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/SOURCES.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)        1 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/dependency_links.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       13 2023-06-09 13:00:26.000000 raw-telegram-api-1.1/raw_telegram_api.egg-info/top_level.txt
--rw-------   0 u0_a665  (10665) u0_a665  (10665)       38 2023-06-09 13:00:26.262230 raw-telegram-api-1.1/setup.cfg
--rw-------   0 u0_a665  (10665) u0_a665  (10665)      242 2023-06-09 12:59:30.000000 raw-telegram-api-1.1/setup.py
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:28:27.394615 raw-telegram-api-1.2/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)     1073 2023-06-09 12:38:58.000000 raw-telegram-api-1.2/LICENSE
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 13:28:27.394615 raw-telegram-api-1.2/PKG-INFO
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      249 2023-06-09 12:54:44.000000 raw-telegram-api-1.2/README.md
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      628 2023-06-09 13:27:02.000000 raw-telegram-api-1.2/pyproject.toml
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:28:27.386615 raw-telegram-api-1.2/raw_telegram/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       20 2023-06-09 12:22:03.000000 raw-telegram-api-1.2/raw_telegram/__init__.py
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      462 2023-06-09 12:31:30.000000 raw-telegram-api-1.2/raw_telegram/api.py
+drwx------   0 u0_a665  (10665) u0_a665  (10665)        0 2023-06-09 13:28:27.394615 raw-telegram-api-1.2/raw_telegram_api.egg-info/
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      783 2023-06-09 13:28:27.000000 raw-telegram-api-1.2/raw_telegram_api.egg-info/PKG-INFO
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      285 2023-06-09 13:28:27.000000 raw-telegram-api-1.2/raw_telegram_api.egg-info/SOURCES.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)        1 2023-06-09 13:28:27.000000 raw-telegram-api-1.2/raw_telegram_api.egg-info/dependency_links.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       17 2023-06-09 13:28:27.000000 raw-telegram-api-1.2/raw_telegram_api.egg-info/requires.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       13 2023-06-09 13:28:27.000000 raw-telegram-api-1.2/raw_telegram_api.egg-info/top_level.txt
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)       38 2023-06-09 13:28:27.394615 raw-telegram-api-1.2/setup.cfg
+-rw-------   0 u0_a665  (10665) u0_a665  (10665)      242 2023-06-09 13:27:26.000000 raw-telegram-api-1.2/setup.py
```

### Comparing `raw-telegram-api-1.1/LICENSE` & `raw-telegram-api-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raw-telegram-api-1.1/PKG-INFO` & `raw-telegram-api-1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raw-telegram-api
-Version: 1.1
+Version: 1.2
 Summary: Raw Telegram API
 Author: mishpro
 Author-email: mishpro <root@venusbiser.ru>
 Project-URL: Homepage, https://github.com/mishpro-programm/raw-telegram-api
 Project-URL: Bug Tracker, https://github.com/mishpro-programm/raw-telegram-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `raw-telegram-api-1.1/pyproject.toml` & `raw-telegram-api-1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raw-telegram-api"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="mishpro", email="root@venusbiser.ru" },
 ]
 description = "Raw Telegram API"
 readme = "README.md"
 requires-python = ">3"
+dependencies = ["requests>=2.30.0"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `raw-telegram-api-1.1/raw_telegram_api.egg-info/PKG-INFO` & `raw-telegram-api-1.2/raw_telegram_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raw-telegram-api
-Version: 1.1
+Version: 1.2
 Summary: Raw Telegram API
 Author: mishpro
 Author-email: mishpro <root@venusbiser.ru>
 Project-URL: Homepage, https://github.com/mishpro-programm/raw-telegram-api
 Project-URL: Bug Tracker, https://github.com/mishpro-programm/raw-telegram-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

