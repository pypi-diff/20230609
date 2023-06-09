# Comparing `tmp/uat-breeze-connect-1.0.14rc8.tar.gz` & `tmp/uat-breeze-connect-1.0.14rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uat-breeze-connect-1.0.14rc8.tar", last modified: Tue Aug 16 05:03:46 2022, max compression
+gzip compressed data, was "uat-breeze-connect-1.0.14rc9.tar", last modified: Mon Aug 22 12:30:39 2022, max compression
```

## Comparing `uat-breeze-connect-1.0.14rc8.tar` & `uat-breeze-connect-1.0.14rc9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-08-16 05:03:46.081105 uat-breeze-connect-1.0.14rc8/
--rw-rw-rw-   0        0        0     1100 2022-08-09 05:48:54.000000 uat-breeze-connect-1.0.14rc8/LICENSE
--rw-rw-rw-   0        0        0    12220 2022-08-16 05:03:46.079871 uat-breeze-connect-1.0.14rc8/PKG-INFO
--rw-rw-rw-   0        0        0    11430 2022-08-16 04:42:38.000000 uat-breeze-connect-1.0.14rc8/README.md
-drwxrwxrwx   0        0        0        0 2022-08-16 05:03:46.065073 uat-breeze-connect-1.0.14rc8/breeze_connect/
--rw-rw-rw-   0        0        0       55 2022-08-09 05:48:54.000000 uat-breeze-connect-1.0.14rc8/breeze_connect/__init__.py
--rw-rw-rw-   0        0        0    70748 2022-08-16 04:43:24.000000 uat-breeze-connect-1.0.14rc8/breeze_connect/breeze_connect.py
--rw-rw-rw-   0        0        0       42 2022-08-16 05:03:46.081105 uat-breeze-connect-1.0.14rc8/setup.cfg
--rw-rw-rw-   0        0        0      725 2022-08-16 04:42:46.000000 uat-breeze-connect-1.0.14rc8/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-16 05:03:46.077363 uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/
--rw-rw-rw-   0        0        0    12220 2022-08-16 05:03:45.000000 uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2022-08-16 05:03:45.000000 uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-16 05:03:45.000000 uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-08-16 05:03:45.000000 uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-08-16 05:03:45.000000 uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-22 12:30:39.463611 uat-breeze-connect-1.0.14rc9/
+-rw-rw-rw-   0        0        0     1100 2022-08-09 05:48:54.000000 uat-breeze-connect-1.0.14rc9/LICENSE
+-rw-rw-rw-   0        0        0    12220 2022-08-22 12:30:39.463110 uat-breeze-connect-1.0.14rc9/PKG-INFO
+-rw-rw-rw-   0        0        0    11430 2022-08-16 04:42:38.000000 uat-breeze-connect-1.0.14rc9/README.md
+drwxrwxrwx   0        0        0        0 2022-08-22 12:30:39.450275 uat-breeze-connect-1.0.14rc9/breeze_connect/
+-rw-rw-rw-   0        0        0       55 2022-08-09 05:48:54.000000 uat-breeze-connect-1.0.14rc9/breeze_connect/__init__.py
+-rw-rw-rw-   0        0        0    70849 2022-08-22 12:26:16.000000 uat-breeze-connect-1.0.14rc9/breeze_connect/breeze_connect.py
+-rw-rw-rw-   0        0        0       42 2022-08-22 12:30:39.464474 uat-breeze-connect-1.0.14rc9/setup.cfg
+-rw-rw-rw-   0        0        0      725 2022-08-22 12:28:26.000000 uat-breeze-connect-1.0.14rc9/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-22 12:30:39.460933 uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/
+-rw-rw-rw-   0        0        0    12220 2022-08-22 12:30:39.000000 uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2022-08-22 12:30:39.000000 uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-22 12:30:39.000000 uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2022-08-22 12:30:39.000000 uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2022-08-22 12:30:39.000000 uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/top_level.txt
```

### Comparing `uat-breeze-connect-1.0.14rc8/LICENSE` & `uat-breeze-connect-1.0.14rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `uat-breeze-connect-1.0.14rc8/PKG-INFO` & `uat-breeze-connect-1.0.14rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc8
+Version: 1.0.14rc9
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `uat-breeze-connect-1.0.14rc8/README.md` & `uat-breeze-connect-1.0.14rc9/README.md`

 * *Files identical despite different names*

### Comparing `uat-breeze-connect-1.0.14rc8/breeze_connect/breeze_connect.py` & `uat-breeze-connect-1.0.14rc9/breeze_connect/breeze_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,18 +582,18 @@
         if self.api_handler:
             return self.api_handler.get_portfolio_positions()
 
     def get_quotes(self, stock_code="", exchange_code="", expiry_date="", product_type="", right="", strike_price=""):
         if self.api_handler:
             return self.api_handler.get_quotes(stock_code, exchange_code, expiry_date, product_type, right, strike_price)
 
-    def get_option_chain_quotes(self):
+    def get_option_chain_quotes(self, stock_code="", exchange_code="", expiry_date="", product_type="", right="", strike_price=""):
         if(self.api_handler):
             return self.api_handler.get_option_chain_quotes(stock_code, exchange_code, expiry_date, product_type, right, strike_price)
-
+        
     def square_off(self, source_flag="", stock_code="", exchange_code="", quantity="", price="", action="", order_type="", validity="", stoploss="", disclosed_quantity="", protection_percentage="", settlement_id="", margin_amount="", open_quantity="", cover_quantity="", product_type="", expiry_date="", right="", strike_price="", validity_date="", trade_password="", alias_name=""):
         if self.api_handler:
             return self.api_handler.square_off(source_flag, stock_code, exchange_code, quantity, price, action, order_type, validity, stoploss, disclosed_quantity, protection_percentage, settlement_id, margin_amount, open_quantity, cover_quantity, product_type, expiry_date, right, strike_price, validity_date, trade_password, alias_name)
 
     def get_trade_list(self, from_date="", to_date="", exchange_code="", product_type="", action="", stock_code=""):
         if self.api_handler:
             return self.api_handler.get_trade_list(from_date, to_date, exchange_code, product_type, action, stock_code)
```

### Comparing `uat-breeze-connect-1.0.14rc8/setup.py` & `uat-breeze-connect-1.0.14rc9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uat-breeze-connect",
-    version="1.0.14rc8",
+    version="1.0.14rc9",
     author="UAT Breeze Connect",
     author_email="test@mail.com",
     description="UAT Breeze Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['python-socketio[client]','requests'],
     url="https://github.com/pypa/sampleproject",
```

### Comparing `uat-breeze-connect-1.0.14rc8/uat_breeze_connect.egg-info/PKG-INFO` & `uat-breeze-connect-1.0.14rc9/uat_breeze_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc8
+Version: 1.0.14rc9
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

