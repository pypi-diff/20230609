# Comparing `tmp/pyxk-0.6.3.tar.gz` & `tmp/pyxk-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.3.tar", last modified: Thu Jun  8 05:57:56 2023, max compression
+gzip compressed data, was "pyxk-0.6.4.tar", last modified: Fri Jun  9 06:26:03 2023, max compression
```

## Comparing `pyxk-0.6.3.tar` & `pyxk-0.6.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.3/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-08 05:57:56.655691 pyxk-0.6.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1530 2023-06-08 05:36:28.000000 pyxk-0.6.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.645691 pyxk-0.6.3/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-08 05:49:20.000000 pyxk-0.6.3/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.645691 pyxk-0.6.3/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.3/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    19667 2023-06-08 05:44:28.000000 pyxk-0.6.3/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      510 2023-06-06 06:55:14.000000 pyxk-0.6.3/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.3/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3401 2023-06-08 05:42:28.000000 pyxk-0.6.3/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4873 2023-06-07 02:30:14.000000 pyxk-0.6.3/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.3/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.3/pyxk/m3u8/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4690 2023-06-07 02:27:20.000000 pyxk-0.6.3/pyxk/m3u8/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2946 2023-06-07 02:27:50.000000 pyxk-0.6.3/pyxk/m3u8/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    12434 2023-06-08 05:49:20.000000 pyxk-0.6.3/pyxk/m3u8/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.3/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7476 2023-06-08 05:49:20.000000 pyxk-0.6.3/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.3/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    16522 2023-06-07 02:31:20.000000 pyxk-0.6.3/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    18885 2023-06-07 02:31:52.000000 pyxk-0.6.3/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.645691 pyxk-0.6.3/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       62 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-08 05:57:56.655691 pyxk-0.6.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      898 2023-06-08 05:37:28.000000 pyxk-0.6.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.679999 pyxk-0.6.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.4/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-09 06:26:03.679999 pyxk-0.6.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1530 2023-06-08 05:36:28.000000 pyxk-0.6.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.659999 pyxk-0.6.4/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-08 05:49:20.000000 pyxk-0.6.4/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.659999 pyxk-0.6.4/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.4/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    19762 2023-06-09 05:18:06.000000 pyxk-0.6.4/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      606 2023-06-08 10:10:07.000000 pyxk-0.6.4/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.669999 pyxk-0.6.4/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.4/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3401 2023-06-08 05:42:28.000000 pyxk-0.6.4/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4873 2023-06-07 02:30:14.000000 pyxk-0.6.4/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.669999 pyxk-0.6.4/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.4/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.4/pyxk/m3u8/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4690 2023-06-07 02:27:20.000000 pyxk-0.6.4/pyxk/m3u8/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2946 2023-06-07 02:27:50.000000 pyxk-0.6.4/pyxk/m3u8/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    12434 2023-06-08 05:49:20.000000 pyxk-0.6.4/pyxk/m3u8/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.669999 pyxk-0.6.4/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.4/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7476 2023-06-08 05:49:20.000000 pyxk-0.6.4/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.4/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    16522 2023-06-07 02:31:20.000000 pyxk-0.6.4/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    18885 2023-06-07 02:31:52.000000 pyxk-0.6.4/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.659999 pyxk-0.6.4/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       62 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-09 06:26:03.679999 pyxk-0.6.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      898 2023-06-09 06:25:59.000000 pyxk-0.6.4/setup.py
```

### Comparing `pyxk-0.6.3/LICENSE` & `pyxk-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/PKG-INFO` & `pyxk-0.6.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.3
+Version: 0.6.4
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.3/README.md` & `pyxk-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/aclient/client.py` & `pyxk-0.6.4/pyxk/aclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 )
 from pyxk.aclient.typedef import (
     StrOrURL,
     Session,
     Response,
     EventLoop,
     CIMDict,
-    Timeout
+    Timeout,
+    URLS
 )
 
 _copy = LazyLoader("_copy", globals(), "copy")
 _yarl = LazyLoader("_yarl", globals(), "yarl")
 aiohttp = LazyLoader("aiohttp", globals(), "aiohttp")
 _selector = LazyLoader("_selector", globals(), "parsel.selector")
 aiohttp_client_exceptions = LazyLoader("aiohttp_client_exceptions", globals(), "aiohttp.client_exceptions")
