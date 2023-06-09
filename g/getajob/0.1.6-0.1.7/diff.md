# Comparing `tmp/getajob-0.1.6.tar.gz` & `tmp/getajob-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.1.6.tar", max compression
+gzip compressed data, was "getajob-0.1.7.tar", max compression
```

## Comparing `getajob-0.1.6.tar` & `getajob-0.1.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       69 2023-06-09 15:47:55.359871 getajob-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/abstractions/models.py
--rw-r--r--   0        0        0     6843 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     3138 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/auth.py
--rw-r--r--   0        0        0     1341 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/__init__.py
--rw-r--r--   0        0        0      170 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      574 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0      737 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      447 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0      823 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0     1530 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     4340 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     5814 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0     1140 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0     1084 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0     1416 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/companies/unit_of_work.py
--rw-r--r--   0        0        0     3135 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1040 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0      799 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/notifications/models.py
--rw-r--r--   0        0        0      537 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/notifications/repository.py
--rw-r--r--   0        0        0      761 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/recruiters/models.py
--rw-r--r--   0        0        0      446 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/recruiters/repository.py
--rw-r--r--   0        0        0     1332 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0     1123 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/clerk_webhook/models.py
--rw-r--r--   0        0        0      843 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/clerk_webhook/repository.py
--rw-r--r--   0        0        0      409 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      345 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0      313 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      334 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0      306 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0      523 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      337 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0      726 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/users/models.py
--rw-r--r--   0        0        0      715 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/contexts/users/users/repository.py
--rw-r--r--   0        0        0     1794 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/models/__init__.py
--rw-r--r--   0        0        0      373 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/models/entities.py
--rw-r--r--   0        0        0      240 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/models/location.py
--rw-r--r--   0        0        0      375 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/utils.py
--rw-r--r--   0        0        0     2527 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/algolia.py
--rw-r--r--   0        0        0     4456 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/clerk.py
--rw-r--r--   0        0        0    10429 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/firebase.py
--rw-r--r--   0        0        0      709 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1303 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      179 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1625 2023-06-09 15:47:55.359871 getajob-0.1.6/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      585 2023-06-09 15:47:55.363872 getajob-0.1.6/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1998 2023-06-09 15:47:55.363872 getajob-0.1.6/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-09 15:47:55.363872 getajob-0.1.6/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      207 2023-06-09 15:47:55.363872 getajob-0.1.6/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1725 2023-06-09 15:47:55.363872 getajob-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 getajob-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-06-09 17:44:52.002529 getajob-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     7004 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     3138 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/auth.py
+-rw-r--r--   0        0        0     1341 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      574 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0      737 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      447 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0      823 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0     1530 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     4340 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     5814 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0     1140 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0     1084 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0     1416 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/companies/unit_of_work.py
+-rw-r--r--   0        0        0     3149 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1040 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      799 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/notifications/models.py
+-rw-r--r--   0        0        0      537 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/notifications/repository.py
+-rw-r--r--   0        0        0      761 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/recruiters/models.py
+-rw-r--r--   0        0        0      446 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/recruiters/repository.py
+-rw-r--r--   0        0        0     1332 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0     1123 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/clerk_webhook/models.py
+-rw-r--r--   0        0        0      843 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/clerk_webhook/repository.py
+-rw-r--r--   0        0        0      409 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      345 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0      313 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      334 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0      306 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0      523 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      337 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0      726 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/users/models.py
+-rw-r--r--   0        0        0      715 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/contexts/users/users/repository.py
+-rw-r--r--   0        0        0     1794 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/models/__init__.py
+-rw-r--r--   0        0        0      373 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/models/entities.py
+-rw-r--r--   0        0        0      240 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/models/location.py
+-rw-r--r--   0        0        0      375 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/utils.py
+-rw-r--r--   0        0        0     2527 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/algolia.py
+-rw-r--r--   0        0        0     4456 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/clerk.py
+-rw-r--r--   0        0        0    10429 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0      709 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1303 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      179 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1334 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      585 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1998 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      207 2023-06-09 17:44:52.002529 getajob-0.1.7/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1725 2023-06-09 17:44:52.006529 getajob-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 getajob-0.1.7/PKG-INFO
```

### Comparing `getajob-0.1.6/getajob/abstractions/models.py` & `getajob-0.1.7/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/abstractions/repository.py` & `getajob-0.1.7/getajob/abstractions/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     FirestoreDB,
 )
 from getajob.vendor.kafka.repository import KafkaRepository
 from getajob.vendor.kafka.models import (
     KafkaEventConfig,
     KafkaEventType,
     BaseKafkaMessage,
-    KafkaDeleteEvent,
 )
 from .models import EntityModels, PaginatedResponse
 
 
 def format_to_schema(document: FirestoreDocument, entity_model: BaseModel) -> BaseModel:
     id_included_dict = {
         "id": document.id,
@@ -96,37 +95,40 @@
         self.kafka_event_config = kafka_event_config
 
         # If kafka given but no configuration, complain about it
         if self.kafka and not self.kafka_event_config:
             raise ValueError("Kafka event topic must be provided")
 
     def _produce_repository_kafka_event(
-        self, event_type: KafkaEventType, data: BaseModel
+        self, event_type: KafkaEventType, object_id: str, data: BaseModel = None
     ):
         if (
             not self.kafka
             or not self.kafka_event_config
             or not self.kafka_event_config.dict()[event_type]
         ):
             return
         self.kafka.publish(
             topic=self.kafka_event_config.topic,
             message=BaseKafkaMessage(
                 message_type=f"{event_type.value}_{self.collection_name}",
-                data=data.dict(),
+                object_id=object_id,
+                data=data.dict() if data else None,
             ),
         )
 
     def get(
         self,
         doc_id: str,
         parent_collections: dict = {},
     ) -> BaseModel:
         res = self.db.get(parent_collections, self.collection_name, doc_id)
-        self._produce_repository_kafka_event(event_type=KafkaEventType.get, data=res)
+        self._produce_repository_kafka_event(
+            event_type=KafkaEventType.get, object_id=doc_id
+        )
         return format_to_schema(res, self.entity_models.entity)
 
     def get_with_filters(
         self,
         doc_id: str,
         filters: t.List[FirestoreFilters],
         parent_collections: dict = {},
@@ -148,15 +150,17 @@
         document_id = provided_id or generate_random_short_code()
         res = self.db.create(
             parent_collections=parent_collections,
             collection_name=self.collection_name,
             document_id=document_id,
             document_data=data_dict,
         )
-        self._produce_repository_kafka_event(event_type=KafkaEventType.create, data=res)
+        self._produce_repository_kafka_event(
+            event_type=KafkaEventType.create, object_id=res.id
+        )
         return format_to_schema(res, self.entity_models.entity)
 
     def update(
         self,
         doc_id: str,
         data: BaseModel,
         parent_collections: dict = {},
@@ -165,25 +169,27 @@
         for key, val in data.dict().items():
             if val is not None:
                 original_item[key] = val
         original_item["updated"] = datetime.now()
         res = self.db.update(
             parent_collections, self.collection_name, doc_id, original_item
         )
-        self._produce_repository_kafka_event(event_type=KafkaEventType.update, data=res)
+        self._produce_repository_kafka_event(
+            event_type=KafkaEventType.update, object_id=doc_id
+        )
         return format_to_schema(res, self.entity_models.entity)
 
     def delete(
         self,
         doc_id: str,
         parent_collections: dict = {},
     ) -> bool:
-        assert self.get(doc_id, parent_collections)
+        deleted_object = self.get(doc_id, parent_collections)
         self._produce_repository_kafka_event(
-            event_type=KafkaEventType.delete, data=KafkaDeleteEvent(id=doc_id)
+            event_type=KafkaEventType.delete, object_id=doc_id, data=deleted_object
         )
         return self.db.delete(parent_collections, self.collection_name, doc_id)
 
     def get_one_by_attribute(
         self,
         attribute: str,
         value: t.Any,
```

### Comparing `getajob-0.1.6/getajob/auth.py` & `getajob-0.1.7/getajob/auth.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/config/settings.py` & `getajob-0.1.7/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/admin/search/repository.py` & `getajob-0.1.7/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/admin/users/models.py` & `getajob-0.1.7/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/ai/text/models.py` & `getajob-0.1.7/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/ai/text/repository.py` & `getajob-0.1.7/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/applications/models.py` & `getajob-0.1.7/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/applications/repository.py` & `getajob-0.1.7/getajob/contexts/applications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/applications/unit_of_work.py` & `getajob-0.1.7/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/companies/models.py` & `getajob-0.1.7/getajob/contexts/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/companies/repository.py` & `getajob-0.1.7/getajob/contexts/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/companies/unit_of_work.py` & `getajob-0.1.7/getajob/contexts/companies/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/jobs/models.py` & `getajob-0.1.7/getajob/contexts/jobs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,16 @@
     benefits: t.Optional[t.List[str]] = None
     background_check_required: t.Optional[bool] = None
     drug_test_required: t.Optional[bool] = None
     felons_accepted: t.Optional[bool] = None
     disability_accepted: t.Optional[bool] = None
 
     ideal_days_to_hire: t.Optional[int] = None
-    internal_reference_code: t.Optional[str]
-    job_associated_company_description: t.Optional[str]
+    internal_reference_code: t.Optional[str] = None
+    job_associated_company_description: t.Optional[str] = None
 
 
 class InternalUpdateJob(UpdateJob):
     position_filled: t.Optional[bool] = None
     view_count: t.Optional[int] = None
```

### Comparing `getajob-0.1.6/getajob/contexts/jobs/repository.py` & `getajob-0.1.7/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/notifications/models.py` & `getajob-0.1.7/getajob/contexts/notifications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/notifications/repository.py` & `getajob-0.1.7/getajob/contexts/notifications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/recruiters/models.py` & `getajob-0.1.7/getajob/contexts/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/static/repository.py` & `getajob-0.1.7/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/users/clerk_webhook/models.py` & `getajob-0.1.7/getajob/contexts/users/clerk_webhook/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/users/clerk_webhook/repository.py` & `getajob-0.1.7/getajob/contexts/users/clerk_webhook/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/users/skills/models.py` & `getajob-0.1.7/getajob/contexts/users/skills/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/users/users/models.py` & `getajob-0.1.7/getajob/contexts/users/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/contexts/users/users/repository.py` & `getajob-0.1.7/getajob/contexts/users/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/exceptions.py` & `getajob-0.1.7/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/algolia.py` & `getajob-0.1.7/getajob/vendor/algolia.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/clerk.py` & `getajob-0.1.7/getajob/vendor/clerk.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/firebase.py` & `getajob-0.1.7/getajob/vendor/firebase.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/kafka/authentication.py` & `getajob-0.1.7/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/kafka/kafka.py` & `getajob-0.1.7/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/kafka/models.py` & `getajob-0.1.7/getajob/vendor/kafka/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,43 +34,26 @@
 class KafkaEventType(str, Enum):
     create = "create"
     update = "update"
     delete = "delete"
     get = "get"
 
 
-class KafkaDeleteEvent(BaseModel):
-    id: str
-
-
 class BaseKafkaMessage(BaseModel):
-    data: dict
+    object_id: str
     message_type: str
     message_time: datetime = datetime.now()
-
-
-class KafkaNotificationsEnum(str, Enum):
-    ...
-
-
-class KafkaCommunicationsEnum(str, Enum):
-    ...
+    data: dict = None
 
 
 class KafkaJobsEnum(str, Enum):
     create_jobs = "create_jobs"
     update_jobs = "update_jobs"
     delete_jobs = "delete_jobs"
     get_jobs = "get_jobs"
 
 
-class KafkaCompaniesEnum(str, Enum):
-    create_companies = "create_companies"
-    update_companies = "update_companies"
-    delete_companies = "delete_companies"
-
-
 class KafkaApplicationsEnum(str, Enum):
     create_applications = "create_applications"
     update_applications = "update_applications"
     delete_applications = "delete_applications"
     get_applications = "get_applications"
```

### Comparing `getajob-0.1.6/getajob/vendor/kafka/repository.py` & `getajob-0.1.7/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/openai.py` & `getajob-0.1.7/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.1.7/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.6/pyproject.toml` & `getajob-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.1.6/PKG-INFO` & `getajob-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (==3.8.4)
```

