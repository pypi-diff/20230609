# Comparing `tmp/nonebot_plugin_animeres-1.0.1.tar.gz` & `tmp/nonebot_plugin_animeres-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animeres-1.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_animeres-1.0.2.tar", max compression
```

## Comparing `nonebot_plugin_animeres-1.0.1.tar` & `nonebot_plugin_animeres-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.1/LICENSE
--rw-r--r--   0        0        0     3155 2023-06-01 02:27:06.839785 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/__init__.py
--rw-r--r--   0        0        0      447 2023-05-30 11:50:00.391161 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/config.py
--rw-r--r--   0        0        0     2761 2023-06-01 02:07:17.139133 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/internal.py
--rw-r--r--   0        0        0     1979 2023-06-01 01:55:55.418675 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/__init__.py
--rw-r--r--   0        0        0     1235 2023-06-01 02:27:45.060418 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/dongmanhuayuan.py
--rw-r--r--   0        0        0     1557 2023-05-30 11:50:29.754653 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/myheartsite.py
--rw-r--r--   0        0        0     1036 2023-05-30 12:07:42.320956 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/schemas.py
--rw-r--r--   0        0        0     1558 2023-05-30 08:09:48.266513 nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/utils.py
--rw-r--r--   0        0        0      946 2023-06-01 02:33:34.562119 nonebot_plugin_animeres-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1648 2023-06-01 02:29:30.768042 nonebot_plugin_animeres-1.0.1/README.md
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3155 2023-06-09 01:27:44.790697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-09 01:27:42.657061 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/config.py
+-rw-r--r--   0        0        0     2763 2023-06-09 01:27:44.930697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/internal.py
+-rw-r--r--   0        0        0     2284 2023-06-09 01:27:42.677060 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/__init__.py
+-rw-r--r--   0        0        0     1186 2023-06-09 01:27:44.792697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/anoneko.py
+-rw-r--r--   0        0        0     1239 2023-06-09 01:27:44.787697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/dongmanhuayuan.py
+-rw-r--r--   0        0        0     1559 2023-06-09 01:27:42.699063 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/myheartsite.py
+-rw-r--r--   0        0        0     1040 2023-06-09 01:27:42.704060 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/schemas.py
+-rw-r--r--   0        0        0     1562 2023-06-09 01:27:42.712059 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/utils.py
+-rw-r--r--   0        0        0     1092 2023-06-09 01:00:48.674867 nonebot_plugin_animeres-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2009 2023-06-08 08:50:27.156567 nonebot_plugin_animeres-1.0.2/README.md
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_animeres-1.0.1/LICENSE` & `nonebot_plugin_animeres-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/__init__.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from nonebot import on_command
 from nonebot.typing import T_State
-from nonebot.params import CommandArg, ArgPlainText
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
-from nonebot.adapters import Message, Bot, Event
+from nonebot.adapters import Bot, Event, Message
+from nonebot.params import CommandArg, ArgPlainText
 
-from .config import Config, plugin_config
 from .resources import search
-from .internal import BaseAnimeSearch
 from .utils import send_forward
+from .internal import BaseAnimeSearch
+from .config import Config, plugin_config
 
 anime_res_cmd = on_command(
     "资源", aliases={"动漫资源"}, priority=plugin_config.animeres_priority
 )
 
 
 @anime_res_cmd.handle()
```

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/internal.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional
-from fake_useragent import UserAgent
 
 from httpx import AsyncClient
+from fake_useragent import UserAgent
+
 from .config import plugin_config
-from .schemas import AnimeRes, Tag
+from .schemas import Tag, AnimeRes
 
 
 class BaseAnimeSearch(ABC):
     """动漫资源搜索基类"""
 
     name: str = ""
     base_url: Optional[str] = None
```

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/__init__.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from typing import Dict, Optional, Type
-from nonebot.log import logger
+from typing import Dict, Type, Optional
 
 from httpx import ConnectError
+from nonebot.log import logger
+
+from ..config import plugin_config
+from ..internal import BaseAnimeSearch
+from .anoneko import AnimeSearch as AnonekoSearch
 from .myheartsite import AnimeSearch as MyHeartSiteSearch
 from .dongmanhuayuan import AnimeSearch as DongManHuaYuanSearch
-from ..internal import BaseAnimeSearch
-from ..config import plugin_config
 
 site: Dict[str, Type[BaseAnimeSearch]] = {
     MyHeartSiteSearch.name: MyHeartSiteSearch,
     DongManHuaYuanSearch.name: DongManHuaYuanSearch,
+    AnonekoSearch.name: AnonekoSearch,
 }
 
 
 async def search(keyword: str) -> Optional[BaseAnimeSearch]:
     """对站点资源进行搜索
 
     Args:
@@ -27,30 +30,30 @@
         if animeres := await search("海贼王"):
             tags = await animeres.get_tags()
             print(tags)
             anime_list = await animeres.get_resources(tags[0])
             print(anime_list)
         ```
     """
