# Comparing `tmp/robocorp_workitems-0.3.0.tar.gz` & `tmp/robocorp_workitems-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_workitems-0.3.0.tar", max compression
+gzip compressed data, was "robocorp_workitems-1.0.0.tar", max compression
```

## Comparing `robocorp_workitems-0.3.0.tar` & `robocorp_workitems-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       47 2023-05-08 07:36:35.571384 robocorp_workitems-0.3.0/README.md
--rw-r--r--   0        0        0      934 2023-05-08 14:34:06.276332 robocorp_workitems-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-08 15:19:03.834122 robocorp_workitems-0.3.0/src/robocorp/workitems/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 07:36:35.572676 robocorp_workitems-0.3.0/src/robocorp/workitems/_workitems/__init__.py
--rw-r--r--   0        0        0    19282 2023-05-08 15:19:03.844911 robocorp_workitems-0.3.0/src/robocorp/workitems/_workitems/_adapter.py
--rw-r--r--   0        0        0      338 2023-05-08 15:19:02.962128 robocorp_workitems-0.3.0/src/robocorp/workitems/_workitems/_types.py
--rw-r--r--   0        0        0    12494 2023-05-08 15:19:03.101716 robocorp_workitems-0.3.0/src/robocorp/workitems/_workitems/_utils.py
--rw-r--r--   0        0        0    44438 2023-05-08 15:19:33.952487 robocorp_workitems-0.3.0/src/robocorp/workitems/_workitems/_workitems.py
--rw-r--r--   0        0        0     8004 2023-05-08 15:19:03.831148 robocorp_workitems-0.3.0/src/robocorp/workitems/workitem.py
--rw-r--r--   0        0        0     1100 2023-05-08 15:14:58.591233 robocorp_workitems-0.3.0/src/robocorp/workitems/workitems.py
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 robocorp_workitems-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5629 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/README.md
+-rw-r--r--   0        0        0      819 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4980 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/__init__.py
+-rw-r--r--   0        0        0    17330 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_adapters.py
+-rw-r--r--   0        0        0     2380 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_context.py
+-rw-r--r--   0        0        0      958 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_exceptions.py
+-rw-r--r--   0        0        0     6520 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_requests.py
+-rw-r--r--   0        0        0     1558 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_types.py
+-rw-r--r--   0        0        0     2331 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_utils.py
+-rw-r--r--   0        0        0     8652 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_workitem.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/py.typed
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 robocorp_workitems-1.0.0/PKG-INFO
```

### Comparing `robocorp_workitems-0.3.0/src/robocorp/workitems/_workitems/_adapter.py` & `robocorp_workitems-1.0.0/src/robocorp/workitems/_adapters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 import json
 import logging
 import os
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
-from robocorp.workitems._workitems._types import State
-from robocorp.workitems._workitems._utils import (
-    JSONType,
-    Requests,
-    deprecation,
-    json_dumps,
-    required_env,
-    resolve_path,
-    url_join,
-)
+from ._exceptions import EmptyQueue
+from ._requests import Requests
+from ._types import State
+from ._utils import JSONType, json_dumps, required_env, resolve_path, url_join
 
 UNDEFINED = object()  # Undefined default value
 ENCODING = "utf-8"
-
-
-class EmptyQueue(IndexError):
-    """Raised when trying to load an input item and none available."""
+LOGGER = logging.getLogger(__name__)
 
 
 class BaseAdapter(ABC):
     """Abstract base class for work item adapters."""
 
     @abstractmethod
     def reserve_input(self) -> str:
@@ -90,47 +81,42 @@
     * RC_PROCESS_ID:            Control room process ID
     * RC_PROCESS_RUN_ID:        Control room process run ID
     * RC_ROBOT_RUN_ID:          Control room robot run ID
 
     * RC_WORKITEM_ID:           Control room work item ID (input)
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
+    def __init__(self) -> None:
         # IDs identifying the current robot run and its input.
-        self._workspace_id = required_env("RC_WORKSPACE_ID")
-        self._process_run_id = required_env("RC_PROCESS_RUN_ID")
-        self._step_run_id = required_env("RC_ACTIVITY_RUN_ID")
+        self._workspace_id: str = required_env("RC_WORKSPACE_ID")
+        self._process_run_id: str = required_env("RC_PROCESS_RUN_ID")
+        self._step_run_id: str = required_env("RC_ACTIVITY_RUN_ID")
         self._initial_item_id: Optional[str] = required_env("RC_WORKITEM_ID")
 
