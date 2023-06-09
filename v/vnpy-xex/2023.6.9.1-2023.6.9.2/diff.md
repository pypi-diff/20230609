# Comparing `tmp/vnpy_xex-2023.6.9.1.tar.gz` & `tmp/vnpy_xex-2023.6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.6.9.1.tar", last modified: Fri Jun  9 07:51:23 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.9.2.tar", last modified: Fri Jun  9 08:34:58 2023, max compression
```

## Comparing `vnpy_xex-2023.6.9.1.tar` & `vnpy_xex-2023.6.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 07:51:23.587828 vnpy_xex-2023.6.9.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 07:51:23.587957 vnpy_xex-2023.6.9.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 07:51:23.588617 vnpy_xex-2023.6.9.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 07:51:23.584049 vnpy_xex-2023.6.9.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    24748 2023-06-09 07:49:55.000000 vnpy_xex-2023.6.9.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 07:51:23.587482 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 07:51:23.000000 vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:34:58.225178 vnpy_xex-2023.6.9.2/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.2/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:34:58.225289 vnpy_xex-2023.6.9.2/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.9.2/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-09 08:34:58.225778 vnpy_xex-2023.6.9.2/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.9.2/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:34:58.222169 vnpy_xex-2023.6.9.2/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.9.2/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25100 2023-06-09 08:32:32.000000 vnpy_xex-2023.6.9.2/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-09 08:34:58.224976 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-09 08:34:58.000000 vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.6.9.1/LICENSE` & `vnpy_xex-2023.6.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.9.1/PKG-INFO` & `vnpy_xex-2023.6.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.6.9.1
+Version: 2023.6.9.2
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.6.9.1/setup.cfg` & `vnpy_xex-2023.6.9.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.6.9.1
+version = 2023.6.9.2
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.6.9.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.9.2/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.9.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.9.2/vnpy_xex/xex_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -505,18 +505,22 @@
         self.gateway.on_order(order)
 
         if not issubclass(exception_type, (ConnectionError, SSLError)):
             self.on_error(exception_type, exception_value, tb, request)
 
     def on_cancel_order(self, data: dict, request: Request) -> None:
         """委托撤单回报"""
-        pass
+        logger.debug(
+            f"on_cancel_order data={beeprint.pp(data, output=False, sort_keys=False)} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
 
     def on_cancel_failed(self, status_code: str, request: Request) -> None:
         """撤单回报函数报错回报"""
+        logger.debug(
+            f"on_cancel_failed {status_code=} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
+
         if request.extra:
             order = request.extra
             order.status = Status.REJECTED
             self.gateway.on_order(order)
 
         msg = f"撤单失败，状态码：{status_code}，信息：{request.response.text}"
         self.gateway.write_log(msg)
```

### Comparing `vnpy_xex-2023.6.9.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.9.2/vnpy_xex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.6.9.1
+Version: 2023.6.9.2
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

