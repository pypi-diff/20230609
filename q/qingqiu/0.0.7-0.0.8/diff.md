# Comparing `tmp/qingqiu-0.0.7.tar.gz` & `tmp/qingqiu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qingqiu-0.0.7.tar", last modified: Fri Apr 14 02:01:44 2023, max compression
+gzip compressed data, was "dist\qingqiu-0.0.8.tar", last modified: Fri Jun  9 05:53:13 2023, max compression
```

## Comparing `qingqiu-0.0.7.tar` & `qingqiu-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 02:01:44.000000 qingqiu-0.0.7/
--rw-rw-rw-   0        0        0      849 2023-04-14 02:01:44.000000 qingqiu-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 02:01:44.000000 qingqiu-0.0.7/qingqiu/
--rw-rw-rw-   0        0        0      929 2023-04-07 12:02:13.000000 qingqiu-0.0.7/qingqiu/__init__.py
--rw-rw-rw-   0        0        0    28054 2023-04-06 07:11:00.000000 qingqiu-0.0.7/qingqiu/check.py
--rw-rw-rw-   0        0        0      958 2022-08-08 12:28:20.000000 qingqiu-0.0.7/qingqiu/conftest.py
--rw-rw-rw-   0        0        0      404 2023-03-30 08:08:56.000000 qingqiu-0.0.7/qingqiu/gl.py
--rw-rw-rw-   0        0        0     7965 2022-08-10 05:44:02.000000 qingqiu-0.0.7/qingqiu/handle.py
--rw-rw-rw-   0        0        0      603 2022-08-10 05:42:27.000000 qingqiu-0.0.7/qingqiu/help.py
--rw-rw-rw-   0        0        0    14208 2023-04-03 07:49:31.000000 qingqiu-0.0.7/qingqiu/qing.py
--rw-rw-rw-   0        0        0    14945 2023-04-11 10:15:21.000000 qingqiu-0.0.7/qingqiu/qiu.py
--rw-rw-rw-   0        0        0       73 2022-07-28 07:10:30.000000 qingqiu-0.0.7/qingqiu/test.py
--rw-rw-rw-   0        0        0     4017 2023-04-10 02:23:22.000000 qingqiu-0.0.7/qingqiu/tools.py
--rw-rw-rw-   0        0        0    17539 2022-08-24 05:50:53.000000 qingqiu-0.0.7/qingqiu/transform.py
-drwxrwxrwx   0        0        0        0 2023-04-14 02:01:44.000000 qingqiu-0.0.7/qingqiu.egg-info/
--rw-rw-rw-   0        0        0      849 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 02:01:44.000000 qingqiu-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-04-14 01:56:34.000000 qingqiu-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:53:13.000000 qingqiu-0.0.8/
+-rw-rw-rw-   0        0        0      849 2023-06-09 05:53:13.000000 qingqiu-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu/
+-rw-rw-rw-   0        0        0      929 2023-04-07 12:02:13.000000 qingqiu-0.0.8/qingqiu/__init__.py
+-rw-rw-rw-   0        0        0    28037 2023-04-17 12:20:01.000000 qingqiu-0.0.8/qingqiu/check.py
+-rw-rw-rw-   0        0        0      958 2022-08-08 12:28:20.000000 qingqiu-0.0.8/qingqiu/conftest.py
+-rw-rw-rw-   0        0        0      404 2023-03-30 08:08:56.000000 qingqiu-0.0.8/qingqiu/gl.py
+-rw-rw-rw-   0        0        0     7965 2022-08-10 05:44:02.000000 qingqiu-0.0.8/qingqiu/handle.py
+-rw-rw-rw-   0        0        0      603 2022-08-10 05:42:27.000000 qingqiu-0.0.8/qingqiu/help.py
+-rw-rw-rw-   0        0        0    14624 2023-06-09 05:47:57.000000 qingqiu-0.0.8/qingqiu/qing.py
+-rw-rw-rw-   0        0        0    14945 2023-04-11 10:15:21.000000 qingqiu-0.0.8/qingqiu/qiu.py
+-rw-rw-rw-   0        0        0     1361 2023-04-14 02:06:13.000000 qingqiu-0.0.8/qingqiu/setup.py
+-rw-rw-rw-   0        0        0       73 2022-07-28 07:10:30.000000 qingqiu-0.0.8/qingqiu/test.py
+-rw-rw-rw-   0        0        0     4204 2023-04-18 02:10:19.000000 qingqiu-0.0.8/qingqiu/tools.py
+-rw-rw-rw-   0        0        0    17539 2022-08-24 05:50:53.000000 qingqiu-0.0.8/qingqiu/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 05:53:13.000000 qingqiu-0.0.8/qingqiu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 05:53:13.000000 qingqiu-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-06-09 05:50:48.000000 qingqiu-0.0.8/setup.py
```

### Comparing `qingqiu-0.0.7/PKG-INFO` & `qingqiu-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qingqiu
-Version: 0.0.7
+Version: 0.0.8
 Summary: 简单得接口测试框架
 Home-page: https://gitee.com/tuboyou/qingqiu
 Author: lixuecheng
 Author-email: lixuechengde@163.com
 License: MIT Licence
 Description: 简单得接口测试框架
 Keywords: pip,easy,requests,auto
