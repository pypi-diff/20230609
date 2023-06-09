# Comparing `tmp/gpt_fn-0.0.1.post2.tar.gz` & `tmp/gpt_fn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.1.post2.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.2.tar", max compression
```

## Comparing `gpt_fn-0.0.1.post2.tar` & `gpt_fn-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1066 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/LICENSE
--rw-r--r--   0        0        0     3023 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/README.md
--rw-r--r--   0        0        0      615 2023-06-09 02:27:24.989294 gpt_fn-0.0.1.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/__init__.py
--rw-r--r--   0        0        0      806 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/ai_function.py
--rw-r--r--   0        0        0      537 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/conftest.py
--rw-r--r--   0        0        0        0 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0     3149 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0     3977 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0      872 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/tests/test_ai_function.py
--rw-r--r--   0        0        0        0 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/__init__.py
--rw-r--r--   0        0        0     1953 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     2412 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/tests/__init__.py
--rw-r--r--   0        0        0      960 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0     5591 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0      685 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     1733 2023-06-09 02:26:56.880685 gpt_fn-0.0.1.post2/src/fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     3441 1970-01-01 00:00:00.000000 gpt_fn-0.0.1.post2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-09 06:31:39.066087 gpt_fn-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3023 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/README.md
+-rw-r--r--   0        0        0      642 2023-06-09 06:32:07.202261 gpt_fn-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/__init__.py
+-rw-r--r--   0        0        0      869 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/ai_function.py
+-rw-r--r--   0        0        0      537 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/conftest.py
+-rw-r--r--   0        0        0      625 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/__init__.py
+-rw-r--r--   0        0        0      284 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0      330 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0     3356 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0     4299 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0      872 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0      490 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     2411 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0     5591 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0      892 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     1733 2023-06-09 06:31:39.070087 gpt_fn-0.0.2/src/fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 gpt_fn-0.0.2/PKG-INFO
```

### Comparing `gpt_fn-0.0.1.post2/LICENSE` & `gpt_fn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/README.md` & `gpt_fn-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/pyproject.toml` & `gpt_fn-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.1.post2"
+version = "0.0.2"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "fn", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-openai = "^0.27.7"
-pydantic = "^1.10.8"
+openai = "^0.27"
+pydantic = "^1.0"
+jinja2 = "^3.0"
 
 [tool.poetry.group.test.dependencies]
 syrupy = "^4.0.2"
 pytest-vcr = "^1.0.2"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "default-unprefixed"
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/ai_function.py` & `gpt_fn-0.0.2/src/fn/ai_function.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from functools import wraps
 from typing import Any, Callable, ParamSpec, TypeVar
 
 import openai
 
+from .prompt import ChatTemplate, Message
 from .utils.signature import FunctionSignature
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def ai_fn(
     fn: Callable[P, T],
 ) -> Callable[P, T]:
     sig = FunctionSignature(fn)
 
     @wraps(fn)
     def inner(*args: Any, **kwargs: Any) -> T:
-        messages = [
-            {
-                "role": "system",
-                "content": sig.instruction(),
-            },
-            {"role": "user", "content": sig.call_line(*args, **kwargs)},
-        ]
+        template = ChatTemplate(
+            messages=[
+                Message(role="system", content=sig.instruction()),
+                Message(role="user", content=sig.call_line(*args, **kwargs)),
+            ]
+        )
 
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
-            messages=messages,
+            messages=template.render(),
             temperature=0.0,
         )
 
         resp = response.choices[0].message["content"]
         return sig.parse(resp)
 
     return inner
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/conftest.py` & `gpt_fn-0.0.2/src/fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/src/fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.2/src/fn/tests/cassettes/test_ai_fabnocci.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -5,69 +5,72 @@
       int):\n```\nOnly respond with your `return` value.\nThe output should be formatted
       as a JSON instance that conforms to the JSON schema below.\n\nAs an example,
       for the schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\":
       \"a list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
       \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
       instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
       is not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\":
-      {\"ret\": {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```\n"},
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
       {"role": "user", "content": "fabnocci(10)"}], "temperature": 0.0}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '886'
+      - '884'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
         "3.11.3", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: '{"id":"chatcmpl-7OmPcggWnB2DrvAwDdSSkXHUb4CwR","object":"chat.completion","created":1686140324,"model":"gpt-3.5-turbo-0301","usage":{"prompt_tokens":200,"completion_tokens":6,"total_tokens":206},"choices":[{"message":{"role":"assistant","content":"{\"ret\":
