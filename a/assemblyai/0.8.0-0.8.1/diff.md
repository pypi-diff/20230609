# Comparing `tmp/assemblyai-0.8.0.tar.gz` & `tmp/assemblyai-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.8.0.tar", last modified: Thu Jun  8 09:27:53 2023, max compression
+gzip compressed data, was "assemblyai-0.8.1.tar", last modified: Fri Jun  9 14:51:54 2023, max compression
```

## Comparing `assemblyai-0.8.0.tar` & `assemblyai-0.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.843318 assemblyai-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 09:27:38.000000 assemblyai-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-08 09:27:53.839318 assemblyai-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-06-08 09:27:38.000000 assemblyai-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22797 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    48521 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:27:53.843318 assemblyai-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 09:27:38.000000 assemblyai-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_auto_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_content_safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_entity_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.189179 assemblyai-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 14:51:43.000000 assemblyai-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-09 14:51:54.189179 assemblyai-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-06-09 14:51:43.000000 assemblyai-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.185179 assemblyai-0.8.1/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48658 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.185179 assemblyai-0.8.1/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:51:54.189179 assemblyai-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 14:51:43.000000 assemblyai-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.185179 assemblyai-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.189179 assemblyai-0.8.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_auto_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_content_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_entity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.8.0/LICENSE` & `assemblyai-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/PKG-INFO` & `assemblyai-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.8.0
+Version: 0.8.1
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -248,15 +248,15 @@
 questions = [
     aai.LemurQuestion(question="What car was the customer interested in?"),
     aai.LemurQuestion(question="What price range is the customer looking for?"),
 ]
 
 results = transcript.lemur.question(questions)
 
-for result in result:
+for result in results:
     print(f"Question: {result.question}")
     print(f"Answer: {result.answer}")
 ```
 
 </details>
 
 ---
```

### Comparing `assemblyai-0.8.0/README.md` & `assemblyai-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 questions = [
     aai.LemurQuestion(question="What car was the customer interested in?"),
     aai.LemurQuestion(question="What price range is the customer looking for?"),
 ]
 
 results = transcript.lemur.question(questions)
 
-for result in result:
+for result in results:
     print(f"Question: {result.question}")
     print(f"Answer: {result.answer}")
 ```
 
 </details>
 
 ---
```

### Comparing `assemblyai-0.8.0/assemblyai/__init__.py` & `assemblyai-0.8.1/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/assemblyai/api.py` & `assemblyai-0.8.1/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/assemblyai/client.py` & `assemblyai-0.8.1/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/assemblyai/lemur.py` & `assemblyai-0.8.1/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/assemblyai/transcriber.py` & `assemblyai-0.8.1/assemblyai/transcriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             if self.transcript.status in (
                 types.TranscriptStatus.completed,
                 types.TranscriptStatus.error,
             ):
                 break
 
-            time.sleep(3)
+            time.sleep(self._client.settings.polling_interval)
 
         return self
 
     def export_subtitles_srt(
         self,
         *,
         chars_per_caption: Optional[int],
```

### Comparing `assemblyai-0.8.0/assemblyai/types.py` & `assemblyai-0.8.1/assemblyai/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
     http_timeout: float = 15.0
     "The default HTTP timeout for general requests"
 
     base_url: str = "https://api.assemblyai.com/v2"
     "The base URL for the AssemblyAI API"
 
+    polling_interval: float = 1.0
+    "The default polling interval for long-running requests (e.g. polling the `Transcript`'s status)"
+
     class Config:
         env_prefix = "assemblyai_"
 
 
 class TranscriptStatus(str, Enum):
     """
     Transcript status
```

### Comparing `assemblyai-0.8.0/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.8.1/assemblyai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.8.0
+Version: 0.8.1
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -248,15 +248,15 @@
 questions = [
     aai.LemurQuestion(question="What car was the customer interested in?"),
     aai.LemurQuestion(question="What price range is the customer looking for?"),
 ]
 
 results = transcript.lemur.question(questions)
 
-for result in result:
+for result in results:
     print(f"Question: {result.question}")
     print(f"Answer: {result.answer}")
 ```
 
 </details>
 
 ---
```

### Comparing `assemblyai-0.8.0/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.8.1/assemblyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/setup.py` & `assemblyai-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.8.0",
+    version="0.8.1",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.8.0/tests/unit/factories.py` & `assemblyai-0.8.1/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_auto_chapters.py` & `assemblyai-0.8.1/tests/unit/test_auto_chapters.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_content_safety.py` & `assemblyai-0.8.1/tests/unit/test_content_safety.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_domains.py` & `assemblyai-0.8.1/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_entity_detection.py` & `assemblyai-0.8.1/tests/unit/test_entity_detection.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_lemur.py` & `assemblyai-0.8.1/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_sentiment_analysis.py` & `assemblyai-0.8.1/tests/unit/test_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_summarization.py` & `assemblyai-0.8.1/tests/unit/test_summarization.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_transcriber.py` & `assemblyai-0.8.1/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.0/tests/unit/test_transcript.py` & `assemblyai-0.8.1/tests/unit/test_transcript.py`

 * *Files identical despite different names*

