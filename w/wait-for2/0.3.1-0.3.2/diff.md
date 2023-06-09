# Comparing `tmp/wait_for2-0.3.1.tar.gz` & `tmp/wait_for2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wait_for2-0.3.1.tar", last modified: Mon Dec 20 10:55:32 2021, max compression
+gzip compressed data, was "wait_for2-0.3.2.tar", last modified: Fri Jun  9 11:05:18 2023, max compression
```

## Comparing `wait_for2-0.3.1.tar` & `wait_for2-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2021-12-20 10:55:32.083172 wait_for2-0.3.1/
--rw-r--r--   0 nandor    (1000) nandor    (1000)      463 2021-12-20 10:49:10.000000 wait_for2-0.3.1/CHANGELOG.md
--rw-r--r--   0 nandor    (1000) nandor    (1000)    10174 2021-01-13 10:57:08.000000 wait_for2-0.3.1/LICENSE
--rw-r--r--   0 nandor    (1000) nandor    (1000)      116 2021-05-14 19:46:35.000000 wait_for2-0.3.1/MANIFEST.in
--rw-r--r--   0 nandor    (1000) nandor    (1000)       46 2021-03-04 08:59:07.000000 wait_for2-0.3.1/NOTICE
--rw-r--r--   0 nandor    (1000) nandor    (1000)     3882 2021-12-20 10:55:32.083172 wait_for2-0.3.1/PKG-INFO
--rw-r--r--   0 nandor    (1000) nandor    (1000)     2996 2021-12-20 10:40:47.000000 wait_for2-0.3.1/README.md
--rw-r--r--   0 nandor    (1000) nandor    (1000)       38 2021-12-20 10:55:32.083172 wait_for2-0.3.1/setup.cfg
--rw-r--r--   0 nandor    (1000) nandor    (1000)     1545 2021-12-20 10:48:30.000000 wait_for2-0.3.1/setup.py
-drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2021-12-20 10:55:32.082172 wait_for2-0.3.1/tests/
--rw-r--r--   0 nandor    (1000) nandor    (1000)        0 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/__init__.py
-drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2021-12-20 10:55:32.082172 wait_for2-0.3.1/tests/common/
--rw-r--r--   0 nandor    (1000) nandor    (1000)        0 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/common/__init__.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)      389 2021-12-20 10:48:15.000000 wait_for2-0.3.1/tests/common/constants.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)     3520 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/common/inner_bind.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)     6493 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/common/resource.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)     1818 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/test_inner_bind.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)      749 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/test_no_wait_result.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)     1610 2021-12-19 18:08:37.000000 wait_for2-0.3.1/tests/test_resource.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)     3953 2021-12-20 10:41:09.000000 wait_for2-0.3.1/tests/test_result_after_cancel.py
-drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2021-12-20 10:55:32.082172 wait_for2-0.3.1/wait_for2/
--rw-r--r--   0 nandor    (1000) nandor    (1000)      402 2021-12-20 10:52:21.000000 wait_for2-0.3.1/wait_for2/__init__.py
--rw-r--r--   0 nandor    (1000) nandor    (1000)     7422 2021-12-19 18:08:37.000000 wait_for2-0.3.1/wait_for2/impl.py
-drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2021-12-20 10:55:32.083172 wait_for2-0.3.1/wait_for2.egg-info/
--rw-r--r--   0 nandor    (1000) nandor    (1000)     3882 2021-12-20 10:55:31.000000 wait_for2-0.3.1/wait_for2.egg-info/PKG-INFO
--rw-r--r--   0 nandor    (1000) nandor    (1000)      462 2021-12-20 10:55:31.000000 wait_for2-0.3.1/wait_for2.egg-info/SOURCES.txt
--rw-r--r--   0 nandor    (1000) nandor    (1000)        1 2021-12-20 10:55:31.000000 wait_for2-0.3.1/wait_for2.egg-info/dependency_links.txt
--rw-r--r--   0 nandor    (1000) nandor    (1000)       10 2021-12-20 10:55:31.000000 wait_for2-0.3.1/wait_for2.egg-info/top_level.txt
+drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2023-06-09 11:05:18.602473 wait_for2-0.3.2/
+-rw-r--r--   0 nandor    (1000) nandor    (1000)      463 2021-12-20 10:49:10.000000 wait_for2-0.3.2/CHANGELOG.md
+-rw-r--r--   0 nandor    (1000) nandor    (1000)    10174 2021-01-13 10:57:08.000000 wait_for2-0.3.2/LICENSE
+-rw-r--r--   0 nandor    (1000) nandor    (1000)      116 2021-05-14 19:46:35.000000 wait_for2-0.3.2/MANIFEST.in
+-rw-r--r--   0 nandor    (1000) nandor    (1000)       46 2021-03-04 08:59:07.000000 wait_for2-0.3.2/NOTICE
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     7493 2023-06-09 11:05:18.602473 wait_for2-0.3.2/PKG-INFO
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     6505 2023-06-09 10:54:55.000000 wait_for2-0.3.2/README.md
+-rw-r--r--   0 nandor    (1000) nandor    (1000)       38 2023-06-09 11:05:18.602473 wait_for2-0.3.2/setup.cfg
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     1645 2023-06-09 10:01:44.000000 wait_for2-0.3.2/setup.py
+drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2023-06-09 11:05:18.599140 wait_for2-0.3.2/tests/
+-rw-r--r--   0 nandor    (1000) nandor    (1000)        0 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/__init__.py
+drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2023-06-09 11:05:18.599140 wait_for2-0.3.2/tests/common/
+-rw-r--r--   0 nandor    (1000) nandor    (1000)        0 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/common/__init__.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)      367 2023-06-09 09:53:44.000000 wait_for2-0.3.2/tests/common/constants.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     3520 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/common/inner_bind.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     6493 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/common/resource.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     1818 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/test_inner_bind.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     2714 2021-12-26 08:58:07.000000 wait_for2-0.3.2/tests/test_lost_cancellation.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)      749 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/test_no_wait_result.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     1610 2021-12-19 18:08:37.000000 wait_for2-0.3.2/tests/test_resource.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     4464 2023-05-24 14:08:23.000000 wait_for2-0.3.2/tests/test_result_after_cancel.py
+drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2023-06-09 11:05:18.599140 wait_for2-0.3.2/wait_for2/
+-rw-r--r--   0 nandor    (1000) nandor    (1000)      402 2023-06-09 11:03:33.000000 wait_for2-0.3.2/wait_for2/__init__.py
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     7422 2021-12-19 18:08:37.000000 wait_for2-0.3.2/wait_for2/impl.py
+drwxr-xr-x   0 nandor    (1000) nandor    (1000)        0 2023-06-09 11:05:18.602473 wait_for2-0.3.2/wait_for2.egg-info/
+-rw-r--r--   0 nandor    (1000) nandor    (1000)     7493 2023-06-09 11:05:18.000000 wait_for2-0.3.2/wait_for2.egg-info/PKG-INFO
+-rw-r--r--   0 nandor    (1000) nandor    (1000)      494 2023-06-09 11:05:18.000000 wait_for2-0.3.2/wait_for2.egg-info/SOURCES.txt
+-rw-r--r--   0 nandor    (1000) nandor    (1000)        1 2023-06-09 11:05:18.000000 wait_for2-0.3.2/wait_for2.egg-info/dependency_links.txt
+-rw-r--r--   0 nandor    (1000) nandor    (1000)       10 2023-06-09 11:05:18.000000 wait_for2-0.3.2/wait_for2.egg-info/top_level.txt
```

### Comparing `wait_for2-0.3.1/LICENSE` & `wait_for2-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wait_for2-0.3.1/setup.py` & `wait_for2-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     license="Apache 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=["wait_for2"],
 )
