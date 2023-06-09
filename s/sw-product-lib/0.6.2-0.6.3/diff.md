# Comparing `tmp/sw_product_lib-0.6.2.tar.gz` & `tmp/sw_product_lib-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_product_lib-0.6.2.tar", max compression
+gzip compressed data, was "sw_product_lib-0.6.3.tar", max compression
```

## Comparing `sw_product_lib-0.6.2.tar` & `sw_product_lib-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1097 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/client/__init__.py
--rw-r--r--   0        0        0    10691 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/client/backend.py
--rw-r--r--   0        0        0     3885 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/client/billing.py
--rw-r--r--   0        0        0     7180 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/client/job.py
--rw-r--r--   0        0        0     2186 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/client/resource.py
--rw-r--r--   0        0        0        0 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/platform/__init__.py
--rw-r--r--   0        0        0      331 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/platform/gql.py
--rw-r--r--   0        0        0    24528 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/service.py
--rw-r--r--   0        0        0    22223 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/types/job.py
--rw-r--r--   0        0        0     8702 2023-06-06 11:16:55.721440 sw_product_lib-0.6.2/sw_product_lib/types/resource.py
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 sw_product_lib-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/__init__.py
+-rw-r--r--   0        0        0    10691 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/backend.py
+-rw-r--r--   0        0        0     3885 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/billing.py
+-rw-r--r--   0        0        0     7180 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/job.py
+-rw-r--r--   0        0        0     2186 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/resource.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/platform/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/platform/gql.py
+-rw-r--r--   0        0        0    27535 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/service.py
+-rw-r--r--   0        0        0     2239 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/types/batch_job.py
+-rw-r--r--   0        0        0    23167 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/types/job.py
+-rw-r--r--   0        0        0     8702 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/types/resource.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 sw_product_lib-0.6.3/PKG-INFO
```

### Comparing `sw_product_lib-0.6.2/pyproject.toml` & `sw_product_lib-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 per-file-ignores = [
     "__init__.py:F401",
     "./docs/*:E402"
 ]
 
 [tool.poetry]
 name = "sw-product-lib"
