# Comparing `tmp/bullmq-0.4.3.tar.gz` & `tmp/bullmq-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.4.3.tar", last modified: Wed Jun  7 09:21:39 2023, max compression
+gzip compressed data, was "bullmq-0.5.0.tar", last modified: Fri Jun  9 05:20:47 2023, max compression
```

## Comparing `bullmq-0.4.3.tar` & `bullmq-0.5.0.tar`

### file list

```diff
@@ -1,61 +1,31 @@
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.733139 bullmq-0.4.3/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-07 09:21:39.732783 bullmq-0.4.3/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.3/README.md
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.705716 bullmq-0.4.3/bullmq/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/backoffs.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.729548 bullmq-0.4.3/bullmq/commands/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/addJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/drain-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getState-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveJobFromActiveToWait-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/pause-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/promote-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/reprocessJob-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/takeLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/updateData-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.3/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.3/bullmq/error_code.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.3/bullmq/event_emitter.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7488 2023-06-06 19:07:05.000000 bullmq-0.4.3/bullmq/job.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4847 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/queue.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1356 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/redis_connection.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    16376 2023-06-06 19:07:05.000000 bullmq-0.4.3/bullmq/scripts.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.3/bullmq/timer.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.732302 bullmq-0.4.3/bullmq/types/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      314 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      207 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/backoff_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1920 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/job_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      395 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/keep_jobs.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      189 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/queue_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      129 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/retry_job_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1190 2023-05-04 10:32:52.000000 bullmq-0.4.3/bullmq/types/worker_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      144 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/utils.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7490 2023-05-29 08:02:35.000000 bullmq-0.4.3/bullmq/worker.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-07 09:21:39.707876 bullmq-0.4.3/bullmq.egg-info/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1574 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       21 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/requires.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-06-07 09:21:39.000000 bullmq-0.4.3/bullmq.egg-info/top_level.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-06-07 09:21:39.733258 bullmq-0.4.3/setup.cfg
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1177 2023-06-07 09:15:53.000000 bullmq-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 05:20:47.313710 bullmq-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-09 05:19:54.000000 bullmq-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-09 05:20:45.000000 bullmq-0.5.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/backoffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-09 05:19:54.000000 bullmq-0.5.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:20:47.313710 bullmq-0.5.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 05:20:47.000000 bullmq-0.5.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 05:20:47.313710 bullmq-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 05:19:54.000000 bullmq-0.5.0/setup.py
```

### Comparing `bullmq-0.4.3/PKG-INFO` & `bullmq-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.3
+Version: 0.5.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # BullMQ For Python
 
 This is the official BullMQ Python library. It is a close port of the NodeJS version of the library.
 Python Queues are interoperable with NodeJS Queues, as both libraries use the same .lua scripts that
 power all the functionality.
```

### Comparing `bullmq-0.4.3/README.md` & `bullmq-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/backoffs.py` & `bullmq-0.5.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/event_emitter.py` & `bullmq-0.5.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/job.py` & `bullmq-0.5.0/bullmq/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,20 @@
     def changePriority(self, opts: dict):
         return self.scripts.changePriority(self.id, opts.get("priority", 0), opts.get("lifo", False))
 
     def updateProgress(self, progress):
         self.progress = progress
         return self.scripts.updateProgress(self.id, progress)
 
+    async def remove(self):
+        removed = await self.scripts.remove(self.id)
+        
+        if not removed:
+            raise Exception(f"Could not remove job {self.id}")
+
     async def moveToFailed(self, err, token:str, fetchNext:bool = False):
         error_message = str(err)
         self.failedReason = error_message
 
         move_to_failed = False
         finished_on = 0
         command = 'moveToFailed'
```

### Comparing `bullmq-0.4.3/bullmq/queue.py` & `bullmq-0.5.0/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/redis_connection.py` & `bullmq-0.5.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/scripts.py` & `bullmq-0.5.0/bullmq/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,20 +32,21 @@
         self.commands = {
             "addJob": self.redisClient.register_script(self.getScript("addJob-8.lua")),
             "changePriority": self.redisClient.register_script(self.getScript("changePriority-4.lua")),
             "extendLock": self.redisClient.register_script(self.getScript("extendLock-2.lua")),
             "getCounts": self.redisClient.register_script(self.getScript("getCounts-1.lua")),
             "getState": self.redisClient.register_script(self.getScript("getState-7.lua")),
             "getStateV2": self.redisClient.register_script(self.getScript("getStateV2-7.lua")),
+            "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
             "moveToActive": self.redisClient.register_script(self.getScript("moveToActive-9.lua")),
             "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
             "moveToFinished": self.redisClient.register_script(self.getScript("moveToFinished-12.lua")),
-            "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
             "obliterate": self.redisClient.register_script(self.getScript("obliterate-2.lua")),
             "pause": self.redisClient.register_script(self.getScript("pause-4.lua")),
+            "removeJob": self.redisClient.register_script(self.getScript("removeJob-1.lua")),
             "reprocessJob": self.redisClient.register_script(self.getScript("reprocessJob-6.lua")),
             "retryJob": self.redisClient.register_script(self.getScript("retryJob-8.lua")),
             "retryJobs": self.redisClient.register_script(self.getScript("retryJobs-6.lua")),
             "saveStacktrace": self.redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
             "updateData": self.redisClient.register_script(self.getScript("updateData-1.lua")),
             "updateProgress": self.redisClient.register_script(self.getScript("updateProgress-2.lua")),
         }
@@ -143,14 +144,20 @@
         result = await self.commands["moveToDelayed"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
                 raise self.finishedErrors(result, job_id, 'moveToDelayed', 'active')
         return None
 
+    async def remove(self, job_id: str):
+        keys = self.getKeys([''])
+        args = [job_id]
+
+        return self.commands["removeJob"](keys=keys, args=args)
+
     def getCounts(self, types):
         keys = self.getKeys([''])
         transformed_types = list(
             map(lambda type: 'wait' if type == 'waiting' else type, types))
 
         return self.commands["getCounts"](keys=keys, args=transformed_types)
```

### Comparing `bullmq-0.4.3/bullmq/timer.py` & `bullmq-0.5.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/types/job_options.py` & `bullmq-0.5.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/types/worker_options.py` & `bullmq-0.5.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq/worker.py` & `bullmq-0.5.0/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.3/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.0/bullmq.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.3
+Version: 0.5.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # BullMQ For Python
 
 This is the official BullMQ Python library. It is a close port of the NodeJS version of the library.
 Python Queues are interoperable with NodeJS Queues, as both libraries use the same .lua scripts that
 power all the functionality.
```

