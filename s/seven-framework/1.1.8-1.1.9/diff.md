# Comparing `tmp/seven_framework-1.1.8.tar.gz` & `tmp/seven_framework-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seven_framework-1.1.8.tar", last modified: Tue Jul 12 06:04:01 2022, max compression
+gzip compressed data, was "dist/seven_framework-1.1.9.tar", last modified: Wed Jul 27 10:34:50 2022, max compression
```

## Comparing `seven_framework-1.1.8.tar` & `seven_framework-1.1.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-12 06:04:01.922226 seven_framework-1.1.8/
--rw-r--r--   0 chenxiaolei   (502) staff       (20)    13260 2022-07-12 06:04:01.921733 seven_framework-1.1.8/PKG-INFO
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     9245 2022-07-12 06:02:11.000000 seven_framework-1.1.8/README.md
--rw-r--r--   0 chenxiaolei   (502) staff       (20)       38 2022-07-12 06:04:01.922402 seven_framework-1.1.8/setup.cfg
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     2099 2022-07-11 09:43:01.000000 seven_framework-1.1.8/setup.py
-drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-12 06:04:01.913631 seven_framework-1.1.8/seven_framework/
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)      530 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/__init__.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)    32368 2022-05-17 10:18:19.000000 seven_framework-1.1.8/seven_framework/base_model.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)      842 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/clickhouse.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)      918 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/coding.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     1550 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/config.py
-drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-12 06:04:01.916182 seven_framework-1.1.8/seven_framework/console/
--rw-r--r--   0 chenxiaolei   (502) staff       (20)      156 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/console/__init__.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     1868 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/console/base_console.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     6339 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/crypto.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)    19046 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/csv.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     2418 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/dict.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     4740 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/es.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)    19079 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/excel.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)    60787 2022-05-24 12:28:56.000000 seven_framework-1.1.8/seven_framework/file.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)      593 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/host.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     9301 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/http.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     2030 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/ip.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     1551 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/json.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)    17002 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/log.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)    15308 2022-07-12 06:00:28.000000 seven_framework-1.1.8/seven_framework/mysql.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     2332 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/notice.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     4886 2022-07-11 09:42:32.000000 seven_framework-1.1.8/seven_framework/os.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     1775 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/qr_code.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     2546 2022-05-17 10:18:19.000000 seven_framework-1.1.8/seven_framework/redis.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     2874 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/sign.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)    21002 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/time.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)      396 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/uuid.py
-drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-12 06:04:01.917827 seven_framework-1.1.8/seven_framework/web_tornado/
--rw-r--r--   0 chenxiaolei   (502) staff       (20)      185 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/web_tornado/__init__.py
-drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-12 06:04:01.919916 seven_framework-1.1.8/seven_framework/web_tornado/base_handler/
--rw-r--r--   0 chenxiaolei   (502) staff       (20)      254 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/web_tornado/base_handler/__init__.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     1130 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/web_tornado/base_handler/base_api_handler.py
--rwxr-xr-x   0 chenxiaolei   (502) staff       (20)     1221 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/web_tornado/base_handler/base_cookie_handler.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)    24020 2022-05-17 10:18:19.000000 seven_framework-1.1.8/seven_framework/web_tornado/base_handler/base_handler.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     1976 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/web_tornado/base_tornado.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     1700 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/web_tornado/monitor.py
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     9536 2022-02-23 12:37:07.000000 seven_framework-1.1.8/seven_framework/work_wechat.py
-drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-12 06:04:01.915303 seven_framework-1.1.8/seven_framework.egg-info/
--rw-r--r--   0 chenxiaolei   (502) staff       (20)    13260 2022-07-12 06:04:01.000000 seven_framework-1.1.8/seven_framework.egg-info/PKG-INFO
--rw-r--r--   0 chenxiaolei   (502) staff       (20)     1275 2022-07-12 06:04:01.000000 seven_framework-1.1.8/seven_framework.egg-info/SOURCES.txt
--rw-r--r--   0 chenxiaolei   (502) staff       (20)        1 2022-07-12 06:04:01.000000 seven_framework-1.1.8/seven_framework.egg-info/dependency_links.txt
--rw-r--r--   0 chenxiaolei   (502) staff       (20)      464 2022-07-12 06:04:01.000000 seven_framework-1.1.8/seven_framework.egg-info/requires.txt
--rw-r--r--   0 chenxiaolei   (502) staff       (20)       16 2022-07-12 06:04:01.000000 seven_framework-1.1.8/seven_framework.egg-info/top_level.txt
+drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-27 10:34:50.839270 seven_framework-1.1.9/
+-rw-r--r--   0 chenxiaolei   (502) staff       (20)    13333 2022-07-27 10:34:50.838887 seven_framework-1.1.9/PKG-INFO
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     9294 2022-07-27 10:34:18.000000 seven_framework-1.1.9/README.md
+-rw-r--r--   0 chenxiaolei   (502) staff       (20)       38 2022-07-27 10:34:50.839408 seven_framework-1.1.9/setup.cfg
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     2099 2022-07-27 10:34:29.000000 seven_framework-1.1.9/setup.py
+drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-27 10:34:50.828229 seven_framework-1.1.9/seven_framework/
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      530 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/__init__.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    32368 2022-05-17 10:18:19.000000 seven_framework-1.1.9/seven_framework/base_model.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      842 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/clickhouse.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      918 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/coding.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1550 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/config.py
+drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-27 10:34:50.832996 seven_framework-1.1.9/seven_framework/console/
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      156 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/console/__init__.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1868 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/console/base_console.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     6339 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/crypto.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    19046 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/csv.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     2418 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/dict.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     4740 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/es.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    19079 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/excel.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    60787 2022-07-12 06:07:08.000000 seven_framework-1.1.9/seven_framework/file.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      593 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/host.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     9301 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/http.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     2030 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/ip.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1551 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/json.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    17002 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/log.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    15308 2022-07-12 06:07:08.000000 seven_framework-1.1.9/seven_framework/mysql.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     2332 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/notice.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     4886 2022-07-12 06:07:08.000000 seven_framework-1.1.9/seven_framework/os.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1775 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/qr_code.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     2546 2022-05-17 10:18:19.000000 seven_framework-1.1.9/seven_framework/redis.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     2874 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/sign.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    21002 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/time.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      396 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/uuid.py
+drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-27 10:34:50.834996 seven_framework-1.1.9/seven_framework/web_tornado/
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      185 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/web_tornado/__init__.py
+drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-27 10:34:50.837737 seven_framework-1.1.9/seven_framework/web_tornado/base_handler/
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      254 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/web_tornado/base_handler/__init__.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1130 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/web_tornado/base_handler/base_api_handler.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1221 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/web_tornado/base_handler/base_cookie_handler.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    24215 2022-07-27 08:10:31.000000 seven_framework-1.1.9/seven_framework/web_tornado/base_handler/base_handler.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1976 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/web_tornado/base_tornado.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1700 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/web_tornado/monitor.py
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     9536 2022-02-23 12:37:07.000000 seven_framework-1.1.9/seven_framework/work_wechat.py
+drwxr-xr-x   0 chenxiaolei   (502) staff       (20)        0 2022-07-27 10:34:50.831382 seven_framework-1.1.9/seven_framework.egg-info/
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)    13333 2022-07-27 10:34:50.000000 seven_framework-1.1.9/seven_framework.egg-info/PKG-INFO
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)     1275 2022-07-27 10:34:50.000000 seven_framework-1.1.9/seven_framework.egg-info/SOURCES.txt
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)        1 2022-07-27 10:34:50.000000 seven_framework-1.1.9/seven_framework.egg-info/dependency_links.txt
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)      464 2022-07-27 10:34:50.000000 seven_framework-1.1.9/seven_framework.egg-info/requires.txt
+-rwxrwxrwx   0 chenxiaolei   (502) staff       (20)       16 2022-07-27 10:34:50.000000 seven_framework-1.1.9/seven_framework.egg-info/top_level.txt
```

### Comparing `seven_framework-1.1.8/PKG-INFO` & `seven_framework-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: seven_framework
-Version: 1.1.8
+Version: 1.1.9
 Summary: seven framework
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_framework
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         
         <!--
          * @Author: ChenXiaolei
          * @Date: 2021-09-08 11:32:28