@@ -50,15 +51,15 @@
         async def parse(self, response: Response, **kwargs):
             print(response.url)
 
     Download.run()
     """
     limit: Optional[int] = None
     timeout: Timeout = None
-    req_kwargs: Optional[dict] = None
+    req_kwargs: Optional[Union[dict, List[dict]]] = None
     async_sleep: Optional[int] = None
     maximum_retry: Optional[int] = None
     headers: Optional[Union[dict, CIMDict]] = None
     semaphore: Union[Optional[int], asyncio.Semaphore] = None
     verify: Optional[bool] = None
     start_urls: Union[List[str], List[Tuple[str, dict]]] = []
     user_agent: Optional[str] = None
@@ -77,15 +78,16 @@
         ("maximum_retry", 20),
         ("user_agent", get_user_agent()),
         ("aiohttp_kwargs", {}),
         ("until_request_succeed", False),
     )
 
     def __init__(self, *, base_url: StrOrURL = None, **kwargs):
-        """init
+        """异步下载器 init
+
         :param limit: aiohttp 并发控制
         :param timeout: 请求超时时间
         :param req_kwargs: start_request请求参数
         :param async_sleep: 异步休眠时间
         :param maximum_retry: 异步请求最大重试次数
         :param headers: 请求头
         :param semaphore: asyncio并发控制
@@ -213,31 +215,20 @@
         """start_urls 默认运行方法"""
         if not self.start_urls or not isinstance(self.start_urls, (list, tuple)):
             raise NotImplementedError(f"{self.__class__.__name__}.start_urls is not available!")
         # req_kwargs
         req_kwargs = self.req_kwargs
         if not req_kwargs or not isinstance(req_kwargs, dict):
             req_kwargs = {}
-        tasks = []
-        for item in self.start_urls:
-            url, cb_kwargs = item, None
-            if isinstance(item, (list, tuple)) and len(item) >= 2:
-                url, cb_kwargs = item[0], dict(item[1])
-            # base_url
-            if not self._base_url:
-                self.base_url = url
-            task = self.request(
-                url=url,
-                callback=self.parse,
-                cb_kwargs=cb_kwargs,
-                **req_kwargs
-            )
-            tasks.append(task)
-        result = await asyncio.gather(*tasks)
-        return result
+        return await self.gather(
+            self.start_urls,
+            self.parse,
+            cb_kwargs_list=req_kwargs,
+            automatic_base_url=True
+        )
 
     async def request(
         self,
         url: StrOrURL,
         callback: Optional[Callable] = None,
         *,
         method: str = "GET",
@@ -326,54 +317,61 @@
                         raise
                     # warnings.warn(f"<{url}> ServerDisconnectedError", stacklevel=4)
                     await self.sleep()
             return ret
 
     async def gather(
         self,
-        urls: List[StrOrURL],
+        urls: URLS,
         callback: Optional[Callable] = None,
         *,
         method: str = "GET",
-        cb_kwargs_list: Optional[List[dict]] = None,
+        cb_kwargs_list: Optional[Union[List[dict], dict]] = None,
         return_exceptions: bool = False,
+        automatic_base_url: bool = False,
         **req_kwargs
     ) -> list:
         """发送url列表，创建异步任务 并发发送
 
         :param urls: Url List
         :param callback: 响应response 回调函数(函数是异步的)
         :param method: 请求方法(default: GET)
         :param cb_kwargs_list: 回调函数关键字参数列表
         :param return_exceptions: 错误传递(default: False)
         :param req_kwargs: 异步请求 request参数
         :return: list
         """
-        # 初始化 cb_kwargs_list
+        if not isinstance(urls, (list, tuple)):
+            raise TypeError(f"urls must be 'tuple' or 'list', not {type(urls).__name__!r}")
+        length = len(urls)
+        # parse cb_kwargs_list
         if isinstance(cb_kwargs_list, dict):
-            cb_kwargs_list = [cb_kwargs_list for _ in enumerate(urls)]
+            cb_kwargs_list = [cb_kwargs_list for _ in range(length)]
         elif isinstance(cb_kwargs_list, (list, tuple)):
-            cb_kwargs_list = cb_kwargs_list[:len(urls)]
+            cb_kwargs_list = cb_kwargs_list[:length]
+            if len(cb_kwargs_list) < length:
+                cb_kwargs_list.extend([{} for _ in range(length-len(cb_kwargs_list))])
         else:
-            cb_kwargs_list = None
-        # 初始化urls
-        _urls, _cb_kw, = [], []
-        for item in urls:
-            url, cb_kwargs = item, None
+            cb_kwargs_list = [{} for _ in range(length)]
+        # parse urls
+        for index, item in enumerate(urls):
+            url, cb_kwargs = None, None
             if isinstance(item, (list, tuple)) and len(item) >= 2:
                 url, cb_kwargs = item[0], dict(item[1])
-            _urls.append(url)
-            _cb_kw.append(cb_kwargs)
-        urls = _urls
-        if not cb_kwargs_list:
-            cb_kwargs_list = _cb_kw
-        del _urls, _cb_kw
+            else:
+                url, cb_kwargs = item, {}
+            urls[index] = url
+            cb_kwargs.update(cb_kwargs_list[index])
+            cb_kwargs_list[index] = cb_kwargs
         # 收集任务
         tasks = []
         for url, cb_kwargs in zip_longest(urls, cb_kwargs_list):
+            # base url
+            if automatic_base_url and not self.base_url:
+                self.base_url = url
             task = self.request(
                 url=url,
                 callback=callback,
                 method=method,
                 cb_kwargs=cb_kwargs,
                 **req_kwargs
             )
```

### Comparing `pyxk-0.6.3/pyxk/aes/_fmtdata.py` & `pyxk-0.6.4/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/aes/cryptor.py` & `pyxk-0.6.4/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/m3u8/enter_point.py` & `pyxk-0.6.4/pyxk/m3u8/enter_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/m3u8/m3u8download.py` & `pyxk-0.6.4/pyxk/m3u8/m3u8download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.4/pyxk/m3u8/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/m3u8/main.py` & `pyxk-0.6.4/pyxk/m3u8/main.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/requests/api.py` & `pyxk-0.6.4/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/requests/entry_point.py` & `pyxk-0.6.4/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/requests/sessions.py` & `pyxk-0.6.4/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk/utils.py` & `pyxk-0.6.4/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/pyxk.egg-info/PKG-INFO` & `pyxk-0.6.4/pyxk.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.3
+Version: 0.6.4
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.3/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.4/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.3/setup.py` & `pyxk-0.6.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as read_file_obj:
     long_description = read_file_obj.read()
 
 setuptools.setup(
     name='pyxk',
-    version='0.6.3',
+    version='0.6.4',
     author='kai139',
     install_requires=[
         'requests', 'pycryptodome', 'rich', 'm3u8', 'aiohttp', 'aiofiles', 'click', 'parsel'
     ],
     entry_points={
         'console_scripts': [
             'm3u8 = pyxk.m3u8.enter_point:main',
```

