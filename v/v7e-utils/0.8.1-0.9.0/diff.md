# Comparing `tmp/v7e_utils-0.8.1.tar.gz` & `tmp/v7e_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v7e_utils-0.8.1.tar", max compression
+gzip compressed data, was "v7e_utils-0.9.0.tar", max compression
```

## Comparing `v7e_utils-0.8.1.tar` & `v7e_utils-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      457 2023-06-01 16:49:48.346892 v7e_utils-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/agil_connect/__init__.py
--rw-r--r--   0        0        0     1207 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/agil_connect/agil_connect.py
--rw-r--r--   0        0        0     3103 2023-05-30 19:44:01.777170 v7e_utils-0.8.1/v7e_utils/agil_connect/panel_connect.py
--rw-r--r--   0        0        0     2544 2023-06-01 16:49:41.214573 v7e_utils-0.8.1/v7e_utils/agil_connect/rh_connect.py
--rw-r--r--   0        0        0       67 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/data_helper/__init__.py
--rw-r--r--   0        0        0    10801 2023-05-02 18:30:45.747778 v7e_utils-0.8.1/v7e_utils/data_helper/data_helper.py
--rw-r--r--   0        0        0      813 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/data_helper/error.py
--rw-r--r--   0        0        0     1015 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/data_helper/record_batch.py
--rw-r--r--   0        0        0     3081 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/data_utils.py
--rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/dataframe_helper/__init__.py
--rw-r--r--   0        0        0     6891 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/dataframe_helper/df_helper.py
--rw-r--r--   0        0        0     5854 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/dataframe_helper/io.py
--rw-r--r--   0        0        0     3053 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/dataframe_helper/utils.py
--rw-r--r--   0        0        0     7836 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/date_utils.py
--rw-r--r--   0        0        0     3676 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/file_utils.py
--rw-r--r--   0        0        0      577 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/model_utils.py
--rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/report_factory/__init__.py
--rw-r--r--   0        0        0      815 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/report_factory/factory.py
--rw-r--r--   0        0        0      494 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/report_factory/loader.py
--rw-r--r--   0        0        0     4217 2023-05-02 18:30:45.747778 v7e_utils-0.8.1/v7e_utils/report_factory/publisher.py
--rw-r--r--   0        0        0     1245 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/report_factory/report_helper.py
--rw-r--r--   0        0        0      508 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/report_factory/reporter.py
--rw-r--r--   0        0        0      387 2023-04-26 20:54:37.830739 v7e_utils-0.8.1/v7e_utils/report_factory/runner.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 v7e_utils-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-06-09 17:32:41.062608 v7e_utils-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/agil_connect/__init__.py
+-rw-r--r--   0        0        0     1207 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/agil_connect/agil_connect.py
+-rw-r--r--   0        0        0     3445 2023-06-09 17:30:53.181792 v7e_utils-0.9.0/v7e_utils/agil_connect/panel_connect.py
+-rw-r--r--   0        0        0     2544 2023-06-01 16:49:41.214573 v7e_utils-0.9.0/v7e_utils/agil_connect/rh_connect.py
+-rw-r--r--   0        0        0       67 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/data_helper/__init__.py
+-rw-r--r--   0        0        0    10801 2023-05-02 18:30:45.747778 v7e_utils-0.9.0/v7e_utils/data_helper/data_helper.py
+-rw-r--r--   0        0        0      813 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/data_helper/error.py
+-rw-r--r--   0        0        0     1015 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/data_helper/record_batch.py
+-rw-r--r--   0        0        0     3081 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/data_utils.py
+-rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/dataframe_helper/__init__.py
+-rw-r--r--   0        0        0     6891 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/dataframe_helper/df_helper.py
+-rw-r--r--   0        0        0     5854 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/dataframe_helper/io.py
+-rw-r--r--   0        0        0     3053 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/dataframe_helper/utils.py
+-rw-r--r--   0        0        0     7836 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/date_utils.py
+-rw-r--r--   0        0        0     3676 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/file_utils.py
+-rw-r--r--   0        0        0      577 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/model_utils.py
+-rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/report_factory/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/report_factory/factory.py
+-rw-r--r--   0        0        0      494 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/report_factory/loader.py
+-rw-r--r--   0        0        0     4217 2023-05-02 18:30:45.747778 v7e_utils-0.9.0/v7e_utils/report_factory/publisher.py
+-rw-r--r--   0        0        0     1245 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/report_factory/report_helper.py
+-rw-r--r--   0        0        0      508 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/report_factory/reporter.py
+-rw-r--r--   0        0        0      387 2023-04-26 20:54:37.830739 v7e_utils-0.9.0/v7e_utils/report_factory/runner.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 v7e_utils-0.9.0/PKG-INFO
```

### Comparing `v7e_utils-0.8.1/v7e_utils/agil_connect/agil_connect.py` & `v7e_utils-0.9.0/v7e_utils/agil_connect/agil_connect.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/agil_connect/panel_connect.py` & `v7e_utils-0.9.0/v7e_utils/agil_connect/panel_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,8 +92,17 @@
 class PanelBusinessUnits(AgilConnection):
     def __init__(self, url=None):
         super().__init__(url)
         self.set_api_endpoint('panel/business-units/')
 
     def get_panel_business_units(self, realm):
         url = self.ensure_url(self.gateway_url, self.api_endpoint)
+        return self.get_result(url, realm)
+    
+class PanelLegalRepresentative(AgilConnection):
+    def __init__(self, url=None):
+        super().__init__(url)
+        self.set_api_endpoint('panel/legal-representative/')
+
+    def get_panel_legal_representative(self, realm):
+        url = self.ensure_url(self.gateway_url, self.api_endpoint)
         return self.get_result(url, realm)
```

### Comparing `v7e_utils-0.8.1/v7e_utils/agil_connect/rh_connect.py` & `v7e_utils-0.9.0/v7e_utils/agil_connect/rh_connect.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/data_helper/data_helper.py` & `v7e_utils-0.9.0/v7e_utils/data_helper/data_helper.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/data_helper/error.py` & `v7e_utils-0.9.0/v7e_utils/data_helper/error.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/data_helper/record_batch.py` & `v7e_utils-0.9.0/v7e_utils/data_helper/record_batch.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/data_utils.py` & `v7e_utils-0.9.0/v7e_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/dataframe_helper/df_helper.py` & `v7e_utils-0.9.0/v7e_utils/dataframe_helper/df_helper.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/dataframe_helper/io.py` & `v7e_utils-0.9.0/v7e_utils/dataframe_helper/io.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/dataframe_helper/utils.py` & `v7e_utils-0.9.0/v7e_utils/dataframe_helper/utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/date_utils.py` & `v7e_utils-0.9.0/v7e_utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/file_utils.py` & `v7e_utils-0.9.0/v7e_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/model_utils.py` & `v7e_utils-0.9.0/v7e_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/report_factory/factory.py` & `v7e_utils-0.9.0/v7e_utils/report_factory/factory.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/report_factory/publisher.py` & `v7e_utils-0.9.0/v7e_utils/report_factory/publisher.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/v7e_utils/report_factory/report_helper.py` & `v7e_utils-0.9.0/v7e_utils/report_factory/report_helper.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.8.1/PKG-INFO` & `v7e_utils-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v7e-utils
-Version: 0.8.1
+Version: 0.9.0
 Summary: A collection of utility functions for V6E projects
 License: MIT
 Author: Luis Valverde
 Author-email: lvalverde@istmocenter.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