-    print(plugin_config.animeres_site)
-    if plugin_config.animeres_site is not None:
-        if anime_search := site.get(plugin_config.animeres_site):
+    if plugin_config.animeres_site is not None:  # 当配置项中有填写资源站点的情况下
+        logger.info(f"使用资源站点 '{plugin_config.animeres_site}'")
+        if anime_search := site.get(plugin_config.animeres_site):  # 获取对应资源站点
             try:
                 search_ = anime_search()
-                if await search_.search(keyword):
+                if await search_.search(keyword):  # 进行搜索
                     return search_
             except ConnectError:
                 logger.error(
                     f"ConnectError: '{plugin_config.animeres_site}' 资源链接失败，尝试为您切换站点"
                 )
-    for i in site:
+    for i in site:  # 如果未能搜索到资源则依次搜索
         search_ = site[i]()
         try:
             if await search_.search(keyword):
-                plugin_config.animeres_site = i
+                plugin_config.animeres_site = i  # 当搜索成功后切换站点
                 logger.success(f"已切换至 '{i}' 站点")
                 return search_
         except ConnectError:
             logger.error(f"ConnectError: '{i}' 资源链接失败，尝试为您切换站点")
     else:
         logger.error("所有站点资源链接失败，可能站点失效或者查网络连接的原因！")
         return None
```

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/dongmanhuayuan.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/dongmanhuayuan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import List
+
 from lxml import etree
-from ..internal import BaseAnimeSearch
-from ..schemas import AnimeRes, Tag
+
 from ..config import plugin_config
+from ..schemas import Tag, AnimeRes
+from ..internal import BaseAnimeSearch
 
 
 class AnimeSearch(BaseAnimeSearch):
     name = "dongmanhuayuan"
     base_url = "https://www.dongmanhuayuan.com"
 
     async def search(self, keyword: str) -> bool:
```

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/resources/myheartsite.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/myheartsite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
+
 from ..config import plugin_config
+from ..schemas import Tag, AnimeRes
 from ..internal import BaseAnimeSearch
-from ..schemas import AnimeRes, Tag
 
 
 class AnimeSearch(BaseAnimeSearch):
     name: str = "myheartsite"
     base_url: str = "https://dmhy.myheartsite.com"
 
     async def search(self, keyword: str) -> bool:
```

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/schemas.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from pydantic import BaseModel, Extra
-from typing import Optional, Union
+from typing import Union, Optional
+
+from pydantic import Extra, BaseModel
+
 from .config import plugin_config
 
 
 class AnimeRes(BaseModel, extra=Extra.allow):
     """动漫资源"""
 
     title: str  # 标题
```

### Comparing `nonebot_plugin_animeres-1.0.1/nonebot_plugin_animeres/utils.py` & `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List
+
 from nonebot.adapters import Event