```

### Comparing `qingqiu-0.0.7/qingqiu/__init__.py` & `qingqiu-0.0.8/qingqiu/__init__.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.7/qingqiu/check.py` & `qingqiu-0.0.8/qingqiu/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 
-import datetime
 import json
 import logging
 import re
 import time
 from .gl import setGlobal,getGlobal
 
 log = logging.getLogger('')
```

### Comparing `qingqiu-0.0.7/qingqiu/conftest.py` & `qingqiu-0.0.8/qingqiu/conftest.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.7/qingqiu/handle.py` & `qingqiu-0.0.8/qingqiu/handle.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.7/qingqiu/help.py` & `qingqiu-0.0.8/qingqiu/help.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.7/qingqiu/qing.py` & `qingqiu-0.0.8/qingqiu/qing.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         self.__funcargs = []
         self.__proxy={'http':None,"https":None}
         self.__headers = dict(self.__find_attr(this,k, 'headers', {}))
         self.__body = self.__find_attr(this,k, 'body')
         self.__body = self.__find_attr(this,k, 'data')
         self.__auth = self.__find_attr(this,k, 'auth', None)
         self.__isMultipart = False
+        self.postJSon=False
         if isinstance(self.__auth, list) or isinstance(self.__auth, tuple):
             if len(self.__auth) == 2:
                 self.setAuth(self.__auth[0], self.__auth[1])
             else:
                 raise Exception("auth is err:"+str(self.__auth))
         else:
             if self.__auth is not None:
@@ -271,18 +272,19 @@
 
     def setBody(self, body):
         self.__body = body
         return self
 
     def setContentTypeJson(self):
         self.__headers['content-type'] = "application/json; charset=utf-8"
+        self.postJSon=True
         return self
 
     def setContenttypeKV(self):
-
+        self.postJSon=False
         self.__headers['content-type'] = "application/x-www-form-urlencoded;charset=utf-8"
         return self
 
     def setContenttypeMultipart(self):
         self.__method = "POST"
         self.__isMultipart = True
         return self
@@ -332,14 +334,15 @@
         return self
 
     
 
     def setHttpProxy(self,http:str =None,https:str =None):
         self.__proxy['http']=str(http)
         self.__proxy['https']=str(https)
+        return self
 
 
     def request(self):
         
         urllib3.disable_warnings()
         try:
             if self.__func is not None:
@@ -388,21 +391,26 @@
                     else:
                         line += l[:100]+"...\n"
                 showStr += line
                 log.info(showStr)
 
             else:
                 if self.__method=="":
-                    if 'content-type' in self.__headers:
+                    if 'content-type' in self.__headers :
                         self.__method="post"
                     else:
                         self.__method="get"
+
                 if isinstance(self.__body,str):
                     self.__body=self.__body.encode()