-version = "0.6.2"
+version = "0.6.3"
 description = "Python library for Strangeworks products to interact with the Strangeworks Platform"
 authors = ["Strangeworks Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^12.4.4"
 gql = "^3.4.1"
 sgqlc = "^16.0"
 aiofiles = "^0.8.0"
 fastapi = "^0.85.0"
 python-jose = {extras = ["cryptography"], version = "^3.3.0"}
-strangeworks-core = "^0.2.0"
+strangeworks-core = "^0.2.1"
 deprecated = "^1.2.13"
 
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
```

### Comparing `sw_product_lib-0.6.2/sw_product_lib/client/backend.py` & `sw_product_lib-0.6.3/sw_product_lib/client/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.2/sw_product_lib/client/billing.py` & `sw_product_lib-0.6.3/sw_product_lib/client/billing.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.2/sw_product_lib/client/job.py` & `sw_product_lib-0.6.3/sw_product_lib/client/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.2/sw_product_lib/client/resource.py` & `sw_product_lib-0.6.3/sw_product_lib/client/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.2/sw_product_lib/service.py` & `sw_product_lib-0.6.3/sw_product_lib/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """product.py."""
 import json
 import os
 import tempfile
 from dataclasses import dataclass
 from functools import singledispatch
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import requests
 from deprecated import deprecated
 from fastapi import Request
 from jose import jwt
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.platform import auth
 from strangeworks_core.platform.gql import API, APIInfo
+from strangeworks_core.types.func import Func
 from strangeworks_core.types.job import Status as JobStatus
+from strangeworks_core.types.machine import Accelerator, Machine
 
 from sw_product_lib.client import backend, billing, resource
 from sw_product_lib.client.billing import BillingTransaction
 from sw_product_lib.platform.gql import ProductAPI
-from sw_product_lib.types import job
+from sw_product_lib.types import batch_job, job
 from sw_product_lib.types.job import AppliedJobTag, File, Job
 from sw_product_lib.types.resource import Resource
 
 
 DEFAULT_PLATFORM_BASE_URL = "https://api.strangeworks.com"
 api_key = os.getenv("PRODUCT_LIB_API_KEY")
 base_url = os.getenv("PRODUCT_LIB_BASE_URL", DEFAULT_PLATFORM_BASE_URL)
@@ -745,15 +747,18 @@
 
 
 def execute_subjob(
     ctx: RequestContext,
     subjob_resource: Resource,
     parent_job: Union[str, Job],
     subjob_path: Optional[str] = None,
-    subjob_payload: Optional[Dict[str, Any]] = None,
+    subjob_json: Optional[Dict[str, Any]] = None,
+    subjob_data: Optional[Any] = None,
+    raw_result: Optional[bool] = False,
+    result_parser: Callable[[Dict[str, Any]], Dict[str, Any]] = Job.from_dict,
 ) -> Job:
     """Execute a subjob.
 
     Parameters
     ----------
     ctx: RequestContext
         contains key-values specific to the current request.
@@ -761,16 +766,25 @@
         The resource to execute the subjob on.
     parent_job: Union[str, Job]
         A string or job object with the parent job slug.
     parent_job_slug: Optional[str]
         The slug of the parent job of the sub-job.
     subjob_path: Optional[str]
         The path to the sub-job.
-    subjob_payload: Optional[Dict[str, Any]]
-        The payload of the sub-job.
+    subjob_json: Optional[Dict[str, Any]]
+        A JSON serializable Python object to send in the body of the Request.
+    subjob_data: Optional[Any]
+        The data to send in the body of the request.
+        This can be a FormData object or anything that can be passed into
+        FormData, e.g. a dictionary, bytes, or file-like object
+    raw_result: Optional[bool]
+        If True, return the raw JSON response from the platform.
+        If False, parse the JSON reponse into a Job object.
+    result_parser: Callable[[Dict[str, Any]], Dict[str, Any]]
+        A callable function that takes a JSON response from the platform and parses it.
 
     Returns
     -------
     Job
         A job object denoting the sub-job.
     """
     parent_slug = parent_job.slug if isinstance(parent_job, Job) else parent_job
@@ -778,13 +792,98 @@
         raise ValueError("parent_job (slug or Job object) must be provided.")
     retval = job.execute_subjob(
         parent_job_slug=parent_slug,
         api_key=ctx.product_api_key,
         proxy_auth_token=ctx._auth_token,
         resource=subjob_resource,
         path=subjob_path,
-        data=subjob_payload,
+        json=subjob_json,
+        data=subjob_data,
         base_url=base_url,
     )
     as_json = retval.json()
 
-    return Job.from_dict(as_json)
+    if raw_result is True:
+        return as_json
+
+    return result_parser(as_json)
+
+
+def get_job_file(ctx: RequestContext, file_path: str):
+    """Call platform to return file belonging to job or one of its child jobs.
+
+    Parameters
+    ----------
+    ctx: RequestContext
+        contains key-values specific to the current request.
+    file_path: str
+        path of the file to be downloaded
+
+    Returns
+    -------
+    json
+        json object containing the file contents
+    """
+
+    retval = job.get_job_file(
+        api_key=ctx.product_api_key, file_path=file_path, base_url=base_url
+    )
+
+    return retval.json()
+
+
+def create_batch_job(
+    ctx: RequestContext,
+    function: Callable[..., Any],
+    fargs: tuple = (),
+    fkwargs: dict[str, Any] = {},
+    machine: Machine = Machine(),
+    accelerator: Optional[Accelerator] = None,
+    requirements_path: Optional[str] = None,
+    job_slug: Optional[str] = None,
+    workspace_member_slug: Optional[str] = None,
+) -> str:
+    """
+    Create a batch job.
+
+    Parameters
+    ----------
+    ctx: RequestContext
+        contains key-values specific to the current request.
+    function: Callable[..., Any]
+        The function to execute.
+    fargs: tuple
+        The function arguments.
+    fkwargs: dict[str, Any]
+        The function keyword arguments.
+    machine: Machine
+        The machine to execute the job on.
+    accelerator: Optional[Accelerator]
+        An accelerator to use.
+    requirements_path: Optional[str]
+        The path to the requirements file.
+    job_slug: Optional[str]
+        The slug of the job.
+    workspace_member_slug: Optional[str]
+        The slug of the workspace member.
+
+    Returns
+    -------
+    batch_job_slug: str
+        The slug of the batch job.
+
+    """
+
+    f = Func(
+        func=function, fargs=fargs, fkwargs=fkwargs, requirements_path=requirements_path
+    )
+
+    return batch_job.new(
+        api=ctx.api or _api(),
+        resource_slug=ctx.resource_slug,
+        decorator_name="",
+        func=f,
+        machine=machine,
+        accelerator=accelerator,
+        job_slug=job_slug,
+        workspace_member_slug=workspace_member_slug,
+    )
```

### Comparing `sw_product_lib-0.6.2/sw_product_lib/types/job.py` & `sw_product_lib-0.6.3/sw_product_lib/types/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
+from urllib.parse import urljoin
 
 import requests
 from strangeworks_core.errors.error import StrangeworksError
+from strangeworks_core.platform import auth
 from strangeworks_core.platform.gql import API, Operation
 from strangeworks_core.types.file import File as FileBase
 from strangeworks_core.types.job import Job as JobBase
 from strangeworks_core.types.job import Status as JobStatus
 from strangeworks_core.utils import str_to_datetime
 
 from .resource import Resource
@@ -729,22 +731,51 @@
 
 def execute_subjob(
     parent_job_slug: str,
     api_key: str,
     proxy_auth_token: str,
     resource: Resource,
     path: Optional[str] = None,
+    json: Optional[Any] = None,
     data: Optional[Any] = None,
     base_url: Optional[str] = None,
 ) -> Job:
     """Execute Sub-job."""
-    sub_job = requests.post(
-        url=resource.proxy_url(base_url=base_url, path=path),
-        headers={
-            "Authorization": f"bearer {proxy_auth_token}",
-            "x-resource-api-token": api_key,
-            "x-strangeworks-parent-job-slug": parent_job_slug,
-        },
-        json=data,
-    )
+    if json is None and data is None:
+        sub_job = requests.get(
+            url=resource.proxy_url(base_url=base_url, path=path),
+            headers={
+                "Authorization": f"bearer {proxy_auth_token}",
+                "x-resource-api-token": api_key,
+                "x-strangeworks-parent-job-slug": parent_job_slug,
+            },
+        )
+    else:
+        sub_job = requests.post(
+            url=resource.proxy_url(base_url=base_url, path=path),
+            headers={
+                "Authorization": f"bearer {proxy_auth_token}",
+                "x-resource-api-token": api_key,
+                "x-strangeworks-parent-job-slug": parent_job_slug,
+            },
+            json=json,
+            data=data,
+        )
 
     return sub_job
+
+
+def get_job_file(
+    api_key: str,
+    file_path: str,
+    base_url: Optional[str] = None,
+) -> Job:
+    """Return a Job File."""
+
+    authtoken = auth.get_token(
+        api_key=api_key,
+        base_url=base_url,
+        auth_url="product/token",
+    )
+    file_url = urljoin(base_url, file_path)
+    res = requests.get(url=file_url, headers={"Authorization": f"bearer {authtoken}"})
+    return res
```

### Comparing `sw_product_lib-0.6.2/sw_product_lib/types/resource.py` & `sw_product_lib-0.6.3/sw_product_lib/types/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.2/PKG-INFO` & `sw_product_lib-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-product-lib
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python library for Strangeworks products to interact with the Strangeworks Platform
 License: Apache-2.0
 Author: Strangeworks Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,8 +14,8 @@
 Requires-Dist: aiofiles (>=0.8.0,<0.9.0)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
 Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: sgqlc (>=16.0,<17.0)
-Requires-Dist: strangeworks-core (>=0.2.0,<0.3.0)
+Requires-Dist: strangeworks-core (>=0.2.1,<0.3.0)
```

