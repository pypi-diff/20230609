# Comparing `tmp/netunicorn-connector-salt-0.3.5.tar.gz` & `tmp/netunicorn-connector-salt-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-salt-0.3.5.tar", last modified: Mon Jun  5 20:24:20 2023, max compression
+gzip compressed data, was "netunicorn-connector-salt-0.3.6.tar", last modified: Thu Jun  8 22:13:47 2023, max compression
```

## Comparing `netunicorn-connector-salt-0.3.5.tar` & `netunicorn-connector-salt-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22508 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/salt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 22:13:25.000000 netunicorn-connector-salt-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-08 22:13:25.000000 netunicorn-connector-salt-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 22:13:25.000000 netunicorn-connector-salt-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.468817 netunicorn-connector-salt-0.3.6/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.468817 netunicorn-connector-salt-0.3.6/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:25.000000 netunicorn-connector-salt-0.3.6/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23108 2023-06-08 22:13:25.000000 netunicorn-connector-salt-0.3.6/src/netunicorn/director/infrastructure/connectors/salt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:13:47.472817 netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-08 22:13:47.000000 netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-08 22:13:47.000000 netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:13:47.000000 netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-08 22:13:47.000000 netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 22:13:47.000000 netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-salt-0.3.5/LICENSE` & `netunicorn-connector-salt-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.5/PKG-INFO` & `netunicorn-connector-salt-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.5
+Version: 0.3.6
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-salt-0.3.5/README.md` & `netunicorn-connector-salt-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.5/pyproject.toml` & `netunicorn-connector-salt-0.3.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-salt"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "SaltStack connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/salt_connector.py` & `netunicorn-connector-salt-0.3.6/src/netunicorn/director/infrastructure/connectors/salt_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections import defaultdict
-from typing import Optional, Tuple, Any
+from typing import Optional, Tuple, Any, Union, cast
 
 import aiohttp
 import yaml
 from netunicorn.base.architecture import Architecture
 from netunicorn.base.deployment import Deployment
 from netunicorn.base.environment_definitions import DockerImage, ShellExecution
 from netunicorn.base.nodes import CountableNodePool, Node
@@ -162,27 +162,39 @@
                 f"Deployments: {deployments_list}"
             )
             self.logger.debug(await response.text())
             return {x.executor_id: Failure(str(e)) for x in deployments_list}
 
         results: dict[str, Result[None, str]] = {}
         for deployment in deployments_list:
-            if salt_return.get(deployment.node.name, {}).get("retcode", 1) != 0:
+            deployment_result: Union[bool, dict] = salt_return.get(deployment.node.name, {})
+            if isinstance(deployment_result, bool):
                 results[deployment.executor_id] = Failure(
-                    str(salt_return.get(deployment.node.name, ""))
+                    "Salt returned False as a result of command without any error message"
                 )
                 self.logger.error(
                     f"Error during deployment of executor {deployment.executor_id}, "
                     f"node {deployment.node}: {str(salt_return.get(deployment.node.name, ''))}"
                 )
-            else:
-                results[deployment.executor_id] = Success(None)
-                self.logger.debug(
-                    f"Deployment of executor {deployment.executor_id} to node {deployment.node} successful"
+                continue
+
+            if isinstance(deployment_result, bool) and deployment_result.get("retcode", 1) != 0:
+                results[deployment.executor_id] = Failure(
+                    str(salt_return.get(deployment.node.name, ""))
                 )
+                self.logger.error(
+                    f"Error during deployment of executor {deployment.executor_id}, "
+                    f"node {deployment.node}: {str(salt_return.get(deployment.node.name, ''))}"
+                )
+                continue
+
+            results[deployment.executor_id] = Success(None)
+            self.logger.debug(
+                f"Deployment of executor {deployment.executor_id} to node {deployment.node} successful"
+            )
         self.logger.debug(f"Finished deployment of {image}, results: {results}")
         return results
 
     @staticmethod
     def __all_salt_results_are_correct(
         results: list[dict[str, dict[str, int | str]]], node_name: str
     ) -> bool:
@@ -381,15 +393,15 @@
             if not result:
                 raise Exception(
                     f"CherryPy returned an empty response - usually that means that node is not available: {result}"
                 )
             result = result['jid']
         except Exception as e:
             self.logger.error(
-                f"Exception during deployment.\n"
+                f"Exception during execution start.\n"
                 f"Experiment id: {experiment_id}\n"
                 f"Error: {e}\n"
                 f"Deployment: {deployment}"
             )
             self.logger.debug(await response.text())
             error = str(e)
```

### Comparing `netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/PKG-INFO` & `netunicorn-connector-salt-0.3.6/src/netunicorn_connector_salt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.5
+Version: 0.3.6
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