+
 from .schemas import AnimeRes
 
 
 def forward(user_id: int, anime_res: List[AnimeRes]):
     """合并转发消息"""
     return [
         {
@@ -33,17 +35,17 @@
         await bot.call_api(
             **send_forward(event, anime_res)
         )
         ```
     """
     try:
         from nonebot.adapters.onebot.v11 import (
+            MessageEvent,
             GroupMessageEvent,
             PrivateMessageEvent,
-            MessageEvent,
         )
 
         if isinstance(event, MessageEvent):
             msg: dict = {
                 "messages": forward(event.self_id, anime_res),
             }
             if isinstance(event, GroupMessageEvent):
```

### Comparing `nonebot_plugin_animeres-1.0.1/pyproject.toml` & `nonebot_plugin_animeres-1.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 [tool.poetry]
 name = "nonebot-plugin-animeres"
-version = "1.0.1"
+version = "1.0.2"
 description = "动漫资源获取插件"
 authors = ["MelodyKnit <2711402357@qq.com>"]
 readme = "README.md"
 license = "GPL-2.0"
 packages = [{include = "nonebot_plugin_animeres"}]
 keywords = ["nonebot", "nonebot2", "animeres", "anime"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0rc1", extras = ["fastapi"] }
-httpx = "^0.24.1"
 lxml = "^4.9.2"
-nonebot-adapter-onebot = { version = "^2.2.3", optional = true }
 fake-useragent = "^1.1.3"
+httpx = ">=0.20.0,<1.0.0"
+nonebot2 = { version = "^2.0.0rc1", extras = ["fastapi"] }
+nonebot-adapter-onebot = { version = "^2.2.3", optional = true }
+
+[tool.poetry.group.dev.dependencies]
+pycln = "^2.1.2"
+isort = "^5.10.1"
+black = "^23.1.0"
+flake8 = "^4.0.1"
+pre-commit = "^3.0.0"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 extend-exclude = '''
 '''
```

### Comparing `nonebot_plugin_animeres-1.0.1/README.md` & `nonebot_plugin_animeres-1.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # 动漫资源获取插件
 
 这个插件主要是网站爬取过来的数据，在使用命令进行搜索时候采用关键字的方式，比如`天气之子`这时搜索的是`天气之子`相关资源，如果获取的资源并不理想或者你只需要生肉（无字幕）资源时，你就需要用`天气之子 raw`或`天气之子 mkv`这种多个关键字空格方式进行获取，这种方式准确度会比直接用`天气之子`精准且效果好，建议采用多关键字的方式进行搜索。
 
+## 使用例子
+
+![使用例子](image/demo.png)
+
 ## 安装
 
 `nb plugin install nonebot-plugin-animeres`
 
 <details>
   <summary>使用pip安装</summary>
 
@@ -18,29 +22,39 @@
   - `资源名称`
 
 ## 配置参数
 
 ```env
 ANIMERES_PROXY=""                      # 设置代理端口
 ANIMERES_SITE=""                       # 选择资源站点
-ANIMERES_FORWARD=false                 # 合并转发的形式发送消息
+ANIMERES_FORWARD=false                 # 适用于QQ的转发形式发送
 ANIMERES_LENGTH=3                      # 每次发送的数量，用-1表示全部取出
 ANIMERES_FORMANT="{title}\n{magnet}"   # 发送的消息格式化
 ANIMERES_ONESKIP=true                  # 当只有一个选项时跳过
 ANIEMRES_PRIORITY=100
 
 ```
 
 ### ANIMERES_PROXY
 
 通过`ANIMERES_PROXY`参数可以设置代理来加速资源的获取或者获取不到的情况
 
+> ANIMERES_PROXY = `http://127.0.0.1:1080`
+
+### ANIMERES_SITE
+
+有些情况下可能某站点关闭或者当前网络访问这个站点不佳可以尝试切换到其它站点，具体可切换站点如下。
+
+- `dongmanhuayuan`
+- `myheartsite`
+- `anoneko`（需要设置代理）
+
 ### ANIMERES_FORWARD
 
-用来发送合并消息
+在QQ中使用的合并转发发送消息
 
 ![合并消息转发](image/forward.png)
 
 ### ANIMERES_FORMANT
 
 格式化字符串
```

### Comparing `nonebot_plugin_animeres-1.0.1/PKG-INFO` & `nonebot_plugin_animeres-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-animeres
-Version: 1.0.1
+Version: 1.0.2
 Summary: 动漫资源获取插件
 License: GPL-2.0
 Keywords: nonebot,nonebot2,animeres,anime
 Author: MelodyKnit
 Author-email: 2711402357@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 动漫资源获取插件
 
 这个插件主要是网站爬取过来的数据，在使用命令进行搜索时候采用关键字的方式，比如`天气之子`这时搜索的是`天气之子`相关资源，如果获取的资源并不理想或者你只需要生肉（无字幕）资源时，你就需要用`天气之子 raw`或`天气之子 mkv`这种多个关键字空格方式进行获取，这种方式准确度会比直接用`天气之子`精准且效果好，建议采用多关键字的方式进行搜索。
 
+## 使用例子
+
+![使用例子](image/demo.png)
+
 ## 安装
 
 `nb plugin install nonebot-plugin-animeres`
 
 <details>
   <summary>使用pip安装</summary>
 
@@ -40,29 +44,39 @@
   - `资源名称`
 
 ## 配置参数
 
 ```env
 ANIMERES_PROXY=""                      # 设置代理端口
 ANIMERES_SITE=""                       # 选择资源站点
-ANIMERES_FORWARD=false                 # 合并转发的形式发送消息
+ANIMERES_FORWARD=false                 # 适用于QQ的转发形式发送
 ANIMERES_LENGTH=3                      # 每次发送的数量，用-1表示全部取出
 ANIMERES_FORMANT="{title}\n{magnet}"   # 发送的消息格式化
 ANIMERES_ONESKIP=true                  # 当只有一个选项时跳过
 ANIEMRES_PRIORITY=100
 
 ```
 
 ### ANIMERES_PROXY
 
 通过`ANIMERES_PROXY`参数可以设置代理来加速资源的获取或者获取不到的情况
 
+> ANIMERES_PROXY = `http://127.0.0.1:1080`
+
+### ANIMERES_SITE
+
+有些情况下可能某站点关闭或者当前网络访问这个站点不佳可以尝试切换到其它站点，具体可切换站点如下。
+
+- `dongmanhuayuan`
+- `myheartsite`
+- `anoneko`（需要设置代理）
+
 ### ANIMERES_FORWARD
 
-用来发送合并消息
+在QQ中使用的合并转发发送消息
 
 ![合并消息转发](image/forward.png)
 
 ### ANIMERES_FORMANT
 
 格式化字符串
```