-                r = requests.request(self.__method, self.URL, headers=self.__headers, verify=False,
+                if(self.postJSon):
+                    r=requests.request(self.__method, self.URL, headers=self.__headers, verify=False,
+                                     allow_redirects=False, auth=self.__auth, json=self.__body, timeout=self.__timeout,proxies=self.__proxy)
+                else:
+                    r = requests.request(self.__method, self.URL, headers=self.__headers, verify=False,
                                      allow_redirects=False, auth=self.__auth, data=self.__body, timeout=self.__timeout,proxies=self.__proxy)
             try:
                 self.res = qiu(r, log, self.__nolog,self.__name)
             except Exception as e:
                 log.error('响应解析出错')
                 raise e
             return self.res
```

### Comparing `qingqiu-0.0.7/qingqiu/qiu.py` & `qingqiu-0.0.8/qingqiu/qiu.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.7/qingqiu/tools.py` & `qingqiu-0.0.8/qingqiu/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: UTF-8 -*-
 
 import base64
-import datetime
+from datetime import datetime,timedelta
 import hashlib
 import inspect
 import json
 import os
-
-import json_tools
+try:
+    import json_tools
+except:
+    pass
 
 import urllib.parse
 
 backup={'lastTime':None}
 
 class tools:
     @staticmethod
@@ -22,40 +24,40 @@
     def time2Stamp(timeFormat=None, returnType='int', ms=False,days=0,hours=0,minutes=0,seconds=0,dayStart=False,dayEnd=False,lastTime=False):
         '''
         timeFormat='2013-10-10 23:40:00' 
         None:当前
         ret 'int' 'str'
         ms 是否毫秒级
         '''
-        to=datetime.datetime.now()
+        to=datetime.now()
         if lastTime:
             if backup['lastTime'] is not None:
                 to=backup['lastTime']
         if timeFormat is not None and isinstance(timeFormat,str):
-            to=datetime.datetime.fromisoformat(timeFormat.strip())
+            to=datetime.strptime(timeFormat.strip(),"%Y-%m-%d %H:%M:%S")
         if dayStart:
             to=to.replace(hour=0,minute=0,second=0,microsecond=0)
         if dayEnd:
             to=to.replace(hour=23,minute=59,second=59,microsecond=0)
-        to=to+datetime.timedelta(days=days,minutes=minutes,hours=hours,seconds=seconds)
+        to=to+timedelta(days=days,minutes=minutes,hours=hours,seconds=seconds)
         backup['lastTime']=to
         timeStamp=to.timestamp()
         if ms:
             timeStamp = timeStamp*1000
         timeStamp=int(to.timestamp())
         if returnType == 'str':
             return str(timeStamp)
         return timeStamp
 
     @staticmethod
     def timeFormat(ts:int=None):
         if ts is None:
-            return str(datetime.datetime.now())
+            return str(datetime.now())
         else:
-            return str(datetime.datetime.fromtimestamp(ts))
+            return str(datetime.fromtimestamp(ts))
 
     @staticmethod
     def showJson(data):
         if isinstance(data,dict) or isinstance(data,list):
             return json.dumps(
                     data, ensure_ascii=False, indent=4)
         elif isinstance(data,str):
@@ -78,27 +80,30 @@
     def diff(a,b,printable=False,ig=None):
         '''
         a dict
         b dict
         printable bool 是否打印不一致的地方
         ig  str add/replace/...:keyname
         '''
-        val= json_tools.diff(a,b)
-        if printable:
-            iggname=""
-            iggval=""
-            if ig is not None:
-                iggname=str(ig).split(':')[0]
-                iggval=str(ig).split(':')[1]
-            for x in val:
-                if iggname!='' and iggname in x:
-                    if str(x[iggname]).endswith(iggval):
-                        continue
-                print(x)
-        return val
+        try:
+            val= json_tools.diff(a,b)
+            if printable:
+                iggname=""
+                iggval=""
+                if ig is not None:
+                    iggname=str(ig).split(':')[0]
+                    iggval=str(ig).split(':')[1]
+                for x in val:
+                    if iggname!='' and iggname in x:
+                        if str(x[iggname]).endswith(iggval):
+                            continue
+                    print(x)
+            return val
+        except :
+            print('如果没安装json_tools，请使用pip install json_tools')
     
 
 
     @staticmethod
     def base64encode(val: str or bytes, return_str=True, encode='utf8') -> str or bytes:
         tmpVal = b'unknown'
         if isinstance(val, bytes):
```

### Comparing `qingqiu-0.0.7/qingqiu/transform.py` & `qingqiu-0.0.8/qingqiu/transform.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.7/qingqiu.egg-info/PKG-INFO` & `qingqiu-0.0.8/qingqiu.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qingqiu
-Version: 0.0.7
+Version: 0.0.8
 Summary: 简单得接口测试框架
 Home-page: https://gitee.com/tuboyou/qingqiu
 Author: lixuecheng
 Author-email: lixuechengde@163.com
 License: MIT Licence
 Description: 简单得接口测试框架
 Keywords: pip,easy,requests,auto
```

### Comparing `qingqiu-0.0.7/setup.py` & `qingqiu-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from setuptools import setup, find_packages
 
 
 
 setup(
 name = "qingqiu",
-version = "0.0.7",
+version = "0.0.8",
 keywords = ["pip", "easy","requests","auto"],
 description = "简单得接口测试框架",
 long_description = "简单得接口测试框架",
 license = "MIT Licence",
 
 url = "https://gitee.com/tuboyou/qingqiu",
 author = "lixuecheng",
```

