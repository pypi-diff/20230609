# Comparing `tmp/vnpy_xex-2023.6.9.3.tar.gz` & `tmp/vnpy_xex-2023.6.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.6.9.3.tar", last modified: Fri Jun  9 08:46:16 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.9.4.tar", last modified: Fri Jun  9 10:29:59 2023, max compression
```

## Comparing `vnpy_xex-2023.6.9.3.tar` & `vnpy_xex-2023.6.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:46:16.427956 vnpy_xex-2023.6.9.3/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.3/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:46:16.428160 vnpy_xex-2023.6.9.3/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.3/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 08:46:16.429616 vnpy_xex-2023.6.9.3/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.3/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:46:16.421006 vnpy_xex-2023.6.9.3/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.3/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25599 2023-06-09 08:44:29.000000 vnpy_xex-2023.6.9.3/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:46:16.427560 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 10:29:59.259737 vnpy_xex-2023.6.9.4/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.4/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 10:29:59.259834 vnpy_xex-2023.6.9.4/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.4/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 10:29:59.260309 vnpy_xex-2023.6.9.4/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.4/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 10:29:59.256852 vnpy_xex-2023.6.9.4/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.4/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25223 2023-06-09 10:29:02.000000 vnpy_xex-2023.6.9.4/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 10:29:59.259541 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 10:29:59.000000 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 10:29:59.000000 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 10:29:59.000000 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 10:29:59.000000 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 10:29:59.000000 vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.6.9.3/LICENSE` & `vnpy_xex-2023.6.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.9.3/PKG-INFO` & `vnpy_xex-2023.6.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.6.9.3
+Version: 2023.6.9.4
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.6.9.3/setup.cfg` & `vnpy_xex-2023.6.9.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.6.9.3
+version = 2023.6.9.4
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.6.9.3/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.9.4/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.9.3/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.9.4/vnpy_xex/xex_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,16 +475,15 @@
                     symbol_contract_map[contract.symbol] = contract
 
             self.gateway.write_log("合约信息查询成功")
             self.query_order()
 
     def on_send_order(self, data: dict, request: Request) -> None:
         """委托下单回报"""
-        logger.debug(
-            f"on_send_order data={beeprint.pp(data, output=False, sort_keys=False)} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
+        pass
 
     def on_send_order_failed(self, status_code: str, request: Request) -> None:
         """委托下单失败服务器报错回报"""
         logger.debug(
             f"on_send_order_failed {status_code=} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
 
         order: OrderData = request.extra
@@ -506,16 +505,15 @@
         self.gateway.on_order(order)
 
         if not issubclass(exception_type, (ConnectionError, SSLError)):
             self.on_error(exception_type, exception_value, tb, request)
 
     def on_cancel_order(self, data: dict, request: Request) -> None:
         """委托撤单回报"""
-        logger.debug(
-            f"on_cancel_order data={beeprint.pp(data, output=False, sort_keys=False)} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
+        pass
 
     def on_cancel_failed(self, status_code: str, request: Request) -> None:
         """撤单回报函数报错回报"""
         logger.debug(
             f"on_cancel_failed {status_code=} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
 
         if request.extra:
```

### Comparing `vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.9.4/vnpy_xex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.6.9.3
+Version: 2023.6.9.4
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

