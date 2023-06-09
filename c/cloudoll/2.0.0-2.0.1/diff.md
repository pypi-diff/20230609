# Comparing `tmp/cloudoll-2.0.0.tar.gz` & `tmp/cloudoll-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.0.0.tar", last modified: Fri Jun  9 06:35:35 2023, max compression
+gzip compressed data, was "cloudoll-2.0.1.tar", last modified: Fri Jun  9 07:31:10 2023, max compression
```

## Comparing `cloudoll-2.0.0.tar` & `cloudoll-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.378219 cloudoll-2.0.0/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.0/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     7008 2023-06-09 06:35:35.377763 cloudoll-2.0.0/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     6375 2023-06-09 06:22:48.000000 cloudoll-2.0.0/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.363990 cloudoll-2.0.0/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.368538 cloudoll-2.0.0/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.369127 cloudoll-2.0.0/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.0/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.370114 cloudoll-2.0.0/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.0/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.371453 cloudoll-2.0.0/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    27881 2023-06-08 13:00:49.000000 cloudoll-2.0.0/cloudoll/orm/mysql.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.373657 cloudoll-2.0.0/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.0/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.0/cloudoll/robot/feishu.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.376835 cloudoll-2.0.0/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    13406 2023-06-08 12:53:24.000000 cloudoll-2.0.0/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.0/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.0/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.0/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.367489 cloudoll-2.0.0/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7008 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      103 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-06-09 06:35:35.378354 cloudoll-2.0.0/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4158 2023-06-09 06:34:21.000000 cloudoll-2.0.0/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.144483 cloudoll-2.0.1/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.1/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7019 2023-06-09 07:31:10.143629 cloudoll-2.0.1/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6386 2023-06-09 06:38:19.000000 cloudoll-2.0.1/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.130463 cloudoll-2.0.1/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.134906 cloudoll-2.0.1/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.135388 cloudoll-2.0.1/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.1/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.136384 cloudoll-2.0.1/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.1/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.137607 cloudoll-2.0.1/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    27881 2023-06-08 13:00:49.000000 cloudoll-2.0.1/cloudoll/orm/mysql.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.139447 cloudoll-2.0.1/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.1/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.1/cloudoll/robot/feishu.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.142777 cloudoll-2.0.1/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    13406 2023-06-08 12:53:24.000000 cloudoll-2.0.1/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.1/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.1/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.1/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.1/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 07:31:10.133597 cloudoll-2.0.1/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7019 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      104 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-06-09 07:31:10.000000 cloudoll-2.0.1/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-06-09 07:31:10.144885 cloudoll-2.0.1/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4153 2023-06-09 07:30:50.000000 cloudoll-2.0.1/setup.py
```

### Comparing `cloudoll-2.0.0/LICENSE` & `cloudoll-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/PKG-INFO` & `cloudoll-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.0
+Version: 2.0.1
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -38,24 +38,35 @@
 - 增加websocket 支持
 
 
 ## Documentation
 
 
 [Docs](https://cloudoll.chuchur.com)
+
 [Docs](https://cloudoll.chuchur.com)
+
 [Structure](https://cloudoll.chuchur.com/structure)
+
 [Config](https://cloudoll.chuchur.com/config)
+
 [Middleware](https://cloudoll.chuchur.com/middleware)
+
 [Router](https://cloudoll.chuchur.com/router)
+
 [View](https://cloudoll.chuchur.com/view)
+
 [Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
+
 [Upload file](https://cloudoll.chuchur.com/file-uploads)
+
 [WebSocket](https://cloudoll.chuchur.com/websockets)
+
 [Mysql](https://cloudoll.chuchur.com/mysql)
+
 [Deployment](https://cloudoll.chuchur.com/deployment)
 
 
 ## 环境准备
 
 - 操作系统：支持 macOS，Linux，Windows
 - 运行环境：最低要求 3.6.0。
```

### Comparing `cloudoll-2.0.0/README.md` & `cloudoll-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,35 @@
 - 增加websocket 支持
 
 
 ## Documentation
 
 
 [Docs](https://cloudoll.chuchur.com)
+
 [Docs](https://cloudoll.chuchur.com)
+
 [Structure](https://cloudoll.chuchur.com/structure)
+
 [Config](https://cloudoll.chuchur.com/config)
+
 [Middleware](https://cloudoll.chuchur.com/middleware)
+
 [Router](https://cloudoll.chuchur.com/router)
+
 [View](https://cloudoll.chuchur.com/view)
+
 [Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
+
 [Upload file](https://cloudoll.chuchur.com/file-uploads)
+
 [WebSocket](https://cloudoll.chuchur.com/websockets)
+
 [Mysql](https://cloudoll.chuchur.com/mysql)
+
 [Deployment](https://cloudoll.chuchur.com/deployment)
 
 
 ## 环境准备
 
 - 操作系统：支持 macOS，Linux，Windows
 - 运行环境：最低要求 3.6.0。
```

### Comparing `cloudoll-2.0.0/cloudoll/error/errors.py` & `cloudoll-2.0.1/cloudoll/error/errors.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/logging/__init__.py` & `cloudoll-2.0.1/cloudoll/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/mail/smtp.py` & `cloudoll-2.0.1/cloudoll/mail/smtp.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/orm/mysql.py` & `cloudoll-2.0.1/cloudoll/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.1/cloudoll/robot/dingtalk.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/robot/feishu.py` & `cloudoll-2.0.1/cloudoll/robot/feishu.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/web/__init__.py` & `cloudoll-2.0.1/cloudoll/web/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/web/html.py` & `cloudoll-2.0.1/cloudoll/web/html.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/web/http.py` & `cloudoll-2.0.1/cloudoll/web/http.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll/web/jwt.py` & `cloudoll-2.0.1/cloudoll/web/jwt.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.0.1/cloudoll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.0
+Version: 2.0.1
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -38,24 +38,35 @@
 - 增加websocket 支持
 
 
 ## Documentation
 
 
 [Docs](https://cloudoll.chuchur.com)
+
 [Docs](https://cloudoll.chuchur.com)
+
 [Structure](https://cloudoll.chuchur.com/structure)
+
 [Config](https://cloudoll.chuchur.com/config)
+
 [Middleware](https://cloudoll.chuchur.com/middleware)
+
 [Router](https://cloudoll.chuchur.com/router)
+
 [View](https://cloudoll.chuchur.com/view)
+
 [Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
+
 [Upload file](https://cloudoll.chuchur.com/file-uploads)
+
 [WebSocket](https://cloudoll.chuchur.com/websockets)
+
 [Mysql](https://cloudoll.chuchur.com/mysql)
+
 [Deployment](https://cloudoll.chuchur.com/deployment)
 
 
 ## 环境准备
 
 - 操作系统：支持 macOS，Linux，Windows
 - 运行环境：最低要求 3.6.0。
```

### Comparing `cloudoll-2.0.0/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.1/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.0/setup.py` & `cloudoll-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 # Package meta-data.
 NAME = "cloudoll"
 DESCRIPTION = "辅助快速创建可分布的微服务。"
 URL = "https://gitee.com/chuchur/cloudoll-py"
 EMAIL = "chuchur@qq.com"
 AUTHOR = "chuchur"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.0.0"
+VERSION = "2.0.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "colorlog",
     "aiomysql",
     "aiopg",
     "aiohttp",
     "aioredis",
-    "aiomcache"
+    "aiomcache",
     "jinja2",
     "pyjwt",
     "aiohttp_session[secure]",
     "PyYAML",
 ]
 
 # What packages are optional?
@@ -91,17 +91,17 @@
 
         self.status("Building Source and Wheel (universal) distribution…")
         os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
         self.status("Uploading the package to PyPI via Twine…")
         os.system("twine upload dist/*")
 
-        # self.status("Pushing git tags…")
-        # os.system("git tag v{0}".format(about["__version__"]))
-        # os.system("git push --tags")
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
```

