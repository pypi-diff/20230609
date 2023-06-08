# Comparing `tmp/motion_python-0.1.60.tar.gz` & `tmp/motion_python-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.60.tar", max compression
+gzip compressed data, was "motion_python-0.1.61.tar", max compression
```

## Comparing `motion_python-0.1.60.tar` & `motion_python-0.1.61.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-08 19:01:25.177814 motion_python-0.1.60/README.md
--rw-r--r--   0        0        0      221 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/component.py
--rw-r--r--   0        0        0    17368 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/execute.py
--rw-r--r--   0        0        0     5737 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/fit_task.py
--rw-r--r--   0        0        0    12513 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/route.py
--rw-r--r--   0        0        0     7755 2023-06-08 19:01:25.177814 motion_python-0.1.60/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-08 19:01:46.775225 motion_python-0.1.60/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.60/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-08 19:23:27.662855 motion_python-0.1.61/README.md
+-rw-r--r--   0        0        0      221 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/component.py
+-rw-r--r--   0        0        0    17368 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/execute.py
+-rw-r--r--   0        0        0     5815 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/fit_task.py
+-rw-r--r--   0        0        0    12513 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/route.py
+-rw-r--r--   0        0        0     7755 2023-06-08 19:23:27.662855 motion_python-0.1.61/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-08 19:23:51.588894 motion_python-0.1.61/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.61/PKG-INFO
```

### Comparing `motion_python-0.1.60/README.md` & `motion_python-0.1.61/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/cli.py` & `motion_python-0.1.61/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/component.py` & `motion_python-0.1.61/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/execute.py` & `motion_python-0.1.61/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/fit_task.py` & `motion_python-0.1.61/motion/fit_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import multiprocessing
+import traceback
 from typing import Any, Callable, List, Optional
 
 import cloudpickle
 import redis
 from redis.lock import Lock
 
 from motion.route import Route
@@ -128,14 +129,15 @@
                                 old_state,
                                 redis_con,
                                 self.instance_name,
                                 self.save_state_func,
                             )
                     except Exception as e:
                         logger.error(f"Error in {self.queue_identifier} fit: {e}")
+                        logger.error(traceback.format_exc())
                     finally:
                         logger.info("Releasing lock.")
                         lock.release()
                 else:
                     logger.error("Lock not acquired; batch lost.")
 
             for identifier in identifiers:
```

### Comparing `motion_python-0.1.60/motion/instance.py` & `motion_python-0.1.61/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.61/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/route.py` & `motion_python-0.1.61/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/motion/utils.py` & `motion_python-0.1.61/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.60/pyproject.toml` & `motion_python-0.1.61/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.60"
+version = "0.1.61"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.60/PKG-INFO` & `motion_python-0.1.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.60
+Version: 0.1.61
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

