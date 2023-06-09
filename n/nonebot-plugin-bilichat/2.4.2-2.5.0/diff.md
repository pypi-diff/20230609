# Comparing `tmp/nonebot_plugin_bilichat-2.4.2.tar.gz` & `tmp/nonebot_plugin_bilichat-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.4.2.tar", last modified: Fri Jun  9 14:15:41 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.5.0.tar", last modified: Fri Jun  9 16:36:34 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.4.2.tar` & `nonebot_plugin_bilichat-2.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-09 14:15:33.823675 nonebot_plugin_bilichat-2.4.2/LICENSE
--rw-r--r--   0        0        0    12555 2023-06-09 14:15:33.823675 nonebot_plugin_bilichat-2.4.2/README.md
--rw-r--r--   0        0        0     8790 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4914 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6463 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    11809 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1499 2023-06-09 14:15:41.951746 nonebot_plugin_bilichat-2.4.2/pyproject.toml
--rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-09 16:36:23.265984 nonebot_plugin_bilichat-2.5.0/LICENSE
+-rw-r--r--   0        0        0    12555 2023-06-09 16:36:23.265984 nonebot_plugin_bilichat-2.5.0/README.md
+-rw-r--r--   0        0        0     9322 2023-06-09 16:36:23.273984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-09 16:36:23.273984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-09 16:36:23.273984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6463 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    11820 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1499 2023-06-09 16:36:34.534059 nonebot_plugin_bilichat-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.4.2/LICENSE` & `nonebot_plugin_bilichat-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/README.md` & `nonebot_plugin_bilichat-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
 from nonebot.adapters.qqguild import Bot as QG_Bot
 from nonebot.adapters.qqguild.event import MessageEvent as QG_ME
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
-from nonebot.params import Depends, RegexGroup, RegexStr
-from nonebot.plugin import PluginMetadata, on_regex, require
+from nonebot.params import Depends
+from nonebot.plugin import PluginMetadata, on_message, require
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_column_basic, get_content_cache, get_video_basic
 from .model.arguments import Options, parser
@@ -66,18 +66,36 @@
         "version": __version__,
         "priority": 1,
     },
 )
 
 
 async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
+    # 检查并提取 raw_bililink
+    if plugin_config.bilichat_only_self and isinstance(event, V11_ME) and event.reply:
+        # 仅自身的情况下，检查是否是回复，是的话则取被回复的消息
+        msg = str(event.reply.message)
+    else:
+        # 其余情况取该条消息
+        msg = str(event.get_message())
+
+    for seg in ("av", "BV", "cv", "b23"):
+        if seg in msg:
+            state["_raw_bililink_"] = msg
+            return True
+    return False
+
+
+async def _permission_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
+    # 检查权限
     # check if self msg
     if str(event.get_user_id()) == str(bot.self_id):
         if plugin_config.bilichat_only_self:
             state["_uid_"] = event.get_session_id()
+            print("_permission_check true")
             return True
         elif not plugin_config.bilichat_enable_self:
             return False
     elif plugin_config.bilichat_only_self:
         return False
     # private msg use user id
     if isinstance(event, (V11_PME, V12_PME, Mirai_PME)):
@@ -96,59 +114,51 @@
         return plugin_config.bilichat_enable_channel
     # other
     else:
         state["_uid_"] = "unkown"
         return plugin_config.bilichat_enable_unkown_src
 
 
-bili = on_regex(
-    r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})",
-    block=plugin_config.bilichat_block,
-    priority=1,
-    rule=Rule(_bili_check),
-)
-
-b23 = on_regex(
-    r"b23.(tv|wtf)[\\/]+(\w+)",
+bilichat = on_message(
     block=plugin_config.bilichat_block,
     priority=1,
-    rule=Rule(_bili_check),
+    rule=Rule(_permission_check, _bili_check),
 )
 
 
 def get_args(event: MESSAGE_EVENT):
     return parser.parse_known_args(
         list(
             chain.from_iterable(
                 shlex.split(str(seg)) if cast(MessageSegment, seg).is_text() else (seg,) for seg in event.get_message()
             )
         ),  # type: ignore
         namespace=Options(),
     )[0]
 
 
-@bili.handle()
-async def get_bili_number_re(state: T_State, bili_number: str = RegexStr()):
-    state["bili_number"] = bili_number
-
-
-@b23.handle()
-async def get_bili_number_b23(state: T_State, b23: Tuple = RegexGroup()):
-    bililink = await b23_extract(list(b23))
+@bilichat.handle()
+async def get_bili_number(state: T_State):
+    raw_bililink = state["_raw_bililink_"]
+    # 如果是 B23 格式的链接，先转为正常的链接
+    if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", raw_bililink):  # type: ignore
+        bililink = await b23_extract(list(b23.groups()))
+    else:
+        bililink = raw_bililink
+    # 提取其 AV BV CV 号
     if matched := re.search(
         r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})", bililink  # type: ignore
     ):
         state["bili_number"] = matched.group()
     else:
         logger.info(f"{bililink} is not video or column")
         raise FinishedException
 
 
-@bili.handle()
-@b23.handle()
+@bilichat.handle()
 async def video_info(
     bot: BOT,
     event: MESSAGE_EVENT,
     state: T_State,
     matcher: Matcher,
     options: Options = Depends(get_args),
 ):
```

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         fans: str,
         title: str = "UP主",
         name_color: str = "black",
     ) -> None:
         self.name: str = name
         self.face: BytesIO = face if isinstance(face, BytesIO) else BytesIO(face)
         self.level: int = level
-        self.name_color: str = name_color
+        self.name_color: str = name_color or "black"
         self.fans: str = fans
         self.title: str = title
 
     @classmethod
     async def from_id(cls, client: AsyncClient, mid: int, name: str, title: str):
         try:
             up_data = await get_user_space_info(mid)
```

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.2/pyproject.toml` & `nonebot_plugin_bilichat-2.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.4.2"
+version = "2.5.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.4.2/PKG-INFO` & `nonebot_plugin_bilichat-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.4.2
+Version: 2.5.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.4.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.5.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

