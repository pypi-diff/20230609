# Comparing `tmp/zhipuai-1.0.3.tar.gz` & `tmp/zhipuai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-1.0.3.tar", last modified: Fri Jun  9 02:23:52 2023, max compression
+gzip compressed data, was "zhipuai-1.0.4.tar", last modified: Fri Jun  9 06:06:24 2023, max compression
```

## Comparing `zhipuai-1.0.3.tar` & `zhipuai-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 02:23:52.608499 zhipuai-1.0.3/
--rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-09 02:23:52.608325 zhipuai-1.0.3/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.3/README.md
--rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-09 02:23:52.608546 zhipuai-1.0.3/setup.cfg
--rw-r--r--   0 haowangai   (501) staff       (20)      899 2023-06-09 02:23:35.000000 zhipuai-1.0.3/setup.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 02:23:52.600630 zhipuai-1.0.3/zhipuai/
--rw-r--r--   0 haowangai   (501) staff       (20)      221 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/__init__.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 02:23:52.601700 zhipuai-1.0.3/zhipuai/examples/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/examples/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1466 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/examples/chatglm6b_example.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1427 2023-06-09 02:23:14.000000 zhipuai-1.0.3/zhipuai/examples/model_api_example.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 02:23:52.607186 zhipuai-1.0.3/zhipuai/model_api/
--rw-r--r--   0 haowangai   (501) staff       (20)      102 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/model_api/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1858 2023-06-09 02:21:28.000000 zhipuai-1.0.3/zhipuai/model_api/api.py
--rw-r--r--   0 haowangai   (501) staff       (20)      246 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/model_api/chatglm_params.py
--rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-06-09 02:21:28.000000 zhipuai-1.0.3/zhipuai/model_api/params.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 02:23:52.607820 zhipuai-1.0.3/zhipuai/utils/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-05 13:56:33.000000 zhipuai-1.0.3/zhipuai/utils/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1252 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/utils/http_client.py
--rw-r--r--   0 haowangai   (501) staff       (20)      700 2023-06-08 03:38:31.000000 zhipuai-1.0.3/zhipuai/utils/jwt_token.py
--rw-r--r--   0 haowangai   (501) staff       (20)     4531 2023-06-08 10:53:33.000000 zhipuai-1.0.3/zhipuai/utils/sse_client.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 02:23:52.601309 zhipuai-1.0.3/zhipuai.egg-info/
--rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-09 02:23:52.000000 zhipuai-1.0.3/zhipuai.egg-info/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)      526 2023-06-09 02:23:52.000000 zhipuai-1.0.3/zhipuai.egg-info/SOURCES.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-06-09 02:23:52.000000 zhipuai-1.0.3/zhipuai.egg-info/dependency_links.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       36 2023-06-09 02:23:52.000000 zhipuai-1.0.3/zhipuai.egg-info/requires.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        8 2023-06-09 02:23:52.000000 zhipuai-1.0.3/zhipuai.egg-info/top_level.txt
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.369118 zhipuai-1.0.4/
+-rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-09 06:06:24.368965 zhipuai-1.0.4/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.4/README.md
+-rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-09 06:06:24.369154 zhipuai-1.0.4/setup.cfg
+-rw-r--r--   0 haowangai   (501) staff       (20)      899 2023-06-09 06:05:00.000000 zhipuai-1.0.4/setup.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.366192 zhipuai-1.0.4/zhipuai/
+-rw-r--r--   0 haowangai   (501) staff       (20)      221 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/__init__.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.367183 zhipuai-1.0.4/zhipuai/examples/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/examples/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1466 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/examples/chatglm6b_example.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1427 2023-06-09 02:23:14.000000 zhipuai-1.0.4/zhipuai/examples/model_api_example.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.367939 zhipuai-1.0.4/zhipuai/model_api/
+-rw-r--r--   0 haowangai   (501) staff       (20)      102 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/model_api/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1858 2023-06-09 02:21:28.000000 zhipuai-1.0.4/zhipuai/model_api/api.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      246 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/model_api/chatglm_params.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-06-09 02:21:28.000000 zhipuai-1.0.4/zhipuai/model_api/params.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.368598 zhipuai-1.0.4/zhipuai/utils/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-05 13:56:33.000000 zhipuai-1.0.4/zhipuai/utils/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1252 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/utils/http_client.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      700 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/utils/jwt_token.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     4531 2023-06-08 10:53:33.000000 zhipuai-1.0.4/zhipuai/utils/sse_client.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.366802 zhipuai-1.0.4/zhipuai.egg-info/
+-rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)      526 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/SOURCES.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/dependency_links.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/requires.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        8 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/top_level.txt
```

### Comparing `zhipuai-1.0.3/setup.py` & `zhipuai-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="zhipuai",
-    version="v1.0.3",
+    version="v1.0.4",
     description="A SDK library for accessing big model apis from ZhipuAI",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Zhipu AI",
     url="https://open.bigmodel.cn/",
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
```

### Comparing `zhipuai-1.0.3/zhipuai/examples/chatglm6b_example.py` & `zhipuai-1.0.4/zhipuai/examples/chatglm6b_example.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.3/zhipuai/examples/model_api_example.py` & `zhipuai-1.0.4/zhipuai/examples/model_api_example.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.3/zhipuai/model_api/api.py` & `zhipuai-1.0.4/zhipuai/model_api/api.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.3/zhipuai/utils/http_client.py` & `zhipuai-1.0.4/zhipuai/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.3/zhipuai/utils/jwt_token.py` & `zhipuai-1.0.4/zhipuai/utils/jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.3/zhipuai/utils/sse_client.py` & `zhipuai-1.0.4/zhipuai/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.3/zhipuai.egg-info/SOURCES.txt` & `zhipuai-1.0.4/zhipuai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

