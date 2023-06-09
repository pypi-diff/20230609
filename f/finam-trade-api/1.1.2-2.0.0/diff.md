# Comparing `tmp/finam-trade-api-1.1.2.tar.gz` & `tmp/finam-trade-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finam-trade-api-1.1.2.tar", last modified: Thu Mar 23 16:01:22 2023, max compression
+gzip compressed data, was "finam-trade-api-2.0.0.tar", last modified: Fri Jun  9 09:38:55 2023, max compression
```

## Comparing `finam-trade-api-1.1.2.tar` & `finam-trade-api-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      414 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/PKG-INFO
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     4117 2023-03-23 15:16:56.000000 finam-trade-api-1.1.2/README.md
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/examples/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)        0 2022-11-09 14:52:24.000000 finam-trade-api-1.1.2/examples/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      235 2022-12-15 17:05:17.000000 finam-trade-api-1.1.2/examples/access_token.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     2276 2023-03-15 08:22:08.000000 finam-trade-api-1.1.2/examples/order.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      400 2022-12-07 13:53:44.000000 finam-trade-api-1.1.2/examples/portfolio.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      419 2022-12-28 11:45:24.000000 finam-trade-api-1.1.2/examples/security.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       92 2023-03-23 15:50:46.000000 finam-trade-api-1.1.2/finam_trade_api/__init__.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/access/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       60 2023-03-23 15:45:44.000000 finam-trade-api-1.1.2/finam_trade_api/access/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      741 2023-03-23 15:45:44.000000 finam-trade-api-1.1.2/finam_trade_api/access/access_token.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      132 2022-12-15 17:05:17.000000 finam-trade-api-1.1.2/finam_trade_api/access/model.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/base_client/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       56 2023-03-23 15:45:44.000000 finam-trade-api-1.1.2/finam_trade_api/base_client/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1561 2023-03-15 15:47:41.000000 finam-trade-api-1.1.2/finam_trade_api/base_client/base.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      438 2023-03-23 15:49:54.000000 finam-trade-api-1.1.2/finam_trade_api/client.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/events/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)        0 2022-11-07 13:44:41.000000 finam-trade-api-1.1.2/finam_trade_api/events/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      255 2023-03-23 15:45:44.000000 finam-trade-api-1.1.2/finam_trade_api/events/event.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       83 2022-11-16 16:07:34.000000 finam-trade-api-1.1.2/finam_trade_api/exceptions.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      212 2022-10-31 14:01:23.000000 finam-trade-api-1.1.2/finam_trade_api/models.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/order/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      810 2023-03-23 15:46:18.000000 finam-trade-api-1.1.2/finam_trade_api/order/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     5143 2023-03-13 15:46:56.000000 finam-trade-api-1.1.2/finam_trade_api/order/model.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     3861 2023-03-23 15:46:18.000000 finam-trade-api-1.1.2/finam_trade_api/order/order.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/portfolio/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      289 2023-03-23 15:48:17.000000 finam-trade-api-1.1.2/finam_trade_api/portfolio/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1317 2022-11-16 16:07:34.000000 finam-trade-api-1.1.2/finam_trade_api/portfolio/model.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1175 2023-03-23 15:48:17.000000 finam-trade-api-1.1.2/finam_trade_api/portfolio/portfolio.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api/securities/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      172 2023-03-23 15:49:39.000000 finam-trade-api-1.1.2/finam_trade_api/securities/__init__.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      524 2022-10-31 14:01:23.000000 finam-trade-api-1.1.2/finam_trade_api/securities/model.py
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1026 2023-03-23 15:49:38.000000 finam-trade-api-1.1.2/finam_trade_api/securities/securities.py
-drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-03-23 16:01:22.764407 finam-trade-api-1.1.2/finam_trade_api.egg-info/
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      414 2023-03-23 16:01:22.000000 finam-trade-api-1.1.2/finam_trade_api.egg-info/PKG-INFO
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1012 2023-03-23 16:01:22.000000 finam-trade-api-1.1.2/finam_trade_api.egg-info/SOURCES.txt
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)        1 2023-03-23 16:01:22.000000 finam-trade-api-1.1.2/finam_trade_api.egg-info/dependency_links.txt
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       46 2023-03-23 16:01:22.000000 finam-trade-api-1.1.2/finam_trade_api.egg-info/requires.txt
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       25 2023-03-23 16:01:22.000000 finam-trade-api-1.1.2/finam_trade_api.egg-info/top_level.txt
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      435 2023-03-23 16:01:22.768407 finam-trade-api-1.1.2/setup.cfg
--rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      598 2023-03-23 16:01:16.000000 finam-trade-api-1.1.2/setup.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.887707 finam-trade-api-2.0.0/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)    35149 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/LICENSE
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      406 2023-06-09 09:38:55.887707 finam-trade-api-2.0.0/PKG-INFO
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     6697 2023-06-09 09:29:53.000000 finam-trade-api-2.0.0/README.md
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/examples/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/examples/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      245 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/examples/access_token.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1012 2023-06-09 09:29:53.000000 finam-trade-api-2.0.0/examples/candles.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     2296 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/examples/order.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      420 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/examples/portfolio.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      429 2023-06-08 17:08:00.000000 finam-trade-api-2.0.0/examples/security.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       92 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/__init__.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api/access/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       60 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/access/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      741 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/access/access_token.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      132 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/access/model.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api/base_client/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       56 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/base_client/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1025 2023-06-09 09:11:08.000000 finam-trade-api-2.0.0/finam_trade_api/base_client/base.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api/candles/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      251 2023-06-09 09:35:11.000000 finam-trade-api-2.0.0/finam_trade_api/candles/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     2228 2023-06-09 09:35:11.000000 finam-trade-api-2.0.0/finam_trade_api/candles/candles.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1167 2023-06-09 09:35:11.000000 finam-trade-api-2.0.0/finam_trade_api/candles/model.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      532 2023-06-08 16:55:34.000000 finam-trade-api-2.0.0/finam_trade_api/client.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api/events/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/events/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      255 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/events/event.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       83 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/exceptions.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      212 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/models.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api/order/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      810 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/order/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     5143 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/order/model.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     3861 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/order/order.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.887707 finam-trade-api-2.0.0/finam_trade_api/portfolio/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      289 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/portfolio/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1317 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/portfolio/model.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1175 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/portfolio/portfolio.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.887707 finam-trade-api-2.0.0/finam_trade_api/securities/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      172 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/securities/__init__.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      524 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/securities/model.py
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1026 2023-06-08 16:06:11.000000 finam-trade-api-2.0.0/finam_trade_api/securities/securities.py
+drwxrwxr-x   0 dboyarshin  (1000) dboyarshin  (1000)        0 2023-06-09 09:38:55.883707 finam-trade-api-2.0.0/finam_trade_api.egg-info/
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      406 2023-06-09 09:38:55.000000 finam-trade-api-2.0.0/finam_trade_api.egg-info/PKG-INFO
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)     1144 2023-06-09 09:38:55.000000 finam-trade-api-2.0.0/finam_trade_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)        1 2023-06-09 09:38:55.000000 finam-trade-api-2.0.0/finam_trade_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       46 2023-06-09 09:38:55.000000 finam-trade-api-2.0.0/finam_trade_api.egg-info/requires.txt
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)       25 2023-06-09 09:38:55.000000 finam-trade-api-2.0.0/finam_trade_api.egg-info/top_level.txt
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      374 2023-06-09 09:38:55.887707 finam-trade-api-2.0.0/setup.cfg
+-rw-rw-r--   0 dboyarshin  (1000) dboyarshin  (1000)      598 2023-06-09 09:29:53.000000 finam-trade-api-2.0.0/setup.py
```

### Comparing `finam-trade-api-1.1.2/examples/order.py` & `finam-trade-api-2.0.0/examples/order.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
-from finam.client import Client
-from finam.order.model import (
+from finam_trade_api.client import Client
+from finam_trade_api.order.model import (
     BoardType,
     CreateOrderRequestModel,
     CreateStopOrderRequestModel,
     DelOrderModel,
     OrdersRequestModel,
     OrderType,
     PropertyType,
```

### Comparing `finam-trade-api-1.1.2/finam_trade_api/access/access_token.py` & `finam-trade-api-2.0.0/finam_trade_api/access/access_token.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/order/__init__.py` & `finam-trade-api-2.0.0/finam_trade_api/order/__init__.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/order/model.py` & `finam-trade-api-2.0.0/finam_trade_api/order/model.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/order/order.py` & `finam-trade-api-2.0.0/finam_trade_api/order/order.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/portfolio/model.py` & `finam-trade-api-2.0.0/finam_trade_api/portfolio/model.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/portfolio/portfolio.py` & `finam-trade-api-2.0.0/finam_trade_api/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/securities/model.py` & `finam-trade-api-2.0.0/finam_trade_api/securities/model.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api/securities/securities.py` & `finam-trade-api-2.0.0/finam_trade_api/securities/securities.py`

 * *Files identical despite different names*

### Comparing `finam-trade-api-1.1.2/finam_trade_api.egg-info/SOURCES.txt` & `finam-trade-api-2.0.0/finam_trade_api.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 examples/__init__.py
 examples/access_token.py
+examples/candles.py
 examples/order.py
 examples/portfolio.py
 examples/security.py
 finam_trade_api/__init__.py
 finam_trade_api/client.py
 finam_trade_api/exceptions.py
 finam_trade_api/models.py
@@ -16,14 +18,17 @@
 finam_trade_api.egg-info/requires.txt
 finam_trade_api.egg-info/top_level.txt
 finam_trade_api/access/__init__.py
 finam_trade_api/access/access_token.py
 finam_trade_api/access/model.py
 finam_trade_api/base_client/__init__.py
 finam_trade_api/base_client/base.py
+finam_trade_api/candles/__init__.py
+finam_trade_api/candles/candles.py
+finam_trade_api/candles/model.py
 finam_trade_api/events/__init__.py
 finam_trade_api/events/event.py
 finam_trade_api/order/__init__.py
 finam_trade_api/order/model.py
 finam_trade_api/order/order.py
 finam_trade_api/portfolio/__init__.py
 finam_trade_api/portfolio/model.py
```

### Comparing `finam-trade-api-1.1.2/setup.py` & `finam-trade-api-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name="finam-trade-api",
     maintainer="DBoyara",
     maintainer_email="boyarshin.den@yandex.ru",
     packages=find_packages(),
-    version="1.1.2",
+    version="2.0.0",
     install_requires=["aiohttp >= 3.8.3, < 4.0.0", "pydantic >= 1.10.2, < 2.0.0"],
     python_requires=">3.7.0, <4",
     license="GNU GPL v.3.0",
     description="Асинхронный REST-клиент для API Finam",
     long_description="Примеры и описание здесь https://github.com/DBoyara/FinamTradeApiPy ",
     url="https://github.com/DBoyara/FinamTradeApiPy",
 )
```

