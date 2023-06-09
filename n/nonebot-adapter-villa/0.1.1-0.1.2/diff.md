# Comparing `tmp/nonebot_adapter_villa-0.1.1.tar.gz` & `tmp/nonebot_adapter_villa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.1.2.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.1.1.tar` & `nonebot_adapter_villa-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/LICENSE
--rw-r--r--   0        0        0     4154 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/README.md
--rw-r--r--   0        0        0      235 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0     4668 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     3247 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     4109 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    13301 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9952 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    11111 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      263 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0     8936 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6279 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4154 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/README.md
+-rw-r--r--   0        0        0      235 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0     4668 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     3247 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     4109 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    13301 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9952 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    11473 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      263 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0     8936 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6279 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.1.2/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.1.1/LICENSE` & `nonebot_adapter_villa-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/README.md` & `nonebot_adapter_villa-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/bot.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from nonebot.typing import overrides
 from nonebot.message import handle_event
 from nonebot.internal.adapter.adapter import Adapter
 
 from nonebot.adapters import Bot as BaseBot
 
+from .utils import log
 from .event import Event, SendMessageEvent
 from .message import Message, MessageSegment
 from .api import (
     Link,
     Image,
     Robot,
     ApiClient,
@@ -217,107 +218,115 @@
             quote = quote[-1]
             quote = QuoteInfo(
                 quoted_message_id=quote.data["msg_id"],
                 quoted_message_send_time=quote.data["msg_send_time"],
                 original_message_id=quote.data["msg_id"],
                 original_message_send_time=quote.data["msg_send_time"],
             )
-
+        if images_msg := (message["image"] or None):
+            images = [
+                Image(
+                    url=seg.data["url"],
+                    size=ImageSize(width=seg.data["width"], height=seg.data["height"])
+                    if seg.data["width"] and seg.data["height"]
+                    else None,
+                    file_size=seg.data["file_size"],
+                )
+                for seg in images_msg
+            ]
+        else:
+            images = None
+        cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
-        images: List[Image] = []
         mentioned = MentionedInfo(type=MentionType.PART)
         for seg in message:
-            if seg.type == "text":
-                message_text += seg.data["text"]
-                message_offset += len(seg.data["text"])
-            elif seg.type == "mention_all":
-                message_text += f"@{seg.data['show_text']} "
-                entities.append(
-                    TextEntity(
-                        offset=message_offset,
-                        length=6,
-                        entity=MentionedAll(show_text=seg.data["show_text"]),
+            try:
+                if seg.type in ("quote", "image"):
+                    continue
+                if seg.type == "text":
+                    seg_text = seg.data["text"]
+                    length = cal_len(seg_text)
+                elif seg.type == "mention_all":
+                    seg_text = f"@{seg.data['show_text']} "
+                    length = cal_len(seg_text)
+                    entities.append(
+                        TextEntity(
+                            offset=message_offset,
+                            length=length,
+                            entity=MentionedAll(show_text=seg.data["show_text"]),
+                        )
                     )
-                )
-                message_offset += 6
-                mentioned.type = MentionType.ALL
-            elif seg.type == "mentioned_robot":
-                message_text += f"@{seg.data['bot_name']} "
-                entities.append(
-                    TextEntity(
-                        offset=message_offset,
-                        length=len(f"@{seg.data['bot_name']}".encode("utf-16")) // 2,
-                        entity=MentionedRobot(
-                            bot_id=seg.data["bot_id"], bot_name=seg.data["bot_name"]
-                        ),
+                    mentioned.type = MentionType.ALL
+                elif seg.type == "mentioned_robot":
+                    seg_text = f"@{seg.data['bot_name']} "
+                    length = cal_len(seg_text)
+                    entities.append(
+                        TextEntity(
+                            offset=message_offset,
+                            length=length,
+                            entity=MentionedRobot(
+                                bot_id=seg.data["bot_id"], bot_name=seg.data["bot_name"]
+                            ),
+                        )
                     )
-                )
-                message_offset += len(f"@{seg.data['bot_name']}") + 1
-                mentioned.user_id_list.append(seg.data["bot_id"])
-            elif seg.type == "mentioned_user":
-                # 需要调用API获取被@的用户的昵称
-                user = await self.get_member(
-                    villa_id=seg.data["villa_id"], uid=seg.data["user_id"]
-                )
-                message_text += f"@{user.basic.nickname} "
-                entities.append(
-                    TextEntity(
-                        offset=message_offset,
-                        length=len(f"@{user.basic.nickname}".encode("utf-16")) // 2,
-                        entity=MentionedUser(
-                            user_id=str(user.basic.uid), user_name=user.basic.nickname
-                        ),
+                    mentioned.user_id_list.append(seg.data["bot_id"])
+                elif seg.type == "mentioned_user":
+                    # 需要调用API获取被@的用户的昵称
+                    user = await self.get_member(
+                        villa_id=seg.data["villa_id"], uid=seg.data["user_id"]
                     )
-                )
-                message_offset += len(f"@{user.basic.nickname}") + 1
-                mentioned.user_id_list.append(str(user.basic.uid))
-            elif seg.type == "villa_room_link":
-                # 需要调用API获取房间的名称
-                room = await self.get_room(
-                    villa_id=seg.data["villa_id"], room_id=seg.data["room_id"]
-                )
-                message_text += f"#{room.room_name} "
-                entities.append(
-                    TextEntity(
-                        offset=message_offset,
-                        length=len(f"#{room.room_name}".encode("utf-16")) // 2,
-                        entity=VillaRoomLink(
-                            villa_id=str(seg.data["villa_id"]),
-                            room_id=str(seg.data["room_id"]),
-                            room_name=room.room_name,
-                        ),
+                    seg_text = f"@{user.basic.nickname} "
+                    length = cal_len(seg_text)
+                    entities.append(
+                        TextEntity(
+                            offset=message_offset,
+                            length=length,
+                            entity=MentionedUser(
+                                user_id=str(user.basic.uid),
+                                user_name=user.basic.nickname,
+                            ),
+                        )
                     )
-                )
-                message_offset += len(f"#{room.room_name} ")
-            elif seg.type == "link":
-                message_text += seg.data["show_text"]
-                entities.append(
-                    TextEntity(
-                        offset=message_offset,
-                        length=len(seg.data["show_text"].encode("utf-16")) // 2,
-                        entity=Link(
-                            url=seg.data["url"], show_text=seg.data["show_text"]
-                        ),
+                    mentioned.user_id_list.append(str(user.basic.uid))
+                elif seg.type == "villa_room_link":
+                    # 需要调用API获取房间的名称
+                    room = await self.get_room(
+                        villa_id=seg.data["villa_id"], room_id=seg.data["room_id"]
                     )
-                )
-                message_offset += len(seg.data["show_text"]) + 1
-            elif seg.type == "image":
-                images.append(
-                    Image(
-                        url=seg.data["url"],
-                        size=ImageSize(
-                            width=seg.data["width"], height=seg.data["height"]
+                    seg_text = f"#{room.room_name} "
+                    length = cal_len(seg_text)
+                    entities.append(
+                        TextEntity(
+                            offset=message_offset,
+                            length=length,
+                            entity=VillaRoomLink(
+                                villa_id=str(seg.data["villa_id"]),
+                                room_id=str(seg.data["room_id"]),
+                                room_name=room.room_name,
+                            ),
                         )
-                        if seg.data["width"] and seg.data["height"]
-                        else None,
-                        file_size=seg.data["file_size"],
                     )
-                )
+                elif seg.type == "link":
+                    seg_text = seg.data["show_text"]
+                    length = cal_len(seg_text)
+                    entities.append(
+                        TextEntity(
+                            offset=message_offset,
+                            length=length,
+                            entity=Link(
+                                url=seg.data["url"], show_text=seg.data["show_text"]
+                            ),
+                        )
+                    )
+                message_offset += length
+                message_text += seg_text
+            except Exception as e:
+                log("WARNING", "error when parse message content", e)
 
         # 不能单独只发图片而没有其他文本内容，塞一个零宽度空格
         if images and not message_text:
             message_text = "\u200B"
 
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
```

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.1/pyproject.toml` & `nonebot_adapter_villa-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.1.1"
+version = "0.1.2"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.1.1/PKG-INFO` & `nonebot_adapter_villa-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.1.1
+Version: 0.1.2
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.1.2 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