-        55}"},"finish_reason":"stop","index":0}]}
-
-        '
+      string: "{\n  \"id\": \"chatcmpl-7POvK29Ub10UemzsvNYhSCImY1xJh\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686288362,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+        \ \"usage\": {\n    \"prompt_tokens\": 199,\n    \"completion_tokens\": 6,\n
+        \   \"total_tokens\": 205\n  },\n  \"choices\": [\n    {\n      \"message\":
+        {\n        \"role\": \"assistant\",\n        \"content\": \"{\\\"ret\\\":
+        55}\"\n      },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n
+        \   }\n  ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d38d6e18fad4a51-TPE
+      - 7d46f515de330728-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 07 Jun 2023 12:18:45 GMT
+      - Fri, 09 Jun 2023 05:26:02 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '833'
+      - '817'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
@@ -77,12 +80,12 @@
       x-ratelimit-remaining-tokens:
       - '89809'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
       - 126ms
       x-request-id:
-      - eb2d55a66a60041db2d644ff01a69853
+      - d1dc3dde477e92ba22a78a13f041b366
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/tests/cassettes/test_ai_fake_hero.yaml` & `gpt_fn-0.0.2/src/fn/tests/cassettes/test_ai_fake_hero.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -9,88 +9,94 @@
       \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
       instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
       is not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\":
       {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
       \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
       \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
       \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
-      \"required\": [\"name\", \"age\"]}}}\n```\n"}, {"role": "user", "content": "fake_hero(5)"}],
+      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
       "temperature": 0.0}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '1199'
+      - '1197'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
         "3.11.3", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
         "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
         PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: '{"id":"chatcmpl-7OmPoZOMSgndBaoo5czGM9vJofGy8","object":"chat.completion","created":1686140336,"model":"gpt-3.5-turbo-0301","usage":{"prompt_tokens":279,"completion_tokens":107,"total_tokens":386},"choices":[{"message":{"role":"assistant","content":"```json\n{\n    \"ret\":
-        [\n        {\n            \"name\": \"Superman\",\n            \"age\": 35\n        },\n        {\n            \"name\":
-        \"Batman\",\n            \"age\": 40\n        },\n        {\n            \"name\":
-        \"Spiderman\",\n            \"age\": 25\n        },\n        {\n            \"name\":
-        \"Wonder Woman\",\n            \"age\": 30\n        },\n        {\n            \"name\":
-        \"Iron Man\",\n            \"age\": 45\n        }\n    ]\n}\n```"},"finish_reason":"stop","index":0}]}
-
-        '
+      string: "{\n  \"id\": \"chatcmpl-7POvLzz9bmjkVW62iee8coYLZUEsD\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686288363,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+        \ \"usage\": {\n    \"prompt_tokens\": 278,\n    \"completion_tokens\": 107,\n
+        \   \"total_tokens\": 385\n  },\n  \"choices\": [\n    {\n      \"message\":
+        {\n        \"role\": \"assistant\",\n        \"content\": \"```json\\n{\\n
+        \   \\\"ret\\\": [\\n        {\\n            \\\"name\\\": \\\"Superman\\\",\\n
+        \           \\\"age\\\": 35\\n        },\\n        {\\n            \\\"name\\\":
+        \\\"Batman\\\",\\n            \\\"age\\\": 40\\n        },\\n        {\\n
+        \           \\\"name\\\": \\\"Spiderman\\\",\\n            \\\"age\\\": 25\\n
+        \       },\\n        {\\n            \\\"name\\\": \\\"Wonder Woman\\\",\\n
+        \           \\\"age\\\": 30\\n        },\\n        {\\n            \\\"name\\\":
+        \\\"Iron Man\\\",\\n            \\\"age\\\": 45\\n        }\\n    ]\\n}\\n```\"\n
+        \     },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n    }\n
+        \ ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d38d72adfeb4a6a-TPE
+      - 7d46f51cfa96a343-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 07 Jun 2023 12:19:04 GMT
+      - Fri, 09 Jun 2023 05:26:08 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '8368'
+      - '5540'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
       - '90000'
       x-ratelimit-remaining-requests:
       - '3499'
       x-ratelimit-remaining-tokens:
-      - '89744'
+      - '89743'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
       - 170ms
       x-request-id:
