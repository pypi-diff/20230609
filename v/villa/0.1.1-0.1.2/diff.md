# Comparing `tmp/villa-0.1.1.tar.gz` & `tmp/villa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.1.1.tar", max compression
+gzip compressed data, was "villa-0.1.2.tar", max compression
```

## Comparing `villa-0.1.1.tar` & `villa-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-08 14:38:00.643531 villa-0.1.1/LICENSE
--rw-r--r--   0        0        0     2399 2023-06-08 14:38:00.643531 villa-0.1.1/README.md
--rw-r--r--   0        0        0     1034 2023-06-08 14:38:00.643531 villa-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      120 2023-06-08 14:38:00.643531 villa-0.1.1/villa/__init__.py
--rw-r--r--   0        0        0    30767 2023-06-08 14:38:00.643531 villa-0.1.1/villa/bot.py
--rw-r--r--   0        0        0     7799 2023-06-08 14:38:00.643531 villa-0.1.1/villa/event.py
--rw-r--r--   0        0        0      473 2023-06-08 14:38:00.643531 villa-0.1.1/villa/exception.py
--rw-r--r--   0        0        0     1504 2023-06-08 14:38:00.643531 villa-0.1.1/villa/log.py
--rw-r--r--   0        0        0    16613 2023-06-08 14:38:00.643531 villa-0.1.1/villa/message.py
--rw-r--r--   0        0        0     9982 2023-06-08 14:38:00.643531 villa-0.1.1/villa/models.py
--rw-r--r--   0        0        0      113 2023-06-08 14:38:00.643531 villa-0.1.1/villa/store.py
--rw-r--r--   0        0        0      794 2023-06-08 14:38:00.643531 villa-0.1.1/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-08 14:38:00.643531 villa-0.1.1/villa/utils.py
--rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 villa-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-09 04:26:48.597982 villa-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2399 2023-06-09 04:26:48.597982 villa-0.1.2/README.md
+-rw-r--r--   0        0        0     1034 2023-06-09 04:26:48.597982 villa-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-06-09 04:26:48.597982 villa-0.1.2/villa/__init__.py
+-rw-r--r--   0        0        0    30542 2023-06-09 04:26:48.597982 villa-0.1.2/villa/bot.py
+-rw-r--r--   0        0        0     7799 2023-06-09 04:26:48.597982 villa-0.1.2/villa/event.py
+-rw-r--r--   0        0        0      473 2023-06-09 04:26:48.601982 villa-0.1.2/villa/exception.py
+-rw-r--r--   0        0        0     1504 2023-06-09 04:26:48.601982 villa-0.1.2/villa/log.py
+-rw-r--r--   0        0        0    16613 2023-06-09 04:26:48.601982 villa-0.1.2/villa/message.py
+-rw-r--r--   0        0        0     9982 2023-06-09 04:26:48.601982 villa-0.1.2/villa/models.py
+-rw-r--r--   0        0        0      113 2023-06-09 04:26:48.601982 villa-0.1.2/villa/store.py
+-rw-r--r--   0        0        0      794 2023-06-09 04:26:48.601982 villa-0.1.2/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-06-09 04:26:48.601982 villa-0.1.2/villa/utils.py
+-rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 villa-0.1.2/PKG-INFO
```

### Comparing `villa-0.1.1/LICENSE` & `villa-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/README.md` & `villa-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/pyproject.toml` & `villa-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.1.1"
+version = "0.1.2"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.1.1/villa/bot.py` & `villa-0.1.2/villa/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -640,112 +640,118 @@
             logger.opt(colors=True).success(
                 f"<b><y>[{event.__class__.__name__}]</y></b> handle completed"
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
         if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
+
+        if images_msg := (message["image"] or None):
+            images_msg: List[ImageSegment]
+            images = [
+                Image(
+                    url=seg.url,
+                    size=ImageSize(width=seg.width, height=seg.height)
+                    if seg.width and seg.height
+                    else None,
+                    file_size=seg.file_size,
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
             try:
+                if seg.type in ("quote", "image"):
+                    continue
                 if isinstance(seg, TextSegment):
-                    message_text += seg.content
-                    message_offset += len(seg.content)
+                    seg_text = seg.content
+                    length = cal_len(seg_text)
                 elif isinstance(seg, MentionAllSegment):
-                    message_text += f"@{seg.show_text} "
+                    seg_text = f"@{seg.data['show_text']} "
+                    length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
-                            length=6,
+                            length=length,
                             entity=MentionedAll(show_text=seg.show_text),
                         )
                     )
-                    message_offset += len(f"@{seg.show_text} ")
                     mentioned.type = MentionType.ALL
                 elif isinstance(seg, MentionRobotSegment):
-                    bot_name = self.bot_info.template.name if self.bot_info else "Bot"
-                    message_text += f"@{bot_name} "
+                    seg_text = f"@{seg.bot_name} "
+                    length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
-                            length=len(f"@{bot_name}".encode("utf-16")) // 2,
+                            length=length,
                             entity=MentionedRobot(
-                                bot_id=self.bot_id, bot_name=bot_name
+                                bot_id=seg.bot_id, bot_name=seg.bot_name
                             ),
                         )
                     )
