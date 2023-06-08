# Comparing `tmp/auth2guard-0.3.1.tar.gz` & `tmp/auth2guard-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth2guard-0.3.1.tar", max compression
+gzip compressed data, was "auth2guard-0.4.0.tar", max compression
```

## Comparing `auth2guard-0.3.1.tar` & `auth2guard-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-03-10 20:48:38.786247 auth2guard-0.3.1/LICENSE
--rw-r--r--   0        0        0     5192 2023-04-02 11:11:04.452348 auth2guard-0.3.1/README.md
--rw-r--r--   0        0        0     2473 2023-04-02 11:11:04.452348 auth2guard-0.3.1/auth2guard/__init__.py
--rw-r--r--   0        0        0     7462 2023-04-26 22:32:30.982947 auth2guard-0.3.1/auth2guard/sentinel.py
--rw-r--r--   0        0        0      637 2023-04-26 22:31:11.824672 auth2guard-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 auth2guard-0.3.1/setup.py
--rw-r--r--   0        0        0     5698 1970-01-01 00:00:00.000000 auth2guard-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-10 20:48:38.786247 auth2guard-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5306 2023-06-08 22:35:02.808450 auth2guard-0.4.0/README.md
+-rw-r--r--   0        0        0     2926 2023-06-08 22:35:02.808450 auth2guard-0.4.0/auth2guard/__init__.py
+-rw-r--r--   0        0        0     8579 2023-06-08 22:35:02.808450 auth2guard-0.4.0/auth2guard/sentinel.py
+-rw-r--r--   0        0        0      637 2023-06-08 22:35:36.456293 auth2guard-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6080 1970-01-01 00:00:00.000000 auth2guard-0.4.0/setup.py
+-rw-r--r--   0        0        0     5812 1970-01-01 00:00:00.000000 auth2guard-0.4.0/PKG-INFO
```

### Comparing `auth2guard-0.3.1/LICENSE` & `auth2guard-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auth2guard-0.3.1/README.md` & `auth2guard-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -300,26 +300,33 @@
 000012b0: 6572 733a 2064 6963 7429 3a0a 2020 2020  ers: dict):.    
 000012c0: 2020 2020 7365 6c66 2e5f 6865 6164 6572      self._header
 000012d0: 7320 3d20 6865 6164 6572 730a 0a20 2020  s = headers..   
 000012e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
 000012f0: 6566 2068 6561 6465 7273 2873 656c 6629  ef headers(self)
 00001300: 202d 3e20 6469 6374 3a0a 2020 2020 2020   -> dict:.      
 00001310: 2020 7265 7475 726e 2073 656c 662e 5f68    return self._h
