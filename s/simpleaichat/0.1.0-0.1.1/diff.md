# Comparing `tmp/simpleaichat-0.1.0.tar.gz` & `tmp/simpleaichat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaichat-0.1.0.tar", last modified: Thu Jun  8 04:36:40 2023, max compression
+gzip compressed data, was "simpleaichat-0.1.1.tar", last modified: Fri Jun  9 04:06:19 2023, max compression
```

## Comparing `simpleaichat-0.1.0.tar` & `simpleaichat-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-08 04:36:40.310901 simpleaichat-0.1.0/
--rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.1.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    15879 2023-06-08 04:36:40.310665 simpleaichat-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    15442 2023-06-08 04:07:08.000000 simpleaichat-0.1.0/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-06-08 04:36:40.310978 simpleaichat-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      938 2023-06-08 04:35:58.000000 simpleaichat-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-08 04:36:40.308759 simpleaichat-0.1.0/simpleaichat/
--rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.1.0/simpleaichat/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    11175 2023-06-08 02:34:09.000000 simpleaichat-0.1.0/simpleaichat/chatgpt.py
--rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.1.0/simpleaichat/cli.py
--rw-r--r--   0 root         (0) staff       (20)     3052 2023-06-03 05:30:50.000000 simpleaichat-0.1.0/simpleaichat/models.py
--rw-r--r--   0 root         (0) staff       (20)    12175 2023-06-08 01:27:02.000000 simpleaichat-0.1.0/simpleaichat/simpleaichat.py
--rw-r--r--   0 root         (0) staff       (20)     2364 2023-06-03 03:44:43.000000 simpleaichat-0.1.0/simpleaichat/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-08 04:36:40.310307 simpleaichat-0.1.0/simpleaichat.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    15879 2023-06-08 04:36:39.000000 simpleaichat-0.1.0/simpleaichat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      387 2023-06-08 04:36:40.000000 simpleaichat-0.1.0/simpleaichat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-06-08 04:36:39.000000 simpleaichat-0.1.0/simpleaichat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       67 2023-06-08 04:36:39.000000 simpleaichat-0.1.0/simpleaichat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       89 2023-06-08 04:36:40.000000 simpleaichat-0.1.0/simpleaichat.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2023-06-08 04:36:40.000000 simpleaichat-0.1.0/simpleaichat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-09 04:06:19.235172 simpleaichat-0.1.1/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    15867 2023-06-09 04:06:19.234935 simpleaichat-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    15430 2023-06-08 14:46:39.000000 simpleaichat-0.1.1/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-06-09 04:06:19.235248 simpleaichat-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      972 2023-06-09 04:05:24.000000 simpleaichat-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-09 04:06:19.232926 simpleaichat-0.1.1/simpleaichat/
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.1.1/simpleaichat/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    11175 2023-06-08 02:34:09.000000 simpleaichat-0.1.1/simpleaichat/chatgpt.py
+-rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.1.1/simpleaichat/cli.py
+-rw-r--r--   0 root         (0) staff       (20)     3052 2023-06-03 05:30:50.000000 simpleaichat-0.1.1/simpleaichat/models.py
+-rw-r--r--   0 root         (0) staff       (20)    12175 2023-06-08 01:27:02.000000 simpleaichat-0.1.1/simpleaichat/simpleaichat.py
+-rw-r--r--   0 root         (0) staff       (20)     2364 2023-06-03 03:44:43.000000 simpleaichat-0.1.1/simpleaichat/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-09 04:06:19.234612 simpleaichat-0.1.1/simpleaichat.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    15867 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      387 2023-06-09 04:06:19.000000 simpleaichat-0.1.1/simpleaichat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       67 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      112 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-06-09 04:06:18.000000 simpleaichat-0.1.1/simpleaichat.egg-info/top_level.txt
```

### Comparing `simpleaichat-0.1.0/LICENSE` & `simpleaichat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.0/PKG-INFO` & `simpleaichat-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
@@ -139,15 +139,15 @@
 print(response)
 ```
 
 ```
 Sacramento was founded on February 27, 1850.
 ```
 
-You can also save chat sessions (as CSV or JSON) and load them later. The API key is (obviously) not saved so you will have to provide that when loading.
+You can also save chat sessions (as CSV or JSON) and load them later. The API key is not saved so you will have to provide that when loading.
 
 ```py3
 ai.save_session()  # CSV, will only save messages
 ai.save_session(format="json", minify=True)  # JSON
 
 ai.load_session("my.csv")
 ai.load_session("my.json")
```

### Comparing `simpleaichat-0.1.0/README.md` & `simpleaichat-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 print(response)
 ```
 
 ```
 Sacramento was founded on February 27, 1850.
 ```
 
-You can also save chat sessions (as CSV or JSON) and load them later. The API key is (obviously) not saved so you will have to provide that when loading.
+You can also save chat sessions (as CSV or JSON) and load them later. The API key is not saved so you will have to provide that when loading.
 
 ```py3
 ai.save_session()  # CSV, will only save messages
 ai.save_session(format="json", minify=True)  # JSON
 
 ai.load_session("my.csv")
 ai.load_session("my.json")
```

### Comparing `simpleaichat-0.1.0/setup.py` & `simpleaichat-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="simpleaichat",
     packages=["simpleaichat"],  # this must be the same as the name above
-    version="0.1.0",
+    version="0.1.1",
     description="A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Max Woolf",
     author_email="max@minimaxir.com",
     url="https://github.com/minimaxir/simpleaichat",
     keywords=["chatgpt", "openai", "text generation", "ai"],
@@ -20,9 +20,10 @@
     install_requires=[
         "pydantic>=1.10",
         "fire>=0.3.0",
         "httpx>=0.24.1",
         "python-dotenv>=1.0.0",
         "orjson>=3.9.0",
         "rich>=13.4.1",
+        "python-dateutil>=2.8.2",
     ],
 )
```

### Comparing `simpleaichat-0.1.0/simpleaichat/chatgpt.py` & `simpleaichat-0.1.1/simpleaichat/chatgpt.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.0/simpleaichat/cli.py` & `simpleaichat-0.1.1/simpleaichat/cli.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.0/simpleaichat/models.py` & `simpleaichat-0.1.1/simpleaichat/models.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.0/simpleaichat/simpleaichat.py` & `simpleaichat-0.1.1/simpleaichat/simpleaichat.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.0/simpleaichat/utils.py` & `simpleaichat-0.1.1/simpleaichat/utils.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.1.0/simpleaichat.egg-info/PKG-INFO` & `simpleaichat-0.1.1/simpleaichat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
@@ -139,15 +139,15 @@
 print(response)
 ```
 
 ```
 Sacramento was founded on February 27, 1850.
 ```
 
-You can also save chat sessions (as CSV or JSON) and load them later. The API key is (obviously) not saved so you will have to provide that when loading.
+You can also save chat sessions (as CSV or JSON) and load them later. The API key is not saved so you will have to provide that when loading.
 
 ```py3
 ai.save_session()  # CSV, will only save messages
 ai.save_session(format="json", minify=True)  # JSON
 
 ai.load_session("my.csv")
 ai.load_session("my.json")
```

