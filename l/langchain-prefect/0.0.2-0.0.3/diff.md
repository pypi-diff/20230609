# Comparing `tmp/langchain-prefect-0.0.2.tar.gz` & `tmp/langchain-prefect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-prefect-0.0.2.tar", last modified: Tue Mar 14 15:46:26 2023, max compression
+gzip compressed data, was "langchain-prefect-0.0.3.tar", last modified: Thu Jun  8 21:59:48 2023, max compression
```

## Comparing `langchain-prefect-0.0.2.tar` & `langchain-prefect-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:46:26.793189 langchain-prefect-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-14 15:46:26.793189 langchain-prefect-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:46:26.797189 langchain-prefect-0.0.2/langchain_prefect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/langchain_prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:46:26.797189 langchain-prefect-0.0.2/langchain_prefect/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/langchain_prefect/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/langchain_prefect/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/langchain_prefect/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/langchain_prefect/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:46:26.793189 langchain-prefect-0.0.2/langchain_prefect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-14 15:46:26.000000 langchain-prefect-0.0.2/langchain_prefect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-14 15:46:26.000000 langchain-prefect-0.0.2/langchain_prefect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:46:26.000000 langchain-prefect-0.0.2/langchain_prefect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-14 15:46:26.000000 langchain-prefect-0.0.2/langchain_prefect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-14 15:46:26.000000 langchain-prefect-0.0.2/langchain_prefect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-14 15:46:26.000000 langchain-prefect-0.0.2/langchain_prefect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-14 15:46:26.793189 langchain-prefect-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:46:26.793189 langchain-prefect-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-03-14 15:45:36.000000 langchain-prefect-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/langchain_prefect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/langchain_prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/langchain_prefect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/langchain_prefect/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/langchain_prefect/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/langchain_prefect/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/langchain_prefect/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/langchain_prefect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-08 21:59:48.000000 langchain-prefect-0.0.3/langchain_prefect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-08 21:59:48.000000 langchain-prefect-0.0.3/langchain_prefect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:59:48.000000 langchain-prefect-0.0.3/langchain_prefect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 21:59:48.000000 langchain-prefect-0.0.3/langchain_prefect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 21:59:48.000000 langchain-prefect-0.0.3/langchain_prefect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 21:59:48.000000 langchain-prefect-0.0.3/langchain_prefect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:59:48.286858 langchain-prefect-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-08 21:58:49.000000 langchain-prefect-0.0.3/versioneer.py
```

### Comparing `langchain-prefect-0.0.2/LICENSE` & `langchain-prefect-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/PKG-INFO` & `langchain-prefect-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-prefect
-Version: 0.0.2
+Version: 0.0.3
 Summary: Orchestrate and observe tools built with langchain.
 Home-page: https://github.com/PrefectHQ/langchain-prefect
 Author: Prefect Technologies
 Author-email: nate@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -36,14 +36,16 @@
     <br>
     <a href="https://prefect-community.slack.com" alt="Slack">
         <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
     <a href="https://discourse.prefect.io/" alt="Discourse">
         <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