-        self._workitem_requests = self._process_requests = None
-        self._init_workitem_requests()
-        self._init_process_requests()
+        self._workitem_requests = self._init_workitem_requests()
+        self._process_requests = self._init_process_requests()
 
-    def _init_workitem_requests(self):
+    def _init_workitem_requests(self) -> Requests:
         # Endpoint for old work items API.
         workitem_host = required_env("RC_API_WORKITEM_HOST")
         workitem_token = required_env("RC_API_WORKITEM_TOKEN")
         route_prefix = (
             url_join(
                 workitem_host, "json-v1", "workspaces", self._workspace_id, "workitems"
             )
             + "/"
         )
         default_headers = {
             "Authorization": f"Bearer {workitem_token}",
             "Content-Type": "application/json",
         }
-        logging.info("Work item API route prefix: %s", route_prefix)
-        self._workitem_requests = Requests(
-            route_prefix, default_headers=default_headers
-        )
+        LOGGER.info("Work item API route prefix: %s", route_prefix)
+        return Requests(route_prefix, default_headers=default_headers)
 
-    def _init_process_requests(self):
+    def _init_process_requests(self) -> Requests:
         # Endpoint for the new process API.
         process_host = required_env("RC_API_PROCESS_HOST")
         process_token = required_env("RC_API_PROCESS_TOKEN")
         process_id = required_env("RC_PROCESS_ID")
         route_prefix = (
             url_join(
                 process_host,
@@ -142,27 +128,27 @@
             )
             + "/"
         )
         default_headers = {
             "Authorization": f"Bearer {process_token}",
             "Content-Type": "application/json",
         }
-        logging.info("Process API route prefix: %s", route_prefix)
-        self._process_requests = Requests(route_prefix, default_headers=default_headers)
+        LOGGER.info("Process API route prefix: %s", route_prefix)
+        return Requests(route_prefix, default_headers=default_headers)
 
     def _pop_item(self):
         # Get the next input work item from the cloud queue.
         url = url_join(
             "runs",
             self._process_run_id,
             "robotRuns",
             self._step_run_id,
             "reserve-next-work-item",
         )
-        logging.info("Reserving new input work item from: %s", url)
+        LOGGER.info("Reserving new input work item from: %s", url)
         response = self._process_requests.post(url)
         return response.json()["workItemId"]
 
     def reserve_input(self) -> str:
         if self._initial_item_id:
             item_id = self._initial_item_id
             self._initial_item_id = None
@@ -180,78 +166,78 @@
         url = url_join(
             "runs",
             self._process_run_id,
             "robotRuns",
             self._step_run_id,
             "release-work-item",
         )
-        body = {"workItemId": item_id, "state": state.value}
+        body: dict[str, Any] = {"workItemId": item_id, "state": state.value}
         if exception:
             for key, value in list(exception.items()):
                 # All values are (and should be) strings (if not `None`).
                 value = value.strip() if value else value
                 if value:
                     exception[key] = value  # keep the stripped string value
                 else:
                     # Exclude `None` & empty string values.
                     del exception[key]
             body["exception"] = exception
 
-        log_func = logging.error if state == State.FAILED else logging.info
+        log_func = LOGGER.error if state == State.FAILED else LOGGER.info
         log_func(
             "Releasing %s input work item %r into %r with exception: %s",
             state.value,
             item_id,
             url,
             exception,
         )
         self._process_requests.post(url, json=body)
 
     def create_output(self, parent_id: str, payload: Optional[JSONType] = None) -> str:
         # Putting "output" for the current input work item identified by `parent_id`.
         url = url_join("work-items", parent_id, "output")
         body = {"payload": payload}
 
-        logging.info("Creating output item: %s", url)
+        LOGGER.info("Creating output item: %s", url)
         response = self._process_requests.post(url, json=body)
         return response.json()["id"]
 
     def load_payload(self, item_id: str) -> JSONType:
         url = url_join(item_id, "data")
 
         def handle_error(resp):
             # NOTE: The API might return 404 if no payload is attached to the work
             # item.
             if not (resp.ok or resp.status_code == 404):
                 self._workitem_requests.handle_error(resp)
 
