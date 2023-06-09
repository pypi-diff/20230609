# Comparing `tmp/vector_vault-2.0.4.tar.gz` & `tmp/vector_vault-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.4.tar", last modified: Thu Jun  8 04:55:05 2023, max compression
+gzip compressed data, was "vector_vault-2.0.5.tar", last modified: Fri Jun  9 20:04:21 2023, max compression
```

## Comparing `vector_vault-2.0.4.tar` & `vector_vault-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:55:05.426277 vector_vault-2.0.4/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:55:05.426146 vector_vault-2.0.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20080 2023-06-08 04:45:19.000000 vector_vault-2.0.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-08 04:55:05.426319 vector_vault-2.0.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-08 04:54:41.000000 vector_vault-2.0.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:55:05.422977 vector_vault-2.0.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      453 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:55:05.425845 vector_vault-2.0.4/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      143 2023-06-08 04:54:12.000000 vector_vault-2.0.4/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.4/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.4/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.4/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.4/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-08 04:35:31.000000 vector_vault-2.0.4/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.4/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.4/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30728 2023-06-08 04:35:55.000000 vector_vault-2.0.4/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.4/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.4/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 20:04:21.536211 vector_vault-2.0.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-09 20:04:21.536071 vector_vault-2.0.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20080 2023-06-08 04:45:19.000000 vector_vault-2.0.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-09 20:04:21.536245 vector_vault-2.0.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-09 20:04:14.000000 vector_vault-2.0.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 20:04:21.532836 vector_vault-2.0.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-09 20:04:21.000000 vector_vault-2.0.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-09 20:04:21.535655 vector_vault-2.0.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.0.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.5/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1954 2023-06-09 19:11:10.000000 vector_vault-2.0.5/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2398 2023-06-08 04:57:38.000000 vector_vault-2.0.5/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.5/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30807 2023-06-09 19:58:53.000000 vector_vault-2.0.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.5/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.5/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.4/LICENSE` & `vector_vault-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/PKG-INFO` & `vector_vault-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.0.4
+Version: 2.0.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.0.4/README.md` & `vector_vault-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/setup.py` & `vector_vault-2.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.4",
+    version="2.0.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.5/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.4
+Version: 2.0.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.0.4/vectorvault/ai.py` & `vector_vault-2.0.5/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/vectorvault/cloudmanager.py` & `vector_vault-2.0.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/vectorvault/creds.py` & `vector_vault-2.0.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/vectorvault/download.py` & `vector_vault-2.0.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/vectorvault/itemize.py` & `vector_vault-2.0.5/vectorvault/itemize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-import datetime 
+# VECTOR VAULT CONFIDENTIAL
+# __________________
+# 
+#  All Rights Reserved.
+# 
+# NOTICE:  All information contained herein is, and remains
+# the property of Vector Vault and its suppliers,
+# if any.  The intellectual and technical concepts contained
+# herein are proprietary to Vector Vault
+# and its suppliers and may be covered by U.S. and Foreign Patents,
+# patents in process, and are protected by trade secret or copyright law.
+# Dissemination of this information or reproduction of this material
+# is strictly forbidden unless prior written permission is obtained
+# from Vector Vault. See license for consent.import datetime 
+
 from .vecreq import call_name_vecs, call_buildpath
 from annoy import AnnoyIndex
 import threading
 from copy import deepcopy
 
 def itemize(vault, x, meta=None, text=None, name=None):
     meta = deepcopy(meta) if meta else {}
```

### Comparing `vector_vault-2.0.4/vectorvault/tools_gpt.py` & `vector_vault-2.0.5/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.4/vectorvault/vault.py` & `vector_vault-2.0.5/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import json
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
 from .ai import AI
 from .itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name
 from .vecreq import call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
+from .tools_gpt import ToolsGPT
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
@@ -50,14 +51,15 @@
         self.items = []
         self.last_time = None
         self.last_chat_time = None
         self.first_run = True
         self.needed_sleep_time = None
         self.saved_already = False
         self.ai = AI()
+        self.tools = ToolsGPT(verbose=verbose)
 
     def get_vaults(self, vault: str = None):
         vault = self.vault if vault is None else vault
         return call_get_vaults(self.user, self.api, vault)
 
     def get_total_vectors(self):
         return call_get_total_vectors(self.user, self.vault, self.api)
```

### Comparing `vector_vault-2.0.4/vectorvault/vecreq.py` & `vector_vault-2.0.5/vectorvault/vecreq.py`

 * *Files identical despite different names*

