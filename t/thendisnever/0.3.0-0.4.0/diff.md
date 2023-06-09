# Comparing `tmp/thendisnever-0.3.0.tar.gz` & `tmp/thendisnever-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thendisnever-0.3.0.tar", max compression
+gzip compressed data, was "thendisnever-0.4.0.tar", max compression
```

## Comparing `thendisnever-0.3.0.tar` & `thendisnever-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.3.0/LICENSE
--rw-r--r--   0        0        0     1693 2023-06-09 02:52:26.624335 thendisnever-0.3.0/README.md
--rw-r--r--   0        0        0      569 2023-06-09 13:50:08.385204 thendisnever-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.3.0/src/thendisnever/__init__.py
--rw-r--r--   0        0        0     3007 2023-06-09 13:56:53.219614 thendisnever-0.3.0/src/thendisnever/thend.py
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 thendisnever-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1703 2023-06-09 15:50:06.292350 thendisnever-0.4.0/README.md
+-rw-r--r--   0        0        0      569 2023-06-09 15:50:14.984298 thendisnever-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.4.0/src/thendisnever/__init__.py
+-rw-r--r--   0        0        0     4422 2023-06-09 16:00:27.901033 thendisnever-0.4.0/src/thendisnever/thend.py
+-rw-r--r--   0        0        0     2542 1970-01-01 00:00:00.000000 thendisnever-0.4.0/PKG-INFO
```

### Comparing `thendisnever-0.3.0/LICENSE` & `thendisnever-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thendisnever-0.3.0/README.md` & `thendisnever-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 A package to make an LLM talk with itself for eternity.
 
 ```python
 from thendisnever.thend import isnever
 isnever(
   model_name='Fredithefish/ScarletPajama-3B-HF', # Default LLM
   prompt='THE END IS NEVER THE END IS NEVER ', # Default prompt
-  max_memory_ratio=0.25 # Default % of latest tokens to remember
+  max_memory_ratio=0.5 # Default % of latest tokens to remember, 0 < % < 1
 )
 ```
 
 ## Notes
 
 - When running `isnever()` for the first time, it will download the model and tokenizer from HuggingFace. This will take a while, but it only needs to be done once.
 - If you want to use the CPU (not recommended because it's slow, but it works), make sure you have [PyTorch for CPU](https://pytorch.org/get-started/locally/) installed.
```

### Comparing `thendisnever-0.3.0/pyproject.toml` & `thendisnever-0.4.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thendisnever"
-version = "0.3.0"
+version = "0.4.0"
 description = "A package to easily make an LLM talk with itself for eternity."
 authors = ["Andrew Hinh <ajhinh@gmail.com>"]
 repository = "https://github.com/andrewhinh/thendisnever"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `thendisnever-0.3.0/PKG-INFO` & `thendisnever-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thendisnever
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package to easily make an LLM talk with itself for eternity.
 Home-page: https://github.com/andrewhinh/thendisnever
 License: MIT
 Author: Andrew Hinh
 Author-email: ajhinh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 A package to make an LLM talk with itself for eternity.
 
 ```python
 from thendisnever.thend import isnever
 isnever(
   model_name='Fredithefish/ScarletPajama-3B-HF', # Default LLM
   prompt='THE END IS NEVER THE END IS NEVER ', # Default prompt
-  max_memory_ratio=0.25 # Default % of latest tokens to remember
+  max_memory_ratio=0.5 # Default % of latest tokens to remember, 0 < % < 1
 )
 ```
 
 ## Notes
 
 - When running `isnever()` for the first time, it will download the model and tokenizer from HuggingFace. This will take a while, but it only needs to be done once.
 - If you want to use the CPU (not recommended because it's slow, but it works), make sure you have [PyTorch for CPU](https://pytorch.org/get-started/locally/) installed.
```

