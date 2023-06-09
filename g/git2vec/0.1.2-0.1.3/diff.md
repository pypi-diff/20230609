# Comparing `tmp/git2vec-0.1.2.tar.gz` & `tmp/git2vec-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.2.tar", last modified: Sat Jun  3 12:00:22 2023, max compression
+gzip compressed data, was "git2vec-0.1.3.tar", last modified: Fri Jun  9 14:01:50 2023, max compression
```

## Comparing `git2vec-0.1.2.tar` & `git2vec-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:00:22.236302 git2vec-0.1.2/
--rw-rw-rw-   0        0        0     2805 2023-06-03 12:00:22.235303 git2vec-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2151 2023-06-03 11:58:52.000000 git2vec-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 12:00:22.224911 git2vec-0.1.2/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-03 01:26:04.000000 git2vec-0.1.2/git2vec/__init__.py
--rw-rw-rw-   0        0        0     4660 2023-06-03 11:42:33.000000 git2vec-0.1.2/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-03 00:41:21.000000 git2vec-0.1.2/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:00:22.234304 git2vec-0.1.2/git2vec.egg-info/
--rw-rw-rw-   0        0        0     2805 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:00:22.236302 git2vec-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-06-03 11:59:12.000000 git2vec-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:01:50.107738 git2vec-0.1.3/
+-rw-rw-rw-   0        0        0     2805 2023-06-09 14:01:50.106736 git2vec-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2151 2023-06-03 12:01:57.000000 git2vec-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 14:01:50.091687 git2vec-0.1.3/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-03 12:01:57.000000 git2vec-0.1.3/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     4805 2023-06-09 14:01:22.000000 git2vec-0.1.3/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-03 12:01:57.000000 git2vec-0.1.3/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:01:50.103737 git2vec-0.1.3/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2805 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 14:01:50.000000 git2vec-0.1.3/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:01:50.108740 git2vec-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-06-09 14:01:33.000000 git2vec-0.1.3/setup.py
```

### Comparing `git2vec-0.1.2/PKG-INFO` & `git2vec-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.2
+Version: 0.1.3
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.2/README.md` & `git2vec-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.2/git2vec/loader.py` & `git2vec-0.1.3/git2vec/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import concurrent.futures
 import os
 from typing import Callable, List, Optional
+import shutil
 
 from langchain.docstore.document import Document
 from langchain.document_loaders.base import BaseLoader
 
 UNWANTED_TYPES = [
     ".ipynb",
     ".yaml",
@@ -12,14 +13,17 @@
     ".json",
     ".png",
     ".jpg",
     ".jpeg",
     ".gif",
     ".svg",
     "csv",
+    "",
+    ".txt",
+
 ]
 
 
 class TurboGitLoader(BaseLoader):
     """
     Loads files from a Git repository into a list of documents in parallel.
 
@@ -132,19 +136,24 @@
     return raw_repo
 
 
 def load(repo, branch="main", return_str=False):
     """ Load the git repo data using TurboGitLoader """
     folder_name = repo.split("/")[-1]
     filter_fn = lambda x: not any([x.endswith(t) for t in UNWANTED_TYPES])
+    repo_path = f"./repo_loader_data/{folder_name}/"
 
+    # load repo data
     repo_docs = TurboGitLoader(
         clone_url=repo,
-        repo_path=f"./repo_loader_data/{folder_name}/",
+        repo_path=repo_path,
         branch=branch,
         file_filter=filter_fn,
     ).load()
 
+    # cleanup repo data
+    shutil.rmtree(repo_path)
+
     if return_str:
         return docs_to_str(repo_docs)
     else:
         return repo_docs
```

### Comparing `git2vec-0.1.2/git2vec/vectordb.py` & `git2vec-0.1.3/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.2/git2vec.egg-info/PKG-INFO` & `git2vec-0.1.3/git2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.2
+Version: 0.1.3
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.2/setup.py` & `git2vec-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1.2',
+    version='0.1.3',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