-         * @LastEditTime: 2022-07-12 14:01:32
+         * @LastEditTime: 2022-07-27 18:33:51
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         
         # seven_framework
         
         ## 天志互联Python开发库
         
+        ### 1.1.9 更新内容
+        * 增加http patch方法
+        
         ### 1.1.8 更新内容
         * 增加os功能
         * 处理MySQL事务OperationalError或者是InternalError异常堵塞的问题
         
         ### 1.1.7 更新内容
         * 修复aws s3 bug
```

### Comparing `seven_framework-1.1.8/README.md` & `seven_framework-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 
 
 <!--
  * @Author: ChenXiaolei
  * @Date: 2021-09-08 11:32:28
- * @LastEditTime: 2022-07-12 14:01:32
+ * @LastEditTime: 2022-07-27 18:33:51
  * @LastEditors: ChenXiaolei
  * @Description: 
 -->
 
 # seven_framework
 
 ## 天志互联Python开发库
 
+### 1.1.9 更新内容
+* 增加http patch方法
+
 ### 1.1.8 更新内容
 * 增加os功能
 * 处理MySQL事务OperationalError或者是InternalError异常堵塞的问题
 
 ### 1.1.7 更新内容
 * 修复aws s3 bug
```

### Comparing `seven_framework-1.1.8/setup.py` & `seven_framework-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 :Author: ChenXiaolei
 :Date: 2020-04-22 21:25:59