+Read the [accompanying article](https://medium.com/the-prefect-blog/keeping-your-eyes-on-your-ai-tools-6428664537da) for background
+
 ## Orchestrate and observe langchain using Prefect
 
 Large Language Models (LLMs) are interesting and useful  -  building apps that use them responsibly feels like a no-brainer. Tools like [Langchain](https://github.com/hwchase17/langchain) make it easier to build apps using LLMs. We need to know details about how our apps work, even when we want to use tools with convenient abstractions that may obfuscate those details.
 
 Prefect is built to help data people build, run, and observe event-driven workflows wherever they want. It provides a framework for creating deployments on a whole slew of runtime environments (from Lambda to Kubernetes), and is cloud agnostic (best supports AWS, GCP, Azure). For this reason, it could be a great fit for observing apps that use LLMs.
 
 ## Features
```

### Comparing `langchain-prefect-0.0.2/README.md` & `langchain-prefect-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     <br>
     <a href="https://prefect-community.slack.com" alt="Slack">
         <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
     <a href="https://discourse.prefect.io/" alt="Discourse">
         <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
+Read the [accompanying article](https://medium.com/the-prefect-blog/keeping-your-eyes-on-your-ai-tools-6428664537da) for background
+
 ## Orchestrate and observe langchain using Prefect
 
 Large Language Models (LLMs) are interesting and useful  -  building apps that use them responsibly feels like a no-brainer. Tools like [Langchain](https://github.com/hwchase17/langchain) make it easier to build apps using LLMs. We need to know details about how our apps work, even when we want to use tools with convenient abstractions that may obfuscate those details.
 
 Prefect is built to help data people build, run, and observe event-driven workflows wherever they want. It provides a framework for creating deployments on a whole slew of runtime environments (from Lambda to Kubernetes), and is cloud agnostic (best supports AWS, GCP, Azure). For this reason, it could be a great fit for observing apps that use LLMs.
 
 ## Features
```

### Comparing `langchain-prefect-0.0.2/langchain_prefect/loaders.py` & `langchain-prefect-0.0.3/langchain_prefect/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,14 @@
                 headers=self.request_headers,
                 params={
                     "per_page": remaining if remaining < per_page else per_page,
                     "page": page,
                     "include": "comments",
                 },
             )
-            print(response.url)
-            exit()
             response.raise_for_status()
             if not (new_issues := response.json()):
                 break
             issues.extend([GitHubIssue(**issue) for issue in new_issues])
             page += 1
         return issues
```

### Comparing `langchain-prefect-0.0.2/langchain_prefect/plugins.py` & `langchain-prefect-0.0.3/langchain_prefect/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for defining Prefect plugins for langchain."""
 
 from contextlib import ContextDecorator
 from functools import wraps
 from typing import Callable
 
-from langchain.schema import BaseLanguageModel, LLMResult
+from langchain.schema import LLMResult
+from langchain.base_language import BaseLanguageModel
 from prefect import Flow
 from prefect import tags as prefect_tags
 
 from langchain_prefect.utilities import (
     flow_wrapped_fn,
     get_prompt_content,
     llm_invocation_summary,
```

### Comparing `langchain-prefect-0.0.2/langchain_prefect/types.py` & `langchain-prefect-0.0.3/langchain_prefect/types.py`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/langchain_prefect/utilities.py` & `langchain-prefect-0.0.3/langchain_prefect/utilities.py`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/langchain_prefect.egg-info/PKG-INFO` & `langchain-prefect-0.0.3/langchain_prefect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-prefect
-Version: 0.0.2
+Version: 0.0.3
 Summary: Orchestrate and observe tools built with langchain.
 Home-page: https://github.com/PrefectHQ/langchain-prefect
 Author: Prefect Technologies
 Author-email: nate@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -36,14 +36,16 @@
     <br>
     <a href="https://prefect-community.slack.com" alt="Slack">
         <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
     <a href="https://discourse.prefect.io/" alt="Discourse">
         <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
+Read the [accompanying article](https://medium.com/the-prefect-blog/keeping-your-eyes-on-your-ai-tools-6428664537da) for background
+
 ## Orchestrate and observe langchain using Prefect
 
 Large Language Models (LLMs) are interesting and useful  -  building apps that use them responsibly feels like a no-brainer. Tools like [Langchain](https://github.com/hwchase17/langchain) make it easier to build apps using LLMs. We need to know details about how our apps work, even when we want to use tools with convenient abstractions that may obfuscate those details.
 
 Prefect is built to help data people build, run, and observe event-driven workflows wherever they want. It provides a framework for creating deployments on a whole slew of runtime environments (from Lambda to Kubernetes), and is cloud agnostic (best supports AWS, GCP, Azure). For this reason, it could be a great fit for observing apps that use LLMs.
 
 ## Features
```

### Comparing `langchain-prefect-0.0.2/langchain_prefect.egg-info/SOURCES.txt` & `langchain-prefect-0.0.3/langchain_prefect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/setup.cfg` & `langchain-prefect-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/setup.py` & `langchain-prefect-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/tests/test_block_standards.py` & `langchain-prefect-0.0.3/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/tests/test_plugins.py` & `langchain-prefect-0.0.3/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/tests/test_utilities.py` & `langchain-prefect-0.0.3/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `langchain-prefect-0.0.2/versioneer.py` & `langchain-prefect-0.0.3/versioneer.py`

 * *Files identical despite different names*

