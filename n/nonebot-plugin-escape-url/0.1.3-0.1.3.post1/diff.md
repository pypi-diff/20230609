# Comparing `tmp/nonebot_plugin_escape_url-0.1.3.tar.gz` & `tmp/nonebot_plugin_escape_url-0.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_escape_url-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_escape_url-0.1.3.post1.tar", max compression
```

## Comparing `nonebot_plugin_escape_url-0.1.3.tar` & `nonebot_plugin_escape_url-0.1.3.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      451 2023-06-02 06:48:22.685102 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/__init__.py
--rw-r--r--   0        0        0      315 2023-06-09 14:51:48.138264 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/config.py
--rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/core.py
--rw-r--r--   0        0        0     1323 2023-06-09 14:51:48.128268 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/onebot_v11.py
--rw-r--r--   0        0        0     1099 2023-06-09 14:51:48.118267 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/qqguild.py
--rw-r--r--   0        0        0      546 2023-06-09 14:51:48.142266 nonebot_plugin_escape_url-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      448 2023-06-09 14:51:48.109265 nonebot_plugin_escape_url-0.1.3/README.md
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-06-02 06:48:22.685102 nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-09 14:51:48.138264 nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/config.py
+-rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/core.py
+-rw-r--r--   0        0        0     1327 2023-06-09 14:54:03.672741 nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/onebot_v11.py
+-rw-r--r--   0        0        0     1103 2023-06-09 14:54:03.668728 nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/qqguild.py
+-rw-r--r--   0        0        0      552 2023-06-09 14:54:03.677744 nonebot_plugin_escape_url-0.1.3.post1/pyproject.toml
+-rw-r--r--   0        0        0      448 2023-06-09 14:51:48.109265 nonebot_plugin_escape_url-0.1.3.post1/README.md
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.3.post1/PKG-INFO
```

### Comparing `nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/core.py` & `nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/onebot_v11.py` & `nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/onebot_v11.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from nonebot import logger, Bot as BaseBot
 from nonebot.typing import overrides
 
 from .config import conf
 from .core import escape_text
 
 try:
-    if "~onebot.v11" in conf.escape_url_ignore_adapters:
+    if "~onebot.v11" not in conf.escape_url_ignore_adapters:
         from nonebot.adapters.onebot.v11 import Bot, Message
 
         _origin_call_api = Bot.call_api
 
 
         @overrides(BaseBot)
         async def call_api(self, api: str, **data: Any) -> Any:
```

### Comparing `nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/qqguild.py` & `nonebot_plugin_escape_url-0.1.3.post1/nonebot_plugin_escape_url/qqguild.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .config import conf
 from .core import escape_text
 
 try:
     from nonebot.adapters.qqguild.api import API_HANDLERS
 
-    if "~qqguild" in conf.escape_url_ignore_adapters:
+    if "~qqguild" not in conf.escape_url_ignore_adapters:
         def _patch(func):
             @wraps(func)
             async def wrapper(*args, **kwargs):
                 content = kwargs.get("content", None)
                 if content is not None:
                     content = escape_text(content, conf.escape_url_replace_dot_by)
                     logger.trace(f"escaped content: {content}")
```

### Comparing `nonebot_plugin_escape_url-0.1.3/pyproject.toml` & `nonebot_plugin_escape_url-0.1.3.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-escape-url"
-version = "0.1.3"
+version = "0.1.3.post1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_escape_url" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_escape_url-0.1.3/PKG-INFO` & `nonebot_plugin_escape_url-0.1.3.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-escape-url
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