-        logging.info("Loading work item payload from: %s", url)
+        LOGGER.info("Loading work item payload from: %s", url)
         response = self._workitem_requests.get(url, _handle_error=handle_error)
         return response.json() if response.ok else {}
 
     def save_payload(self, item_id: str, payload: JSONType):
         url = url_join(item_id, "data")
 
-        logging.info("Saving work item payload to: %s", url)
+        LOGGER.info("Saving work item payload to: %s", url)
         self._workitem_requests.put(url, json=payload)
 
     def list_files(self, item_id: str) -> List[str]:
         url = url_join(item_id, "files")
 
-        logging.info("Listing work item files at: %s", url)
+        LOGGER.info("Listing work item files at: %s", url)
         response = self._workitem_requests.get(url)
 
         return [item["fileName"] for item in response.json()]
 
     def get_file(self, item_id: str, name: str) -> bytes:
         # Robocorp API returns URL for S3 download.
         file_id = self.file_id(item_id, name)
         url = url_join(item_id, "files", file_id)
 
-        logging.info("Downloading work item file at: %s", url)
+        LOGGER.info("Downloading work item file at: %s", url)
         response = self._workitem_requests.get(url)
         file_url = response.json()["url"]
 
         # Perform the actual file download.
         response = self._workitem_requests.get(
             file_url,
             _handle_error=lambda resp: resp.raise_for_status(),
@@ -264,15 +250,15 @@
         # Note that here the `original_name` is useless here. (used with `FileAdapter`
         #   only)
         del original_name
 
         # Robocorp API returns pre-signed POST details for S3 upload.
         url = url_join(item_id, "files")
         body = {"fileName": str(name), "fileSize": len(content)}
-        logging.info(
+        LOGGER.info(
             "Adding work item file into: %s (name: %s, size: %d)",
             url,
             body["fileName"],
             body["fileSize"],
         )
         response = self._workitem_requests.post(url, json=body)
         data = response.json()
@@ -301,19 +287,16 @@
 
         files = response.json()
         if not files:
             raise FileNotFoundError("No files in work item")
 
         matches = [item for item in files if item["fileName"] == name]
         if not matches:
-            raise FileNotFoundError(
-                "File with name '{name}' not in: {names}".format(
-                    name=name, names=", ".join(item["fileName"] for item in files)
-                )
-            )
+            names = ", ".join(item["fileName"] for item in files)
+            raise FileNotFoundError(f"File with name '{name}' not in: {names}")
 
         # Duplicate filenames should never exist,
         # but use last item just in case
         return matches[-1]["fileId"]
 
 
 class FileAdapter(BaseAdapter):
@@ -329,126 +312,108 @@
 
     Optional environment variables:
 
     * RPA_INPUT_WORKITEM_PATH:  Path to work items input database file
     * RPA_OUTPUT_WORKITEM_PATH:  Path to work items output database file
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self) -> None:
+        self._input_path: Optional[Path] = None
+        self._output_path: Optional[Path] = None
+
+        self._inputs: List[Dict[str, Any]] = self.load_database()
+        self._outputs: List[Dict[str, Any]] = []
+        self._index: int = 0
 
-        self._input_path = UNDEFINED
-        self._output_path = UNDEFINED
+    @property
+    def input_path(self) -> Path:
+        if self._input_path is None:
+            path = os.getenv("RC_WORKITEM_INPUT_PATH") or os.getenv(
+                "RPA_INPUT_WORKITEM_PATH"
+            )
+            if not path:
+                raise RuntimeError(
+                    "No input path defined, "
+                    + "set environment variable 'RC_WORKITEM_INPUT_PATH'"
+                )
 
-        self.inputs: List[Dict[str, Any]] = self.load_database()
-        self.outputs: List[Dict[str, Any]] = []
-        self.index: int = 0
+            self._input_path = resolve_path(path)
+
+        return self._input_path
+
+    @property
+    def output_path(self) -> Path:
+        if self._output_path is None:
+            path = os.getenv("RC_WORKITEM_OUTPUT_PATH") or os.getenv(
+                "RPA_OUTPUT_WORKITEM_PATH"
+            )
+            if not path:
+                raise RuntimeError(
+                    "No output path defined, "
+                    + "set environment variable 'RC_WORKITEM_OUTPUT_PATH'"
+                )
+
+            self._output_path = resolve_path(path)
+            self._output_path.parent.mkdir(parents=True, exist_ok=True)
+
+        return self._output_path
 
     def _get_item(self, item_id: str) -> Tuple[str, Dict[str, Any]]:
         # The work item ID is analogue to inputs/outputs list queues index.
         idx = int(item_id)
-        if idx < len(self.inputs):
-            return "input", self.inputs[idx]
+        if idx < len(self._inputs):
+            return "input", self._inputs[idx]
 
-        if idx < (len(self.inputs) + len(self.outputs)):
-            return "output", self.outputs[idx - len(self.inputs)]
+        if idx < (len(self._inputs) + len(self._outputs)):
+            return "output", self._outputs[idx - len(self._inputs)]
 
         raise ValueError(f"Unknown work item ID: {item_id}")
 
+    def _save_to_disk(self, source: str) -> None:
+        if source == "input":
+            path = self.input_path
+            data = self._inputs
+        else:
+            path = self.output_path
+            data = self._outputs
+
+        with open(path, "w", encoding=ENCODING) as fd:
+            fd.write(json_dumps(data, indent=4))
+
+        LOGGER.info("Saved into %s file: %s", source, path)
+
     def reserve_input(self) -> str:
-        if self.index >= len(self.inputs):
+        if self._index >= len(self._inputs):
             raise EmptyQueue("No work items in the input queue")
 
         try:
-            return str(self.index)
+            return str(self._index)
         finally:
-            self.index += 1
+            self._index += 1
 
     def release_input(
         self, item_id: str, state: State, exception: Optional[dict] = None
     ):
         # Nothing happens for now on releasing local dev input Work Items.
-        log_func = logging.error if state == State.FAILED else logging.info
+        log_func = LOGGER.error if state == State.FAILED else LOGGER.info
         log_func(
             "Releasing item %r with %s state and exception: %s",
             item_id,
             state.value,
             exception,
         )
 
-    @property
-    def input_path(self) -> Optional[Path]:
-        if self._input_path is UNDEFINED:
-            # pylint: disable=invalid-envvar-default
-            old_path = os.getenv("RPA_WORKITEMS_PATH")
-            if old_path:
-                deprecation(
-                    "Work items load - Old path style usage detected, please use the "
-                    "'RPA_INPUT_WORKITEM_PATH' env var instead "
-                    "(more details under documentation: https://robocorp.com/docs/development-guide/control-room/data-pipeline#developing-with-work-items-locally)"  # noqa: E501
-                )
-            path = os.getenv("RPA_INPUT_WORKITEM_PATH", default=old_path)
-            if path:
-                logging.info("Resolving input path: %s", path)
-                self._input_path = resolve_path(path)
-            else:
-                # Will raise `TypeError` during inputs loading and will populate the
-                # list with one empty initial input.
-                self._input_path = None
-
-        return self._input_path
-
-    @property
-    def output_path(self) -> Path:
-        if self._output_path is UNDEFINED:
-            # This is usually set once per loaded input work item.
-            new_path = os.getenv("RPA_OUTPUT_WORKITEM_PATH")
-            if new_path:
-                self._output_path = resolve_path(new_path)
-                self._output_path.parent.mkdir(parents=True, exist_ok=True)
-            else:
-                deprecation(
-                    "Work items save - Old path style usage detected, please use the "
-                    "'RPA_OUTPUT_WORKITEM_PATH' env var instead "
-                    "(more details under documentation: https://robocorp.com/docs/development-guide/control-room/data-pipeline#developing-with-work-items-locally)"  # noqa: E501
-                )
-                if not self.input_path:
-                    raise RuntimeError(
-                        "You must provide a path for at least one of the input or "
-                        "output work items files"
-                    )
-                self._output_path = self.input_path.with_suffix(".output.json")
-
-        return self._output_path
-
-    def _save_to_disk(self, source: str) -> None:
-        if source == "input":
-            if not self.input_path:
-                raise RuntimeError(
-                    "Can't save an input item without a path defined, use "
-                    "'RPA_INPUT_WORKITEM_PATH' env for this matter"
-                )
-            path = self.input_path
-            data = self.inputs
-        else:
-            path = self.output_path
-            data = self.outputs
-
-        with open(path, "w", encoding=ENCODING) as fd:
-            fd.write(json_dumps(data, indent=4))
-
-        logging.info("Saved into %s file: %s", source, path)
-
     def create_output(self, _: str, payload: Optional[JSONType] = None) -> str:
         # Note that the `parent_id` is not used during local development.
         item: Dict[str, Any] = {"payload": payload, "files": {}}
-        self.outputs.append(item)
+        self._outputs.append(item)
 
         self._save_to_disk("output")
-        return str(len(self.inputs) + len(self.outputs) - 1)  # new output work item ID
+        item_id = str(len(self._inputs) + len(self._outputs) - 1)
+        return item_id
 
     def load_payload(self, item_id: str) -> JSONType:
         _, item = self._get_item(item_id)
         return item.get("payload", {})
 
     def save_payload(self, item_id: str, payload: JSONType):
         source, item = self._get_item(item_id)
@@ -480,49 +445,45 @@
 
         parent = (
             self.input_path.parent if source == "input" else self.output_path.parent
         )
         path = parent / original_name  # the file on disk will keep its original name
         with open(path, "wb") as fd:
             fd.write(content)
-        logging.info("Created file: %s", path)
+        LOGGER.info("Created file: %s", path)
         files[name] = original_name  # file path relative to the work item
 
         self._save_to_disk(source)
 
     def remove_file(self, item_id: str, name: str):
         source, item = self._get_item(item_id)
         files = item.get("files", {})
 
         path = files[name]
-        logging.info("Would remove file: %s", path)
+        LOGGER.info("Would remove file: %s", path)
         # Note that the file doesn't get removed from disk as well.
         del files[name]
 
         self._save_to_disk(source)
 
     def load_database(self) -> List:
         try:
             try:
                 with open(self.input_path, "r", encoding=ENCODING) as infile:
                     data = json.load(infile)
             except (TypeError, FileNotFoundError):
-                logging.warning("No input work items file found: %s", self.input_path)
+                LOGGER.warning("No input work items file found: %s", self.input_path)
                 data = []
 
-            if isinstance(data, list):
-                assert all(
-                    isinstance(d, dict) for d in data
-                ), "Items should be dictionaries"
-                if len(data) == 0:
-                    data.append({"payload": {}})
-                return data
-
-            # Attempt to migrate from old format
-            assert isinstance(data, dict), "Not a list or dictionary"
-            deprecation("Work items file as mapping is deprecated")
-            workspace = next(iter(data.values()))
-            work_item = next(iter(workspace.values()))
-            return [{"payload": work_item}]
-        except Exception as exc:  # pylint: disable=broad-except
-            logging.exception("Invalid work items file because of: %s", exc)
+            if not isinstance(data, list):
+                raise ValueError("Expected list of items")
+
+            if any(not isinstance(d, dict) for d in data):
+                raise ValueError("Items should be dictionaries")
+
+            if len(data) == 0:
+                data.append({"payload": {}})
+
+            return data
+        except Exception as exc:
+            LOGGER.exception("Invalid work items file because of: %s", exc)
             return [{"payload": {}}]
```

### Comparing `robocorp_workitems-0.3.0/src/robocorp/workitems/workitem.py` & `robocorp_workitems-1.0.0/src/robocorp/workitems/_workitem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,254 +1,305 @@
 import copy
 import fnmatch
+import json
 import logging
 import os
+from glob import glob
 from pathlib import Path
-from shutil import copy2
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
-from robocorp.workitems._workitems._adapter import BaseAdapter
-from robocorp.workitems._workitems._types import Error, State
-from robocorp.workitems._workitems._utils import JSONType, is_json_equal, truncate
-
-
-# TODO: Split into input and output items
-class WorkItem:
-    """Base class for input and output work items.
-
-    Args:
-        adapter:   Adapter instance
-        item_id:   Work item ID (optional)
-        parent_id: Parent work item's ID (optional)
-
-    """
-
-    def __init__(
-        self,
-        adapter: BaseAdapter,
-        item_id: Optional[str] = None,
-        parent_id: Optional[str] = None,
-    ):
-        #: Adapter for loading/saving content
-        self.adapter = adapter
-        #: This item's and/or parent's ID
-        self.id: Optional[str] = item_id
-        self.parent_id: Optional[str] = parent_id
-        assert self.id is not None or self.parent_id is not None
-        #: Item's state on release; can be set once
-        self.state: Optional[State] = None
-        #: Remote JSON payload, and queued changes
-        self._payload: JSONType = {}
-        self._payload_cache: JSONType = {}
-        #: Remote attached files, and queued changes
-        self._files: List[str] = []
-        self._files_to_add: Dict[str, Path] = {}
-        self._files_to_remove: List[str] = []
+from ._adapters import BaseAdapter
+from ._exceptions import ApplicationException, BusinessException, to_exception_type
+from ._types import Email, ExceptionType, JSONType, PathType, State
+from ._utils import truncate
+
+LOGGER = logging.getLogger(__name__)
+
+
+class Input:
+    def __init__(self, item_id: str, adapter: BaseAdapter):
+        self._adapter = adapter
+        self._id = item_id
+        self._payload: JSONType = self._adapter.load_payload(self.id)
+        self._files: List[str] = self._adapter.list_files(self.id)
+        self._state: Optional[State] = None
+        self._outputs: list[Output] = []
 
     def __repr__(self):
-        payload = truncate(str(self.payload), 64)
-        files = len(self.files)
-        return f"WorkItem(id={self.id}, payload={payload}, files={files}, state={self.state})"
+        payload = truncate(json.dumps(self._payload), 64)
+        return (
+            "Input["
+            + f"id={self._id},"
+            + f"payload={payload},"
+            + f"files={self._files},"
+            + f"state={self._state}]"
+        )
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        if exc_type is not None:
-            self.fail(message=str(exc_value))
-        else:
+        if self.released:
+            return False
+
+        if exc_type is None:
             self.done()
+            return False
+
+        exception_type = to_exception_type(exc_type)
+        code = getattr(exc_value, "code", None)
+        message = getattr(exc_value, "message", str(exc_value))
+
+        self.fail(exception_type=exception_type, code=code, message=message)
+
+        # Do not propagate library-specific exceptions
+        return exc_type in (ApplicationException, BusinessException)
 
     @property
-    def is_dirty(self):
-        """Check if work item has unsaved changes."""
-        return (
-            self.id is None
-            or not is_json_equal(self._payload, self._payload_cache)
-            or self._files_to_add
-            or self._files_to_remove
-        )
+    def id(self):
+        return self._id
 
     @property
     def payload(self):
-        return self._payload_cache
-
-    @payload.setter
-    def payload(self, value):
-        self._payload_cache = value
+        return copy.deepcopy(self._payload)
 
     @property
     def files(self):
-        """List of filenames, including local files pending upload and
-        excluding files pending removal.
-        """
-        current = [item for item in self._files if item not in self._files_to_remove]
-        current.extend(self._files_to_add)
-        return list(sorted(set(current)))
+        return list(self._files)
 
     @property
-    def released(self):
-        return self.state is not None
+    def state(self):
+        return self._state
 
-    def load(self):
-        """Load data payload and list of files."""
-        self._payload = self.adapter.load_payload(self.id)
-        self._payload_cache = copy.deepcopy(self._payload)
-
-        self._files = self.adapter.list_files(self.id)
-        self._files_to_add = {}
-        self._files_to_remove = []
+    @property
+    def released(self):
+        return self._state is not None
 
-    def save(self):
-        """Save data payload and attach/remove files."""
-        if self.id is None:
-            self.id = self.adapter.create_output(self.parent_id, payload=self.payload)
-        else:
-            self.adapter.save_payload(self.id, self.payload)
+    @property
+    def outputs(self):
+        return list(self._outputs)
 
-        for name in self._files_to_remove:
-            self.adapter.remove_file(self.id, name)
+    def email(
+        self,
+        html=True,
+        encoding="utf-8",
+        ignore_errors=False,
+    ) -> Optional[Email]:
+        email = self._parse_email()
+        if email is None:
+            raise ValueError("No email in work item")
+
+        if email.errors and not ignore_errors:
+            raise ValueError("\n".join(email.errors))
+
+        if html and "__mail.html" in self._files:
+            content = self._adapter.get_file(self.id, "__mail.html")
+            email.html = content.decode(encoding)
+
+        return email
+
+    def _parse_email(self) -> Optional[Email]:
+        if not isinstance(self._payload, dict):
+            return None
+
+        # Email was successfully parsed by Control Room
+        if "email" in self._payload:
+            try:
+                fields = self._payload["email"]
+                email = Email.from_dict(fields)  # type: ignore
+                return email
+            except Exception as exc:
+                LOGGER.warning("Malformed 'email' field: %s", exc)
+
+        # Email parsing by Control Room failed (payload or attachments too big)
+        if "failedEmail" in self._payload:
+            try:
+                fields = self._payload["failedEmail"]
+                email = Email.from_dict(fields)  # type: ignore
+                email.errors = self._parse_email_errors(self._payload)
+                return email
+            except Exception as exc:
+                LOGGER.warning("Malformed 'failedEmail' field: %s", exc)
+
+        return None
+
+    def _parse_email_errors(self, payload: dict[str, Any]) -> list[str]:
+        errors = payload.get("errors", [])
+        if not isinstance(errors, list):
+            LOGGER.warning("Expected 'errors' as 'list', was '%s'", type(errors))
+            return []
+
+        result = []
+        for err in errors:
+            msg = err["message"]
+            if files := err.get("files"):
+                names = ", ".join(f["name"] for f in files)
+                msg += f" ({names})"
+            result.append(msg)
 
-        for name, path in self._files_to_add.items():
-            with open(path, "rb") as infile:
-                self.adapter.add_file(
-                    self.id, name, original_name=path.name, content=infile.read()
-                )
+        return result
 
-        # Empty unsaved values
-        self._payload = self._payload_cache
-        self._payload_cache = copy.deepcopy(self._payload)
-
-        self._files = self.files
-        self._files_to_add = {}
-        self._files_to_remove = []
-
-    def get_file(self, name, path=None) -> str:
-        """Load an attached file and store it on the local filesystem.
-
-        :param name: Name of attached file
-        :param path: Destination path. Default to current working directory.
-        :returns:    Path to created file
-        """
+    def download_file(self, name: str, path: Optional[PathType] = None) -> Path:
         if name not in self.files:
-            raise FileNotFoundError(f"No such file: {name}")
+            raise KeyError(name)
 
-        if not path:
+        if path is None:
             root = os.getenv("ROBOT_ROOT", "")
-            path = os.path.join(root, name)
-
-        if name in self._files_to_add:
-            local_path = self._files_to_add[name]
-            if Path(local_path).resolve() != Path(path).resolve():
-                copy2(local_path, path)
+            path = Path(root) / name
         else:
-            content = self.adapter.get_file(self.id, name)
-            with open(path, "wb") as outfile:
-                outfile.write(content)
-
-        # Always return absolute path
-        return str(Path(path).resolve())
-
-    # TODO: implement file pattern get
-    def get_files(self, pattern, dirname=None) -> List[str]:
-        paths = []
-        for name in self.files:
-            if fnmatch.fnmatch(name, pattern):
-                if dirname:
-                    path = self.get_file(name, os.path.join(dirname, name))
-                else:
-                    path = self.get_file(name)
-                paths.append(path)
-
-        logging.info("Downloaded %d file(s)", len(paths))
-        return paths
-
-    def add_file(self, path, name=None):
-        """Add file to current work item. Does not upload
-        until ``save()`` is called.
-
-        :param path: Path to file to upload
-        :param name: Name of file in work item. If not given,
-                     name of file on disk is used.
-        """
-        path = Path(path).resolve()
-
-        if path in self._files_to_add.values():
-            logging.warning("File already added: %s", path)
+            path = Path(path)
 
-        if not path.is_file():
-            raise FileNotFoundError(f"Not a valid file: {path}")
-
-        name = name or path.name
-        self._files_to_add[name] = path
+        content = self._adapter.get_file(self.id, name)
+        with open(path, "wb") as fd:
+            fd.write(content)
 
-        if name in self._files_to_remove:
-            self._files_to_remove.remove(name)
+        return path.absolute()
 
-        return name
-
-    def remove_file(self, name, missing_ok=True):
-        """Remove file from current work item. Change is not applied
-        until ``save()`` is called.
+    def download_files(self, pattern: str, path: Optional[Path] = None) -> List[Path]:
+        if path is None:
+            root = os.getenv("ROBOT_ROOT", "")
+            path = Path(root)
+        else:
+            path = Path(path)
 
-        :param name: Name of attached file
-        """
-        if not missing_ok and name not in self.files:
-            raise FileNotFoundError(f"No such file: {name}")
+        path.mkdir(parents=True, exist_ok=True)
 
-        if name in self._files:
-            self._files_to_remove.append(name)
+        paths = []
+        for name in self.files:
+            if not fnmatch.fnmatch(name, pattern):
+                continue
 
-        if name in self._files_to_add:
-            del self._files_to_add[name]
+            filepath = (path / name).absolute()
+            paths.append(filepath)
 
-        return name
+            content = self._adapter.get_file(self._id, name)
+            with open(filepath, "wb") as fd:
+                fd.write(content)
 
-    def create_output(
-        self,
-        variables: Optional[dict] = None,
-        files: Optional[Union[str, List[str]]] = None,
-        save: bool = True,
-    ):
-        # TODO: Implement
-        raise NotImplementedError
+        return paths
 
-    def _ensure_releasable(self):
-        # TODO: Move these checks elsewhere
-        if self.state is not None:
-            raise RuntimeError("Input work item already released")
-        if self.parent_id is None:
-            raise RuntimeError("Cannot set state on output item")
-        if self.id is not None:
-            raise RuntimeError("Cannot set state on input item with null ID")
+    def create_output(self) -> "Output":
+        item = Output(parent_id=self.id, adapter=self._adapter)
+        self._outputs.append(item)
+        return item
 
     def done(self):
-        """Mark item status as DONE."""
-        self._ensure_releasable()
+        if self._state is not None:
+            raise RuntimeError("Work item already released")
 
         state = State.DONE
-
-        self.adapter.release_input(self.id, state, exception=None)
-        self.state = state
+        self._adapter.release_input(self._id, state, exception=None)
+        self._state = state
 
     def fail(
         self,
-        exception_type: Union[Error, str] = Error.APPLICATION,
+        exception_type: Union[ExceptionType, str] = ExceptionType.APPLICATION,
         code: Optional[str] = None,
         message: Optional[str] = None,
     ):
-        self._ensure_releasable()
-        state = State.FAILED
+        if self._state is not None:
+            raise RuntimeError("Work item already released")
 
         type_ = (
             exception_type
-            if isinstance(exception_type, Error)
-            else Error(exception_type.upper())
+            if isinstance(exception_type, ExceptionType)
+            else ExceptionType(exception_type.upper())
         )
+
         exception = {
             "type": type_.value,
             "code": code,
             "message": message,
         }
 
-        self.adapter.release_input(self.id, state, exception=exception)
-        self.state = state
+        state = State.FAILED
+        self._adapter.release_input(self._id, state, exception=exception)
+        self._state = state
+
+
+class Output:
+    def __init__(self, parent_id: str, adapter: BaseAdapter):
+        self._adapter = adapter
+        self._parent_id = parent_id
+        self._id: Optional[str] = None
+        self._payload: JSONType = {}
+        self._files: Dict[str, Path] = {}
+
+    def __repr__(self):
+        payload = truncate(str(self.payload), 64)
+        return (
+            "Output["
+            + f"parent={self._parent_id},"
+            + f"payload={payload},"
+            + f"files={self.files},"
+            + f"saved={self.saved}]"
+        )
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        if exc_type is not None:
+            self.save()
+
+    @property
+    def id(self):
+        return self._id
+
+    @property
+    def parent_id(self):
+        return self._parent_id
+
+    @property
+    def payload(self):
+        return self._payload
+
+    @payload.setter
+    def payload(self, value):
+        self._payload = value
+
+    @property
+    def files(self):
+        return list(self._files.keys())
+
+    @property
+    def saved(self):
+        return self._id is not None
+
+    def save(self):
+        if self.saved:
+            raise RuntimeError("Output already saved")
+
+        self._id = self._adapter.create_output(self.parent_id, payload=self.payload)
+
+        for name, path in self._files.items():
+            with open(path, "rb") as fd:
+                self._adapter.add_file(
+                    self._id,
+                    name,
+                    original_name=path.name,
+                    content=fd.read(),
+                )
+
+    def add_file(self, path: Union[Path, str], name: Optional[str] = None) -> Path:
+        path = Path(path).resolve()
+        name = name or path.name
+
+        if not path.is_file():
+            raise FileNotFoundError(f"Not a valid file: {path}")
+
+        if name in self._files:
+            LOGGER.warning('File with name "%s" already exists', name)
+
+        self._files[name] = path
+        return path
+
+    def add_files(self, pattern: str) -> list[Path]:
+        matches = glob(pattern, recursive=False)
+
+        paths = []
+        for match in matches:
+            path = self.add_file(match)
+            paths.append(path)
+
+        LOGGER.info("Added %d file(s)", len(paths))
+        return paths
```

