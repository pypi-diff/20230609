# Comparing `tmp/langchainplus_sdk-0.0.6.tar.gz` & `tmp/langchainplus_sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.6.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.7.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.6.tar` & `langchainplus_sdk-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     8124 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/README.md
--rw-r--r--   0        0        0      529 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1198 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/docker-compose.yaml
--rw-r--r--   0        0        0    12934 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/main.py
--rw-r--r--   0        0        0    20044 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/client.py
--rw-r--r--   0        0        0      250 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/__init__.py
--rw-r--r--   0        0        0     1419 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/evaluator.py
--rw-r--r--   0        0        0     1545 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     7178 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     7001 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     3235 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      879 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     8124 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/README.md
+-rw-r--r--   0        0        0      529 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1198 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    12934 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/cli/main.py
+-rw-r--r--   0        0        0       95 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/cli/ngrok_config.yaml
+-rw-r--r--   0        0        0    21360 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0      250 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/evaluation/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1545 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     4850 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     8627 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     3271 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      879 2023-06-08 22:22:29.715989 langchainplus_sdk-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.7/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.6/README.md` & `langchainplus_sdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/__init__.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/cli/docker-compose.yaml` & `langchainplus_sdk-0.0.7/langchainplus_sdk/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/cli/main.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/cli/main.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     FeedbackCreate,
     FeedbackSourceBase,
     FeedbackSourceType,
     ListFeedbackQueryParams,
     ListRunsQueryParams,
     ModelFeedbackSource,
     Run,
