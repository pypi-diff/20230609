# Comparing `tmp/nonebot_plugin_escape_url-0.1.2.post2.tar.gz` & `tmp/nonebot_plugin_escape_url-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_escape_url-0.1.2.post2.tar", max compression
+gzip compressed data, was "nonebot_plugin_escape_url-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_escape_url-0.1.2.post2.tar` & `nonebot_plugin_escape_url-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      451 2023-06-02 06:48:22.685102 nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/__init__.py
--rw-r--r--   0        0        0      240 2023-06-02 00:25:18.879236 nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/config.py
--rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/core.py
--rw-r--r--   0        0        0     1148 2023-06-02 00:25:54.493031 nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/onebot_v11.py
--rw-r--r--   0        0        0      915 2023-06-02 00:25:54.503107 nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/qqguild.py
--rw-r--r--   0        0        0      552 2023-06-02 06:48:22.680100 nonebot_plugin_escape_url-0.1.2.post2/pyproject.toml
--rw-r--r--   0        0        0      223 2023-05-31 15:17:18.124586 nonebot_plugin_escape_url-0.1.2.post2/README.md
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.2.post2/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-06-02 06:48:22.685102 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-09 14:51:48.138264 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/config.py
+-rw-r--r--   0        0        0     1055 2023-06-02 02:59:27.534005 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/core.py
+-rw-r--r--   0        0        0     1323 2023-06-09 14:51:48.128268 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/onebot_v11.py
+-rw-r--r--   0        0        0     1099 2023-06-09 14:51:48.118267 nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/qqguild.py
+-rw-r--r--   0        0        0      546 2023-06-09 14:51:48.142266 nonebot_plugin_escape_url-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      448 2023-06-09 14:51:48.109265 nonebot_plugin_escape_url-0.1.3/README.md
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/core.py` & `nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/onebot_v11.py` & `nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/onebot_v11.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
+from typing import Any
+
+from nonebot import logger, Bot as BaseBot
 from nonebot.typing import overrides
 
 from .config import conf
+from .core import escape_text
 
 try:
-    from typing import Any, Union
-
-    from nonebot import logger, Bot as BaseBot
-    from nonebot.adapters.onebot.v11 import Bot, Event, Message, MessageSegment
-
-    from .core import escape_text
-
-    _origin_call_api = Bot.call_api
+    if "~onebot.v11" in conf.escape_url_ignore_adapters:
+        from nonebot.adapters.onebot.v11 import Bot, Message
 
+        _origin_call_api = Bot.call_api
 
-    @overrides(BaseBot)
-    async def call_api(self, api: str, **data: Any) -> Any:
-        if api == 'send_msg':
-            message = data.get("message", None)
 
-            if isinstance(message, str):
-                message = escape_text(message, conf.escape_url_replace_dot_by)
-            elif isinstance(message, Message):
-                for seg in message:
-                    if seg.type == 'text':
-                        seg.data['text'] = escape_text(seg.data['text'], conf.escape_url_replace_dot_by)
+        @overrides(BaseBot)
+        async def call_api(self, api: str, **data: Any) -> Any:
+            if api == 'send_msg':
+                message = data.get("message", None)
 
-            logger.trace(f"escaped message: {message}")
-            data['message'] = message
-        return await _origin_call_api(self, api, **data)
+                if isinstance(message, str):
+                    message = escape_text(message, conf.escape_url_replace_dot_by)
+                elif isinstance(message, Message):
+                    for seg in message:
+                        if seg.type == 'text':
+                            seg.data['text'] = escape_text(seg.data['text'], conf.escape_url_replace_dot_by)
 
+                logger.trace(f"escaped message: {message}")
+                data['message'] = message
+            return await _origin_call_api(self, api, **data)
 
-    Bot.call_api = call_api
 
-    logger.opt(colors=True).success("Patched <y>OneBot V11</y> Adapter")
+        Bot.call_api = call_api
 
+        logger.opt(colors=True).success("Patched <y>OneBot V11</y> Adapter")
+    else:
+        logger.opt(colors=True).info("Skipped patching <y>OneBot V11</y> Adapter")
 except ImportError as e:
     pass
```

### Comparing `nonebot_plugin_escape_url-0.1.2.post2/nonebot_plugin_escape_url/qqguild.py` & `nonebot_plugin_escape_url-0.1.3/nonebot_plugin_escape_url/qqguild.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+from functools import wraps
+
+from nonebot import logger
+
 from .config import conf
+from .core import escape_text
 
 try:
-    from functools import wraps
-
-    from nonebot import logger
     from nonebot.adapters.qqguild.api import API_HANDLERS
 
-    from .core import escape_text
-
-
-    def _patch(func):
-        @wraps(func)
-        async def wrapper(*args, **kwargs):
-            content = kwargs.get("content", None)
-            if content is not None:
-                content = escape_text(content, conf.escape_url_replace_dot_by)
-                logger.trace(f"escaped content: {content}")
-                kwargs["content"] = content
-
-            return await func(*args, **kwargs)
-
-        return wrapper
-
-
-    API_HANDLERS["post_messages"] = _patch(API_HANDLERS["post_messages"])
-    API_HANDLERS["post_dms_messages"] = _patch(API_HANDLERS["post_dms_messages"])
-
-    logger.opt(colors=True).success("Patched <y>QQ Guild</y> Adapter")
-
+    if "~qqguild" in conf.escape_url_ignore_adapters:
+        def _patch(func):
+            @wraps(func)
+            async def wrapper(*args, **kwargs):
+                content = kwargs.get("content", None)
+                if content is not None:
+                    content = escape_text(content, conf.escape_url_replace_dot_by)
+                    logger.trace(f"escaped content: {content}")
+                    kwargs["content"] = content
+
+                return await func(*args, **kwargs)
+
+            return wrapper
+
+
+        API_HANDLERS["post_messages"] = _patch(API_HANDLERS["post_messages"])
+        API_HANDLERS["post_dms_messages"] = _patch(API_HANDLERS["post_dms_messages"])
+
+        logger.opt(colors=True).success("Patched <y>QQ Guild</y> Adapter")
+    else:
+        logger.opt(colors=True).info("Skipped patching <y>QQ Guild</y> Adapter")
 except ImportError as e:
     pass
```

### Comparing `nonebot_plugin_escape_url-0.1.2.post2/pyproject.toml` & `nonebot_plugin_escape_url-0.1.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-escape-url"
-version = "0.1.2.post2"
+version = "0.1.3"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_escape_url" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

