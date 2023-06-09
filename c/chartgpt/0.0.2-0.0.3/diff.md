# Comparing `tmp/chartgpt-0.0.2.tar.gz` & `tmp/chartgpt-0.0.3.tar.gz`

## Comparing `chartgpt-0.0.2.tar` & `chartgpt-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0  4224175 2020-02-02 00:00:00.000000 chartgpt-0.0.2/demo.html
--rw-r--r--   0        0        0  3670734 2020-02-02 00:00:00.000000 chartgpt-0.0.2/demo.ipynb
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 chartgpt-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 chartgpt-0.0.2/requirements.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/chartgpt.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/constants.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/llm.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/prompts/base.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 chartgpt-0.0.2/chartgpt/prompts/generate_python_code.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.2/docs/api-generated.md
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 chartgpt-0.0.2/docs/index.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 chartgpt-0.0.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.2/LICENSE
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 chartgpt-0.0.2/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 chartgpt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 chartgpt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/__main__.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/chartgpt.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/constants.py
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/llm.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/prompts/base.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/prompts/generate_python_code.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/api-generated.md
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/index.md
+-rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/assets/dash.png
+-rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/assets/notebook.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.3/tests/test_run_code.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 chartgpt-0.0.3/README.md
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 chartgpt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 chartgpt-0.0.3/PKG-INFO
```

### Comparing `chartgpt-0.0.2/mkdocs.yml` & `chartgpt-0.0.3/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     default_handler: python
 
 theme:
   name: material
   palette:
   - media: '(prefers-color-scheme: light)'
     scheme: default
-    primary: teal
+    primary: indigo
     accent: amber
     toggle:
-      icon: material/lightbulb
-      name: Switch to light mode
+      icon: material/brightness-2
+      name: Switch to dark mode
   - media: '(prefers-color-scheme: dark)'
     scheme: slate
-    primary: teal
+    primary: indigo
     accent: amber
     toggle:
-      icon: material/lightbulb-outline
-      name: Switch to dark mode
+      icon: material/weather-sunny
+      name: Switch to light mode
   features:
   - search.suggest
   - search.highlight
   - content.tabs.link
   icon:
     repo: fontawesome/brands/github-alt
   logo: https://avatars.githubusercontent.com/u/119681016?s=200&v=4
   language: fr
 repo_name: chatgpt/chart
 repo_url: https://github.com/chatgpt/chart
-edit_uri: ''
+edit_uri: ''
```

### Comparing `chartgpt-0.0.2/chartgpt/constants.py` & `chartgpt-0.0.3/chartgpt/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Constants used in the pandasai package.
 
-It includes Start & End Code tags, Whitelisted Python Packages and While List Builtin Methods.
+It includes Start & End Code tags, Whitelisted Python Packages and While List \
+Builtin Methods.
 
 """
 
-START_CODE_TAG = "<startCode>"
-END_CODE_TAG = "<endCode>"
+START_CODE_TAG = "```"
+END_CODE_TAG = "```"
 WHITELISTED_LIBRARIES = [
     "numpy",
     "matplotlib",
 ]
 WHITELISTED_BUILTINS = [
     "abs",
     "all",
@@ -71,8 +72,8 @@
     "str",
     "sum",
     "super",
     "tuple",
     "type",
     "vars",
     "zip",
-]
+]
```

### Comparing `chartgpt-0.0.2/chartgpt/llm.py` & `chartgpt-0.0.3/chartgpt/llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,105 @@
 import os
 import re
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 
 import openai
 
 from .constants import END_CODE_TAG, START_CODE_TAG
 from .prompts.base import Prompt
 
-# from abc import ABC, abstractmethod
-
 
 class LLM:
+    """LLM class for generating code from a prompt.
+
+    Args:
+        model_name (str, optional): Model name. Defaults to "text-davinci-003".
+        temperature (int, optional): Temperature. Defaults to 0.2.
+        max_tokens (int, optional): Max tokens. Defaults to 1000.
+        top_p (int, optional): Top p. Defaults to 1.
+        frequency_penalty (int, optional): Frequency penalty. Defaults to 0.
+        presence_penalty (int, optional): Presence penalty. Defaults to 0.
+        api_key (str, optional): OpenAI API key. Defaults to None.
+
+    Raises:
+        ValueError: If no API key is provided.
+
+    Returns:
+        str: Generated code
+    """
+
     def __init__(
         self,
-        temperature: int = 0.2,
         model_name: str = "text-davinci-003",
+        temperature: int = 0.2,
         max_tokens: int = 1000,
+        top_p: int = 1,
+        frequency_penalty: int = 0,
+        presence_penalty: int = 0,
+        api_key: str = None,
     ):
+        self.model_name = model_name
         self.temperature = temperature
         self.max_tokens = max_tokens
-        self.top_p = 1
-        self.frequency_penalty = 0
-        self.presence_penalty = 0
+        self.top_p = top_p
+        self.frequency_penalty = frequency_penalty
+        self.presence_penalty = presence_penalty
+
+        self.api_key = api_key or os.getenv("OPENAI_API_KEY") or None
+        if self.api_key is None:
+            raise ValueError("Please provide an OpenAI API key")
+        openai.api_key = self.api_key
 
     def _extract_code(self, response: str, separator: str = "```") -> str:
         """
         Extract the code from the response.
 
         Args:
             response (str): Response
             separator (str, optional): Separator. Defaults to "```".
 
