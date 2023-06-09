# Comparing `tmp/pix_framework-0.8.8.tar.gz` & `tmp/pix_framework-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.8.8.tar", max compression
+gzip compressed data, was "pix_framework-0.8.9.tar", max compression
```

## Comparing `pix_framework-0.8.8.tar` & `pix_framework-0.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-05-24 12:57:32.450202 pix_framework-0.8.8/LICENSE
--rw-r--r--   0        0        0      549 2023-05-24 12:57:32.450202 pix_framework-0.8.8/README.md
--rw-r--r--   0        0        0      799 2023-05-24 12:57:32.450202 pix_framework-0.8.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0     7524 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/calendar/availability.py
--rw-r--r--   0        0        0    31886 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0        0 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/discovery/__init__.py
--rw-r--r--   0        0        0     5835 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/discovery/calendar_factory.py
--rw-r--r--   0        0        0     6967 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/discovery/case_arrival.py
--rw-r--r--   0        0        0     4903 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/discovery/gateway_probabilities.py
--rw-r--r--   0        0        0     5621 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/discovery/resource_pools.py
--rw-r--r--   0        0        0        0 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/input.py
--rw-r--r--   0        0        0        0 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/io/__init__.py
--rw-r--r--   0        0        0    38326 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/io/bpm_graph.py
--rw-r--r--   0        0        0     2058 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-24 12:57:32.450202 pix_framework-0.8.8/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-24 12:57:32.454201 pix_framework-0.8.8/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-05-24 12:57:32.454201 pix_framework-0.8.8/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 pix_framework-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 15:10:45.934945 pix_framework-0.8.9/LICENSE
+-rw-r--r--   0        0        0      549 2023-06-08 15:10:45.934945 pix_framework-0.8.9/README.md
+-rw-r--r--   0        0        0      799 2023-06-08 15:10:45.934945 pix_framework-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0     7524 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/calendar/availability.py
+-rw-r--r--   0        0        0    31886 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     5835 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/calendar_factory.py
+-rw-r--r--   0        0        0     6967 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/case_arrival.py
+-rw-r--r--   0        0        0     4903 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0     5621 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/resource_pools.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    38326 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2284 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 pix_framework-0.8.9/PKG-INFO
```

### Comparing `pix_framework-0.8.8/LICENSE` & `pix_framework-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/README.md` & `pix_framework-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/pyproject.toml` & `pix_framework-0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.8.8"
+version = "0.8.9"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = [
     "David Chapela de la Campa <david.chapela.delacampa@gmail.com>",
     "Ihar Suvorau <ihar.suvorau@gmail.com>",
 ]
 readme = "README.md"
 packages = [{ include = "pix_framework", from = "src" }]
```

### Comparing `pix_framework-0.8.8/src/pix_framework/calendar/availability.py` & `pix_framework-0.8.9/src/pix_framework/calendar/availability.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/calendar/resource_calendar.py` & `pix_framework-0.8.9/src/pix_framework/calendar/resource_calendar.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/discovery/calendar_factory.py` & `pix_framework-0.8.9/src/pix_framework/discovery/calendar_factory.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/discovery/case_arrival.py` & `pix_framework-0.8.9/src/pix_framework/discovery/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/discovery/gateway_probabilities.py` & `pix_framework-0.8.9/src/pix_framework/discovery/gateway_probabilities.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/discovery/resource_pools.py` & `pix_framework-0.8.9/src/pix_framework/discovery/resource_pools.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.8.9/src/pix_framework/enhancement/multitasking.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.8.9/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/input.py` & `pix_framework-0.8.9/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/io/bpm_graph.py` & `pix_framework-0.8.9/src/pix_framework/io/bpm_graph.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/log_ids.py` & `pix_framework-0.8.9/src/pix_framework/log_ids.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     enabling_activity: str = (
         "enabling_activity"  # Label of the activity instance enabling the current one
     )
     available_time: str = "available_time"  # Last availability time of the resource who performed this activity instance
     estimated_start_time: str = (
         "estimated_start_time"  # Estimated start time of the activity instance
     )
+    batch_id: str = "batch_instance_id"  # ID of the batch instance this activity instance belongs to, if any
+    batch_type: str = "batch_instance_type"  # Type of the batch instance this activity instance belongs to, if any
 
     @staticmethod
     def from_dict(config: dict) -> "EventLogIDs":
         return EventLogIDs(**config)
 
     def to_dict(self) -> dict:
         return {attr.name: getattr(self, attr.name) for attr in fields(self.__class__)}
```

### Comparing `pix_framework-0.8.8/src/pix_framework/log_split/log_split.py` & `pix_framework-0.8.9/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/statistics/distribution.py` & `pix_framework-0.8.9/src/pix_framework/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/src/pix_framework/statistics/utils.py` & `pix_framework-0.8.9/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.8/PKG-INFO` & `pix_framework-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.8.8
+Version: 0.8.9
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

