# Comparing `tmp/vnpy_xex-2023.6.9.2.tar.gz` & `tmp/vnpy_xex-2023.6.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.6.9.2.tar", last modified: Fri Jun  9 08:34:58 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.9.3.tar", last modified: Fri Jun  9 08:46:16 2023, max compression
```

## Comparing `vnpy_xex-2023.6.9.2.tar` & `vnpy_xex-2023.6.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:34:58.225178 vnpy_xex-2023.6.9.2/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.2/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:34:58.225289 vnpy_xex-2023.6.9.2/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.2/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 08:34:58.225778 vnpy_xex-2023.6.9.2/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.2/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:34:58.222169 vnpy_xex-2023.6.9.2/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.2/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25100 2023-06-09 08:32:32.000000 vnpy_xex-2023.6.9.2/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:34:58.224976 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:46:16.427956 vnpy_xex-2023.6.9.3/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.3/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:46:16.428160 vnpy_xex-2023.6.9.3/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.3/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 08:46:16.429616 vnpy_xex-2023.6.9.3/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.3/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:46:16.421006 vnpy_xex-2023.6.9.3/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.3/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25599 2023-06-09 08:44:29.000000 vnpy_xex-2023.6.9.3/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:46:16.427560 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 08:46:16.000000 vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.6.9.2/LICENSE` & `vnpy_xex-2023.6.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.9.2/PKG-INFO` & `vnpy_xex-2023.6.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.6.9.2
+Version: 2023.6.9.3
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.6.9.2/setup.cfg` & `vnpy_xex-2023.6.9.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.6.9.2
+version = 2023.6.9.3
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.6.9.2/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.9.3/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.9.2/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.9.3/vnpy_xex/xex_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,14 +404,15 @@
         self.add_request(
             method="POST",
             path="v1/trade/order/batchOrder",
             callback=self.on_cancel_order,
             params=params,
             data=data,
             on_failed=self.on_cancel_failed,
+            on_error=self.on_cancel_error,
             extra=order
         )
 
     def start_user_stream(self):
         """开启账户信息推送"""
         self.trade_ws_api.connect(WEBSOCKET_TRADE_HOST, self.proxy_host, self.proxy_port)
 
@@ -521,14 +522,23 @@
             order = request.extra
             order.status = Status.REJECTED
             self.gateway.on_order(order)
 
         msg = f"撤单失败，状态码：{status_code}，信息：{request.response.text}"
         self.gateway.write_log(msg)
 
+    def on_cancel_error(
+            self, exception_type: type, exception_value: Exception, tb, request: Request
+    ):
+        logger.debug(
+            f"on_cancel_error {exception_type=} {exception_value=} {tb=} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
+
+        if not issubclass(exception_type, (ConnectionError, SSLError)):
+            self.on_error(exception_type, exception_value, tb, request)
+
     def on_keep_user_stream(self, data: dict, request: Request) -> None:
         """延长listenKey有效期回报"""
         pass
 
     def on_keep_user_stream_error(
             self, exception_type: type, exception_value: Exception, tb, request: Request
     ) -> None:
```

### Comparing `vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.9.3/vnpy_xex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.6.9.2
+Version: 2023.6.9.3
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

