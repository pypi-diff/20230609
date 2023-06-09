# Comparing `tmp/idoctorai-0.2.1.tar.gz` & `tmp/idoctorai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.2.1.tar", max compression
+gzip compressed data, was "idoctorai-0.3.1.tar", max compression
```

## Comparing `idoctorai-0.2.1.tar` & `idoctorai-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.2.1/LICENSE
--rw-r--r--   0        0        0    19001 2023-06-07 12:41:32.619799 idoctorai-0.2.1/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.2.1/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.2.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.2.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.2.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.2.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.2.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.2.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.2.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.2.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.2.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.2.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11096 2023-06-07 12:25:21.036958 idoctorai-0.2.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.2.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.2.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.2.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.2.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.2.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.2.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.2.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.2.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.2.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.2.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.2.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1511 2023-06-07 12:41:32.620825 idoctorai-0.2.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1396 2023-06-07 12:41:32.621795 idoctorai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-07 12:41:32.591875 idoctorai-0.2.1/README.md
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 idoctorai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.1/LICENSE
+-rw-r--r--   0        0        0    19001 2023-06-08 05:58:42.811892 idoctorai-0.3.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2332 2023-06-09 12:47:59.549794 idoctorai-0.3.1/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11261 2023-06-09 13:00:38.629850 idoctorai-0.3.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3209 2023-06-09 10:29:55.340192 idoctorai-0.3.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1454 2023-06-09 13:01:37.250641 idoctorai-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.1/README.md
+-rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 idoctorai-0.3.1/PKG-INFO
```

### Comparing `idoctorai-0.2.1/LICENSE` & `idoctorai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/__init__.py` & `idoctorai-0.3.1/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/constants.py` & `idoctorai-0.3.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/exceptions.py` & `idoctorai-0.3.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/helpers/_optional.py` & `idoctorai-0.3.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/helpers/anonymizer.py` & `idoctorai-0.3.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/helpers/cache.py` & `idoctorai-0.3.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/helpers/from_excel.py` & `idoctorai-0.3.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/helpers/notebook.py` & `idoctorai-0.3.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/helpers/save_chart.py` & `idoctorai-0.3.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/llm/azure_openai.py` & `idoctorai-0.3.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/llm/base.py` & `idoctorai-0.3.1/pandasai/llm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,18 +232,23 @@
                     "content": value,
                 }
             ],
         }
 
         if self.stop is not None:
             params["stop"] = [self.stop]
-
+      
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
+    
+    def langchain_input(self, value:str) -> str:
+        response = self.langchain.__call__(value)
+        # print(response)
+        return response
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
 
     LLM base class is extended to be used with HuggingFace LLM Modes APIs
```

### Comparing `idoctorai-0.2.1/pandasai/llm/fake.py` & `idoctorai-0.3.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/llm/google_palm.py` & `idoctorai-0.3.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/llm/open_assistant.py` & `idoctorai-0.3.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/llm/openai.py` & `idoctorai-0.3.1/pandasai/llm/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import openai
 from dotenv import load_dotenv
 
 from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
 from ..prompts.base import Prompt
 from .base import BaseOpenAI
 
+from ..langchain import LangChain
+
 load_dotenv()
 
 
 class OpenAI(BaseOpenAI):
     """OpenAI LLM using BaseOpenAI Class.
 
     An API call to OpenAi API is sent and response is recorded and returned.
@@ -39,14 +41,15 @@
         "gpt-4-32k-0314",
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0301",
     ]
     _supported_completion_models = ["text-davinci-003"]
 
     model: str = "gpt-3.5-turbo"
+    langchain: LangChain
 
     def __init__(
         self,
         api_token: Optional[str] = None,
         **kwargs,
     ):
         """
@@ -59,14 +62,17 @@
         """
 
         self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("OpenAI API key is required")
         openai.api_key = self.api_token
 
+        # langchain 
+        self.langchain = LangChain(api_token=self.api_token)
+
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API"""
         return {
             **super()._default_params,
@@ -89,15 +95,16 @@
             str: Response
         """
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value) + suffix)
         elif self.model in self._supported_chat_models:
-            response = self.chat_completion(str(instruction) + str(value) + suffix)
+            # response = self.chat_completion(str(instruction) + str(value) + suffix)
+            response = self.langchain_input(str(instruction) + str(value) + suffix)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
```

### Comparing `idoctorai-0.2.1/pandasai/llm/starcoder.py` & `idoctorai-0.3.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/prompts/base.py` & `idoctorai-0.3.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.3.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.3.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/prompts/generate_python_code.py` & `idoctorai-0.3.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/prompts/generate_response.py` & `idoctorai-0.3.1/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.3.1/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.2.1/pyproject.toml` & `idoctorai-0.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.2.1"
-description = "this is idoctorai"
+version = "0.3.1"
+description = "this is idoctorai, Generate code with natural speech"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
+langchain = "0.0.194"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `idoctorai-0.2.1/PKG-INFO` & `idoctorai-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.2.1
-Summary: this is idoctorai
+Version: 0.3.1
+Summary: this is idoctorai, Generate code with natural speech
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
+Requires-Dist: langchain (==0.0.194)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## idoctorai
 
-this is idoctorai
+this is idoctorai, generate code with nlp
+
+use langchain generate code in this version
+
+
```

