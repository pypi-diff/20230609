# Comparing `tmp/pywencai-0.8.9.tar.gz` & `tmp/pywencai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.9.tar", max compression
+gzip compressed data, was "pywencai-0.9.0.tar", max compression
```

## Comparing `pywencai-0.8.9.tar` & `pywencai-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-06-01 02:57:57.055427 pywencai-0.8.9/LICENSE
--rw-r--r--   0        0        0     3043 2023-06-01 02:57:57.055427 pywencai-0.8.9/README.md
--rw-r--r--   0        0        0      612 2023-06-01 02:57:57.055427 pywencai-0.8.9/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/__init__.py
--rw-r--r--   0        0        0     5118 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/convert.py
--rw-r--r--   0        0        0      433 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/headers.py
--rw-r--r--   0        0        0    39677 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4306 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/wencai.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 pywencai-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-09 16:19:20.730540 pywencai-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3402 2023-06-09 16:19:20.730540 pywencai-0.9.0/README.md
+-rw-r--r--   0        0        0      612 2023-06-09 16:19:20.730540 pywencai-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-09 16:19:20.730540 pywencai-0.9.0/pywencai/__init__.py
+-rw-r--r--   0        0        0     5118 2023-06-09 16:19:20.730540 pywencai-0.9.0/pywencai/convert.py
+-rw-r--r--   0        0        0      433 2023-06-09 16:19:20.730540 pywencai-0.9.0/pywencai/headers.py
+-rw-r--r--   0        0        0    39677 2023-06-09 16:19:20.734540 pywencai-0.9.0/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     5023 2023-06-09 16:19:20.734540 pywencai-0.9.0/pywencai/wencai.py
+-rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pywencai-0.9.0/PKG-INFO
```

### Comparing `pywencai-0.8.9/LICENSE` & `pywencai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.9/README.md` & `pywencai-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 ```
 
 # Demo
 
 ```python
 import pywencai
 
-res = pywencai.get(question='退市股票', sort_key='退市@退市日期', sort_order='asc')
+res = pywencai.get(query='退市股票', sort_key='退市@退市日期', sort_order='asc')
 print(res)
 ```
 
-[demo.ipynb](./demo.ipynb)
-
 # API
 
 ## get(**kwargs)
 
 根据问财语句查询结果
 
 ### 参数
 
-#### question
+#### query
 
 必填，查询问句
 
+> 老版本的question参数1.0版本以后会弃用，请以后统一使用query参数
+
 #### sort_key
 
 非必填，指定用于排序的字段，值为返回结果的列名
 
 #### sort_order
 
 非必填，排序规则，至为`asc`（升序）或`desc`（降序）
@@ -98,22 +98,28 @@
 非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
 
 #### request_params
 
 非必填，默认为`{}`，可以设置额外的request参数
 
 ```python
-pywencai.get(question='昨日涨幅', sort_order='asc', loop=True, log=True, request_params={ 'proxies': proxies, 'timeout': (5, 10) })
+pywencai.get(query='昨日涨幅', sort_order='asc', loop=True, log=True, request_params={ 'proxies': proxies, 'timeout': (5, 10) })
 ```
 > 具体参数参看：[https://requests.readthedocs.io/en/latest/api/#requests.request](https://requests.readthedocs.io/en/latest/api/#requests.request)
 
 #### no_detail
 
 非必填，默认为`False`，当为`True`时，查询一些**详情类问题**不再会返回字典，而返回`None`，可以保证查询结果类型一直为`pd.DataFrame`或`None`。
 
+#### find
+
+非必填，默认为`None`，可以传一个数组，例如`['600519', '0000010']`，数组内的对应标的会排列在DataFrame的最前面。
+
+**【注意】** 1、该参数只有结果范围DataFrame时有效。2、配置该参数后，loop参数会失效，结果只会返回前100条。
+
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
 
 当查询的是详情时，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
```

### Comparing `pywencai-0.8.9/pyproject.toml` & `pywencai-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.9"
+version = "0.9.0"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.8.9/pywencai/convert.py` & `pywencai-0.9.0/pywencai/convert.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.9/pywencai/hexin-v.js` & `pywencai-0.9.0/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.9/pywencai/wencai.py` & `pywencai-0.9.0/pywencai/wencai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+from typing import List
+
 import requests as rq
 import pandas as pd
 import time
 import logging
 import pydash as _
 from pywencai.convert import convert
 from pywencai.headers import headers
@@ -39,15 +41,14 @@
         'perpage': 10,
         'page': 1,
         'source': 'Ths_iwencai_Xuangu',
         'secondary_intent': query_type,
         'question': question
     }
 