```

### Comparing `wait_for2-0.3.1/tests/common/inner_bind.py` & `wait_for2-0.3.2/tests/common/inner_bind.py`

 * *Files identical despite different names*

### Comparing `wait_for2-0.3.1/tests/common/resource.py` & `wait_for2-0.3.2/tests/common/resource.py`

 * *Files identical despite different names*

### Comparing `wait_for2-0.3.1/tests/test_inner_bind.py` & `wait_for2-0.3.2/tests/test_inner_bind.py`

 * *Files identical despite different names*

### Comparing `wait_for2-0.3.1/tests/test_no_wait_result.py` & `wait_for2-0.3.2/tests/test_no_wait_result.py`

 * *Files identical despite different names*

### Comparing `wait_for2-0.3.1/tests/test_resource.py` & `wait_for2-0.3.2/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `wait_for2-0.3.1/tests/test_result_after_cancel.py` & `wait_for2-0.3.2/tests/test_result_after_cancel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import asyncio
 
 import pytest
 
 import wait_for2
-from tests.common.constants import BUILTIN_PREFERS_TIMEOUT_OVER_RESULT, BUILTIN_PREFERS_TIMEOUT_OVER_EXCEPTION
+from tests.common.constants import (
+    BUILTIN_PREFERS_TIMEOUT_OVER_RESULT,
+    BUILTIN_PREFERS_TIMEOUT_OVER_EXCEPTION,
+    BUILTIN_PROPAGATES_CUSTOM_CANCEL,
+)
 
 
 async def _result_at_cancel(result, delay=0.0):
     # WARNING: this should not be something to do normally, but this reliably produces a race condition state.
     try:
         while True:
             await asyncio.sleep(0.1)
@@ -24,35 +28,40 @@
     except asyncio.CancelledError:
         await asyncio.sleep(delay)
         raise error
 
 
 @pytest.mark.asyncio
 async def test_result_after_cancel_builtin():
-    # Builtin prioritizes timeout even if result is received.
+    # 1. At natural timeout, a result or exception should be prioritized.
     sentinel = object()
     if BUILTIN_PREFERS_TIMEOUT_OVER_RESULT:
+        # Builtin prioritizes timeout even if result is received.
         with pytest.raises(asyncio.TimeoutError):
             await asyncio.wait_for(_result_at_cancel(sentinel), timeout=0.5)
     else:
+        # Builtin returns result instead of the timeout.
         assert await asyncio.wait_for(_result_at_cancel(sentinel), timeout=0.5) is sentinel
     sentinel_error = Exception()
     if BUILTIN_PREFERS_TIMEOUT_OVER_EXCEPTION:
         # Builtin prioritizes timeout even if error is raised.
         with pytest.raises(asyncio.TimeoutError):
             await asyncio.wait_for(_exception_at_cancel(sentinel_error), timeout=0.5)
     else:
-        # Builtin propagates an error instead of the timeout though.
+        # Builtin propagates an error instead of the timeout.
         try:
             await asyncio.wait_for(_exception_at_cancel(sentinel_error), timeout=0.5)
         except Exception as e:
             assert sentinel_error is e
         else:
             assert False, "did not raise"
 
+    # NOTE: At natural timeout, if an explicit cancellation occurs, the cancellation should have priority, even though
+    # the result will be lost due to the lack of support for handling the race-condition.
+
 
 @pytest.mark.asyncio
 async def test_result_after_cancel_wf2():
     handled = []
 
     def race_handler(r, ex):
         handled.append((r, ex))
@@ -80,30 +89,30 @@
             wf = asyncio.create_task(
                 wait_for2.wait_for(_result_at_cancel(sentinel, delay=0.5), timeout=0.5, race_handler=rh)
             )
             await asyncio.sleep(0.75)
             wf.cancel()
             await wf
         except wait_for2.CancelledWithResultError:
-            assert False, "this does not work because the task does not propagate the custom exception"
+            assert BUILTIN_PROPAGATES_CUSTOM_CANCEL, "task does not propagate the custom exception"
         except asyncio.CancelledError:
-            pass  # as expected
+            assert not BUILTIN_PROPAGATES_CUSTOM_CANCEL, "custom exception should be propagated"
         else:
             assert False, "did not raise"
         assert handled == [(sentinel, False)]
         del handled[:]
 
         try:
             wf = asyncio.create_task(
                 wait_for2.wait_for(_exception_at_cancel(sentinel_error, delay=0.5), timeout=0.5, race_handler=rh)
             )
             await asyncio.sleep(0.75)
             wf.cancel()
             await wf
         except wait_for2.CancelledWithResultError:
-            assert False, "this does not work because the task does not propagate the custom exception"
+            assert BUILTIN_PROPAGATES_CUSTOM_CANCEL, "task does not propagate the custom exception"
         except asyncio.CancelledError:
-            pass  # as expected
+            assert not BUILTIN_PROPAGATES_CUSTOM_CANCEL, "custom exception should be propagated"
         else:
             assert False, "did not raise"
         assert handled == [(sentinel_error, True)]
         del handled[:]
```

### Comparing `wait_for2-0.3.1/wait_for2/impl.py` & `wait_for2-0.3.2/wait_for2/impl.py`

 * *Files identical despite different names*

