# Comparing `tmp/quick_batch-0.1.8.tar.gz` & `tmp/quick_batch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.8.tar", max compression
+gzip compressed data, was "quick_batch-0.1.9.tar", max compression
```

## Comparing `quick_batch-0.1.8.tar` & `quick_batch-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     4187 2023-05-30 23:49:42.799400 quick_batch-0.1.8/README.md
--rw-r--r--   0        0        0      685 2023-05-30 23:49:42.799400 quick_batch-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      120 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/__init__.py
--rw-r--r--   0        0        0      644 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/main.py
--rw-r--r--   0        0        0      831 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/manual_scaler.py
--rwxr-xr-x   0        0        0     1215 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1747 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0     5224 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3252 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      721 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/runner.py
--rw-r--r--   0        0        0      551 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0      146 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_client.py
--rw-r--r--   0        0        0     2088 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     1244 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_dockerfile.py
--rw-r--r--   0        0        0     4624 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1951 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     2033 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4722 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     3207 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     4429 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 quick_batch-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4187 2023-05-31 12:51:46.856980 quick_batch-0.1.9/README.md
+-rw-r--r--   0        0        0      685 2023-05-31 12:51:46.856980 quick_batch-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/__init__.py
+-rw-r--r--   0        0        0      644 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/main.py
+-rw-r--r--   0        0        0      731 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/manual_scaler.py
+-rwxr-xr-x   0        0        0     1215 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1747 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0     5224 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3252 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      711 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/runner.py
+-rw-r--r--   0        0        0      551 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_client.py
+-rw-r--r--   0        0        0     2088 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     1244 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_dockerfile.py
+-rw-r--r--   0        0        0     4582 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1951 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     2033 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4307 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     3103 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     4429 2023-05-31 12:51:46.856980 quick_batch-0.1.9/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 quick_batch-0.1.9/PKG-INFO
```

### Comparing `quick_batch-0.1.8/README.md` & `quick_batch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/pyproject.toml` & `quick_batch-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.8"
+version = "0.1.9"
 description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
 
 [tool.poetry.scripts]
```

### Comparing `quick_batch-0.1.8/quick_batch/main.py` & `quick_batch-0.1.9/quick_batch/main.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/manual_scaler.py` & `quick_batch-0.1.9/quick_batch/manual_scaler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from utilities.manage_client import create_client
-from utilities.manage_services import scaleup_processor_service
+from utilities.manage_services import update_processor_service
 
 
 def scaler(num_processors=None):
     # check num_processors is an integer
     try:
         num_processors = int(num_processors)
     except ValueError:
         raise ValueError("FAILURE: num_processors must be an integer")
 
     # check basic value of num_processors
     if num_processors < 1:
-        raise ValueError("FAILURE: pip num_processors must be greater than 0")
-
-    # create client
-    client = create_client()
+        raise ValueError("FAILURE: num_processors must be greater than 0")
 
     # print update
-    print(f"INFO: manual default scale override --> " + # noqa
-          "scaling processor service to {num_processors} instances...")
+    print("INFO: manual default scale override --> " +
+          "scaling processor service " + str(num_processors) +
+          " to  instances...")
 
     # scale up processor service
-    scaleup_processor_service(client, num_processors)
+    update_processor_service(num_processors)
 
     # print update
     print("INFO: ...complete")
```

### Comparing `quick_batch-0.1.8/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.9/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.9/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.9/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.9/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.9/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.9/quick_batch/queue_app/queue_app/apis.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.9/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.9/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/runner.py` & `quick_batch-0.1.9/quick_batch/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from utilities.manage_setup import setup_client
 from utilities.manage_setup import reset_workspace
 from utilities.manage_setup import setup_workspace
 from utilities.manage_queue import monitor_queue
-from utilities.manage_services import scaleup_processor_service
+from utilities.manage_services import update_processor_service
 
 
 def run(config):
     # setup
     client, input_path, output_path, processor, num_processors, \
         logger = setup_client(config)
 
     # reset workspace
     reset_workspace(client)
 
     # create workspace
     setup_workspace(client, config,  processor, input_path, output_path)
 
     # scale up processor service
-    scaleup_processor_service(client, num_processors)
+    update_processor_service(num_processors)
 
     # monitor queue
     monitor_queue(client)
 
     # close log
     logger.close_log()
