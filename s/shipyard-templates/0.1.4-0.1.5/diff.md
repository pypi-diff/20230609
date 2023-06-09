# Comparing `tmp/shipyard_templates-0.1.4.tar.gz` & `tmp/shipyard_templates-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.1.4.tar", max compression
+gzip compressed data, was "shipyard_templates-0.1.5.tar", max compression
```

## Comparing `shipyard_templates-0.1.4.tar` & `shipyard_templates-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.1.4/README.md
--rw-r--r--   0        0        0      342 2023-05-23 14:13:44.147230 shipyard_templates-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      358 2023-05-16 19:54:06.644392 shipyard_templates-0.1.4/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      552 2023-05-12 18:48:21.819618 shipyard_templates-0.1.4/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0     1965 2023-05-12 18:48:21.819681 shipyard_templates-0.1.4/shipyard_templates/database.py
--rw-r--r--   0        0        0      267 2023-05-12 18:48:21.819750 shipyard_templates-0.1.4/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:48:21.819815 shipyard_templates-0.1.4/shipyard_templates/etl.py
--rw-r--r--   0        0        0      245 2023-05-12 18:48:21.819876 shipyard_templates-0.1.4/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      235 2023-05-12 18:48:21.819939 shipyard_templates-0.1.4/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      753 2023-05-23 14:13:00.186819 shipyard_templates-0.1.4/shipyard_templates/projectmanagement.py
--rw-r--r--   0        0        0      543 2023-05-23 01:46:27.306492 shipyard_templates-0.1.4/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      280 2023-05-12 18:48:21.820063 shipyard_templates-0.1.4/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.1.5/README.md
+-rw-r--r--   0        0        0      342 2023-06-06 18:57:29.879970 shipyard_templates-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      373 2023-06-06 18:57:29.880703 shipyard_templates-0.1.5/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-12 18:48:21.819618 shipyard_templates-0.1.5/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0     1965 2023-05-12 18:48:21.819681 shipyard_templates-0.1.5/shipyard_templates/database.py
+-rw-r--r--   0        0        0      267 2023-05-12 18:48:21.819750 shipyard_templates-0.1.5/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:48:21.819815 shipyard_templates-0.1.5/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      245 2023-05-12 18:48:21.819876 shipyard_templates-0.1.5/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      235 2023-05-12 18:48:21.819939 shipyard_templates-0.1.5/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      993 2023-06-06 18:57:29.881235 shipyard_templates-0.1.5/shipyard_templates/projectmanagement.py
+-rw-r--r--   0        0        0      543 2023-05-23 01:46:27.306492 shipyard_templates-0.1.5/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      280 2023-05-12 18:48:21.820063 shipyard_templates-0.1.5/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.5/PKG-INFO
```

### Comparing `shipyard_templates-0.1.4/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.1.5/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.4/shipyard_templates/database.py` & `shipyard_templates-0.1.5/shipyard_templates/database.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.4/shipyard_templates/etl.py` & `shipyard_templates-0.1.5/shipyard_templates/etl.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.4/shipyard_templates/projectmanagement.py` & `shipyard_templates-0.1.5/shipyard_templates/projectmanagement.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from abc import ABC, abstractmethod
 from .shipyard_logger import ShipyardLogger
 
 
+class ExitCodeError(Exception):
+    def __init__(self, message, exit_code):
+        super().__init__(message)
+        self.message = message
+        self.exit_code = exit_code
+
+
 class ProjectManagement(ABC):
     # Class level exit codes
     # general exit codes
     EXIT_CODE_INVALID_CREDENTIALS = 200
     EXIT_CODE_BAD_REQUEST = 201
+    EXIT_CODE_TICKET_NOT_FOUND = 202
+    EXIT_CODE_INVALID_ISSUE_TYPE = 203
+    EXIT_CODE_INVALID_STATUS = 204
     EXIT_CODE_UNKNOWN_ERROR = 299
 
-    # API TIMEOUT
-    EXIT_CODE_API_TIMEOUT = 30
     def __init__(self, access_token: str, **kwargs) -> None:
         self.logger = ShipyardLogger().logger
         self.access_token = access_token
 
     @abstractmethod
     def create_ticket(self, **kwargs):
         pass
```

### Comparing `shipyard_templates-0.1.4/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.1.5/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.4/PKG-INFO` & `shipyard_templates-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-templates
-Version: 0.1.4
+Version: 0.1.5
 Summary: Super classes for blueprint development
 License: Apache-2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

