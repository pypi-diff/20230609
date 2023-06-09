# Comparing `tmp/bigc-0.2.8.tar.gz` & `tmp/bigc-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigc-0.2.8.tar", max compression
+gzip compressed data, was "bigc-0.2.9.tar", max compression
```

## Comparing `bigc-0.2.8.tar` & `bigc-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-05-08 18:38:58.364096 bigc-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0     1596 2023-05-08 18:38:58.364096 bigc-0.2.8/README.md
--rw-r--r--   0        0        0       32 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/api.py
--rw-r--r--   0        0        0     6458 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/api_client.py
--rw-r--r--   0        0        0       49 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/data/__init__.py
--rw-r--r--   0        0        0      482 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/data/order_status.py
--rw-r--r--   0        0        0     1639 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/exceptions.py
--rw-r--r--   0        0        0      431 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/__init__.py
--rw-r--r--   0        0        0     1741 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/carts.py
--rw-r--r--   0        0        0     1180 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/categories.py
--rw-r--r--   0        0        0     4116 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/checkouts.py
--rw-r--r--   0        0        0     1178 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/customer_groups.py
--rw-r--r--   0        0        0     4346 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/customers.py
--rw-r--r--   0        0        0     4504 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/orders.py
--rw-r--r--   0        0        0     1414 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/product_variants.py
--rw-r--r--   0        0        0     2682 2023-05-08 18:38:58.368097 bigc-0.2.8/bigc/resources/products.py
--rw-r--r--   0        0        0     1205 2023-05-08 18:38:58.368097 bigc-0.2.8/bigc/resources/webhooks.py
--rw-r--r--   0        0        0      557 2023-05-08 18:38:58.368097 bigc-0.2.8/bigc/utils.py
--rw-r--r--   0        0        0      770 2023-05-08 18:38:58.368097 bigc-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-24 15:24:15.119393 bigc-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0     1596 2023-05-24 15:24:15.119393 bigc-0.2.9/README.md
+-rw-r--r--   0        0        0       32 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/api.py
+-rw-r--r--   0        0        0     6867 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/api_client.py
+-rw-r--r--   0        0        0       49 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/data/__init__.py
+-rw-r--r--   0        0        0      482 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/data/order_status.py
+-rw-r--r--   0        0        0     2402 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/exceptions.py
+-rw-r--r--   0        0        0      431 2023-05-24 15:24:15.119393 bigc-0.2.9/bigc/resources/__init__.py
+-rw-r--r--   0        0        0     1741 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/carts.py
+-rw-r--r--   0        0        0     1180 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/categories.py
+-rw-r--r--   0        0        0     4116 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/checkouts.py
+-rw-r--r--   0        0        0     1178 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/customer_groups.py
+-rw-r--r--   0        0        0     4346 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/customers.py
+-rw-r--r--   0        0        0     4701 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/orders.py
+-rw-r--r--   0        0        0     1414 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/product_variants.py
+-rw-r--r--   0        0        0     2682 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/products.py
+-rw-r--r--   0        0        0     1205 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/resources/webhooks.py
+-rw-r--r--   0        0        0      557 2023-05-24 15:24:15.123393 bigc-0.2.9/bigc/utils.py
+-rw-r--r--   0        0        0      770 2023-05-24 15:24:15.123393 bigc-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.9/PKG-INFO
```

### Comparing `bigc-0.2.8/LICENSE.txt` & `bigc-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/README.md` & `bigc-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/api.py` & `bigc-0.2.9/bigc/api.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/carts.py` & `bigc-0.2.9/bigc/resources/carts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/categories.py` & `bigc-0.2.9/bigc/resources/categories.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/checkouts.py` & `bigc-0.2.9/bigc/resources/checkouts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/customer_groups.py` & `bigc-0.2.9/bigc/resources/customer_groups.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/customers.py` & `bigc-0.2.9/bigc/resources/customers.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/orders.py` & `bigc-0.2.9/bigc/resources/orders.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         payload = {
             "items": items,
             "payments": payments,
             **kwargs,
         }
         return self._api.v3.post(f'/orders/{order_id}/payment_actions/refunds', json=payload)
 
-    def all_refunds(self, order_id: Optional[int]) -> Iterator[dict]:
+    def all_refunds(self, order_id: Optional[int] = None) -> Iterator[dict]:
         """Return an iterator for all refunds, optionally filtered by order"""
         if order_id:
             endpoint = f'/orders/{order_id}/payment_actions/refunds'
         else:
             endpoint = '/orders/payment_actions/refunds'
         return self._api.v3.get_many(endpoint)
 
@@ -105,7 +105,11 @@
         payload = {
             'order_address_id': order_address_id,
             'items': items,
             **kwargs,
         }
 
         return self._api.v2.post(f'/orders/{order_id}/shipments', json=payload)
+
+    def all_coupons(self, order_id: int) -> Iterator[dict]:
+        """Return an iterator for all coupons in an order"""
+        return self._api.v2.get_many(f'/orders/{order_id}/coupons')
```

### Comparing `bigc-0.2.8/bigc/resources/product_variants.py` & `bigc-0.2.9/bigc/resources/product_variants.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/products.py` & `bigc-0.2.9/bigc/resources/products.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/resources/webhooks.py` & `bigc-0.2.9/bigc/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/bigc/utils.py` & `bigc-0.2.9/bigc/utils.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.8/pyproject.toml` & `bigc-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigc"
-version = "0.2.8"
+version = "0.2.9"
 description = "Unofficial client for the BigCommerce API"
 license = "MIT"
 authors = ["Ryan Thomson <ryan@medshift.com>", "Dillon Hartley <dillon@medshift.com>", "Adam Walsh <adam@medshift.com>"]
 readme = "README.md"
 homepage = "https://github.com/MedShift/bigc"
 repository = "https://github.com/MedShift/bigc.git"
 keywords = ["bigcommerce", "api", "client"]
```

### Comparing `bigc-0.2.8/PKG-INFO` & `bigc-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigc
-Version: 0.2.8
+Version: 0.2.9
 Summary: Unofficial client for the BigCommerce API
 Home-page: https://github.com/MedShift/bigc
 License: MIT
 Keywords: bigcommerce,api,client
 Author: Ryan Thomson
 Author-email: ryan@medshift.com
 Requires-Python: >=3.9,<4.0
```