-:LastEditTime: 2022-07-11 17:43:00
+:LastEditTime: 2022-07-27 18:34:29
 :LastEditors: ChenXiaolei
 :Description: 
 """
 from __future__ import print_function
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_framework",
-    version="1.1.8",
+    version="1.1.9",
     author="seven",
     author_email="tech@gao7.com",
     description="seven framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/python/seven_framework",
```

### Comparing `seven_framework-1.1.8/seven_framework/__init__.py` & `seven_framework-1.1.9/seven_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/base_model.py` & `seven_framework-1.1.9/seven_framework/base_model.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/clickhouse.py` & `seven_framework-1.1.9/seven_framework/clickhouse.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/coding.py` & `seven_framework-1.1.9/seven_framework/coding.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/config.py` & `seven_framework-1.1.9/seven_framework/config.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/console/base_console.py` & `seven_framework-1.1.9/seven_framework/console/base_console.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/crypto.py` & `seven_framework-1.1.9/seven_framework/crypto.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/csv.py` & `seven_framework-1.1.9/seven_framework/csv.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/dict.py` & `seven_framework-1.1.9/seven_framework/dict.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/es.py` & `seven_framework-1.1.9/seven_framework/es.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/excel.py` & `seven_framework-1.1.9/seven_framework/excel.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/file.py` & `seven_framework-1.1.9/seven_framework/file.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/host.py` & `seven_framework-1.1.9/seven_framework/host.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/http.py` & `seven_framework-1.1.9/seven_framework/http.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/ip.py` & `seven_framework-1.1.9/seven_framework/ip.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/json.py` & `seven_framework-1.1.9/seven_framework/json.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/log.py` & `seven_framework-1.1.9/seven_framework/log.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/mysql.py` & `seven_framework-1.1.9/seven_framework/mysql.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/notice.py` & `seven_framework-1.1.9/seven_framework/notice.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/os.py` & `seven_framework-1.1.9/seven_framework/os.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/qr_code.py` & `seven_framework-1.1.9/seven_framework/qr_code.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/redis.py` & `seven_framework-1.1.9/seven_framework/redis.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/sign.py` & `seven_framework-1.1.9/seven_framework/sign.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/time.py` & `seven_framework-1.1.9/seven_framework/time.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/web_tornado/base_handler/base_api_handler.py` & `seven_framework-1.1.9/seven_framework/web_tornado/base_handler/base_api_handler.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/web_tornado/base_handler/base_cookie_handler.py` & `seven_framework-1.1.9/seven_framework/web_tornado/base_handler/base_cookie_handler.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/web_tornado/base_handler/base_handler.py` & `seven_framework-1.1.9/seven_framework/web_tornado/base_handler/base_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: ChenXiaolei
 :Date: 2020-03-06 23:17:54
-:LastEditTime: 2022-04-07 14:20:59
+:LastEditTime: 2022-07-27 16:10:14
 :LastEditors: ChenXiaolei
 :Description: Handler基础类
 """
 
 # base import
 import tornado.web
 import time
@@ -67,14 +67,18 @@
         await asyncio.get_event_loop().run_in_executor(self.executor,
                                                        self.head_async, *args)
 
     async def options(self, *args, **kwargs):
         await asyncio.get_event_loop().run_in_executor(self.executor,
                                                        self.options_async, *args)
 
+    async def patch(self, *args, **kwargs):
+        await asyncio.get_event_loop().run_in_executor(self.executor,
+                                                       self.patch_async, *args)
+
     def prepare(self, *args, **argkw):
         """
         :Description: 置于任何请求方法前被调用(请勿重写此函数,可重写prepare_ext)
         :last_editors: ChenXiaolei
         """
         # 标记日志请求关联
         self._build_http_log()
```

### Comparing `seven_framework-1.1.8/seven_framework/web_tornado/base_tornado.py` & `seven_framework-1.1.9/seven_framework/web_tornado/base_tornado.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/web_tornado/monitor.py` & `seven_framework-1.1.9/seven_framework/web_tornado/monitor.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework/work_wechat.py` & `seven_framework-1.1.9/seven_framework/work_wechat.py`

 * *Files identical despite different names*

### Comparing `seven_framework-1.1.8/seven_framework.egg-info/PKG-INFO` & `seven_framework-1.1.9/seven_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: seven-framework
-Version: 1.1.8
+Version: 1.1.9
 Summary: seven framework
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_framework
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         
         <!--
          * @Author: ChenXiaolei
          * @Date: 2021-09-08 11:32:28
-         * @LastEditTime: 2022-07-12 14:01:32
+         * @LastEditTime: 2022-07-27 18:33:51
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         
         # seven_framework
         
         ## 天志互联Python开发库
         
+        ### 1.1.9 更新内容
+        * 增加http patch方法
+        
         ### 1.1.8 更新内容
         * 增加os功能
         * 处理MySQL事务OperationalError或者是InternalError异常堵塞的问题
         
         ### 1.1.7 更新内容
         * 修复aws s3 bug
```

### Comparing `seven_framework-1.1.8/seven_framework.egg-info/SOURCES.txt` & `seven_framework-1.1.9/seven_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

