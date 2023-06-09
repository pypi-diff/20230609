# Comparing `tmp/bullmq-0.5.0.tar.gz` & `tmp/bullmq-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.5.0.tar", last modified: Fri Jun  9 05:20:47 2023, max compression
+gzip compressed data, was "bullmq-0.5.1.tar", last modified: Fri Jun  9 16:05:39 2023, max compression
```

## Comparing `bullmq-0.5.0.tar` & `bullmq-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 05:20:47.313710 bullmq-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-09 05:19:54.000000 bullmq-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-09 05:20:45.000000 bullmq-0.5.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/backoffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 05:20:47.313710 bullmq-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 05:19:54.000000 bullmq-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.595871 bullmq-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 16:05:39.595871 bullmq-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-09 16:04:15.000000 bullmq-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.587871 bullmq-0.5.1/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-09 16:05:37.000000 bullmq-0.5.1/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.595871 bullmq-0.5.1/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/changePriority-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getState-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/pause-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/promote-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.595871 bullmq-0.5.1/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.591871 bullmq-0.5.1/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 16:05:39.599871 bullmq-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 16:04:15.000000 bullmq-0.5.1/setup.py
```

### Comparing `bullmq-0.5.0/PKG-INFO` & `bullmq-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.0
+Version: 0.5.1
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.0/README.md` & `bullmq-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/backoffs.py` & `bullmq-0.5.1/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/event_emitter.py` & `bullmq-0.5.1/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/job.py` & `bullmq-0.5.1/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/queue.py` & `bullmq-0.5.1/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/redis_connection.py` & `bullmq-0.5.1/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/scripts.py` & `bullmq-0.5.1/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/timer.py` & `bullmq-0.5.1/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/types/job_options.py` & `bullmq-0.5.1/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/types/worker_options.py` & `bullmq-0.5.1/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq/worker.py` & `bullmq-0.5.1/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.0/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.1/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.0
+Version: 0.5.1
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.0/setup.py` & `bullmq-0.5.1/setup.py`

 * *Files identical despite different names*

