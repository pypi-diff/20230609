# Comparing `tmp/meilisearch_python_async-1.3.0.tar.gz` & `tmp/meilisearch_python_async-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.3.0.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.4.0.tar", max compression
```

## Comparing `meilisearch_python_async-1.3.0.tar` & `meilisearch_python_async-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/LICENSE
--rw-r--r--   0        0        0     5759 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/README.md
--rw-r--r--   0        0        0      151 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0       18 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22205 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     1886 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89041 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11471 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2286 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 meilisearch_python_async-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5759 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/README.md
+-rw-r--r--   0        0        0      151 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0       18 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22205 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89041 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11932 2023-06-09 01:38:23.377640 meilisearch_python_async-1.4.0/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2286 2023-06-09 01:38:23.377640 meilisearch_python_async-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.0/PKG-INFO
```

### Comparing `meilisearch_python_async-1.3.0/LICENSE` & `meilisearch_python_async-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/README.md` & `meilisearch_python_async-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/client.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 class MeilisearchCommunicationError(MeilisearchError):
     """Error when connecting to Meilisearch."""
 
     def __str__(self) -> str:
         return f"MeilisearchCommunicationError, {self.message}"
 
 
+class MeilisearchTaskFailedError(MeilisearchError):
+    """Error when a task is in the failed status."""
+
+    def __str__(self) -> str:
+        return f"MeilisearchTaskFailedError, {self.message}"
+
+
 class MeilisearchTimeoutError(MeilisearchError):
     """Error when Meilisearch operation takes longer than expected."""
 
     def __str__(self) -> str:
         return f"MeilisearchTimeoutError, {self.message}"
```

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/index.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.3.0/meilisearch_python_async/task.py` & `meilisearch_python_async-1.4.0/meilisearch_python_async/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from typing import TYPE_CHECKING
 from urllib.parse import urlencode
 
 from httpx import AsyncClient
 
 from meilisearch_python_async._http_requests import HttpRequests
-from meilisearch_python_async.errors import MeilisearchTimeoutError
+from meilisearch_python_async.errors import MeilisearchTaskFailedError, MeilisearchTimeoutError
 from meilisearch_python_async.models.task import TaskInfo, TaskStatus
 
 if TYPE_CHECKING:
     from meilisearch_python_async.client import Client  # pragma: no cover
 
 
 async def cancel_tasks(
@@ -228,35 +228,39 @@
 
 async def wait_for_task(
     client: AsyncClient | Client,
     task_id: int,
     *,
     timeout_in_ms: int | None = 5000,
     interval_in_ms: int = 50,
+    raise_for_status: bool = False,
 ) -> TaskStatus:
     """Wait until Meilisearch processes a task, and get its status.
 
     Args:
 
         client: An httpx AsyncClient or meilisearch_python_async Client instance.
         task_id: Identifier of the task to retrieve.
         timeout_in_ms: Amount of time in milliseconds to wait before raising a
             MeilisearchTimeoutError. `None` can also be passed to wait indefinitely. Be aware that
             if the `None` option is used the wait time could be very long. Defaults to 5000.
         interval_in_ms: Time interval in miliseconds to sleep between requests. Defaults to 50.
+        raise_for_status: When set to `True` a MeilisearchTaskFailedError will be raised if a task
+            has a failed status. Defaults to False.
 
     Returns:
 
         Details of the processed update status.
 
     Raises:
 
         MeilisearchCommunicationError: If there was an error communicating with the server.
         MeilisearchApiError: If the Meilisearch API returned an error.
         MeilisearchTimeoutError: If the connection times out.
+        MeilisearchTaskFailedError: If `raise_for_status` is `True` and a task has a failed status.
 
     Examples:
 
         >>> from meilisearch_python_async import Client
         >>> from meilisearch_python_async.task import wait_for_task
         >>> >>> documents = [
         >>>     {"id": 1, "title": "Movie 1", "genre": "comedy"},
@@ -274,14 +278,16 @@
     elapsed_time = 0.0
 
     if timeout_in_ms:
         while elapsed_time < timeout_in_ms:
             response = await http_requests.get(url)
             status = TaskStatus(**response.json())
             if status.status in ("succeeded", "failed"):
+                if raise_for_status and status.status == "failed":
+                    raise MeilisearchTaskFailedError(f"Task {task_id} failed")
                 return status
             await sleep(interval_in_ms / 1000)
             time_delta = datetime.now() - start_time
             elapsed_time = time_delta.seconds * 1000 + time_delta.microseconds / 1000
         raise MeilisearchTimeoutError(
             f"timeout of {timeout_in_ms}ms has exceeded on process {task_id} when waiting for pending update to resolve."
         )
```

### Comparing `meilisearch_python_async-1.3.0/pyproject.toml` & `meilisearch_python_async-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.3.0"
+version = "1.4.0"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.3.0/PKG-INFO` & `meilisearch_python_async-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
```

