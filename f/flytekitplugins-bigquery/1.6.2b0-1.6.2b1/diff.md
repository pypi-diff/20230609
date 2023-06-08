# Comparing `tmp/flytekitplugins-bigquery-1.6.2b0.tar.gz` & `tmp/flytekitplugins-bigquery-1.6.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.6.2b0.tar", last modified: Thu Jun  1 20:41:52 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.6.2b1.tar", last modified: Thu Jun  8 23:49:40 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.6.2b0.tar` & `flytekitplugins-bigquery-1.6.2b1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.155790 flytekitplugins-bigquery-1.6.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 20:41:52.151790 flytekitplugins-bigquery-1.6.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-01 20:41:31.000000 flytekitplugins-bigquery-1.6.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.151790 flytekitplugins-bigquery-1.6.2b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.151790 flytekitplugins-bigquery-1.6.2b0/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 20:41:31.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-01 20:41:31.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins/bigquery/backend_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-01 20:41:31.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.151790 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:52.000000 flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:41:52.155790 flytekitplugins-bigquery-1.6.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-01 20:41:50.000000 flytekitplugins-bigquery-1.6.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-08 23:49:38.000000 flytekitplugins-bigquery-1.6.2b1/setup.py
```

### Comparing `flytekitplugins-bigquery-1.6.2b0/PKG-INFO` & `flytekitplugins-bigquery-1.6.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.2b0/README.md` & `flytekitplugins-bigquery-1.6.2b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.2b0/flytekitplugins/bigquery/backend_plugin.py` & `flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import datetime
+import json
+from dataclasses import asdict, dataclass
 from typing import Dict, Optional
 
 import grpc
-from flyteidl.service.external_plugin_service_pb2 import (
-    SUCCEEDED,
-    TaskCreateResponse,
-    TaskDeleteResponse,
-    TaskGetResponse,
-)
+from flyteidl.admin.agent_pb2 import SUCCEEDED, CreateTaskResponse, DeleteTaskResponse, GetTaskResponse, Resource
 from google.cloud import bigquery
 
 from flytekit import FlyteContextManager, StructuredDataset, logger
 from flytekit.core.type_engine import TypeEngine
-from flytekit.extend.backend.base_plugin import BackendPluginBase, BackendPluginRegistry, convert_to_flyte_state
+from flytekit.extend.backend.base_agent import AgentBase, AgentRegistry, convert_to_flyte_state
 from flytekit.models import literals
 from flytekit.models.literals import LiteralMap
 from flytekit.models.task import TaskTemplate
 from flytekit.models.types import LiteralType, StructuredDatasetType
 
 pythonTypeToBigQueryType: Dict[type, str] = {
     # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types#data_type_sizes
@@ -26,25 +23,30 @@
     datetime.datetime: "DATETIME",
     float: "FLOAT64",
     int: "INT64",
     str: "STRING",
 }
 
 
-class BigQueryPlugin(BackendPluginBase):
+@dataclass
+class Metadata:
+    job_id: str
+
+
+class BigQueryAgent(AgentBase):
     def __init__(self):
         super().__init__(task_type="bigquery_query_job_task")
 
     def create(
         self,
         context: grpc.ServicerContext,
         output_prefix: str,
         task_template: TaskTemplate,
         inputs: Optional[LiteralMap] = None,
-    ) -> TaskCreateResponse:
+    ) -> CreateTaskResponse:
         job_config = None
         if inputs:
             ctx = FlyteContextManager.current_context()
             python_interface_inputs = {
                 name: TypeEngine.guess_python_type(lt.type) for name, lt in task_template.interface.inputs.items()
             }
             native_inputs = TypeEngine.literal_map_to_kwargs(ctx, inputs, python_interface_inputs)
@@ -57,19 +59,22 @@
                 ]
             )
 
         custom = task_template.custom
         client = bigquery.Client(project=custom["ProjectID"], location=custom["Location"])
         query_job = client.query(task_template.sql.statement, job_config=job_config)
 
-        return TaskCreateResponse(job_id=str(query_job.job_id))
+        return CreateTaskResponse(
+            resource_meta=json.dumps(asdict(Metadata(job_id=str(query_job.job_id)))).encode("utf-8")
+        )
 
-    def get(self, context: grpc.ServicerContext, job_id: str) -> TaskGetResponse:
+    def get(self, context: grpc.ServicerContext, resource_meta: bytes) -> GetTaskResponse:
         client = bigquery.Client()
-        job = client.get_job(job_id)
+        metadata = Metadata(**json.loads(resource_meta.decode("utf-8")))
+        job = client.get_job(metadata.job_id)
         cur_state = convert_to_flyte_state(str(job.state))
         res = None
 
         if cur_state == SUCCEEDED:
             ctx = FlyteContextManager.current_context()
             output_location = f"bq://{job.destination.project}:{job.destination.dataset_id}.{job.destination.table_id}"
             res = literals.LiteralMap(
@@ -79,16 +84,17 @@
                         StructuredDataset(uri=output_location),
                         StructuredDataset,
                         LiteralType(structured_dataset_type=StructuredDatasetType(format="")),
                     )
                 }
             )
 
-        return TaskGetResponse(state=cur_state, outputs=res.to_flyte_idl())
+        return GetTaskResponse(resource=Resource(state=cur_state, outputs=res.to_flyte_idl()))
 
-    def delete(self, context: grpc.ServicerContext, job_id: str) -> TaskDeleteResponse:
+    def delete(self, context: grpc.ServicerContext, resource_meta: bytes) -> DeleteTaskResponse:
         client = bigquery.Client()
-        client.cancel_job(job_id)
-        return TaskDeleteResponse()
+        metadata = Metadata(**json.loads(resource_meta.decode("utf-8")))
+        client.cancel_job(metadata.job_id)
+        return DeleteTaskResponse()
 
 
-BackendPluginRegistry.register(BigQueryPlugin())
+AgentRegistry.register(BigQueryAgent())
```

### Comparing `flytekitplugins-bigquery-1.6.2b0/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.2b0/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.2b0/setup.py` & `flytekitplugins-bigquery-1.6.2b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.6.2b0"
+__version__ = "1.6.2b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```