-    count = 0
     log and logger.info(f'获取condition开始')
 
     def do():
         res = rq.request(
             method='POST',
             url='http://www.iwencai.com/customized/chart/get-robot-data',
             json=data,
@@ -78,38 +79,56 @@
 
 def get_page(**kwargs):
     '''获取每页数据'''
     retry = kwargs.pop('retry', 10)
     sleep = kwargs.pop('sleep', 0)
     log = kwargs.pop('log', False)
     cookie = kwargs.pop('cookie', None)
+    find = kwargs.pop('find', None)
+    query_type = kwargs.get('query_type', 'stock')
     request_params = kwargs.get('request_params', {})
-
-    data = {
-        'perpage': 100,
-        'page': 1,
-        'source': 'Ths_iwencai_Xuangu',
-        **kwargs
-    }
-    count = 0
+    if find is None:
+        data = {
+            'perpage': 100,
+            'page': 1,
+            'source': 'Ths_iwencai_Xuangu',
+            **kwargs
+        }
+        target_url = 'http://www.iwencai.com/gateway/urp/v7/landing/getDataList'
+        path = 'answer.components.0.data.datas'
+    else:
+        if isinstance(find, List):
+            # 传入股票代码列表时，拼接
+            find = ','.join(find)
+        data = {
+            'perpage': 500,
+            'page': 1,
+            'source': 'Ths_iwencai_Xuangu',
+            'query_type': query_type,
+            'question': find,
+            **kwargs
+        }
+        target_url = 'http://www.iwencai.com/unifiedwap/unified-wap/v2/stock-pick/find'
+        path = 'data.data.datas'
+    
     log and logger.info(f'第{data.get("page")}页开始')
 
     def do():
         res = rq.request(
             method='POST',
-            url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
+            url=target_url,
             data=data,
             headers=headers(cookie),
             timeout=(5, 10),
             **request_params
         )
-        result = json.loads(res.text)
-        list = result['answer']['components'][0]['data']['datas']
+        result_do = json.loads(res.text)
+        data_list = _.get(result_do, path)
         log and logger.info(f'第{data.get("page")}页成功')
-        return pd.DataFrame.from_dict(list)
+        return pd.DataFrame.from_dict(data_list)
     
     result = while_do(do, retry, sleep, log)
 
     if result is None:
         log and logger.error(f'第{data.get("page")}页失败')
 
     return result
@@ -149,15 +168,16 @@
     '''获取结果'''
     kwargs = {replace_key(key): value for key, value in kwargs.items()}
     params = get_robot_data(**kwargs)
     data = params.get('data')
     condition = _.get(data, 'condition')
     if condition is not None:
         kwargs = {**kwargs, **data}
-        if loop:
+        find = kwargs.get('find', None)
+        if loop and find is None:
             return loop_page(loop, **kwargs)
         else:
             return get_page(**kwargs)
     else:
         no_detail = kwargs.get('no_detail')
         if no_detail != True:
             return data
```

### Comparing `pywencai-0.8.9/PKG-INFO` & `pywencai-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.9
+Version: 0.9.0
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,32 +36,32 @@
 ```
 
 # Demo
 
 ```python
 import pywencai
 
-res = pywencai.get(question='退市股票', sort_key='退市@退市日期', sort_order='asc')
+res = pywencai.get(query='退市股票', sort_key='退市@退市日期', sort_order='asc')
 print(res)
 ```
 
-[demo.ipynb](./demo.ipynb)
-
 # API
 
 ## get(**kwargs)
 
 根据问财语句查询结果
 
 ### 参数
 
-#### question
+#### query
 
 必填，查询问句
 
+> 老版本的question参数1.0版本以后会弃用，请以后统一使用query参数
+
 #### sort_key
 
 非必填，指定用于排序的字段，值为返回结果的列名
 
 #### sort_order
 
 非必填，排序规则，至为`asc`（升序）或`desc`（降序）
@@ -117,22 +117,28 @@
 非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
 
 #### request_params
 
 非必填，默认为`{}`，可以设置额外的request参数
 
 ```python
-pywencai.get(question='昨日涨幅', sort_order='asc', loop=True, log=True, request_params={ 'proxies': proxies, 'timeout': (5, 10) })
+pywencai.get(query='昨日涨幅', sort_order='asc', loop=True, log=True, request_params={ 'proxies': proxies, 'timeout': (5, 10) })
 ```
 > 具体参数参看：[https://requests.readthedocs.io/en/latest/api/#requests.request](https://requests.readthedocs.io/en/latest/api/#requests.request)
 
 #### no_detail
 
 非必填，默认为`False`，当为`True`时，查询一些**详情类问题**不再会返回字典，而返回`None`，可以保证查询结果类型一直为`pd.DataFrame`或`None`。
 
+#### find
+
+非必填，默认为`None`，可以传一个数组，例如`['600519', '0000010']`，数组内的对应标的会排列在DataFrame的最前面。
+
+**【注意】** 1、该参数只有结果范围DataFrame时有效。2、配置该参数后，loop参数会失效，结果只会返回前100条。
+
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
 
 当查询的是详情时，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
```

