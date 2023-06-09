# Comparing `tmp/nonebot_plugin_al-0.1.1.tar.gz` & `tmp/nonebot_plugin_al-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_al-0.1.1.tar` & `nonebot_plugin_al-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-05-30 14:08:53.643151 nonebot_plugin_al-0.1.1/LICENSE
--rw-r--r--   0        0        0     2198 2023-06-07 15:22:18.943516 nonebot_plugin_al-0.1.1/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0      776 2023-06-06 14:05:44.522832 nonebot_plugin_al-0.1.1/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3338 2023-06-07 15:07:11.428916 nonebot_plugin_al-0.1.1/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0    41657 2023-06-07 15:07:11.516516 nonebot_plugin_al-0.1.1/nonebot_plugin_al/ship.json
--rw-r--r--   0        0        0     1002 2023-06-07 15:09:28.649531 nonebot_plugin_al-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1566 2023-06-07 15:07:11.098960 nonebot_plugin_al-0.1.1/README.md
--rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1526 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/README.md
+-rw-r--r--   0        0        0     2133 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0      757 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3245 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0    41850 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/nonebot_plugin_al/ship.json
+-rw-r--r--   0        0        0      943 2023-06-08 04:02:09.614663 nonebot_plugin_al-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.1.1/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.1.2/nonebot_plugin_al/api.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import aiohttp
-from bs4 import BeautifulSoup
-
-async def get_data(url:str ,mode = None):
-    """获取网页内容"""
-    headers = {
-    'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
-    }
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url, headers=headers, timeout=600) as response:
-            if response.status == 200:
-                if mode == "html":
-                    html = await response.text()  # 获取网页源代码
-                    soup = BeautifulSoup(html, 'html.parser')  # 创建BeautifulSoup对象
-                    return soup
-                else:
-                    return await response.read()
-            else:
-                return None
+import aiohttp
+from bs4 import BeautifulSoup
+
+async def get_data(url:str ,mode = None):
+    """获取网页内容"""
+    headers = {
+    'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+    }
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url, headers=headers, timeout=600) as response:
+            if response.status == 200:
+                if mode == "html":
+                    html = await response.text()  # 获取网页源代码
+                    soup = BeautifulSoup(html, 'html.parser')  # 创建BeautifulSoup对象
+                    return soup
+                else:
+                    return await response.read()
+            else:
+                return None
```

### Comparing `nonebot_plugin_al-0.1.1/pyproject.toml` & `nonebot_plugin_al-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[tool.poetry]
-name = "nonebot_plugin_al"
-version = "0.1.1"
-description = "Azuer L plugin for NoneBot2"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "GPLv3"
-readme = "README.md"
-homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
-repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
-keywords = ["game", "nonebot2", "plugin","bilibili"]
-classifiers = [
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Operating System :: OS Independent",
-]
-include = [
-    "LICENSE","README.md"
-]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = ">=2.2.1"
-nonebot_plugin_htmlrender = "^2.0.0"
-aiohttp = ">=3.8.3"
-bs4 = "^0.0.1"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot_plugin_al"
+version = "0.1.2"
+description = "Azuer L plugin for NoneBot2"
+authors = ["Agnes_Digital <Z735803792@163.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
+repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
+keywords = ["game", "nonebot2", "plugin","bilibili"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Operating System :: OS Independent",
+]
+include = [
+    "LICENSE","README.md"
+]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+nonebot2 = "^2.0.0"
+nonebot-adapter-onebot = ">=2.2.1"
+nonebot_plugin_htmlrender = "^0.2.0.3"
+aiohttp = ">=3.8.3"
+bs4 = "^0.0.1"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_al-0.1.1/README.md` & `nonebot_plugin_al-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-<div align="center">
-  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
-  <br>
-  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot_plugin_AL 0.1.0
-
-_✨Nonebot & 碧蓝航线攻略✨_
-
-<a href="https://github.com/Agnes4m/nonebot_plugin_AL/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_AL" alt="stars">
-</a>
-<a href="https://github.com/Agnes4m/nonebot_plugin_AL/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_AL" alt="issues">
-</a>
-<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
-        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_AL">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_AL.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_AL">
-    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_AL" alt="pypi download">
-</a>
-    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
-
-</div>
-
-## 指令
-
-- 碧蓝帮助 | 碧蓝指令
-- 显示的指令为【碧蓝】+xxx
-
-## 功能
-
-1、b站wiki井号榜一图流
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_AL 0.1.0
+
+_✨Nonebot & 碧蓝航线攻略✨_
+
+<a href="https://github.com/Agnes4m/nonebot_plugin_AL/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_AL" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_AL/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_AL" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_AL">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_AL.svg" alt="pypi">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_AL">
+    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_AL" alt="pypi download">
+</a>
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
+
+</div>
+
+## 指令
+
+- 碧蓝帮助 | 碧蓝指令
+- 显示的指令为【碧蓝】+xxx
+
+## 功能
+
+1、b站wiki井号榜一图流
 2、舰船图鉴
```

### Comparing `nonebot_plugin_al-0.1.1/PKG-INFO` & `nonebot_plugin_al-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.1.1
+Version: 0.1.2
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
-License: GPLv3
+License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: nonebot_plugin_htmlrender (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.1.1 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.1.2 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
-License: GPLv3 Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
+License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
-License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
-License :: Other/Proprietary License Classifier: Operating System :: OS
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3) Requires-Dist: bs4
 (>=0.0.1,<0.0.2) Requires-Dist: nonebot-adapter-onebot (>=2.2.1) Requires-Dist:
 nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_htmlrender
-(>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
+(>=0.2.0.3,<0.3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
 nonebot_plugin_AL Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_AL 0.1.0 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
    [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python] [NoneBot]
 ## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ - æ¾ç¤ºçæä»¤ä¸ºãç¢§èã+xxx ##
 åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹å¾é´
```

