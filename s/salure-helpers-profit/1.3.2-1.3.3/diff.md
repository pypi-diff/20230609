# Comparing `tmp/salure_helpers_profit-1.3.2.tar.gz` & `tmp/salure_helpers_profit-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-1.3.2.tar", last modified: Tue Jun  6 16:24:49 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-1.3.3.tar", last modified: Fri Jun  9 07:21:58 2023, max compression
```

## Comparing `salure_helpers_profit-1.3.2.tar` & `salure_helpers_profit-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-06 16:24:28.000000 salure_helpers_profit-1.3.2/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-06-06 16:24:28.000000 salure_helpers_profit-1.3.2/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-06-06 16:24:28.000000 salure_helpers_profit-1.3.2/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-06-06 16:24:28.000000 salure_helpers_profit-1.3.2/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   133377 2023-06-06 16:24:28.000000 salure_helpers_profit-1.3.2/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 16:24:49.000000 salure_helpers_profit-1.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-06 16:24:28.000000 salure_helpers_profit-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-09 07:21:43.000000 salure_helpers_profit-1.3.3/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-06-09 07:21:43.000000 salure_helpers_profit-1.3.3/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-06-09 07:21:43.000000 salure_helpers_profit-1.3.3/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-06-09 07:21:43.000000 salure_helpers_profit-1.3.3/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   133788 2023-06-09 07:21:43.000000 salure_helpers_profit-1.3.3/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 07:21:58.000000 salure_helpers_profit-1.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-09 07:21:43.000000 salure_helpers_profit-1.3.3/setup.py
```

### Comparing `salure_helpers_profit-1.3.2/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-1.3.3/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.2/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-1.3.3/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.2/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-1.3.3/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.2/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-1.3.3/salure_helpers/profit/profit_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     def update_creditor(self,method: str, data: dict, overload_fields: dict = None) -> requests.Response:
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: The custom fields in this dataset. Give the key of the field and the value. For example: {DFEDS8-DSF9uD-DDSA: 'Vrij veld'}
         :param method: request type
         :return: status code for request and optional error message
         """
-        allowed_fields = ['person_id', 'internal_id', 'match_person_on', 'log_birthname_seperately', 'collective_account', 'preferred_delivery_method']
+        allowed_fields = ['person_id', 'internal_id', 'match_person_on', 'log_birthname_seperately', 'collective_account', 'preferred_delivery_method', 'automatic_payment', 'compact', 'payment_specification']
         required_fields = ['creditor_id']
 
         if method != 'PUT' and method != 'POST' and method != 'DELETE':
             raise ValueError('Parameter method should be PUT, POST or DELETE (in uppercase)')
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
@@ -316,15 +316,15 @@
 
         base_body = {
             "KnPurchaseRelationPer": {
                 "Element": {
                     "@CrId": data['creditor_id'],
                     "Fields": {
                         "CuId": "EUR",
-                        "isCr": True
+                        "IsCr": True
                     },
                     "Objects": {
                         "KnPerson": {
                             "Element": {
                                 "Fields": {
                                     "MatchPer": "0" if "match_person_on" not in data else data['match_person_on'],
                                 },
@@ -338,14 +338,17 @@
         }
 
         # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update = {}
         fields_to_update.update({"PaCd": data['payment_condition']}) if 'person_id' in data else fields_to_update
         fields_to_update.update({"ColA": data['collective_account']}) if 'collective_account' in data else fields_to_update
         fields_to_update.update({"InPv": data['preferred_delivery_method']}) if 'preferred_delivery_method' in data else fields_to_update
+        fields_to_update.update({"AuPa": data['automatic_payment']}) if 'automatic_payment' in data else fields_to_update
+        fields_to_update.update({"PaCo": data['compact']}) if 'compact' in data else fields_to_update
+        fields_to_update.update({"PaSp": data['payment_specification']}) if 'payment_specification' in data else fields_to_update
 
         base_body['KnPurchaseRelationPer']['Element']['Fields'].update(fields_to_update)
 
         # Update the request body with update fields
         fields_to_update = {}
         fields_to_update.update({"BcId": data['internal_id']}) if 'internal_id' in data else fields_to_update
         fields_to_update.update({"BcCo": data['person_id']}) if 'person_id' in data else fields_to_update
```

### Comparing `salure_helpers_profit-1.3.2/setup.py` & `salure_helpers_profit-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='1.3.2',
+    version='1.3.3',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