-        Raises:
-            NoCodeFoundError: No code found in the response
-
         Returns:
             str: Extracted code from the response
         """
         code = response
         match = re.search(
             rf"{START_CODE_TAG}(.*)({END_CODE_TAG}|{END_CODE_TAG.replace('<', '</')})",
             code,
             re.DOTALL,
         )
         if match:
             code = match.group(1).strip()
         if len(code.split(separator)) > 1:
             code = code.split(separator)[1]
-        print(code)
+
+        if "fig.show()" in code:
+            code = code.replace("fig.show()", "fig")
 
         return code
 
     def generate_code(self, instruction: Prompt, prompt: str) -> str:
         """
         Generate the code based on the instruction and the given prompt.
 
         Returns:
             str: Code
         """
-
-        prompt = str(instruction) + prompt
-
-        return self._extract_code(
-            self.completion(prompt)
-        )
+        return self._extract_code(self.completion(str(instruction) + prompt))
 
     @property
     def _default_params(self) -> Dict[str, Any]:
-
         """
         Get the default parameters for calling OpenAI API
 
         Returns (Dict): A dict of OpenAi API parameters
 
         """
 
         return {
-            "model": "text-davinci-003",
+            "model": self.model_name,
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
             "top_p": self.top_p,
             "frequency_penalty": self.frequency_penalty,
             "presence_penalty": self.presence_penalty,
         }
```

### Comparing `chartgpt-0.0.2/chartgpt/prompts/base.py` & `chartgpt-0.0.3/chartgpt/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.2/chartgpt/prompts/generate_python_code.py` & `chartgpt-0.0.3/chartgpt/prompts/generate_python_code.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from .base import Prompt
-from chartgpt.constants import START_CODE_TAG, END_CODE_TAG
 from datetime import date
 
+from chartgpt.constants import END_CODE_TAG, START_CODE_TAG
+
+from .base import Prompt
+
 
 class GeneratePythonCodePrompt(Prompt):
     context: str = """
-You are ChartGPT, a data scientist working at a startup. You are asked to analyze a dataset and create a chart.
+You are ChartGPT, a data scientist working at a startup. You are asked to analyze a \
+dataset and create a chart.
 Today is {today_date}.
 You are given a dataset `df` with the following columns: {df_columns}.
 
-When asked about the data, your response must include a python code that uses the library Plotly to make a chart using the dataframe `df`.
-Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
+When asked about the data, your response must include a python code that uses the \
+library Plotly to make a chart using the dataframe `df`. If necessary, you can filter \
+the dataframe `df`. If the question in complex, feel free to use Plotly Graph Objects \
+instead of Plotly Express.
+Using the provided dataframe, df, return the python code and make sure to prefix the \
+requested python code with {START_CODE_TAG} exactly and suffix the code with \
+{END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, **kwargs):
         super().__init__(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
```

### Comparing `chartgpt-0.0.2/docs/index.md` & `chartgpt-0.0.3/docs/index.md`

 * *Files identical despite different names*

