# Comparing `tmp/vnpy_xex-2023.6.8.1.tar.gz` & `tmp/vnpy_xex-2023.6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.6.8.1.tar", last modified: Thu Jun  8 07:00:53 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.9.1.tar", last modified: Fri Jun  9 07:51:23 2023, max compression
```

## Comparing `vnpy_xex-2023.6.8.1.tar` & `vnpy_xex-2023.6.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-08 07:00:53.989498 vnpy_xex-2023.6.8.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.8.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-08 07:00:53.989599 vnpy_xex-2023.6.8.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.8.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-08 07:00:53.990116 vnpy_xex-2023.6.8.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.8.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-08 07:00:53.987252 vnpy_xex-2023.6.8.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.8.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    24678 2023-06-08 06:56:06.000000 vnpy_xex-2023.6.8.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-08 07:00:53.989300 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-08 07:00:53.000000 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-08 07:00:53.000000 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-08 07:00:53.000000 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-08 07:00:53.000000 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-08 07:00:53.000000 vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 07:51:23.587828 vnpy_xex-2023.6.9.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 07:51:23.587957 vnpy_xex-2023.6.9.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 07:51:23.588617 vnpy_xex-2023.6.9.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 07:51:23.584049 vnpy_xex-2023.6.9.1/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.1/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    24748 2023-06-09 07:49:55.000000 vnpy_xex-2023.6.9.1/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 07:51:23.587482 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.6.8.1/LICENSE` & `vnpy_xex-2023.6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.8.1/PKG-INFO` & `vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vnpy_xex
-Version: 2023.6.8.1
+Name: vnpy-xex
+Version: 2023.6.9.1
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.6.8.1/setup.cfg` & `vnpy_xex-2023.6.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.6.8.1
+version = 2023.6.9.1
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.6.8.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.9.1/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.8.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.9.1/vnpy_xex/xex_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,28 +339,30 @@
             return self.order_count
 
     def send_order(self, *reqs: OrderRequest) -> str:
         """委托下单 批量下单"""
         vt_orderids = []  # 单号
         order_params = []  # 下单参数
         for req in reqs:
+            req.price = round_to(req.price, symbol_contract_map[req.symbol].pricetick)
+            req.volume = round_to(req.volume, symbol_contract_map[req.symbol].min_volume)
             # 生成本地委托号
             orderid: str = str(self.connect_time + self._new_order_id())
 
             # 推送提交中事件
             order: OrderData = req.create_order_data(
                 orderid,
                 self.gateway_name
             )
             order.datetime = datetime.now(CHINA_TZ)
             self.gateway.on_order(order)
             order_params.append({"isCreate": True,
                                  "symbol": req.symbol,
-                                 "price": round_to(req.price, symbol_contract_map[req.symbol].pricetick),
-                                 "totalAmount": round_to(req.volume, symbol_contract_map[req.symbol].min_volume),
+                                 "price": req.price,
+                                 "totalAmount": req.volume,
                                  "tradeType": ORDERTYPE_VT2XEX[req.type],
                                  "direction": DIRECTION_VT2XEX[req.direction],
                                  "clientOrderId": orderid})
             vt_orderids.append(order.vt_orderid)
         # 批量下单请求
         data: dict = {
             "security": Security.SIGNED
```

### Comparing `vnpy_xex-2023.6.8.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vnpy-xex
-Version: 2023.6.8.1
+Name: vnpy_xex
+Version: 2023.6.9.1
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

