# Comparing `tmp/task_processing-0.9.0.tar.gz` & `tmp/task_processing-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/task_processing-0.9.0.tar", last modified: Mon Aug 15 17:04:10 2022, max compression
+gzip compressed data, was "dist/task_processing-0.9.1.tar", last modified: Tue Aug 16 00:54:37 2022, max compression
```

## Comparing `task_processing-0.9.0.tar` & `task_processing-0.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-15 17:04:10.000000 task_processing-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-15 17:04:10.000000 task_processing-0.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/runners/
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/runners/promise.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/runners/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/runners/async_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/runners/subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/task_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/plugins/mesos/
--rw-r--r--   0 runner    (1001) docker     (121)     5349 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/translator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5540 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/retrying_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/mesos_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    26780 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/execution_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     8931 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/logging_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/mesos_task_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/timeout_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4908 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/task_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/mesos_pod_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/mesos/resource_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/plugins/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/persistence/file_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/persistence/dynamodb_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13074 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/task_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/kube_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    26592 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/kubernetes_pod_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8912 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/plugins/stateful/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/stateful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/plugins/stateful/stateful_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/interfaces/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/interfaces/task_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/interfaces/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/interfaces/event.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-08-15 17:03:52.000000 task_processing-0.9.0/task_processing/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-15 17:03:52.000000 task_processing-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-08-15 17:03:52.000000 task_processing-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-15 17:04:10.000000 task_processing-0.9.0/task_processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-08-15 17:03:52.000000 task_processing-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-16 00:54:37.000000 task_processing-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-16 00:54:37.000000 task_processing-0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/runners/
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/promise.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/async_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/task_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/mesos/
+-rw-r--r--   0 runner    (1001) docker     (121)     5349 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5540 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/retrying_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/mesos_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26780 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/execution_framework.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8931 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/logging_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/mesos_task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/timeout_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4908 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/task_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/mesos_pod_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/resource_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/persistence/
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/persistence/file_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/persistence/dynamodb_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/persistence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13074 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/task_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/kube_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27449 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/kubernetes_pod_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8912 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/stateful/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/stateful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/stateful/stateful_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-16 00:54:17.000000 task_processing-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-08-16 00:54:17.000000 task_processing-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-08-16 00:54:17.000000 task_processing-0.9.1/README.md
```

### Comparing `task_processing-0.9.0/task_processing/runners/promise.py` & `task_processing-0.9.1/task_processing/runners/promise.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/runners/sync.py` & `task_processing-0.9.1/task_processing/runners/sync.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/runners/async_runner.py` & `task_processing-0.9.1/task_processing/runners/async_runner.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/runners/subscription.py` & `task_processing-0.9.1/task_processing/runners/subscription.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/task_processor.py` & `task_processing-0.9.1/task_processing/task_processor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/translator.py` & `task_processing-0.9.1/task_processing/plugins/mesos/translator.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/retrying_executor.py` & `task_processing-0.9.1/task_processing/plugins/mesos/retrying_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/constraints.py` & `task_processing-0.9.1/task_processing/plugins/mesos/constraints.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/mesos_executor.py` & `task_processing-0.9.1/task_processing/plugins/mesos/mesos_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/execution_framework.py` & `task_processing-0.9.1/task_processing/plugins/mesos/execution_framework.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/logging_executor.py` & `task_processing-0.9.1/task_processing/plugins/mesos/logging_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/mesos_task_executor.py` & `task_processing-0.9.1/task_processing/plugins/mesos/mesos_task_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/timeout_executor.py` & `task_processing-0.9.1/task_processing/plugins/mesos/timeout_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/__init__.py` & `task_processing-0.9.1/task_processing/plugins/mesos/__init__.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/task_config.py` & `task_processing-0.9.1/task_processing/plugins/mesos/task_config.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/metrics.py` & `task_processing-0.9.1/task_processing/plugins/mesos/metrics.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/mesos/resource_helpers.py` & `task_processing-0.9.1/task_processing/plugins/mesos/resource_helpers.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/persistence/file_persistence.py` & `task_processing-0.9.1/task_processing/plugins/persistence/file_persistence.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/persistence/dynamodb_persistence.py` & `task_processing-0.9.1/task_processing/plugins/persistence/dynamodb_persistence.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/kubernetes/task_metadata.py` & `task_processing-0.9.1/task_processing/plugins/kubernetes/task_metadata.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/kubernetes/task_config.py` & `task_processing-0.9.1/task_processing/plugins/kubernetes/task_config.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/kubernetes/types.py` & `task_processing-0.9.1/task_processing/plugins/kubernetes/types.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/kubernetes/kube_client.py` & `task_processing-0.9.1/task_processing/plugins/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/kubernetes/kubernetes_pod_executor.py` & `task_processing-0.9.1/task_processing/plugins/kubernetes/kubernetes_pod_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,28 @@
 
     def __init__(
         self,
         namespace: str,
         version: Optional[str] = None,
         kubeconfig_path: Optional[str] = None,
         task_configs: Optional[Collection[KubernetesTaskConfig]] = [],
+        emit_events_without_state_transitions: bool = False,
+
     ) -> None:
         if not version:
             version = "unknown_task_processing"
         user_agent = f"{namespace}/v{version}"
         self.kube_client = KubeClient(kubeconfig_path=kubeconfig_path, user_agent=user_agent)
         self.namespace = namespace
