# Comparing `tmp/thendisnever-0.2.0.tar.gz` & `tmp/thendisnever-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thendisnever-0.2.0.tar", max compression
+gzip compressed data, was "thendisnever-0.3.0.tar", max compression
```

## Comparing `thendisnever-0.2.0.tar` & `thendisnever-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.2.0/LICENSE
--rw-r--r--   0        0        0     1693 2023-06-09 02:52:26.624335 thendisnever-0.2.0/README.md
--rw-r--r--   0        0        0      569 2023-06-09 02:47:28.797807 thendisnever-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.2.0/src/thendisnever/__init__.py
--rw-r--r--   0        0        0     2800 2023-06-08 17:49:38.772382 thendisnever-0.2.0/src/thendisnever/thend.py
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 thendisnever-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1693 2023-06-09 02:52:26.624335 thendisnever-0.3.0/README.md
+-rw-r--r--   0        0        0      569 2023-06-09 13:50:08.385204 thendisnever-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.3.0/src/thendisnever/__init__.py
+-rw-r--r--   0        0        0     3007 2023-06-09 13:56:53.219614 thendisnever-0.3.0/src/thendisnever/thend.py
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 thendisnever-0.3.0/PKG-INFO
```

### Comparing `thendisnever-0.2.0/LICENSE` & `thendisnever-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thendisnever-0.2.0/README.md` & `thendisnever-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `thendisnever-0.2.0/pyproject.toml` & `thendisnever-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thendisnever"
-version = "0.2.0"
+version = "0.3.0"
 description = "A package to easily make an LLM talk with itself for eternity."
 authors = ["Andrew Hinh <ajhinh@gmail.com>"]
 repository = "https://github.com/andrewhinh/thendisnever"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `thendisnever-0.2.0/src/thendisnever/thend.py` & `thendisnever-0.3.0/src/thendisnever/thend.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,23 @@
                 AutoModelForCausalLM, # To generate the response
                 TextStreamer # To stream the response
             ) # To import the necessary classes
 
             # Setup the model
             model = AutoModelForCausalLM.from_pretrained(model_name) # To load the model
             tokenizer = AutoTokenizer.from_pretrained(model_name) # To load the tokenizer
-            streamer = TextStreamer(tokenizer) # To create the streamer
+            streamer = TextStreamer(
+                tokenizer, # To tokenize the response
+                skip_prompt=True # To skip the prompt when streaming
+            ) # To create the streamer
 
             # Setup the conversation loop
             max_length = model.config.max_length # To get the max length of the model
             max_memory = int(max_length * max_memory_ratio) # To calculate the max memory of the model
+            print(prompt) # To print the initial prompt since it's not streamed
             while True: # To loop the conversation
                 inputs = tokenizer(
                     [prompt], # wrapping prompt as a list since inputs are usually a batch
                     return_tensors="pt" # To return PyTorch tensors
                 ) # To tokenize the prompt
                 response = model.generate(
                     **inputs, # **inputs unpacks the dictionary into keyword arguments
```

### Comparing `thendisnever-0.2.0/PKG-INFO` & `thendisnever-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thendisnever
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package to easily make an LLM talk with itself for eternity.
 Home-page: https://github.com/andrewhinh/thendisnever
 License: MIT
 Author: Andrew Hinh
 Author-email: ajhinh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