-00001320: 6561 6465 7273 0a0a 6175 7468 3267 7561  eaders..auth2gua
-00001330: 7264 2e73 6574 5f63 6f6e 6669 6728 6a77  rd.set_config(jw
-00001340: 6b3d 277b 2270 223a 222d 3770 4376 4c6c  k='{"p":"-7pCvLl
-00001350: 7a73 4e49 5244 3775 7462 4c5a 7142 2e2e  zsNIRD7utbLZqB..
-00001360: 2e27 290a 0a40 6175 7468 3267 7561 7264  .')..@auth2guard
-00001370: 2e76 616c 6964 6174 6528 5b22 7465 7374  .validate(["test
-00001380: 3122 5d2c 2061 6e64 5f76 616c 6964 6174  1"], and_validat
-00001390: 696f 6e3d 5472 7565 2c20 746f 6b65 6e5f  ion=True, token_
-000013a0: 636f 6e74 656e 743d 5472 7565 290a 6465  content=True).de
-000013b0: 6620 726f 7574 655f 6361 6c6c 6261 636b  f route_callback
-000013c0: 2872 6571 7565 7374 2c20 746f 6b65 6e5f  (request, token_
-000013d0: 636f 6e74 656e 743a 2064 6963 7429 3a0a  content: dict):.
-000013e0: 2020 2020 7061 7373 0a0a 7265 7175 6573      pass..reques
-000013f0: 7420 3d20 5265 7175 6573 7428 6865 6164  t = Request(head
-00001400: 6572 733d 7b22 4175 7468 6f72 697a 6174  ers={"Authorizat
-00001410: 696f 6e22 3a20 6622 4261 7369 6320 5858  ion": f"Basic XX
-00001420: 5822 7d29 0a72 6f75 7465 5f63 616c 6c62  X"}).route_callb
-00001430: 6163 6b28 7265 7175 6573 743d 7265 7175  ack(request=requ
-00001440: 6573 7429 0a60 6060                      est).```
+00001320: 6561 6465 7273 0a0a 0a61 7574 6832 6775  eaders...auth2gu
+00001330: 6172 642e 7365 745f 636f 6e66 6967 286a  ard.set_config(j
+00001340: 776b 3d27 7b22 7022 3a22 2d37 7043 764c  wk='{"p":"-7pCvL
+00001350: 6c7a 734e 4952 4437 7574 624c 5a71 422e  lzsNIRD7utbLZqB.
+00001360: 2e2e 2729 0a0a 0a40 6175 7468 3267 7561  ..')...@auth2gua
+00001370: 7264 2e76 616c 6964 6174 6528 0a20 2020  rd.validate(.   
+00001380: 2061 6c6c 6f77 6564 5f73 636f 7065 733d   allowed_scopes=
+00001390: 5b22 7465 7374 3122 5d2c 200a 2020 2020  ["test1"], .    
+000013a0: 7363 6f70 655f 616e 645f 7661 6c69 6461  scope_and_valida
+000013b0: 7469 6f6e 3d54 7275 652c 200a 2020 2020  tion=True, .    
+000013c0: 696e 6a65 6374 5f74 6f6b 656e 5f63 6f6e  inject_token_con
+000013d0: 7465 6e74 3d54 7275 652c 0a20 2020 2061  tent=True,.    a
+000013e0: 6c6c 6f77 6564 5f61 7564 6965 6e63 6573  llowed_audiences
+000013f0: 3d5b 2274 6573 7431 225d 2c0a 2020 2020  =["test1"],.    
+00001400: 6175 6469 656e 6365 5f61 6e64 5f76 616c  audience_and_val
+00001410: 6964 6174 696f 6e3d 5472 7565 0a29 0a64  idation=True.).d
+00001420: 6566 2072 6f75 7465 5f63 616c 6c62 6163  ef route_callbac
+00001430: 6b28 7265 7175 6573 742c 2074 6f6b 656e  k(request, token
+00001440: 5f63 6f6e 7465 6e74 3a20 6469 6374 293a  _content: dict):
+00001450: 0a20 2020 2070 6173 730a 0a0a 7265 7175  .    pass...requ
+00001460: 6573 7420 3d20 5265 7175 6573 7428 6865  est = Request(he
+00001470: 6164 6572 733d 7b22 4175 7468 6f72 697a  aders={"Authoriz
+00001480: 6174 696f 6e22 3a20 6622 4261 7369 6320  ation": f"Basic 
+00001490: 5858 5822 7d29 0a72 6f75 7465 5f63 616c  XXX"}).route_cal
+000014a0: 6c62 6163 6b28 7265 7175 6573 743d 7265  lback(request=re
+000014b0: 7175 6573 7429 0a60 6060                 quest).```
```

### Comparing `auth2guard-0.3.1/auth2guard/__init__.py` & `auth2guard-0.4.0/auth2guard/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,36 @@
 from typing import List, Union, Type
 
 from auth2guard.sentinel import Sentinel
 
 
 def validate(
     allowed_scopes: List[str],
-    and_validation: bool = True,
+    scope_and_validation: bool = True,
     inject_token_content: bool = False,
+    allowed_audiences: List[str] = None,
+    audience_and_validation: bool = True,
 ) -> Sentinel:
     """
     This is a decorator for you routes. Will return a Sentinel instance.
     :param allowed_scopes: List of scopes that is required for access this route
-    :param and_validation: Boolean to define if the allowed_scopes is AND operation or a OR operaion
+    :param scope_and_validation: Boolean to define if the allowed_scopes
+    is AND operation or a OR operaion
     :param inject_token_content: Boolean will inject the token_content
+    :param allowed_audiences: List of audiences that is required for access this route
+    :param audience_and_validation: Boolean to define if the allowed_audiences
+    is AND operation or a OR operaion
     :return: Sentinel function wrapper
     """
     return Sentinel(
         allowed_scopes=set(allowed_scopes),
-        and_validation=and_validation,
+        scope_and_validation=scope_and_validation,
         inject_token_content=inject_token_content,
+        allowed_audiences=set(allowed_audiences) if allowed_audiences else None,
+        audience_and_validation=audience_and_validation,
     )
 
 
 def set_config(
     jwk: Union[dict, str, bytes] = None,
     http_header_name_token: str = None,
     request_token_callback=None,
```

### Comparing `auth2guard-0.3.1/auth2guard/sentinel.py` & `auth2guard-0.4.0/auth2guard/sentinel.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,19 +100,28 @@
         if not hasattr(request_token_callback, "__call__"):
             cls.exception_raiser(
                 exception_type=ExceptionType.CONFIG_ERROR,
                 message="request_token_callback.wrong_type",
             )
         cls.__config.update({"request_token_callback": request_token_callback})
 
-    def __init__(
-        self, allowed_scopes: set, and_validation: bool, inject_token_content: bool
+    def __init__(  # pylint: disable=R0913
+        self,
+        allowed_scopes: set,
+        scope_and_validation: bool,
+        inject_token_content: bool,
+        allowed_audiences: set = None,
+        audience_and_validation: bool = False,
     ):
+        if allowed_audiences is None:
+            allowed_audiences = {}
         self.__allowed_scopes = allowed_scopes
-        self.__and_validation = and_validation
+        self.__allowed_audiences = allowed_audiences
+        self.__scope_and_validation = scope_and_validation
+        self.__audience_and_validation = audience_and_validation
         self.__inject_token_content = inject_token_content
 
     def __call__(self, func):
         is_sync_function = asyncio.iscoroutinefunction(func)
         if is_sync_function:
 
             async def async_checker(*args, request: Request, **kwargs):
@@ -181,26 +190,46 @@
                     message="authentication.expired_token",
                 )
             self.exception_raiser(
                 exception_type=ExceptionType.NOT_FROM_ORIGIN,
                 message="authentication.not_from_origin",
             )
 
-    def _supervision(self, request: Request) -> dict:
-        token_type_and_content = self.__get_token(request=request)
-        token_content = self.__decode_token(token_content=token_type_and_content[1])
+    def _validate_scope(self, token_content: dict):
         token_scope = token_content.get("scope", "")
         scopes = set(
             token_scope.split(" ") if isinstance(token_scope, str) else token_scope
         )
         scopes_sub_set = self.__allowed_scopes - scopes
-        and_validation_satisfied = not scopes_sub_set and self.__and_validation
-        or_operation_satisfied = (
-            bool(len(self.__allowed_scopes) - len(scopes_sub_set))
-            and not self.__and_validation
-        )
-        if not (and_validation_satisfied or or_operation_satisfied):
+        if self.__scope_and_validation:
+            return not scopes_sub_set
+
+        or_operation_satisfied = [
+            scope in token_scope for scope in self.__allowed_scopes
+        ]
+        return any(or_operation_satisfied)
+
+    def _validate_audience(self, token_content: dict):
+        if not self.__allowed_audiences:
+            return True
+        token_aud = token_content.get("aud", "")
+        scopes = set(token_aud.split(" ") if isinstance(token_aud, str) else token_aud)
+        audiences_sub_set = self.__allowed_audiences - scopes
+        if self.__audience_and_validation:
+            return not audiences_sub_set
+
+        or_operation_satisfied = [
+            audience in token_aud for audience in self.__allowed_audiences
+        ]
+        return any(or_operation_satisfied)
+
+    def _supervision(self, request: Request) -> dict:
+        token_type_and_content = self.__get_token(request=request)
+        token_content = self.__decode_token(token_content=token_type_and_content[1])
+        scope_validation = self._validate_scope(token_content=token_content)
+        audience_validation = self._validate_audience(token_content=token_content)
+        if not (scope_validation and audience_validation):
             self.exception_raiser(
                 exception_type=ExceptionType.UNAUTHORIZED,
                 message="authentication.unauthorized",
             )
         return token_content
```

### Comparing `auth2guard-0.3.1/pyproject.toml` & `auth2guard-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auth2guard"
-version = "0.3.1"
+version = "0.4.0"
 description = "OAuth 2.0 scope validator"
 authors = ["Marco Sievers de Almeida Ximit Gaia <im.ximit@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "auth2guard"},
     { include = "auth2guard/**/*.py" },
```

### Comparing `auth2guard-0.3.1/setup.py` & `auth2guard-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['jwt>=1.3.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'auth2guard',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'OAuth 2.0 scope validator',
-    'long_description': '```\n░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░\n░░░░░░░  ░░░░░░░░░░░░░░░░░░░   ░░░░░░░░░░░░░░░░░░░░░░░░░░     ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   ░\n▒▒▒▒▒▒  ▒  ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒   ▒▒▒   ▒▒▒▒▒▒▒   ▒  ▒▒▒▒▒  ▒▒▒▒   ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒   ▒\n▒▒▒▒▒  ▒▒   ▒▒▒▒▒   ▒▒   ▒    ▒  ▒   ▒▒▒▒▒▒  ▒▒▒▒▒   ▒  ▒▒▒▒▒▒▒▒▒▒▒   ▒▒   ▒▒▒▒   ▒▒▒▒▒  ▒    ▒▒▒▒▒▒   ▒\n▓▓▓▓   ▓▓▓   ▓▓▓▓   ▓▓   ▓▓▓   ▓▓▓     ▓▓▓▓▓▓▓▓▓   ▓▓▓   ▓▓▓▓▓▓▓▓▓▓   ▓▓   ▓▓   ▓▓   ▓▓▓   ▓▓▓▓▓   ▓   ▓\n▓▓▓       ▓   ▓▓▓   ▓▓   ▓▓▓   ▓▓▓   ▓▓  ▓▓▓▓▓   ▓▓▓▓▓   ▓▓▓      ▓   ▓▓   ▓   ▓▓▓   ▓▓▓   ▓▓▓▓  ▓▓▓   ▓\n▓▓   ▓▓▓▓▓▓▓   ▓▓   ▓▓   ▓▓▓   ▓ ▓  ▓▓▓   ▓▓   ▓▓▓▓▓▓▓▓   ▓▓▓▓  ▓▓▓   ▓▓   ▓   ▓▓▓   ▓▓▓   ▓▓▓▓  ▓▓▓   ▓\n█   █████████   ███      ████   ██  ███   █         ████      ███████      ███   █    █    █████   █   █\n████████████████████████████████████████████████████████████████████████████████████████████████████████\nBy: CenturyBoys\n```\n\nA simple route decorator JWT scope validator.\n\nThis project work with the follow frameworks:\n\n✅ [FastApi](https://fastapi.tiangolo.com/)\n\n✅ [aiohttp](https://docs.aiohttp.org/en/stable/)\n\n## Config\n\nConfiguration are exposed and can be set in any time including out of the use scope.\n\nObs: all configs are saved as singleton.\n\n### jwk\n\nThe jwk key to validate JWT can be bytes, str or dict. This config need to be set!\n\n### http_header_name_token\n\nIf your application use a custom header to send the authentication token you can use this param to indicate his name. By default, the value is \'Authorization\'\n\n### request_token_callback\n\nIf to extract the request token you need to perform some operation you can set a callback for it. Will receive the request as param and must return a str with token type and the token \'Basic XXX\'\n\n```python\nimport auth2guard\n\nclass Request:\n    def __init__(self, headers: dict):\n        self._headers = headers\n\n    @property\n    def headers(self) -> dict:\n        return self._headersclass\n    \nrequest = Request(headers={"x-token": f"Basic Akj817Hakn122i..."})\n\ndef request_token_callback(request: Request):\n        return request.headers.get("x-token")\n    \n    \nauth2guard.set_config(\n    jwk=\'{"p":"-7pCvLlzsNIRD7utbLZqB...\',\n    http_header_name_token="x-token",\n    request_token_callback=request_token_callback\n)\n```\n\n## Exceptions\n\nThe package raise exceptions for some cases se bellow.\n\nObs: By default, all exception are ValueError.\n\n### token_not_found\nError when token was not found. \n\nObs: The config `request_token_callback` can be the problem.\n\n### not_from_origin\nError when token was generated not by the giving JWK. \n\nObs: Validate the config jwk.\n\n### expired\nError when exp JWT param exceeded the time.\n\n### unauthorized\nError when the JWT has not all necessary scope to proceed.\n\n```python\nimport auth2guard\n\nclass MyException(Exception):\n    pass\n\nauth2guard.overwrite_exceptions(unauthorized=MyException)\n```\n\n## Validator\n\nCan be used as decorator and receive a list of scopes. The validator will operate AND validation or a OR validation with the token scope content. For the AND validation all scopes in the `allowed_scopes` param need to be present in the jwt scope and in the OR if any scope is present that\'s enough. You can receive the token content if you want by setting `token_content` to `True` this will inject the param `token_content: dict` into your function as `kwargs`\n\n```python\nimport auth2guard\n\n\nclass Request:\n    def __init__(self, headers: dict):\n        self._headers = headers\n\n    @property\n    def headers(self) -> dict:\n        return self._headers\n\nauth2guard.set_config(jwk=\'{"p":"-7pCvLlzsNIRD7utbLZqB...\')\n\n@auth2guard.validate(["test1"], and_validation=True, token_content=True)\ndef route_callback(request, token_content: dict):\n    pass\n\nrequest = Request(headers={"Authorization": f"Basic XXX"})\nroute_callback(request=request)\n```',
+    'long_description': '```\n░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░\n░░░░░░░  ░░░░░░░░░░░░░░░░░░░   ░░░░░░░░░░░░░░░░░░░░░░░░░░     ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   ░\n▒▒▒▒▒▒  ▒  ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒   ▒▒▒   ▒▒▒▒▒▒▒   ▒  ▒▒▒▒▒  ▒▒▒▒   ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒   ▒\n▒▒▒▒▒  ▒▒   ▒▒▒▒▒   ▒▒   ▒    ▒  ▒   ▒▒▒▒▒▒  ▒▒▒▒▒   ▒  ▒▒▒▒▒▒▒▒▒▒▒   ▒▒   ▒▒▒▒   ▒▒▒▒▒  ▒    ▒▒▒▒▒▒   ▒\n▓▓▓▓   ▓▓▓   ▓▓▓▓   ▓▓   ▓▓▓   ▓▓▓     ▓▓▓▓▓▓▓▓▓   ▓▓▓   ▓▓▓▓▓▓▓▓▓▓   ▓▓   ▓▓   ▓▓   ▓▓▓   ▓▓▓▓▓   ▓   ▓\n▓▓▓       ▓   ▓▓▓   ▓▓   ▓▓▓   ▓▓▓   ▓▓  ▓▓▓▓▓   ▓▓▓▓▓   ▓▓▓      ▓   ▓▓   ▓   ▓▓▓   ▓▓▓   ▓▓▓▓  ▓▓▓   ▓\n▓▓   ▓▓▓▓▓▓▓   ▓▓   ▓▓   ▓▓▓   ▓ ▓  ▓▓▓   ▓▓   ▓▓▓▓▓▓▓▓   ▓▓▓▓  ▓▓▓   ▓▓   ▓   ▓▓▓   ▓▓▓   ▓▓▓▓  ▓▓▓   ▓\n█   █████████   ███      ████   ██  ███   █         ████      ███████      ███   █    █    █████   █   █\n████████████████████████████████████████████████████████████████████████████████████████████████████████\nBy: CenturyBoys\n```\n\nA simple route decorator JWT scope validator.\n\nThis project work with the follow frameworks:\n\n✅ [FastApi](https://fastapi.tiangolo.com/)\n\n✅ [aiohttp](https://docs.aiohttp.org/en/stable/)\n\n## Config\n\nConfiguration are exposed and can be set in any time including out of the use scope.\n\nObs: all configs are saved as singleton.\n\n### jwk\n\nThe jwk key to validate JWT can be bytes, str or dict. This config need to be set!\n\n### http_header_name_token\n\nIf your application use a custom header to send the authentication token you can use this param to indicate his name. By default, the value is \'Authorization\'\n\n### request_token_callback\n\nIf to extract the request token you need to perform some operation you can set a callback for it. Will receive the request as param and must return a str with token type and the token \'Basic XXX\'\n\n```python\nimport auth2guard\n\nclass Request:\n    def __init__(self, headers: dict):\n        self._headers = headers\n\n    @property\n    def headers(self) -> dict:\n        return self._headersclass\n    \nrequest = Request(headers={"x-token": f"Basic Akj817Hakn122i..."})\n\ndef request_token_callback(request: Request):\n        return request.headers.get("x-token")\n    \n    \nauth2guard.set_config(\n    jwk=\'{"p":"-7pCvLlzsNIRD7utbLZqB...\',\n    http_header_name_token="x-token",\n    request_token_callback=request_token_callback\n)\n```\n\n## Exceptions\n\nThe package raise exceptions for some cases se bellow.\n\nObs: By default, all exception are ValueError.\n\n### token_not_found\nError when token was not found. \n\nObs: The config `request_token_callback` can be the problem.\n\n### not_from_origin\nError when token was generated not by the giving JWK. \n\nObs: Validate the config jwk.\n\n### expired\nError when exp JWT param exceeded the time.\n\n### unauthorized\nError when the JWT has not all necessary scope to proceed.\n\n```python\nimport auth2guard\n\nclass MyException(Exception):\n    pass\n\nauth2guard.overwrite_exceptions(unauthorized=MyException)\n```\n\n## Validator\n\nCan be used as decorator and receive a list of scopes. The validator will operate AND validation or a OR validation with the token scope content. For the AND validation all scopes in the `allowed_scopes` param need to be present in the jwt scope and in the OR if any scope is present that\'s enough. You can receive the token content if you want by setting `token_content` to `True` this will inject the param `token_content: dict` into your function as `kwargs`\n\n```python\nimport auth2guard\n\n\nclass Request:\n    def __init__(self, headers: dict):\n        self._headers = headers\n\n    @property\n    def headers(self) -> dict:\n        return self._headers\n\n\nauth2guard.set_config(jwk=\'{"p":"-7pCvLlzsNIRD7utbLZqB...\')\n\n\n@auth2guard.validate(\n    allowed_scopes=["test1"], \n    scope_and_validation=True, \n    inject_token_content=True,\n    allowed_audiences=["test1"],\n    audience_and_validation=True\n)\ndef route_callback(request, token_content: dict):\n    pass\n\n\nrequest = Request(headers={"Authorization": f"Basic XXX"})\nroute_callback(request=request)\n```',
     'author': 'Marco Sievers de Almeida Ximit Gaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `auth2guard-0.3.1/PKG-INFO` & `auth2guard-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth2guard
-Version: 0.3.1
+Version: 0.4.0
 Summary: OAuth 2.0 scope validator
 License: Apache-2.0
 Author: Marco Sievers de Almeida Ximit Gaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -119,16 +119,25 @@
     def __init__(self, headers: dict):
         self._headers = headers
 
     @property
     def headers(self) -> dict:
         return self._headers
 
+
 auth2guard.set_config(jwk='{"p":"-7pCvLlzsNIRD7utbLZqB...')
 
-@auth2guard.validate(["test1"], and_validation=True, token_content=True)
+
+@auth2guard.validate(
+    allowed_scopes=["test1"], 
+    scope_and_validation=True, 
+    inject_token_content=True,
+    allowed_audiences=["test1"],
+    audience_and_validation=True
+)
 def route_callback(request, token_content: dict):
     pass
 
+
 request = Request(headers={"Authorization": f"Basic XXX"})
 route_callback(request=request)
 ```
```

