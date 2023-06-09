# Comparing `tmp/revChatGPT-6.1.2.tar.gz` & `tmp/revChatGPT-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.1.2.tar", last modified: Wed Jun  7 17:13:41 2023, max compression
+gzip compressed data, was "revChatGPT-6.1.3.tar", last modified: Fri Jun  9 10:15:30 2023, max compression
```

## Comparing `revChatGPT-6.1.2.tar` & `revChatGPT-6.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.256803 revChatGPT-6.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    54723 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-09 10:15:29.000000 revChatGPT-6.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:30.069503 revChatGPT-6.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    54410 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-09 10:15:30.000000 revChatGPT-6.1.3/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 10:15:30.000000 revChatGPT-6.1.3/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:15:30.000000 revChatGPT-6.1.3/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 10:15:30.000000 revChatGPT-6.1.3/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 10:15:30.000000 revChatGPT-6.1.3/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:30.073503 revChatGPT-6.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-09 10:15:03.000000 revChatGPT-6.1.3/tests/test_recipient.py
```

### Comparing `revChatGPT-6.1.2/LICENSE` & `revChatGPT-6.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/PKG-INFO` & `revChatGPT-6.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.2
+Version: 6.1.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.1.2/README.md` & `revChatGPT-6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/setup.py` & `revChatGPT-6.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.1.2",
+    version="6.1.3",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.1.2/src/revChatGPT/V1.py` & `revChatGPT-6.1.3/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -890,16 +890,14 @@
             data=json.dumps(data),
             timeout=timeout,
         ) as response:
             await self.__check_response(response)
 
             finish_details = None
             async for line in response.aiter_lines():
-                # remove b' and ' at the beginning and end and ignore case
-                line = str(line)[2:-1]
                 if line.lower() == "internal server error":
                     log.error(f"Internal Server Error: {line}")
                     error = t.Error(
                         source="ask",
                         message="Internal Server Error",
                         code=t.ErrorType.SERVER_ERROR,
                     )
@@ -907,14 +905,16 @@
                 if not line or line is None:
                     continue
                 if "data: " in line:
                     line = line[6:]
                 if line == "[DONE]":
                     break
 
+                # print(line)
+
                 # DO NOT REMOVE THIS
                 line = line.replace('\\"', '"')
                 line = line.replace("\\'", "'")
                 line = line.replace("\\\\", "\\")
 
                 try:
                     line = json.loads(line)
@@ -1233,48 +1233,42 @@
         :param node_id: UUID of node
 
         Returns:
             str: A URL to the shared link
         """
         convo_id = convo_id or self.conversation_id
         node_id = node_id or self.parent_id
-        headers = {
-            "Content-Type": "application/json",
-            "origin": "https://chat.openai.com",
-            "referer": f"https://chat.openai.com/c/{convo_id}",
-        }
         # First create the share
         payload = {
             "conversation_id": convo_id,
             "current_node_id": node_id,
             "is_anonymous": anonymous,
         }
         url = f"{self.base_url}share/create"
         response = await self.session.post(
             url,
             data=json.dumps(payload),
-            headers=headers,
         )
         await self.__check_response(response)
         share_url = response.json().get("share_url")
         # Then patch the share to make public
         share_id = response.json().get("share_id")
         url = f"{self.base_url}share/{share_id}"
+        print(url)
         payload = {
             "share_id": share_id,
             "highlighted_message_id": node_id,
             "title": title or response.json().get("title", "New chat"),
             "is_public": True,
             "is_visible": True,
             "is_anonymous": True,
         }
         response = await self.session.patch(
             url,
             data=json.dumps(payload),
-            headers=headers,
         )
         await self.__check_response(response)
         return share_url
 
     async def gen_title(self, convo_id: str, message_id: str) -> None:
         """
         Generate title for conversation
```

### Comparing `revChatGPT-6.1.2/src/revChatGPT/V3.py` & `revChatGPT-6.1.3/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/src/revChatGPT/__init__.py` & `revChatGPT-6.1.3/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/src/revChatGPT/__main__.py` & `revChatGPT-6.1.3/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.1.3/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/src/revChatGPT/typings.py` & `revChatGPT-6.1.3/src/revChatGPT/typings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 A module that contains all the types used in this project
 """
 import os
 from enum import Enum
 from typing import Union
+import platform
 
 
-SUPPORT_ADD_NOTES = [
-    int(each) for each in __import__("platform").python_version_tuple()
-][0] >= 3 and [int(each) for each in __import__("platform").python_version_tuple()][
-    1
-] >= 11
+python_version = [each for each in platform.python_version_tuple()]
+SUPPORT_ADD_NOTES = int(python_version[0]) >= 3 and int(python_version[1]) >= 11
 
 
 class ChatbotError(Exception):
     """
     Base class for all Chatbot errors in this Project
     """
```

### Comparing `revChatGPT-6.1.2/src/revChatGPT/utils.py` & `revChatGPT-6.1.3/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.2/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.1.3/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.2
+Version: 6.1.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