+
+        # Pod modified events that did not result in a pod state transition are usually not
+        # forwarded, but some consumers are interested in container state changes. This
+        # variable controls whether such additional pod modified events are forwarded.
+        self.emit_events_without_state_transitions = emit_events_without_state_transitions
+
         self.stopping = False
         self.task_metadata: PMap[str, KubernetesTaskMetadata] = pmap()
 
         self.task_metadata_lock = threading.RLock()
         if task_configs:
             for task_config in task_configs:
                 self._initialize_existing_task(task_config)
@@ -327,18 +335,30 @@
                     raw=raw_event,
                     task_config=task_metadata.task_config,
                     platform_type="lost"
                 )
             )
             return
 
-        logger.info(
-            f"Ignoring MODIFIED event for {pod_name} as it did not result "
-            "in a state transition",
-        )
+        if self.emit_events_without_state_transitions:
+            self.event_queue.put(
+                task_event(
+                    task_id=pod_name,
+                    terminal=False,
+                    timestamp=time.time(),
+                    raw=raw_event,
+                    task_config=task_metadata.task_config,
+                    platform_type="running",
+                )
+            )
+        else:
+            logger.info(
+                f"Ignoring MODIFIED event for {pod_name} as it did not result "
+                "in a state transition",
+            )
 
     def _process_pod_event(self, event: PodEvent) -> None:
         """
         Router for handling Pod events based on event type. Currently, we only look at
         MODIFIED and DELETED events (we ignore ADDED since we handle all processing for
         those when we create Pods in the first place).
```

### Comparing `task_processing-0.9.0/task_processing/plugins/kubernetes/utils.py` & `task_processing-0.9.1/task_processing/plugins/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/plugins/stateful/stateful_executor.py` & `task_processing-0.9.1/task_processing/plugins/stateful/stateful_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/interfaces/task_executor.py` & `task_processing-0.9.1/task_processing/interfaces/task_executor.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/interfaces/runner.py` & `task_processing-0.9.1/task_processing/interfaces/runner.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/interfaces/event.py` & `task_processing-0.9.1/task_processing/interfaces/event.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/metrics.py` & `task_processing-0.9.1/task_processing/metrics.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing/utils.py` & `task_processing-0.9.1/task_processing/utils.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/LICENSE` & `task_processing-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/setup.py` & `task_processing-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/task_processing.egg-info/SOURCES.txt` & `task_processing-0.9.1/task_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.0/README.md` & `task_processing-0.9.1/README.md`

 * *Files identical despite different names*