+    RunCreate,
+    RunTypeEnum,
+    RunUpdate,
     TracerSession,
 )
 from langchainplus_sdk.utils import (
     LangChainPlusAPIError,
     LangChainPlusError,
     LangChainPlusUserError,
     raise_for_status_with_text,
@@ -177,14 +180,57 @@
         # TODO: Make this more robust server-side
         if "detail" in result and "already exists" in result["detail"]:
             file_name = csv_file if isinstance(csv_file, str) else csv_file[0]
             file_name = file_name.split("/")[-1]
             raise ValueError(f"Dataset {file_name} already exists")
         return Dataset(**result)
 
+    def create_run(
+        self,
+        name: str,
+        inputs: Dict[str, Any],
+        run_type: Union[str, RunTypeEnum],
+        **kwargs: Any,
+    ) -> Run:
+        """Persist a run to the LangChain+ API."""
+        run_create = RunCreate(
+            **kwargs,
+            name=name,
+            inputs=inputs,
+            run_type=run_type,
+        )
+        headers = {**self._headers, "Accept": "application/json"}
+        request_with_retries(
+            "post",
+            f"{self.api_url}/runs",
+            request_kwargs={
+                "data": run_create.json(exclude_none=True),
+                "headers": headers,
+            },
+            retry_config=self.retry_config,
+        )
+        return Run(**run_create.dict(exclude_none=True))
+
+    def update_run(
+        self,
+        run_id: ID_TYPE,
+        **kwargs: Any,
+    ) -> None:
+        """Update a run to the LangChain+ API."""
+        run_update = RunUpdate(
+            **kwargs,
+        )
+        headers = {**self._headers, "Accept": "application/json"}
+        request_with_retries(
+            "patch",
+            f"{self.api_url}/runs/{run_id}",
+            request_kwargs={"data": run_update.json(), "headers": headers},
+            retry_config=self.retry_config,
+        )
+
     def read_run(self, run_id: ID_TYPE) -> Run:
         """Read a run from the LangChain+ API."""
         response = self._get_with_retries(f"/runs/{run_id}")
         return Run(**response.json())
 
     def list_runs(
         self,
```

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/evaluator.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/string_evaluator.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/schemas.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,207 +1,320 @@
 """Schemas for the langchainplus API."""
 from __future__ import annotations
 
-import logging
 import os
-from concurrent.futures import Future, ThreadPoolExecutor
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Union
+from enum import Enum
+from typing import Any, Dict, List, Optional, Sequence, Union
 from uuid import UUID, uuid4
 
-from pydantic import Field, root_validator
-from tenacity import (
-    before_sleep_log,
-    retry_if_exception_type,
-    stop_after_attempt,
-    wait_exponential_jitter,
+from pydantic import (
+    BaseModel,
+    Field,
+    StrictBool,
+    StrictFloat,
+    StrictInt,
+    root_validator,
 )
+from typing_extensions import Literal
 
-from langchainplus_sdk.schemas import RunBase, RunTypeEnum, RunUpdate
-from langchainplus_sdk.utils import (
-    LangChainPlusAPIError,
-    get_runtime_environment,
-    request_with_retries,
-)
+from langchainplus_sdk.utils import get_runtime_environment
 
-logger = logging.getLogger(__name__)
-_THREAD_POOL_EXECUTOR: Optional[ThreadPoolExecutor] = None
+SCORE_TYPE = Union[StrictBool, StrictInt, StrictFloat, None]
+VALUE_TYPE = Union[Dict, StrictBool, StrictInt, StrictFloat, str, None]
 
 
-def _ensure_thread_pool() -> ThreadPoolExecutor:
-    """Ensure a thread pool exists in the current context."""
-    global _THREAD_POOL_EXECUTOR
-    if _THREAD_POOL_EXECUTOR is None:
-        _THREAD_POOL_EXECUTOR = ThreadPoolExecutor(max_workers=1)
-    return _THREAD_POOL_EXECUTOR
-
-
-def await_all_runs() -> None:
-    """Flush the thread pool."""
-    global _THREAD_POOL_EXECUTOR
-    if _THREAD_POOL_EXECUTOR is not None:
-        _THREAD_POOL_EXECUTOR.shutdown(wait=True)
-        _THREAD_POOL_EXECUTOR = None
-
-
-def _default_retry_config() -> Dict[str, Any]:
-    return dict(
-        stop=stop_after_attempt(3),
-        wait=wait_exponential_jitter(initial=1, max=10),
-        retry=retry_if_exception_type(LangChainPlusAPIError),
-        before_sleep=before_sleep_log(logger, logging.WARNING),
-    )
+class ExampleBase(BaseModel):
+    """Example base model."""
+
+    dataset_id: UUID
+    inputs: Dict[str, Any]
+    outputs: Optional[Dict[str, Any]] = Field(default=None)
+
+    class Config:
+        frozen = True
+
+
+class ExampleCreate(ExampleBase):
+    """Example create model."""
+
+    id: Optional[UUID]
+    created_at: datetime = Field(default_factory=datetime.utcnow)
+
+
+class Example(ExampleBase):
+    """Example model."""
+
+    id: UUID
+    created_at: datetime
+    modified_at: Optional[datetime] = Field(default=None)
+    runs: List[Run] = Field(default_factory=list)
 
 
-class RunTree(RunBase):
-    """Run Schema with back-references for posting runs."""
+class ExampleUpdate(BaseModel):
+    """Update class for Example."""
+
+    dataset_id: Optional[UUID] = None
+    inputs: Optional[Dict[str, Any]] = None
+    outputs: Optional[Dict[str, Any]] = None
+
+    class Config:
+        frozen = True
+
+
+class DatasetBase(BaseModel):
+    """Dataset base model."""
 
     name: str
-    id: Optional[UUID] = Field(default_factory=uuid4)
-    parent_run: Optional[RunTree] = Field(default=None, exclude=True)
-    child_runs: List[RunTree] = Field(
-        default_factory=list, exclude={"__all__": {"parent_run_id"}}
-    )
-    session_name: str = Field(default="default")
-    session_id: Optional[UUID] = Field(default=None)
-    execution_order: int = 1
-    child_execution_order: int = 1
-    api_url: str = Field(
-        default=os.environ.get("LANGCHAIN_ENDPOINT", "http://localhost:1984"),
-        exclude=True,
-    )
-    api_key: Optional[str] = Field(
-        default=os.environ.get("LANGCHAIN_API_KEY"), exclude=True
-    )
-    retry_config: Dict[str, Any] = Field(
-        default_factory=_default_retry_config, exclude=True
-    )
+    description: Optional[str] = None
+
+    class Config:
+        frozen = True
+
+
+class DatasetCreate(DatasetBase):
+    """Dataset create model."""
+
+    id: Optional[UUID]
+    created_at: datetime = Field(default_factory=datetime.utcnow)
+
+
+class Dataset(DatasetBase):
+    """Dataset ORM model."""
+
+    id: UUID
+    created_at: datetime
+    modified_at: Optional[datetime] = Field(default=None)
+
+
+class RunTypeEnum(str, Enum):
+    """Enum for run types."""
+
+    tool = "tool"
+    chain = "chain"
+    llm = "llm"
+
+
+class RunBase(BaseModel):
+    """Base Run schema."""
+
+    id: Optional[UUID]
+    start_time: datetime = Field(default_factory=datetime.utcnow)
+    end_time: datetime = Field(default_factory=datetime.utcnow)
+    extra: dict = Field(default_factory=dict)
+    error: Optional[str]
+    execution_order: int
+    serialized: dict
+    inputs: dict
+    outputs: Optional[dict]
+    reference_example_id: Optional[UUID]
+    run_type: RunTypeEnum
+    parent_run_id: Optional[UUID]
+
+
+class Run(RunBase):
+    """Run schema when loading from the DB."""
+
+    id: UUID
+    name: str
+    child_runs: List[Run] = Field(default_factory=list)
 
     @root_validator(pre=True)
-    def infer_defaults(cls, values: dict) -> dict:
+    def assign_name(cls, values: dict) -> dict:
         """Assign name to the run."""
         if "name" not in values:
-            if "serialized" not in values:
-                raise ValueError("Must provide either name or serialized.")
-            if "name" not in values["serialized"]:
-                raise ValueError(
-                    "Must provide either name or serialized with a name attribute."
-                )
             values["name"] = values["serialized"]["name"]
-        elif "serialized" not in values:
-            values["serialized"] = {"name": values["name"]}
-        if "execution_order" not in values:
-            values["execution_order"] = 1
-        if "child_execution_order" not in values:
-            values["child_execution_order"] = values["execution_order"]
-        if values.get("session_name") is None:
-            values["session_name"] = os.environ.get("LANGCHAIN_SESSION", "default")
-        if values.get("parent_run") is not None:
-            values["parent_run_id"] = values["parent_run"].id
-        extra = values.get("extra", {})
-        extra["runtime"] = get_runtime_environment()
-        values["extra"] = extra
         return values
 
-    @property
-    def _headers(self) -> Dict[str, str]:
-        headers = {"Content-Type": "application/json"}
-        if self.api_key:
-            headers["x-api-key"] = self.api_key
-        return headers
-
-    def end(
-        self,
-        *,
-        outputs: Optional[Dict] = None,
-        error: Optional[str] = None,
-        end_time: Optional[datetime] = None,
-    ) -> None:
-        """Set the end time of the run and all child runs."""
-        self.end_time = end_time or datetime.utcnow()
-        if outputs is not None:
-            self.outputs = outputs
-        if error is not None:
-            self.error = error
-        if self.parent_run:
-            self.parent_run.child_execution_order = max(
-                self.parent_run.child_execution_order,
-                self.child_execution_order,
+
+def infer_default_run_values(values: Dict[str, Any]) -> Dict[str, Any]:
+    if "name" not in values:
+        if "serialized" not in values:
+            raise ValueError("Must provide either name or serialized.")
+        if "name" not in values["serialized"]:
+            raise ValueError(
+                "Must provide either name or serialized with a name attribute."
             )
+        values["name"] = values["serialized"]["name"]
+    elif "serialized" not in values:
+        values["serialized"] = {"name": values["name"]}
+    if "execution_order" not in values:
+        values["execution_order"] = 1
+    if "child_execution_order" not in values:
+        values["child_execution_order"] = values["execution_order"]
+    if values.get("parent_run") is not None:
+        values["parent_run_id"] = values["parent_run"].id
+    extra = values.get("extra", {})
+    if "runtime" not in extra:
+        extra["runtime"] = {}
+    runtime_env = get_runtime_environment()
+    for k, v in runtime_env.items():
+        if k not in extra["runtime"]:
+            extra["runtime"][k] = v
+    values["extra"] = extra
+    return values
+
+
+class RunCreate(RunBase):
+    """Run create schema."""
+
+    id: UUID = Field(default_factory=uuid4)
+    name: str
+    session_name: str = Field(
+        default_factory=lambda: os.environ.get("LANGCHAIN_SESSION", "default")
+    )
+    child_runs: Optional[List[RunCreate]] = None
+
+    @root_validator(pre=True)
+    def add_runtime_env(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """Add env info to the run."""
+        return infer_default_run_values(values)
+
+
+class RunUpdate(BaseModel):
+    end_time: Optional[datetime]
+    error: Optional[str]
+    outputs: Optional[dict]
+    parent_run_id: Optional[UUID]
+    reference_example_id: Optional[UUID]
+
+
+class ListRunsQueryParams(BaseModel):
+    """Query params for GET /runs endpoint."""
+
+    id: Optional[List[UUID]]
+    """Filter runs by id."""
+    parent_run: Optional[UUID]
+    """Filter runs by parent run."""
+    run_type: Optional[RunTypeEnum]
+    """Filter runs by type."""
+    session: Optional[UUID] = Field(default=None, alias="session_id")
+    """Only return runs within a session."""
+    reference_example: Optional[UUID]
+    """Only return runs that reference the specified dataset example."""
+    execution_order: Optional[int]
+    """Filter runs by execution order."""
+    error: Optional[bool]
+    """Whether to return only runs that errored."""
+    offset: Optional[int]
+    """The offset of the first run to return."""
+    limit: Optional[int]
+    """The maximum number of runs to return."""
+    start_time: Optional[datetime] = Field(
+        default=None,
+        alias="start_before",
+        description="Query Runs that started <= this time",
+    )
+    end_time: Optional[datetime] = Field(
+        default=None,
+        alias="end_after",
+        description="Query Runs that ended >= this time",
+    )
+
+    class Config:
+        extra = "forbid"
+        frozen = True
+
+    @root_validator
+    def validate_time_range(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """Validate that start_time <= end_time."""
+        start_time = values.get("start_time")
+        end_time = values.get("end_time")
+        if start_time and end_time and start_time > end_time:
+            raise ValueError("start_time must be <= end_time")
+        return values
+
+
+class FeedbackSourceBase(BaseModel):
+    type: str
+    metadata: Optional[Dict[str, Any]] = None
+
+    class Config:
+        frozen = True
+
+
+class APIFeedbackSource(FeedbackSourceBase):
+    """API feedback source."""
+
+    type: Literal["api"] = "api"
+
+
+class ModelFeedbackSource(FeedbackSourceBase):
+    """Model feedback source."""
+
+    type: Literal["model"] = "model"
+
+
+class FeedbackSourceType(Enum):
+    """Feedback source type."""
+
+    API = "api"
+    """General feedback submitted from the API."""
+    MODEL = "model"
+    """Model-assisted feedback."""
+
+
+class FeedbackBase(BaseModel):
+    """Feedback schema."""
+
+    created_at: datetime = Field(default_factory=datetime.utcnow)
+    """The time the feedback was created."""
+    modified_at: datetime = Field(default_factory=datetime.utcnow)
+    """The time the feedback was last modified."""
+    run_id: UUID
+    """The associated run ID this feedback is logged for."""
+    key: str
+    """The metric name, tag, or aspect to provide feedback on."""
+    score: SCORE_TYPE = None
+    """Value or score to assign the run."""
+    value: VALUE_TYPE = None
+    """The display value, tag or other value for the feedback if not a metric."""
+    comment: Optional[str] = None
+    """Comment or explanation for the feedback."""
+    correction: Union[str, dict, None] = None
+    """Correction for the run."""
+    feedback_source: Optional[FeedbackSourceBase] = None
+    """The source of the feedback."""
+
+    class Config:
+        frozen = True
+
+
+class FeedbackCreate(FeedbackBase):
+    """Schema used for creating feedback."""
+
+    id: UUID = Field(default_factory=uuid4)
+
+    feedback_source: FeedbackSourceBase
+    """The source of the feedback."""
+
+
+class Feedback(FeedbackBase):
+    """Schema for getting feedback."""
+
+    id: UUID
+    feedback_source: Optional[FeedbackSourceBase] = None
+    """The source of the feedback. In this case"""
+
+
+class ListFeedbackQueryParams(BaseModel):
+    """Query Params for listing feedbacks."""
+
+    run: Optional[Sequence[UUID]] = None
+    limit: int = 100
+    offset: int = 0
+
+    class Config:
+        """Config for query params."""
+
+        extra = "forbid"
+        frozen = True
+
+
+class TracerSession(BaseModel):
+    """TracerSession schema for the V2 API."""
 
-    def create_child(
-        self,
-        name: str,
-        run_type: Union[str, RunTypeEnum],
-        *,
-        run_id: Optional[UUID] = None,
-        serialized: Optional[Dict] = None,
-        inputs: Optional[Dict] = None,
-        outputs: Optional[Dict] = None,
-        error: Optional[str] = None,
-        reference_example_id: Optional[UUID] = None,
-        start_time: Optional[datetime] = None,
-        end_time: Optional[datetime] = None,
-        extra: Optional[Dict] = None,
-    ) -> RunTree:
-        """Add a child run to the run tree."""
-        execution_order = self.child_execution_order + 1
-        serialized_ = serialized or {"name": name}
-        run = RunTree(
-            name=name,
-            id=run_id or uuid4(),
-            serialized=serialized_,
-            inputs=inputs or {},
-            outputs=outputs or {},
-            error=error,
-            run_type=run_type,
-            reference_example_id=reference_example_id,
-            start_time=start_time or datetime.utcnow(),
-            end_time=end_time or datetime.utcnow(),
-            execution_order=execution_order,
-            child_execution_order=execution_order,
-            extra=extra or {},
-            parent_run=self,
-            session_name=self.session_name,
-            api_url=self.api_url,
-            api_key=self.api_key,
-        )
-        self.child_runs.append(run)
-        return run
-
-    def _post(self, data: str) -> None:
-        """Post the run tree to the API."""
-        request_with_retries(
-            "post",
-            f"{self.api_url}/runs",
-            request_kwargs={
-                "data": data,
-                "headers": self._headers,
-            },
-            retry_config=self.retry_config,
-        )
-
-    def post(self, exclude_child_runs: bool = True) -> Future:
-        """Post the run tree to the API asynchronously."""
-        executor = _ensure_thread_pool()
-        exclude = {"child_runs"} if exclude_child_runs else None
-        data = self.json(exclude=exclude, exclude_none=True)
-        return executor.submit(self._post, data=data)
-
-    def _patch(self, data: str) -> None:
-        """Patch the run tree to the API."""
-        request_with_retries(
-            "patch",
-            f"{self.api_url}/runs/{self.id}",
-            request_kwargs={
-                "data": data,
-                "headers": self._headers,
-            },
-            retry_config=self.retry_config,
-        )
-
-    def patch(self) -> Future:
-        """Patch the run tree to the API in a background thread."""
-        executor = _ensure_thread_pool()
-        run_update = RunUpdate(**self.dict(exclude_none=True))
-        data = run_update.json(exclude_none=True)
-        return executor.submit(self._patch, data=data)
+    id: UUID
+    start_time: datetime = Field(default_factory=datetime.utcnow)
+    name: Optional[str] = None
+    extra: Optional[Dict[str, Any]] = None
+    tenant_id: UUID
```

### Comparing `langchainplus_sdk-0.0.6/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.7/langchainplus_sdk/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,12 +81,13 @@
 @lru_cache(maxsize=1)
 def get_runtime_environment() -> dict:
     """Get information about the environment."""
     # Lazy import to avoid circular imports
     from langchainplus_sdk import __version__
 
     return {
-        "library_version": __version__,
+        "sdk_version": __version__,
+        "library": "langchainplus_sdk",
         "platform": platform.platform(),
         "runtime": "python",
         "runtime_version": platform.python_version(),
     }
```

### Comparing `langchainplus_sdk-0.0.6/pyproject.toml` & `langchainplus_sdk-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.6"
+version = "0.0.7"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.scripts]
```

### Comparing `langchainplus_sdk-0.0.6/PKG-INFO` & `langchainplus_sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

