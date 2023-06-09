# Comparing `tmp/bmsdna_lakeapi-0.6.7.tar.gz` & `tmp/bmsdna_lakeapi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.6.7.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.7.0.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.6.7.tar` & `bmsdna_lakeapi-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/README.md
--rw-r--r--   0        0        0      337 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6595 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9383 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6030 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11077 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12618 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15559 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6754 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1452 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6470 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4291 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3763 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1998 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-09 19:14:25.049285 bmsdna_lakeapi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-09 19:14:25.049285 bmsdna_lakeapi-0.7.0/README.md
+-rw-r--r--   0        0        0      337 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6595 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9385 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6030 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11077 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12618 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15585 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6887 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6467 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4291 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3763 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1999 2023-06-09 19:14:25.057285 bmsdna_lakeapi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.7.0/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.6.7/LICENSE` & `bmsdna_lakeapi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/README.md` & `bmsdna_lakeapi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 
 ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "0") == "1"
 
+
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
     ) -> None:
         super().__init__()
```

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import duckdb
 import polars as pl
 import pyarrow as pa
 import pypika
 import pypika.queries as fn
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
-from deltalake import DeltaTable, Metadata, PyDeltaTableError
+from deltalake import DeltaTable, Metadata
+from deltalake.exceptions import DeltaError
 from fastapi import (
     APIRouter,
     BackgroundTasks,
     Depends,
     Header,
     HTTPException,
     Query,
```

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportUndefinedVariable=false, reportGeneralTypeIssues=false
+
 import datetime
 from typing import Any, Dict, List, Literal, Union, cast, Optional, Iterable
 from bmsdna.lakeapi.context.df_base import ResultData
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
 from fastapi import Query
 from pydantic import BaseModel, create_model
@@ -13,15 +15,15 @@
 import pyarrow as pa
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 
 def _make_model(v, name):
     if type(v) is dict:
-        return create_model(name, **{k: _make_model(v, k) for k, v in v.items()}), ...
+        return create_model(name, **{k: _make_model(v, k) for k, v in v.items()}), ... # type: ignore
     return type(v), None
 
 
 def make_model(v: Dict, name: str):
     return _make_model(v, name)[0]
 
 
@@ -74,15 +76,15 @@
         assert isinstance(st, pa.StructType)
         res = {
             st.field(ind).name: get_schema_for(model_ns, st.field(ind).name, st.field(ind).type)
             for ind in range(0, st.num_fields)
         }
         return (
             Union[
-                create_model(model_ns + ("_" + field_name if field_name else ""), **res, __base__=TypeBaseModel),
+                create_model(model_ns + ("_" + field_name if field_name else ""), **res, __base__=TypeBaseModel), # type: ignore
                 None,
             ],
             None,
         )
     if pa.types.is_list(field_type) or pa.types.is_large_list(field_type):
         if field_type.value_type is None:
             return (Union[List[Any], None], [])
@@ -156,15 +158,15 @@
                             param.real_default if not param.required else ...,
                         )
         for sc in search or []:
             query_params[sc.name] = (
                 Optional[str],
                 None,
             )
-        query_model = create_model(name + "Parameter", **query_params)
+        query_model = create_model(name + "Parameter", **query_params) # type: ignore
         return query_model
     return empty_model
 
 
 class TypeBaseModel(BaseModel):
     class Config:
         orm_mode = True
@@ -174,8 +176,8 @@
     schema = frame.arrow_schema()
     props = {
         k: get_schema_for(name, schema.field(k).name, schema.field(k).type)
         for k in schema.names
         if not should_hide_colname(k)
     }
 
-    return create_model(name, **props, __base__=TypeBaseModel)
+    return create_model(name, **props, __base__=TypeBaseModel) # type: ignore
```

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/partition_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,25 @@
     if file_type == "delta":
         delta_uri = os.path.join(
             basic_config.data_path,
             uri,
         )
         if not os.path.exists(os.path.join(delta_uri, "_delta_log")):
             return paramslist
-        from deltalake import DeltaTable, PyDeltaTableError
+        from deltalake import DeltaTable
+        from deltalake.exceptions import DeltaError
 
         try:
             part_cols = DeltaTable(delta_uri).metadata().partition_columns
             if part_cols and len(part_cols) > 0:
                 all_names = [(p.colname or p.name).lower() for p in paramslist]
                 new_params = list(paramslist)
                 for pc in part_cols:
                     if pc.lower() not in all_names and not should_hide_colname(pc):
                         from bmsdna.lakeapi.core.types import Param
 
                         new_params.append(Param(pc, operators=["="], colname=pc))
                 return new_params
-        except PyDeltaTableError as err:
+        except DeltaError as err:
             return paramslist  # this is not critical here
 
     return paramslist
```

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         url=url, content=content, format=format, out=temp_file.name, basic_config=basic_config
     )
 
     def clean_up():
         if close_context:
             context.close()
             logger.debug("closed context")
-        temp_file.close()   
+        temp_file.close()
 
         for f in additional_files:
             os.remove(f)
 
     fr = FileResponseWCharset(
         path=temp_file.name,
         headers=headers,
```

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.7/pyproject.toml` & `bmsdna_lakeapi-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.6.7"
+version = "0.7.0"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = "^0.95.1"
-deltalake = "^0.9.0"
 pyyaml = "^6.0"
 aiocache = "^0.12.1"
 pypika = "^0.48.9"
 duckdb = "^0.8.0"
 polars = "^0.18.0"
 
 # schema stuff
@@ -26,14 +24,16 @@
 
 # auth
 argon2-cffi = {version = "^21.3.0", optional=true}
 
 xlsxwriter = "^3.1.0"
 pyjwt = {version = "^2.6.0", optional = true}
 "ruamel.yaml" = {version = "^0.17.26", optional = true}
+fastapi = "^0.96.0"
+deltalake = "^0.10.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.308"
 black = "^23.3.0"
 uvicorn = "^0.22.0"
 psutil = "^5.9.5"
```

### Comparing `bmsdna_lakeapi-0.6.7/PKG-INFO` & `bmsdna_lakeapi-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.6.7
+Version: 0.7.0
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: auth
 Provides-Extra: polars
 Provides-Extra: schema
 Provides-Extra: useradd
 Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) ; extra == "auth"
-Requires-Dist: deltalake (>=0.9.0,<0.10.0)
+Requires-Dist: deltalake (>=0.10.0,<0.11.0)
 Requires-Dist: duckdb (>=0.8.0,<0.9.0)
-Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "schema"
 Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "auth"
 Requires-Dist: pypika (>=0.48.9,<0.49.0)
 Requires-Dist: python2jsonschema (>=0.8,<0.9) ; extra == "schema"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: ruamel.yaml (>=0.17.26,<0.18.0) ; extra == "useradd"
```

