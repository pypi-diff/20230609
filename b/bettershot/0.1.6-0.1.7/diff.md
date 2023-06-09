# Comparing `tmp/bettershot-0.1.6.tar.gz` & `tmp/bettershot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.6.tar", max compression
+gzip compressed data, was "bettershot-0.1.7.tar", max compression
```

## Comparing `bettershot-0.1.6.tar` & `bettershot-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.6/README.md
--rw-r--r--   0        0        0     1595 2023-06-08 02:43:56.731715 bettershot-0.1.6/bettershot/__init__.py
--rw-r--r--   0        0        0      309 2023-06-08 02:43:54.711289 bettershot-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 bettershot-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.7/README.md
+-rw-r--r--   0        0        0     1764 2023-06-09 00:31:43.785880 bettershot-0.1.7/bettershot/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-09 00:31:52.595387 bettershot-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 bettershot-0.1.7/PKG-INFO
```

### Comparing `bettershot-0.1.6/bettershot/__init__.py` & `bettershot-0.1.7/bettershot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 import requests
 import json 
 from langchain.schema import (AIMessage, HumanMessage, SystemMessage)
 
 url = "https://bettershot-w6mm.zeet-berri.zeet.app/openai_listener"
 
-def log(messages, completion, openai_api_key): 
-    payload = {
-    "messages": messages,
-    "completion": completion,
-    "openai_api_key": openai_api_key
-    }
-    headers = {
-        "Content-Type": "application/json",
-    }
-    response = requests.post(url, headers=headers, data=json.dumps(payload))
-    print(response)
-    return {"response" : response}
+# def log(messages, completion, user_email, openai_api_key): 
+#     payload = {
+#     "messages": messages,
+#     "completion": completion,
+#     "openai_api_key": openai_api_key
+#     }
+#     headers = {
+#         "Content-Type": "application/json",
+#     }
+#     response = requests.post(url, headers=headers, data=json.dumps(payload))
+#     print(response)
+#     return {"response" : response}
 
-def log_langchain(messages, completion, openai_api_key):
+def log(messages, completion, user_email, openai_api_key):
     raw_messages = []
     for message in messages: 
         if isinstance(message, SystemMessage):
             # messages': [{'role': 'user', 'content': "Hey! how's it going?"}]
             raw_message = {"role": "system", "content": message.content}
         elif isinstance(message, HumanMessage):
             raw_message = {"role": "system", "content": message.content}
         elif isinstance(message, AIMessage):
             raw_message = {"role": "ai", "content": message.content}
+        else: 
+            raw_message = message
         raw_messages.append(raw_message)
     if isinstance(completion, AIMessage):
         raw_completion = {"choices":[{"message": {"content": completion.content}}]}
+    else: 
+        raw_completion = completion
     payload = {
         "messages": raw_messages,
         "completion": raw_completion,
-        "openai_api_key": openai_api_key
+        "openai_api_key": openai_api_key, 
+        "user_email": user_email
     }
     headers = {
         "Content-Type": "application/json",
     }
     response = requests.post(url, headers=headers, data=json.dumps(payload))
     print(response)
     return {"response" : response}
```