-                    message_offset += len(f"@{bot_name}") + 1
-                    mentioned.user_id_list.append(self.bot_id)
+                    mentioned.user_id_list.append(seg.bot_id)
                 elif isinstance(seg, MentionUserSegment):
                     # 需要调用API获取被@的用户的昵称
                     user = await self.get_member(villa_id=seg.villa_id, uid=seg.user_id)
-                    message_text += f"@{user.basic.nickname} "
+                    seg_text = f"@{user.basic.nickname} "
+                    length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
-                            length=len(f"@{user.basic.nickname}".encode("utf-16")) // 2,
+                            length=length,
                             entity=MentionedUser(
                                 user_id=str(user.basic.uid),
                                 user_name=user.basic.nickname,
                             ),
                         )
                     )
-                    message_offset += len(f"@{user.basic.nickname}") + 1
                     mentioned.user_id_list.append(str(user.basic.uid))
                 elif isinstance(seg, RoomLinkSegment):
                     # 需要调用API获取房间的名称
                     room = await self.get_room(
                         villa_id=seg.villa_id, room_id=seg.room_id
                     )
-                    message_text += f"#{room.room_name} "
+                    seg_text = f"#{room.room_name} "
+                    length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
-                            length=len(f"#{room.room_name}".encode("utf-16")) // 2,
+                            length=length,
                             entity=VillaRoomLink(
                                 villa_id=str(seg.villa_id),
                                 room_id=str(seg.room_id),
                                 room_name=room.room_name,
                             ),
                         )
                     )
-                    message_offset += len(f"#{room.room_name} ")
-                elif isinstance(seg, LinkSegment):
-                    show_text = seg.show_text or seg.url
-                    message_text += show_text
+                else:
+                    seg: LinkSegment
+                    seg_text = seg.show_text
+                    length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
-                            length=len(show_text.encode("utf-16")) // 2,
-                            entity=Link(
-                                url=seg.url, show_text=seg.show_text or seg.url
-                            ),
-                        )
-                    )
-                    message_offset += len(show_text) + 1
-                elif isinstance(seg, ImageSegment):
-                    images.append(
-                        Image(
-                            url=seg.url,
-                            size=ImageSize(width=seg.width, height=seg.height)
-                            if (seg.width and seg.height)
-                            else None,
-                            file_size=seg.file_size,
+                            length=seg_text,
+                            entity=Link(url=seg.url, show_text=seg.show_text),
                         )
                     )
+                message_offset += length
+                message_text += seg_text
             except Exception as e:
                 logger.opt(exception=e).warning("error when parse message content")
 
         # 不能单独只发图片而没有其他文本内容
         if images and not message_text:
-            message_text = "图片"
+            message_text = "\u200B"
 
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
         return MessageContentInfo(
             content=MessageContent(text=message_text, entities=entities, images=images),
             mentionedInfo=mentioned,
             quote=quote,
```

### Comparing `villa-0.1.1/villa/event.py` & `villa-0.1.2/villa/event.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/villa/log.py` & `villa-0.1.2/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/villa/message.py` & `villa-0.1.2/villa/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     @staticmethod
     def room_link(villa_id: int, room_id: int) -> "RoomLink":
         return RoomLink(villa_id=villa_id, room_id=room_id)
 
     @staticmethod
     def link(url: str, show_text: Optional[str] = None) -> "Link":
-        return Link(url=url, show_text=show_text)
+        return Link(url=url, show_text=show_text or url)
 
     @staticmethod
     def image(
         url: str,
         width: Optional[int] = None,
         height: Optional[int] = None,
         file_size: Optional[int] = None,
@@ -126,15 +126,15 @@
 
 
 class Link(MessageSegment):
     """链接消息段"""
 
     type: Literal["link"] = "link"
     url: str
-    show_text: Optional[str] = None
+    show_text: str
 
 
 class Image(MessageSegment):
     """图片消息段"""
 
     type: Literal["image"] = "image"
     url: str
@@ -243,27 +243,27 @@
 
         返回:
             Self: 消息对象
         """
         self.__root__.append(RoomLink(villa_id=villa_id, room_id=room_id))
         return self
 
-    def link(self, url: str, text: Optional[str] = None) -> Self:
+    def link(self, url: str, show_text: Optional[str] = None) -> Self:
         """说明
 
         详细说明
 
         参数:
             url: 参数说明
             text: 参数说明. 默认为 None.
 
         返回:
             Self: 返回说明
         """
-        self.__root__.append(Link(url=url, show_text=text or url))
+        self.__root__.append(Link(url=url, show_text=show_text or url))
         return self
 
     def image(
         self,
         url: str,
         width: Optional[int] = None,
         height: Optional[int] = None,
```

### Comparing `villa-0.1.1/villa/models.py` & `villa-0.1.2/villa/models.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/villa/typing.py` & `villa-0.1.2/villa/typing.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/villa/utils.py` & `villa-0.1.2/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.1/PKG-INFO` & `villa-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.1.1
+Version: 0.1.2
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

