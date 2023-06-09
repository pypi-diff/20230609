# Comparing `tmp/fastapi-elasticsearch-0.5.3.tar.gz` & `tmp/fastapi-elasticsearch-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastapi-elasticsearch-0.5.3.tar", last modified: Tue Jul  6 01:45:06 2021, max compression
+gzip compressed data, was "fastapi-elasticsearch-0.6.0.tar", last modified: Fri Jun  9 21:06:50 2023, max compression
```

## Comparing `fastapi-elasticsearch-0.5.3.tar` & `fastapi-elasticsearch-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dell      (1000) dell      (1000)        0 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/
-drwxr-xr-x   0 dell      (1000) dell      (1000)        0 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch.egg-info/
--rw-r--r--   0 dell      (1000) dell      (1000)       22 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 dell      (1000) dell      (1000)        1 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 dell      (1000) dell      (1000)       65 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 dell      (1000) dell      (1000)     3461 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 dell      (1000) dell      (1000)      326 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 dell      (1000) dell      (1000)       38 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/setup.cfg
--rw-r--r--   0 dell      (1000) dell      (1000)      643 2021-04-04 15:05:26.000000 fastapi-elasticsearch-0.5.3/setup.py
--rw-r--r--   0 dell      (1000) dell      (1000)     3461 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/PKG-INFO
-drwxr-xr-x   0 dell      (1000) dell      (1000)        0 2021-07-06 01:45:06.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch/
--rw-r--r--   0 dell      (1000) dell      (1000)     9078 2021-07-06 01:41:08.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch/api.py
--rw-r--r--   0 dell      (1000) dell      (1000)       91 2021-07-06 01:44:14.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch/__init__.py
--rw-r--r--   0 dell      (1000) dell      (1000)      721 2021-04-03 18:13:19.000000 fastapi-elasticsearch-0.5.3/fastapi_elasticsearch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     9000 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-09 19:32:59.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8567 2023-06-08 14:19:14.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/api.py
+-rw-r--r--   0 root         (0) root         (0)      721 2021-04-03 18:13:19.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9000 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-09 21:06:32.000000 fastapi-elasticsearch-0.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fastapi-elasticsearch-0.5.3/setup.py` & `fastapi-elasticsearch-0.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import os
 import pathlib
 
 from setuptools import find_packages, setup
 
-from fastapi_elasticsearch import __version__
-
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "../README.md").read_text()
 
 required = (HERE / "requirements.txt").read_text().splitlines()
 
 setup(
     name="fastapi-elasticsearch",
-    version=__version__,
+    version="0.6.0",
     description="Query Utility for Elasticsearch",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/euler-io/fastapi-elasticsearch",
     license="LGPL-2.1 License",
     packages=find_packages(exclude=("development",)),
     install_requires=required,
```

### Comparing `fastapi-elasticsearch-0.5.3/fastapi_elasticsearch/api.py` & `fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-import inspect
-from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import forge
-from elasticsearch import Elasticsearch
-from fastapi import Depends, FastAPI, Query, Request, params
-from fastapi.datastructures import Default, DefaultPlaceholder
-from fastapi.dependencies.utils import (get_dependant, get_param_field,
-                                        get_typed_signature,
-                                        request_params_to_args)
-from fastapi.encoders import DictIntStrAny, SetIntStr
-from fastapi.routing import APIRoute, APIRouter
+from fastapi import Depends, Query
+from fastapi.dependencies.utils import analyze_param, get_typed_signature
 from fastapi.types import DecoratedCallable
-from starlette import routing
-from starlette.responses import JSONResponse, Response
-from starlette.routing import BaseRoute
-from starlette.types import ASGIApp
 
 
 def combine(functions: List[Callable]):
     args_list = []
     funcs = []
     combined_args = {}
     for func in functions:
         if not callable(func):
             raise TypeError("Arguments must be callable")
         signature = get_typed_signature(func)
         signature_params = signature.parameters
         func_arg_names = set({})
         for param_name, param in signature_params.items():
-            param_field = get_param_field(
-                param=param,
+            type_annotation, depends, param_field = analyze_param(
                 param_name=param_name,
-                default_field_info=param.default
+                annotation=param.annotation,
+                value=param.default,
+                is_path_param=False,
             )
             arg = forge.arg(
                 name=param_field.name,
                 type=param_field.outer_type_,
                 default=param.default
             )
             if param_name in combined_args:
@@ -51,16 +40,16 @@
         funcs.append((func, func_arg_names))
 
     def combined_functions(*args, **kwargs):
         result = []
         for (func, arg_names) in funcs:
             func_kwargs = dict((k, kwargs[k]) for k in arg_names)
             result.append(func(*args, **func_kwargs))
-        return result 
- 
+        return result
+
     new_args = tuple(combined_args.values())
     return forge.sign(*new_args)(combined_functions)
 
 
 class ElasticsearchAPIQueryBuilder():
     def __init__(self,
                  *,
```

### Comparing `fastapi-elasticsearch-0.5.3/fastapi_elasticsearch/utils.py` & `fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/utils.py`

 * *Files identical despite different names*

