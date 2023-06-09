# Comparing `tmp/magic_decorator-0.0.4.tar.gz` & `tmp/magic_decorator-0.0.5.tar.gz`

## Comparing `magic_decorator-0.0.4.tar` & `magic_decorator-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/magic_decorator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/LICENSE
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/magic_decorator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/PKG-INFO
```

### Comparing `magic_decorator-0.0.4/magic_decorator.py` & `magic_decorator-0.0.5/magic_decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,14 +38,21 @@
             ),
             alias="return",
         )
 
     return Answer
 
 
+SYSTEM_PROMPT = (
+    "You are now the following python function:\n"
+    "```\n"
+    "{function_code}\n"
+    "```\n\n"
+    "{json_prompt}"
+)
 def magic(return_thought=False, **openai_kwargs):
     def wrapper(func):
         @wraps(func)
         def do_magic(*args, **kwargs):
             function_code = _function_stringfy(func)
             arguments = []
             for arg in args:
@@ -57,20 +64,17 @@
             return_annotation = inspect.signature(func).return_annotation
             return_model = get_return_model(return_annotation)
             json_prompt = get_json_format_prompt(return_model)
 
             messages = [
                 {
                     "role": "system",
-                    "content": (
-                        f"You are now the following python function:\n"
-                        "```\n"
-                        f"{function_code}\n"
-                        f"```\n\n"
-                        f"{json_prompt}"
+                    "content": SYSTEM_PROMPT.format(
+                        function_code=function_code,
+                        json_prompt=json_prompt,
                     ),
                 },
                 {
                     "role": "user",
                     "content": arguments_string,
                 },
             ]
@@ -98,7 +102,56 @@
                 return bot_says["return"], bot_says["thought"]
             else:
                 return bot_says["return"]
 
         return do_magic
 
     return wrapper
+
+try:
+    from langchain.chains import LLMChain
+    from langchain.chat_models import AzureChatOpenAI
+    from langchain.base_language import BaseLanguageModel
+    from langchain.schema import BaseOutputParser
+    from langchain.prompts import SystemMessagePromptTemplate, HumanMessagePromptTemplate, ChatPromptTemplate
+
+    def magic_langchain(llm: BaseLanguageModel):
+        def wrapper(func):
+            function_code = _function_stringfy(func)
+            return_annotation = inspect.signature(func).return_annotation
+            return_model = get_return_model(return_annotation)
+            json_prompt = get_json_format_prompt(return_model)
+
+            system_prompt = SYSTEM_PROMPT.format(
+                function_code=function_code,
+                json_prompt=json_prompt,
+            ).replace("{", "{{").replace("}", "}}")
+
+            argument_list = list(inspect.signature(func).parameters.keys())
+            arguments = ", ".join(["{" + key + "}" for key in argument_list])
+            user_prompt = f"{func.__name__}({arguments})"
+
+            class SickJSONParser(BaseOutputParser):
+                def parse(self, text: str):
+                    return sick_json.parse(
+                        text,
+                        pydantic_model=return_model,
+                    )["return"]
+
+            template = ChatPromptTemplate(
+                input_variables=argument_list,
+                messages=[
+                    SystemMessagePromptTemplate.from_template(system_prompt),
+                    HumanMessagePromptTemplate.from_template(user_prompt),
+                ],
+                output_parser=SickJSONParser(),
+            )
+
+            chain = LLMChain(
+                llm=llm,
+                prompt=template,
+            )
+
+            return chain
+        return wrapper
+except Exception as e:
+    pass
```

### Comparing `magic_decorator-0.0.4/.gitignore` & `magic_decorator-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.4/LICENSE` & `magic_decorator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.4/README.md` & `magic_decorator-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,8 +60,18 @@
 ```python
 cold_magic = magic(model="gpt-4", temperature=0)
 @cold_magic
 def func():
     ...
 ```
 
+Added a decorator for langchain. In this case, it becomes LLMChain.
+```python
+llm = SomeLLMModels()
+@magic_langchain(llm=llm)
+def mychain():
+    ...
+
+mychain.predict_and_parse()
+```
+
 There is no preprocessing, no postprocessing, and no error handling in this module. It's just code to do a simple thing, so there are no prompts to encourage better answers.
```

### Comparing `magic_decorator-0.0.4/pyproject.toml` & `magic_decorator-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "magic-decorator"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name="Kim Minjong", email="make.dirty.code@gmail.com"},
 ]
 description = "A magic function decorator using OpenAI ChatCompletion"
 readme = "README.md"
 requires-python = ">=3.7.1"
 dependencies = ["openai>0.27", "sick-json"]
```

### Comparing `magic_decorator-0.0.4/PKG-INFO` & `magic_decorator-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-decorator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A magic function decorator using OpenAI ChatCompletion
 Author-email: Kim Minjong <make.dirty.code@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
@@ -74,8 +74,18 @@
 ```python
 cold_magic = magic(model="gpt-4", temperature=0)
 @cold_magic
 def func():
     ...
 ```
 
+Added a decorator for langchain. In this case, it becomes LLMChain.
+```python
+llm = SomeLLMModels()
+@magic_langchain(llm=llm)
+def mychain():
+    ...
+
+mychain.predict_and_parse()
+```
+
 There is no preprocessing, no postprocessing, and no error handling in this module. It's just code to do a simple thing, so there are no prompts to encourage better answers.
```