-      - d2d4d5d57580ee44084c40aab7007629
+      - 87cb42ea1e3cc020be707c2c3121c079
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/tests/test_ai_function.py` & `gpt_fn-0.0.2/src/fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/src/fn/utils/pydantic_parser.py` & `gpt_fn-0.0.2/src/fn/utils/pydantic_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pydantic import BaseModel, ValidationError
 from pydantic.generics import GenericModel
 
 T = TypeVar("T", bound=BaseModel)
 
 
-class ParserException(Exception):
+class ParserError(Exception):
     pass
 
 
 PYDANTIC_FORMAT_INSTRUCTIONS = """The output should be formatted as a JSON instance that conforms to the JSON schema below.
 
 As an example, for the schema {{"properties": {{"foo": {{"title": "Foo", "description": "a list of strings", "type": "array", "items": {{"type": "string"}}}}}}, "required": ["foo"]}}}}
 the object {{"foo": ["bar", "baz"]}} is a well-formatted instance of the schema. The object {{"properties": {{"foo": ["bar", "baz"]}}}} is not well-formatted.
@@ -34,15 +34,15 @@
             if match:
                 json_str = match.group()
             json_object = json.loads(json_str)
             return self.pydantic_model.parse_obj(json_object)
         except (json.JSONDecodeError, ValidationError) as e:
             name = self.pydantic_model.__name__
             msg = f"Failed to parse {name} from completion {text}. Got: {e}"
-            raise ParserException(msg)
+            raise ParserError(msg)
 
     def get_format_instructions(self) -> str:
         schema = self.pydantic_model.schema()
 
         # Remove extraneous fields.
         reduced_schema = schema
         if "title" in reduced_schema:
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/utils/signature.py` & `gpt_fn-0.0.2/src/fn/utils/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def function_line(self) -> str:
         # NOTE: return type is instrcutive by parser
         f = str(self.sig.replace(return_annotation=inspect.Signature.empty))
 
         return f"def {self.fn.__name__}{f}:"
 
     def description(self) -> str:
-        desc = inspect.cleandoc(self.fn.__doc__ or "")
+        desc = clean_docstring(self.fn.__doc__ or "")
 
         return desc
 
     def call_line(self, *args: Any, **kwargs: Any) -> str:
         return format_call_line(self.fn, *args, **kwargs)
 
     def parse(self, text: str) -> Any:
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.0.2/src/fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/src/fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.0.2/src/fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/src/fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.0.2/src/fn/utils/tests/test_pydantic_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import pytest
 from pydantic import BaseModel, Field
 from syrupy.assertion import SnapshotAssertion
 
-from ..pydantic_parser import PydanticParser
+from ..pydantic_parser import ParserError, PydanticParser
 
 
 class Receipt(BaseModel):
     """The Receipt for user"""
 
     amount: float
     currency: str = Field(description="ISO 4217 currency code")
@@ -16,7 +17,12 @@
     snapshot: SnapshotAssertion,
 ) -> None:
     assert snapshot == PydanticParser[Receipt](pydantic_model=Receipt).get_format_instructions()
 
 
 def test_parse_output(snapshot: SnapshotAssertion) -> None:
     assert snapshot == PydanticParser[Receipt](pydantic_model=Receipt).parse('{"amount": 1.0, "currency": "USD", "customer": "John Doe"}')
+
+
+def test_pydantic_parser_fail() -> None:
+    with pytest.raises(ParserError):
+        PydanticParser[Receipt](pydantic_model=Receipt).parse('{"amount": 1.0, "currency": "USD"}')
```

### Comparing `gpt_fn-0.0.1.post2/src/fn/utils/tests/test_signature.py` & `gpt_fn-0.0.2/src/fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.1.post2/PKG-INFO` & `gpt_fn-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.0.1.post2
+Version: 0.0.2
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.7,<0.28.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: jinja2 (>=3.0,<4.0)
+Requires-Dist: openai (>=0.27,<0.28)
+Requires-Dist: pydantic (>=1.0,<2.0)
 Description-Content-Type: text/markdown
 
 # GPT-Fn
 
 GPT-Fn is a lightweight utility library designed to seamlessly integrate AI capabilities into your software applications. Our focus is on providing essential utilities that make it easy to incorporate artificial intelligence into your codebase without unnecessary complexities.
 
 ## Features
```

