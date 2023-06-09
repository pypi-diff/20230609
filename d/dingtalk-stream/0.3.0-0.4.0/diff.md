# Comparing `tmp/dingtalk-stream-0.3.0.tar.gz` & `tmp/dingtalk-stream-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.3.0.tar", last modified: Tue Jun  6 12:16:13 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.4.0.tar", last modified: Fri Jun  9 05:09:00 2023, max compression
```

## Comparing `dingtalk-stream-0.3.0.tar` & `dingtalk-stream-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/dingtalk_stream/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 05:09:00.000000 dingtalk-stream-0.4.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:09:00.699623 dingtalk-stream-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-09 05:08:59.000000 dingtalk-stream-0.4.0/setup.py
```

### Comparing `dingtalk-stream-0.3.0/LICENSE` & `dingtalk-stream-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.3.0/PKG-INFO` & `dingtalk-stream-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.3.0/README.md` & `dingtalk-stream-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.3.0/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.4.0/dingtalk_stream/chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding:utf-8 -*-
 
 import json
-import uuid
 import requests
 import platform
 import hashlib
-from .stream import CallbackHandler
+from .stream import CallbackHandler, CallbackMessage
+from .frames import AckMessage, Headers
+from concurrent.futures import ThreadPoolExecutor
+import uuid
 
 
 class AtUser(object):
     def __init__(self):
         self.dingtalk_id = None
         self.staff_id = None
         self.extensions = {}
@@ -268,24 +270,25 @@
             'Accept': '*/*',
             'x-acs-dingtalk-access-token': access_token,
             'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
                            '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
                            ) % platform.python_version(),
         }
 
+        card_biz_id = self._gen_card_id(incoming_message)
         body = {"cardTemplateId": "StandardCard",
                 "robotCode": self.dingtalk_client.credential.client_id,
                 "cardData": json.dumps(card_data),
                 "sendOptions": {
                     # "atUserListJson": "String",
                     # "atAll": at_all,
                     # "receiverListJson": "String",
                     # "cardPropertyJson": "String"
                 },
-                "cardBizId": self._gen_card_id(incoming_message)
+                "cardBizId": card_biz_id
                 }
 
         if incoming_message.conversation_type == '2':
             body["openConversationId"] = incoming_message.conversation_id
         elif incoming_message.conversation_type == '1':
             single_chat_receiver = {
                 "userId": incoming_message.sender_staff_id
@@ -300,19 +303,20 @@
         url = 'https://api.dingtalk.com/v1.0/im/v1.0/robot/interactiveCards/send'
         try:
             response = requests.post(url,
                                      headers=request_headers,
                                      json=body)
             response.raise_for_status()
 
-            return response.json
+            return card_biz_id
         except Exception as e:
-            return {}
+            self.logger.error('reply card failed, error=%s', e)
+            return ""
 
-    def update_card(self, card_data: dict, incoming_message: ChatbotMessage):
+    def update_card(self, card_biz_id: str, card_data: dict):
         """
         回复互动卡片。由于sessionWebhook不支持发送互动卡片，所以需要使用OpenAPI，当前仅支持自建应用。
         https://open.dingtalk.com/document/orgapp/robots-send-interactive-cards
         :param card_data: 卡片数据内容，interactive_card.py中有一些简单的样例，高阶需求请至卡片搭建平台：https://card.dingtalk.com/card-builder
         :param incoming_message: 回调数据源，主要是为了取到card_biz_id
         :return:
         """
@@ -326,17 +330,16 @@
             'Accept': '*/*',
             'x-acs-dingtalk-access-token': access_token,
             'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
                            '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
                            ) % platform.python_version(),
         }
 
-        card_id = self._gen_card_id(incoming_message)
         values = {
-            'cardBizId': card_id,
+            'cardBizId': card_biz_id,
             'cardData': json.dumps(card_data),
         }
         url = 'https://api.dingtalk.com/v1.0/im/robots/interactiveCards'
         try:
             response = requests.put(url,
                                     headers=request_headers,
                                     data=json.dumps(values))
@@ -344,11 +347,49 @@
         except Exception as e:
             self.logger.error('update card failed, error=%s, response=%s', e, response.text)
             return response.status_code
         return response.json()
 
     @staticmethod
     def _gen_card_id(msg: ChatbotMessage):
-        factor = '%s_%s_%s_%s' % (msg.sender_id, msg.sender_corp_id, msg.conversation_id, msg.message_id)
+        factor = '%s_%s_%s_%s_%s' % (
+            msg.sender_id, msg.sender_corp_id, msg.conversation_id, msg.message_id, str(uuid.uuid1()))
         m = hashlib.sha256()
         m.update(factor.encode('utf-8'))
         return m.hexdigest()
+
+
+class AsyncChatbotHandler(ChatbotHandler):
+    """
+    多任务执行handler，注意：process函数重载的时候不要用 async
+    """
+
+    async_executor: ThreadPoolExecutor = ThreadPoolExecutor(max_workers=8)
+
+    def __init__(self, max_workers: int = 8):
+        super(AsyncChatbotHandler, self).__init__()
+        self.async_executor = ThreadPoolExecutor(max_workers=max_workers)
+
+    def process(self, message):
+        '''
+        不要用 async 修饰
+        :param message:
+        :return:
+        '''
+        return AckMessage.STATUS_NOT_IMPLEMENT, 'not implement'
+
+    async def raw_process(self, callback_message: CallbackMessage):
+        def func():
+            try:
+                self.process(callback_message)
+            except Exception as e:
+                self.logger.error('async process exception, error=%s', e)
+
+        self.async_executor.submit(func)
+
+        ack_message = AckMessage()
+        ack_message.code = AckMessage.STATUS_OK
+        ack_message.headers.message_id = callback_message.headers.message_id
+        ack_message.headers.content_type = Headers.CONTENT_TYPE_APPLICATION_JSON
+        ack_message.message = "ok"
+        ack_message.data = callback_message.data
+        return ack_message
```

### Comparing `dingtalk-stream-0.3.0/dingtalk_stream/frames.py` & `dingtalk-stream-0.4.0/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.3.0/dingtalk_stream/handlers.py` & `dingtalk-stream-0.4.0/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.3.0/dingtalk_stream/stream.py` & `dingtalk-stream-0.4.0/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.3.0/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.4.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.3.0/setup.py` & `dingtalk-stream-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.3.0',
+    version='0.4.0',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

