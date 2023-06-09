# Comparing `tmp/qdrant_haystack-1.0.2.tar.gz` & `tmp/qdrant_haystack-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-1.0.2.tar", max compression
+gzip compressed data, was "qdrant_haystack-1.0.3.tar", max compression
```

## Comparing `qdrant_haystack-1.0.2.tar` & `qdrant_haystack-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/LICENSE
--rw-r--r--   0        0        0     3160 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/README.md
--rw-r--r--   0        0        0      764 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2285 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    20289 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-05-16 14:51:23.634444 qdrant_haystack-1.0.2/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 11:42:00.938619 qdrant_haystack-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3160 2023-06-09 11:42:00.938619 qdrant_haystack-1.0.3/README.md
+-rw-r--r--   0        0        0      764 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2291 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    20093 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.3/PKG-INFO
```

### Comparing `qdrant_haystack-1.0.2/LICENSE` & `qdrant_haystack-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.2/README.md` & `qdrant_haystack-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.2/pyproject.toml` & `qdrant_haystack-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "1.0.2"
+version = "1.0.3"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
```

### Comparing `qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,17 @@
 class QdrantToHaystack:
     def __init__(self, content_field: str, name_field: str, embedding_field: str):
         self.content_field = content_field
         self.name_field = name_field
         self.embedding_field = embedding_field
 
     def point_to_document(self, point: QdrantPoint) -> Document:
+        payload = {**point.payload}
         return Document(
-            content=point.payload.pop(self.content_field),
-            content_type=point.payload.pop("content_type"),
-            id=point.payload.pop("id"),
-            meta=point.payload.pop("meta"),
+            content=payload.pop(self.content_field),
+            content_type=payload.pop("content_type"),
+            id=payload.pop("id"),
+            meta=payload.pop("meta"),
             score=point.score if hasattr(point, "score") else None,
             embedding=np.array(point.vector) if point.vector else None,
-            id_hash_keys=point.payload.pop("id_hash_keys"),
+            id_hash_keys=payload.pop("id_hash_keys"),
         )
```

### Comparing `qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.2/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from haystack import Document, Label
 from haystack.document_stores import BaseDocumentStore
 from haystack.document_stores.base import get_batches_from_generator
 from haystack.errors import DocumentStoreError
 from haystack.nodes import DenseRetriever
 from haystack.schema import FilterType
 from qdrant_client import grpc
-from qdrant_client.conversions import common_types as types
 from qdrant_client.http import models as rest
 from qdrant_client.http.exceptions import UnexpectedResponse
 from tqdm import tqdm
 
 from qdrant_haystack.document_stores.converters import (
     HaystackToQdrant,
     QdrantToHaystack,
@@ -59,20 +58,19 @@
         progress_bar: bool = True,
         duplicate_documents: str = "overwrite",
         recreate_index: bool = False,
         shard_number: Optional[int] = None,
         replication_factor: Optional[int] = None,
         write_consistency_factor: Optional[int] = None,
         on_disk_payload: Optional[bool] = None,
-        hnsw_config: Optional[Union[types.HnswConfigDiff, dict]] = None,
-        optimizers_config: Optional[types.OptimizersConfigDiff] = None,
-        wal_config: Optional[types.WalConfigDiff] = None,
-        quantization_config: Optional[types.QuantizationConfig] = None,
-        init_from: Optional[types.InitFrom] = None,
-        **kwargs,
+        hnsw_config: Optional[dict] = None,
+        optimizers_config: Optional[dict] = None,
+        wal_config: Optional[dict] = None,
+        quantization_config: Optional[dict] = None,
+        init_from: Optional[dict] = None,
     ):
         super().__init__()
 
         self.client = qdrant_client.QdrantClient(
             location=location,
             url=url,
             port=port,
@@ -80,15 +78,14 @@
             prefer_grpc=prefer_grpc,
             https=https,
             api_key=api_key,
             prefix=prefix,
             timeout=timeout,
             host=host,
             path=path,
-            **kwargs,
         )
 
         # Store the Qdrant specific attributes
         self.shard_number = shard_number
         self.replication_factor = replication_factor
         self.write_consistency_factor = write_consistency_factor
         self.on_disk_payload = on_disk_payload
```

### Comparing `qdrant_haystack-1.0.2/PKG-INFO` & `qdrant_haystack-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-haystack
-Version: 1.0.2
+Version: 1.0.3
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

