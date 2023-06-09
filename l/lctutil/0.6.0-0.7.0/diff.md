# Comparing `tmp/lctutil-0.6.0.tar.gz` & `tmp/lctutil-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctutil-0.6.0.tar", last modified: Fri May 12 09:30:11 2023, max compression
+gzip compressed data, was "lctutil-0.7.0.tar", last modified: Fri Jun  9 02:57:06 2023, max compression
```

## Comparing `lctutil-0.6.0.tar` & `lctutil-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 09:30:11.700879 lctutil-0.6.0/
--rw-rw-rw-   0        0        0      328 2023-05-12 09:30:11.699878 lctutil-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 09:30:11.694878 lctutil-0.6.0/lctutil/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.6.0/lctutil/__init__.py
--rw-rw-rw-   0        0        0     3419 2023-05-12 07:23:14.000000 lctutil-0.6.0/lctutil/ac_matcher.py
--rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.6.0/lctutil/extract_base_info.py
--rw-rw-rw-   0        0        0     1526 2023-05-12 07:23:51.000000 lctutil-0.6.0/lctutil/openai.py
--rw-rw-rw-   0        0        0     1217 2023-05-12 07:50:18.000000 lctutil-0.6.0/lctutil/stock_infos.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:30:11.698878 lctutil-0.6.0/lctutil.egg-info/
--rw-rw-rw-   0        0        0      328 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 09:30:11.700879 lctutil-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-05-12 09:27:44.000000 lctutil-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:57:06.028493 lctutil-0.7.0/
+-rw-rw-rw-   0        0        0      328 2023-06-09 02:57:06.027493 lctutil-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 02:57:06.022496 lctutil-0.7.0/lctutil/
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.7.0/lctutil/__init__.py
+-rw-rw-rw-   0        0        0     3419 2023-05-12 07:23:14.000000 lctutil-0.7.0/lctutil/ac_matcher.py
+-rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.7.0/lctutil/extract_base_info.py
+-rw-rw-rw-   0        0        0     1654 2023-06-09 02:55:18.000000 lctutil-0.7.0/lctutil/openai.py
+-rw-rw-rw-   0        0        0     1341 2023-06-09 02:48:03.000000 lctutil-0.7.0/lctutil/stock_infos.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:57:06.026492 lctutil-0.7.0/lctutil.egg-info/
+-rw-rw-rw-   0        0        0      328 2023-06-09 02:57:05.000000 lctutil-0.7.0/lctutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-09 02:57:05.000000 lctutil-0.7.0/lctutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:57:05.000000 lctutil-0.7.0/lctutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-09 02:57:05.000000 lctutil-0.7.0/lctutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 02:57:05.000000 lctutil-0.7.0/lctutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:57:06.028493 lctutil-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-06-09 02:54:13.000000 lctutil-0.7.0/setup.py
```

### Comparing `lctutil-0.6.0/lctutil/ac_matcher.py` & `lctutil-0.7.0/lctutil/ac_matcher.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.6.0/lctutil/extract_base_info.py` & `lctutil-0.7.0/lctutil/extract_base_info.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.6.0/lctutil/openai.py` & `lctutil-0.7.0/lctutil/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 
 from typing import List
 import os, openai
 from tenacity import retry, wait_random_exponential, stop_after_attempt
 
-proxy = "socks5://127.0.0.1:1080"
-openai.proxy = {"http": proxy, "https": proxy}
+use_proxy = os.getenv("USE_PROXY")  or True
+
+if use_proxy:
+    proxy = "socks5://127.0.0.1:1080"
+    openai.proxy = {"http": proxy, "https": proxy}
 
 _apikeystr = os.getenv("API_KEYS")  or ""
 apikeys = _apikeystr.split(";")
 api_k_index = 0
 openai.api_key = apikeys[api_k_index]
 api_k_num = len(apikeys)
 
@@ -17,31 +20,33 @@
     global api_k_index
     api_k_index = api_k_index % api_k_num
     openai.api_key = apikeys[api_k_index] 
     api_k_index = api_k_index + 1
 
 
 @retry(wait=wait_random_exponential(min=9, max=20), stop=stop_after_attempt(3))
-def get_embeddings(texts: List[str]) -> List[List[float]]:
+def get_embeddings(texts: List[str], model="text-embedding-ada-002") -> List[List[float]]:
     set_api_key_inturn()
     if type(texts) == "str": texts = [texts]
-    response = openai.Embedding.create(input=texts, model="text-embedding-ada-002")
+    response = openai.Embedding.create(input=texts, model=model)
     data = response["data"]  # type: ignore
     return [result["embedding"] for result in data]
 
 
 @retry(wait=wait_random_exponential(min=9, max=20), stop=stop_after_attempt(3))
 def get_chat_completion(
     messages,
-    model="gpt-3.5-turbo"  # use "gpt-4" for better results
+    model="gpt-3.5-turbo",  # use "gpt-4" for better results
+    stream = False
 ):
     set_api_key_inturn()
     # call the OpenAI chat completion API with the given messages
     response = openai.ChatCompletion.create(
         model=model,
-        messages=messages
+        messages=messages,
+        stream=stream
     )
 
     choices = response["choices"]  # type: ignore
     completion = choices[0].message.content.strip()
     print(f"Completion: \n{completion}")
     return completion
```

### Comparing `lctutil-0.6.0/lctutil/stock_infos.py` & `lctutil-0.7.0/lctutil/stock_infos.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,14 @@
 
 
 _filename = os.getenv("STOCK_INFO_FILE")
 loadcodes(_filename)
 
 
 def get_code_or_name(ele):
-    return code_name_kv.get(ele, "")
+    return code_name_kv.get(ele, "")
+
+def get_name(ele):
+    if '0' <= ele[0] and ele[0] <= '9':
+        return code_name_kv.get(ele, ele)
+
+    return ele
```

### Comparing `lctutil-0.6.0/setup.py` & `lctutil-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lctutil',
-    version='0.6.0',
+    version='0.7.0',
     packages=find_packages(),
     install_requires=[
         "pyahocorasick",
         "openai",
         "tenacity"
     ],
     py_modules=["lctutil"],
```