```

### Comparing `quick_batch-0.1.8/quick_batch/utilities/__init__.py` & `quick_batch-0.1.9/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_containers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_dockerfile.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_dockerfile.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             pass
 
         # Pull the image
         pulled_image = client.images.pull(image_name)
 
         # Tag the pulled image with a new name
         tagged_image = pulled_image.tag(new_tag)
-        
+
         print('SUCCESS: Pulling and tagging image complete!')
         return True
 
     except docker.errors.APIError as e:
         print(f"FAILURE: Error occurred while pulling and tagging the image: {e}")
         return False
 
@@ -53,16 +53,15 @@
         return False  # The file is empty
 
     return True  # The file exists and is not empty
 
 
 # build processor_app docker image
 @log_exceptions
-def build_processor_image(client,
-                          dockerfile_path,
+def build_processor_image(dockerfile_path,
                           requirements_path,
                           processor):
 
     # create container path for dockerfile
     container_dockerfile_path = os.path.join(processor_path, 'Dockerfile')
 
     # copy dockerfile to processor_path directory
```

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_loggers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_requirements.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 
-import time
 import docker
 from utilities import processor_path, \
     queue_path
 from utilities import log_exceptions
+import subprocess
 
 
 @log_exceptions
-def scaleup_processor_service(client, num_processors):
-    # get processor_service from client
-    processor_service = client.services.get('processor_app')
-
-    # if num_processors < 5 scale up immeadiately
-    if num_processors < 5:
-        processor_service.scale(num_processors)
-        return
-    else:
-        # scale up processor service to num_processors in increments of 5
-        for i in range(5, num_processors + 1, 5):
-            # report scale update in progress
-            print(f"Scaling processor service to {i} instances...")
-
-            # update processor service scale
-            processor_service.scale(min(i, num_processors))
-            time.sleep(30)
-
-            # report update complete
-            print("...complete")
-
-            # break if i >= num_processors
-            if i >= num_processors:
-                break
-        return
+def update_processor_service(num_processors):
+    process = subprocess.run(['docker', 'service', 'update', '--replicas',
+                             str(num_processors), 'processor_app'],
+                             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                             check=True)
+
+    # Print the command output and error
+    print(process.stdout.decode('utf-8'))
+    print(process.stderr.decode('utf-8'))
+
+    return
 
 
 @log_exceptions
 def remove_service(client, service_name):
     if service_name in [service.name for service in client.services.list()]:
         # remove service
         client.services.get(service_name).remove()
```

### Comparing `quick_batch-0.1.8/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.9/quick_batch/utilities/manage_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from utilities.manage_services import remove_all_services
 from utilities.manage_swarm import leave_swarm
 from utilities.manage_swarm import create_swarm
 from utilities.manage_networks import create_network
 from utilities.manage_services import create_queue_service
 from utilities.manage_services import create_processor_service
 from utilities.manage_queue import monitor_queue_app_containers
-from utilities.manage_images import pull_and_tag_image
 
 
 @log_exceptions
 def setup_client(config):
     # setup logger
     logger = setup_logger(config)
 
@@ -39,26 +38,24 @@
 
     # create docker client
     client = create_client()
 
     # # try to pull and tag image
     # pull_success = pull_and_tag_image(client, 'jermwatt/quick_batch_queue_app',
     #                                   'quick_batch_queue_app')
-
     # if not successful, build image
     # if not pull_success:
     manage_images.build_queue_image(client)
 
     # # try to pull and tag image
     # pull_success = pull_and_tag_image(client, image_name, 'quick_batch_processor_app')
 
     # # if not successful, build image
     # if not pull_success:
-    manage_images.build_processor_image(client,
-                                        dockerfile_path,
+    manage_images.build_processor_image(dockerfile_path,
                                         requirements_path,
                                         processor)
 
     return client, input_path, output_path, processor, num_processors, logger
 
 
 @log_exceptions
```

### Comparing `quick_batch-0.1.8/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.9/quick_batch/utilities/param_checks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.8/PKG-INFO` & `quick_batch-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-batch
-Version: 0.1.8
+Version: 0.1.9
 Summary: ultra simple command line tool for docker-scaling batch processing
 Home-page: https://github.com/jermwatt/quick_batch
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

