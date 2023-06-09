# Comparing `tmp/GoogleBard-1.3.0.tar.gz` & `tmp/GoogleBard-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.3.0.tar", last modified: Thu Jun  1 17:39:12 2023, max compression
+gzip compressed data, was "GoogleBard-1.3.1.tar", last modified: Fri Jun  9 10:19:34 2023, max compression
```

## Comparing `GoogleBard-1.3.0.tar` & `GoogleBard-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:39:12.496398 GoogleBard-1.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.440179 GoogleBard-1.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-09 10:19:14.000000 GoogleBard-1.3.1/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.444179 GoogleBard-1.3.1/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 10:19:34.000000 GoogleBard-1.3.1/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.3.0/LICENSE` & `GoogleBard-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.3.0/PKG-INFO` & `GoogleBard-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.3.0
+Version: 1.3.1
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.3.0/README.md` & `GoogleBard-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.3.0/setup.py` & `GoogleBard-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.3.0",
+    version="1.3.1",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.3.0/src/Bard.py` & `GoogleBard-1.3.1/src/Bard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import argparse
+import asyncio
 import json
 import os
 import random
 import re
 import string
 import sys
+from typing import Dict
+from typing import List
 
 import httpx
-import asyncio
 from prompt_toolkit import prompt
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.console import Console
 from rich.markdown import Markdown
 
-from typing import List, Dict
-
 
 def __create_session() -> PromptSession:
     return PromptSession(history=InMemoryHistory())
 
 
 def __create_completer(commands: list, pattern_str: str = "$") -> WordCompleter:
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
@@ -57,30 +57,30 @@
         self,
         session_id: str,
         proxy: dict = None,
         timeout: int = 20,
     ):
         self.loop = asyncio.get_event_loop()
         self.async_chatbot = self.loop.run_until_complete(
-            AsyncChatbot.create(session_id, proxy, timeout)
+            AsyncChatbot.create(session_id, proxy, timeout),
         )
 
     def save_conversation(self, file_path: str, conversation_name: str):
         return self.loop.run_until_complete(
-            self.async_chatbot.save_conversation(file_path, conversation_name)
+            self.async_chatbot.save_conversation(file_path, conversation_name),
         )
 
     def load_conversations(self, file_path: str) -> List[Dict]:
         return self.loop.run_until_complete(
-            self.async_chatbot.load_conversations(file_path)
+            self.async_chatbot.load_conversations(file_path),
         )
 
     def load_conversation(self, file_path: str, conversation_name: str) -> bool:
         return self.loop.run_until_complete(
-            self.async_chatbot.load_conversation(file_path, conversation_name)
+            self.async_chatbot.load_conversation(file_path, conversation_name),
         )
 
     def ask(self, message: str) -> dict:
         return self.loop.run_until_complete(self.async_chatbot.ask(message))
 
 
 class AsyncChatbot:
@@ -207,15 +207,15 @@
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
-            "bl": "boq_assistant-bard-web-server_20230530.14_p0",
+            "bl": "boq_assistant-bard-web-server_20230606.12_p0",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
 
         # message arr -> data["f.req"]. Message is double json stringified
         message_struct = [
             [message],
@@ -232,20 +232,20 @@
             data=data,
             timeout=self.timeout,
         )
         chat_data = json.loads(resp.content.splitlines()[3])[0][2]
         if not chat_data:
             return {"content": f"Google Bard encountered an error: {resp.content}."}
         json_chat_data = json.loads(chat_data)
-        images = set()
+        images = []
         if len(json_chat_data) >= 3:
             if len(json_chat_data[4][0]) >= 4:
                 if json_chat_data[4][0][4]:
                     for img in json_chat_data[4][0][4]:
-                        images.add(img[0][0][0])
+                        images.append(img[0][0][0])
         results = {
             "content": json_chat_data[0][0],
             "conversation_id": json_chat_data[1][0],
             "response_id": json_chat_data[1][1],
             "factualityQueries": json_chat_data[3],
             "textQuery": json_chat_data[2][0] if json_chat_data[2] is not None else "",
             "choices": [{"id": i[0], "content": i[1]} for i in json_chat_data[4]],
```

### Comparing `GoogleBard-1.3.0/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.3.1/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.3.0
+Version: 1.3.1
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

