# Comparing `tmp/thendisnever-0.1.0.tar.gz` & `tmp/thendisnever-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thendisnever-0.1.0.tar", max compression
+gzip compressed data, was "thendisnever-0.2.0.tar", max compression
```

## Comparing `thendisnever-0.1.0.tar` & `thendisnever-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.1.0/LICENSE
--rw-r--r--   0        0        0     1968 2023-06-09 02:25:23.344497 thendisnever-0.1.0/README.md
--rw-r--r--   0        0        0      569 2023-06-09 02:41:57.919493 thendisnever-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.1.0/src/thendisnever/__init__.py
--rw-r--r--   0        0        0     2800 2023-06-08 17:49:38.772382 thendisnever-0.1.0/src/thendisnever/thend.py
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 thendisnever-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1693 2023-06-09 02:52:26.624335 thendisnever-0.2.0/README.md
+-rw-r--r--   0        0        0      569 2023-06-09 02:47:28.797807 thendisnever-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.2.0/src/thendisnever/__init__.py
+-rw-r--r--   0        0        0     2800 2023-06-08 17:49:38.772382 thendisnever-0.2.0/src/thendisnever/thend.py
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 thendisnever-0.2.0/PKG-INFO
```

### Comparing `thendisnever-0.1.0/LICENSE` & `thendisnever-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thendisnever-0.1.0/README.md` & `thendisnever-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # The End is Never
 
 A package to make an LLM talk with itself for eternity.
 
 ```python
-from thendisnever.theend import isnever
+from thendisnever.thend import isnever
 isnever(
   model_name='Fredithefish/ScarletPajama-3B-HF', # Default LLM
   prompt='THE END IS NEVER THE END IS NEVER ', # Default prompt
   max_memory_ratio=0.25 # Default % of latest tokens to remember
 )
 ```
 
 ## Notes
 
-- For the default LLM (which you can change as shown above), you'll need at least:
-  - ~ 6GB of free disk space
-  - ~ 15GB of RAM
 - When running `isnever()` for the first time, it will download the model and tokenizer from HuggingFace. This will take a while, but it only needs to be done once.
 - If you want to use the CPU (not recommended because it's slow, but it works), make sure you have [PyTorch for CPU](https://pytorch.org/get-started/locally/) installed.
 
 ## Contributing
 
 1. Install [poetry](https://python-poetry.org/docs/#installation) if necessary.
 1. Create and setup the poetry environment:
@@ -35,32 +32,21 @@
 
 1. Build the package:
 
     ```bash
     poetry build
     ```
 
-1. Add `TestPyPI` as a source:
-
-    ```bash
-    poetry config repositories.testpypi https://test.pypi.org/legacy/
-    ```
-
-1. Publish the package to `TestPyPI`:
-
-    ```bash
-    poetry publish -r testpypi
-    ```
-
 1. Test the package in a fresh environment:
 
     ```bash
-    pip install --index-url https://test.pypi.org/simple/ --no-deps --upgrade thendisnever
+    pip install dist/thendisnever-<version>.tar.gz
     ```
 
 1. Once confirmed to work, make a PR from a feature branch to main on GitHub.
 1. Once PR is merged, [email me](ajhinh@gmail.com) to be added as a collaborator on PyPI.
 1. Once added as a collaborator, publish the package to `PyPI`:
   
       ```bash
+      poetry config pypi-token.pypi <your-token> # Get your token from https://pypi.org/manage/account/token/
       poetry publish
       ```
```

### Comparing `thendisnever-0.1.0/pyproject.toml` & `thendisnever-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thendisnever"
-version = "0.1.0"
+version = "0.2.0"
 description = "A package to easily make an LLM talk with itself for eternity."
 authors = ["Andrew Hinh <ajhinh@gmail.com>"]
 repository = "https://github.com/andrewhinh/thendisnever"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `thendisnever-0.1.0/src/thendisnever/thend.py` & `thendisnever-0.2.0/src/thendisnever/thend.py`

 * *Files identical despite different names*

### Comparing `thendisnever-0.1.0/PKG-INFO` & `thendisnever-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thendisnever
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package to easily make an LLM talk with itself for eternity.
 Home-page: https://github.com/andrewhinh/thendisnever
 License: MIT
 Author: Andrew Hinh
 Author-email: ajhinh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,27 +20,24 @@
 Description-Content-Type: text/markdown
 
 # The End is Never
 
 A package to make an LLM talk with itself for eternity.
 
 ```python
-from thendisnever.theend import isnever
+from thendisnever.thend import isnever
 isnever(
   model_name='Fredithefish/ScarletPajama-3B-HF', # Default LLM
   prompt='THE END IS NEVER THE END IS NEVER ', # Default prompt
   max_memory_ratio=0.25 # Default % of latest tokens to remember
 )
 ```
 
 ## Notes
 
-- For the default LLM (which you can change as shown above), you'll need at least:
-  - ~ 6GB of free disk space
-  - ~ 15GB of RAM
 - When running `isnever()` for the first time, it will download the model and tokenizer from HuggingFace. This will take a while, but it only needs to be done once.
 - If you want to use the CPU (not recommended because it's slow, but it works), make sure you have [PyTorch for CPU](https://pytorch.org/get-started/locally/) installed.
 
 ## Contributing
 
 1. Install [poetry](https://python-poetry.org/docs/#installation) if necessary.
 1. Create and setup the poetry environment:
@@ -56,33 +53,22 @@
 
 1. Build the package:
 
     ```bash
     poetry build
     ```
 
-1. Add `TestPyPI` as a source:
-
-    ```bash
-    poetry config repositories.testpypi https://test.pypi.org/legacy/
-    ```
-
-1. Publish the package to `TestPyPI`:
-
-    ```bash
-    poetry publish -r testpypi
-    ```
-
 1. Test the package in a fresh environment:
 
     ```bash
-    pip install --index-url https://test.pypi.org/simple/ --no-deps --upgrade thendisnever
+    pip install dist/thendisnever-<version>.tar.gz
     ```
 
 1. Once confirmed to work, make a PR from a feature branch to main on GitHub.
 1. Once PR is merged, [email me](ajhinh@gmail.com) to be added as a collaborator on PyPI.
 1. Once added as a collaborator, publish the package to `PyPI`:
   
       ```bash
+      poetry config pypi-token.pypi <your-token> # Get your token from https://pypi.org/manage/account/token/
       poetry publish
       ```
```

