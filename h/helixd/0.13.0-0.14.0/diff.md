# Comparing `tmp/helixd-0.13.0.tar.gz` & `tmp/helixd-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helixd-0.13.0.tar", last modified: Tue May 16 15:02:02 2023, max compression
+gzip compressed data, was "helixd-0.14.0.tar", last modified: Fri Jun  9 10:09:26 2023, max compression
```

## Comparing `helixd-0.13.0.tar` & `helixd-0.14.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-04-15 11:18:20.000000 helixd-0.13.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-05-16 15:02:02.285746 helixd-0.13.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/helixd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9625 2023-05-16 14:48:15.000000 helixd-0.13.0/helixd/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/helixd.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 15:02:02.285746 helixd-0.13.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-05-16 14:58:41.000000 helixd-0.13.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9933 2023-05-16 14:46:48.000000 helixd-0.13.0/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2023-04-15 11:18:20.000000 helixd-0.13.0/tests/test_stack.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 10:09:26.871860 helixd-0.14.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-04-15 11:18:20.000000 helixd-0.14.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-06-09 10:09:26.871860 helixd-0.14.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 10:09:26.871860 helixd-0.14.0/helixd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9594 2023-06-09 09:50:04.000000 helixd-0.14.0/helixd/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 10:09:26.871860 helixd-0.14.0/helixd.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-06-09 10:09:26.000000 helixd-0.14.0/helixd.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-06-09 10:09:26.000000 helixd-0.14.0/helixd.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-09 10:09:26.000000 helixd-0.14.0/helixd.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-06-09 10:09:26.000000 helixd-0.14.0/helixd.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-06-09 10:09:26.000000 helixd-0.14.0/helixd.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-09 10:09:26.871860 helixd-0.14.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-06-09 10:03:13.000000 helixd-0.14.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 10:09:26.871860 helixd-0.14.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-06-09 09:50:04.000000 helixd-0.14.0/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2023-06-09 09:50:04.000000 helixd-0.14.0/tests/test_stack.py
```

### Comparing `helixd-0.13.0/LICENSE` & `helixd-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helixd-0.13.0/PKG-INFO` & `helixd-0.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helixd
-Version: 0.13.0
+Version: 0.14.0
 Summary: Minimalist LXD API client
 Home-page: https://zebr0.io/projects/helixd
 Download-URL: https://gitlab.com/zebr0/helixd
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helixd-0.13.0/helixd/__init__.py` & `helixd-0.14.0/helixd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import enum
 import string
 import time
 
 import requests
 import requests_unixsocket
 
-KEY_DEFAULT = "lxd-stack"
 URL_DEFAULT = "http+unix://%2Fvar%2Fsnap%2Flxd%2Fcommon%2Flxd%2Funix.socket"
 
 
 class ResourceType(enum.Enum):
     """
     Enumerates the various LXD resource types managed by the library.
     """
@@ -73,95 +72,91 @@
             if response_json.get("type") == "async":
                 operation = self.session.get(self.url + response_json.get("operation") + "/wait").json().get("metadata")
                 if operation.get("status_code") != 200:
                     raise requests.HTTPError(operation.get("err"))
 
         self.session.hooks["response"].append(hook)
 
-    def exists(self, config: dict, resource_type: ResourceType) -> bool:
+    def exists(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> bool:
         """
         :param config: the resource's configuration
-        :param resource_type: the resource's type
+        :param resource_type: the resource's type, defaults to INSTANCES
         :return: whether the resource exists or not
         """
 
         try:
             self.session.get(self.url + resource_type.path(config) + "/" + config.get("name"))
             return True
         except requests.HTTPError:
             return False
 
     def create(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
-        Creates a resource if it doesn't exist.
+        Creates a resource.
         The required configuration depends on the resource's type (see helixd.Client).
 
         :param config: the resource's desired configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         type_path = resource_type.path(config)
         resource_path = type_path + "/" + config.get("name")
 
-        if not self.exists(config, resource_type):
-            print("creating", resource_path)
-            self.session.post(self.url + type_path, json=config)
+        print("creating", resource_path)
+        self.session.post(self.url + type_path, json=config)
 
     def delete(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
-        Deletes a resource if it exists.
+        Deletes a resource.
 
         :param config: the resource's configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
-        if self.exists(config, resource_type):
-            print(f"deleting", resource_path)
-            self.session.delete(self.url + resource_path)
+        print(f"deleting", resource_path)
+        self.session.delete(self.url + resource_path)
 
     def is_running(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> bool:
         """
         :param config: the resource's configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         :return: whether the resource is running or not
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
         return self.session.get(self.url + resource_path).json().get("metadata").get("status") == "Running"
 
     def start(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
-        Starts a resource if it's not running.
+        Starts a resource.
 
         :param config: the resource's configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
-        if not self.is_running(config, resource_type):
-            print("starting", resource_path)
-            self.session.put(self.url + resource_path + "/state", json={"action": "start"})
+        print("starting", resource_path)
+        self.session.put(self.url + resource_path + "/state", json={"action": "start"})
 
     def stop(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
-        Stops a resource if it's running.
+        Stops a resource.
 
         :param config: the resource's configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
-        if self.exists(config, resource_type) and self.is_running(config, resource_type):
-            print("stopping", resource_path)
-            self.session.put(self.url + resource_path + "/state", json={"action": "stop"})
+        print("stopping", resource_path)
+        self.session.put(self.url + resource_path + "/state", json={"action": "stop"})
 
     def get_ip_address(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES, device: str = "eth0", family: str = "inet", attempts: int = 10, delay: float = 0.3) -> str:
         """
         :param config: the resource's configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         :param device: the resource's network device, defaults to eth0
         :param family: the address' family, i.e. inet for IPv4 or inet6 for IPv6, defaults to inet
@@ -185,41 +180,45 @@
         The required configurations depend on the resource's type (see helixd.Client).
 
         :param stack: the stack as a dictionary
         """
 
         for resource_type in ResourceType:
             for config in stack.get(resource_type.name()) or []:
-                self.create(config, resource_type)
+                if not self.exists(config, resource_type):
+                    self.create(config, resource_type)
 
     def delete_stack(self, stack: dict) -> None:
         """
         Deletes the resources in the given stack if they exist.
 
         :param stack: the stack as a dictionary
         """
 
         for resource_type in reversed(ResourceType):
             for config in stack.get(resource_type.name()) or []:
-                self.delete(config, resource_type)
+                if self.exists(config, resource_type):
+                    self.delete(config, resource_type)
 
     def start_stack(self, stack: dict) -> None:
         """
         Starts the resources in the given stack if they're not running.
 
         :param stack: the stack as a dictionary
         """
 
         for resource_type in [ResourceType.INSTANCES]:
             for config in stack.get(resource_type.name()) or []:
-                self.start(config, resource_type)
+                if not self.is_running(config, resource_type):
+                    self.start(config, resource_type)
 
     def stop_stack(self, stack: dict) -> None:
         """
         Stops the resources in the given stack if they're running.
 
         :param stack: the stack as a dictionary
         """
 
         for resource_type in [ResourceType.INSTANCES]:
             for config in stack.get(resource_type.name()) or []:
-                self.stop(config, resource_type)
+                if self.exists(config, resource_type) and self.is_running(config, resource_type):
+                    self.stop(config, resource_type)
```

### Comparing `helixd-0.13.0/helixd.egg-info/PKG-INFO` & `helixd-0.14.0/helixd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helixd
-Version: 0.13.0
+Version: 0.14.0
 Summary: Minimalist LXD API client
 Home-page: https://zebr0.io/projects/helixd
 Download-URL: https://gitlab.com/zebr0/helixd
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helixd-0.13.0/setup.py` & `helixd-0.14.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="helixd",
-    version="0.13.0",
+    version="0.14.0",
     description="Minimalist LXD API client",
     long_description="TODO",
     long_description_content_type="text/markdown",
     author="Thomas JOUANNOT",
     author_email="mazerty@gmail.com",
     url="https://zebr0.io/projects/helixd",
     download_url="https://gitlab.com/zebr0/helixd",
```

### Comparing `helixd-0.13.0/tests/test_client.py` & `helixd-0.14.0/tests/test_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 
 def test_create_storage_pool(client, capsys):
     config = {"name": "test-storage-pool", "driver": "dir"}
 
     client.create(config, ResourceType.STORAGE_POOLS)
     assert client.exists(config, ResourceType.STORAGE_POOLS)
-    client.create(config, ResourceType.STORAGE_POOLS)  # idempotent
 
     assert capsys.readouterr().out == CREATE_STORAGE_POOL_OUTPUT
 
 
 CREATE_VOLUME_OUTPUT = """
 creating /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 """.lstrip()
@@ -73,60 +72,56 @@
 def test_create_volume(client, capsys):
     subprocess.run("lxc storage create test-storage-pool dir", shell=True)  # given
 
     config = {"name": "test-volume", "parent": "test-storage-pool"}
 
     client.create(config, ResourceType.VOLUMES)
     assert client.exists(config, ResourceType.VOLUMES)
-    client.create(config, ResourceType.VOLUMES)  # idempotent
 
     assert capsys.readouterr().out == CREATE_VOLUME_OUTPUT
 
 
 CREATE_NETWORK_OUTPUT = """
 creating /1.0/networks/test-network
 """.lstrip()
 
 
 def test_create_network(client, capsys):
     config = {"name": "test-network"}
 
     client.create(config, ResourceType.NETWORKS)
     assert client.exists(config, ResourceType.NETWORKS)
-    client.create(config, ResourceType.NETWORKS)  # idempotent
 
     assert capsys.readouterr().out == CREATE_NETWORK_OUTPUT
 
 
 CREATE_PROFILE_OUTPUT = """
 creating /1.0/profiles/test-profile
 """.lstrip()
 
 
 def test_create_profile(client, capsys):
     config = {"name": "test-profile"}
 
     client.create(config, ResourceType.PROFILES)
     assert client.exists(config, ResourceType.PROFILES)
-    client.create(config, ResourceType.PROFILES)  # idempotent
 
     assert capsys.readouterr().out == CREATE_PROFILE_OUTPUT
 
 
 CREATE_INSTANCE_OUTPUT = """
 creating /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_create_instance(client, capsys):
     config = {"name": "test-instance", "source": {"type": "none"}}
 
     client.create(config, ResourceType.INSTANCES)
     assert client.exists(config, ResourceType.INSTANCES)
-    client.create(config, ResourceType.INSTANCES)  # idempotent
 
     assert capsys.readouterr().out == CREATE_INSTANCE_OUTPUT
 
 
 DELETE_STORAGE_POOL_OUTPUT = """
 creating /1.0/storage-pools/test-storage-pool
 deleting /1.0/storage-pools/test-storage-pool
@@ -136,15 +131,14 @@
 def test_delete_storage_pool(client, capsys):
     config = {"name": "test-storage-pool", "driver": "dir"}
 
     client.create(config, ResourceType.STORAGE_POOLS)  # given
 
     client.delete(config, ResourceType.STORAGE_POOLS)
     assert not client.exists(config, ResourceType.STORAGE_POOLS)
-    client.delete(config, ResourceType.STORAGE_POOLS)  # idempotent
 
     assert capsys.readouterr().out == DELETE_STORAGE_POOL_OUTPUT
 
 
 DELETE_VOLUME_OUTPUT = """
 creating /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 deleting /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
@@ -155,15 +149,14 @@
     # given
     subprocess.run("lxc storage create test-storage-pool dir", shell=True)
     config = {"name": "test-volume", "parent": "test-storage-pool"}
     client.create(config, ResourceType.VOLUMES)
 
     client.delete(config, ResourceType.VOLUMES)
     assert not client.exists(config, ResourceType.VOLUMES)
-    client.delete(config, ResourceType.VOLUMES)  # idempotent
 
     assert capsys.readouterr().out == DELETE_VOLUME_OUTPUT
 
 
 DELETE_NETWORK_OUTPUT = """
 creating /1.0/networks/test-network
 deleting /1.0/networks/test-network
@@ -173,15 +166,14 @@
 def test_delete_network(client, capsys):
     config = {"name": "test-network"}
 
     client.create(config, ResourceType.NETWORKS)  # given
 
     client.delete(config, ResourceType.NETWORKS)
     assert not client.exists(config, ResourceType.NETWORKS)
-    client.delete(config, ResourceType.NETWORKS)  # idempotent
 
     assert capsys.readouterr().out == DELETE_NETWORK_OUTPUT
 
 
 DELETE_PROFILE_OUTPUT = """
 creating /1.0/profiles/test-profile
 deleting /1.0/profiles/test-profile
@@ -191,15 +183,14 @@
 def test_delete_profile(client, capsys):
     config = {"name": "test-profile"}
 
     client.create(config, ResourceType.PROFILES)  # given
 
     client.delete(config, ResourceType.PROFILES)
     assert not client.exists(config, ResourceType.PROFILES)
-    client.delete(config, ResourceType.PROFILES)  # idempotent
 
     assert capsys.readouterr().out == DELETE_PROFILE_OUTPUT
 
 
 DELETE_INSTANCE_OUTPUT = """
 creating /1.0/instances/test-instance
 deleting /1.0/instances/test-instance
@@ -209,15 +200,14 @@
 def test_delete_instance(client, capsys):
     config = {"name": "test-instance", "source": {"type": "none"}}
 
     client.create(config, ResourceType.INSTANCES)  # given
 
     client.delete(config, ResourceType.INSTANCES)
     assert not client.exists(config, ResourceType.INSTANCES)
-    client.delete(config, ResourceType.INSTANCES)  # idempotent
 
     assert capsys.readouterr().out == DELETE_INSTANCE_OUTPUT
 
 
 TEST_INSTANCE_CONFIG = {
     "name": "test-instance",
     "profiles": ["default"],
@@ -249,46 +239,37 @@
 START_OUTPUT = """
 creating /1.0/instances/test-instance
 starting /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_start(client, capsys):
-    # first, trying to start a non-existent instance should fail
-    with pytest.raises(Exception):
-        client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
-
     client.create(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
 
     client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
     time.sleep(0.2)
     assert client.is_running(TEST_INSTANCE_CONFIG)
-    client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)  # idempotent
 
     assert capsys.readouterr().out == START_OUTPUT
 
 
 STOP_OUTPUT = """
 creating /1.0/instances/test-instance
 starting /1.0/instances/test-instance
 stopping /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_stop(client, capsys):
-    # first, trying to stop a non-existent instance shouldn't fail
-    client.stop(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
-
     client.create(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
     client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
     time.sleep(0.2)
 
     client.stop(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
     assert not client.is_running(TEST_INSTANCE_CONFIG)
-    client.stop(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)  # idempotent
 
     assert capsys.readouterr().out == STOP_OUTPUT
 
 
 def test_get_ip_address_ok(client, capsys):
     client.create(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
     client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
```

### Comparing `helixd-0.13.0/tests/test_stack.py` & `helixd-0.14.0/tests/test_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,30 @@
     Replaces them by a log system to trace the calls.
 
     :return: the log list
     """
 
     log = []
 
-    def build_mock(string):
+    def exists_mock(_, *args):
+        return ("create", *args) in log and not ("delete", *args) in log
+
+    def is_running_mock(_, *args):
+        return ("start", *args) in log and not ("stop", *args) in log
+
+    def build_operation_mock(string):
         def mock(_, *args):
             log.append((string, *args))
 
         return mock
 
+    monkeypatch.setattr(Client, "is_running", is_running_mock)
+    monkeypatch.setattr(Client, "exists", exists_mock)
     for function in [CREATE, START, STOP, DELETE]:
-        monkeypatch.setattr(Client, function, build_mock(function))
+        monkeypatch.setattr(Client, function, build_operation_mock(function))
 
     return log
 
 
 STORAGE_POOL_CONFIG = {"name": "test-storage-pool", "driver": "dir"}
 NETWORK_CONFIG = {"name": "test-network"}
 PROFILE_CONFIG = {"name": "test-profile"}
@@ -38,42 +46,39 @@
     "storage-pools": [STORAGE_POOL_CONFIG],
     "networks": [NETWORK_CONFIG],
     "profiles": [PROFILE_CONFIG],
     "instances": [INSTANCE_A_CONFIG, INSTANCE_B_CONFIG]
 }
 
 
-def test_create_stack(client, mock_client):
-    client.create_stack(LXD_STACK)
-
-    assert mock_client == [(CREATE, STORAGE_POOL_CONFIG, ResourceType.STORAGE_POOLS),
-                           (CREATE, NETWORK_CONFIG, ResourceType.NETWORKS),
-                           (CREATE, PROFILE_CONFIG, ResourceType.PROFILES),
-                           (CREATE, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
-                           (CREATE, INSTANCE_B_CONFIG, ResourceType.INSTANCES)]
+def test_stack(client, mock_client):
+    client.stop_stack(LXD_STACK)  # first, trying to stop a non-existent instance shouldn't do anything
 
+    client.create_stack(LXD_STACK)
+    client.create_stack(LXD_STACK)  # idempotent
 
-def test_start_stack(client, mock_client):
     client.start_stack(LXD_STACK)
+    client.start_stack(LXD_STACK)  # idempotent
 
-    assert mock_client == [(START, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
-                           (START, INSTANCE_B_CONFIG, ResourceType.INSTANCES)]
-
-
-def test_stop_stack(client, mock_client):
     client.stop_stack(LXD_STACK)
+    client.stop_stack(LXD_STACK)  # idempotent
 
-    assert mock_client == [(STOP, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
-                           (STOP, INSTANCE_B_CONFIG, ResourceType.INSTANCES)]
-
-
-def test_delete_stack(client, mock_client):
     client.delete_stack(LXD_STACK)
+    client.delete_stack(LXD_STACK)  # idempotent
 
-    assert mock_client == [(DELETE, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
+    assert mock_client == [(CREATE, STORAGE_POOL_CONFIG, ResourceType.STORAGE_POOLS),
+                           (CREATE, NETWORK_CONFIG, ResourceType.NETWORKS),
+                           (CREATE, PROFILE_CONFIG, ResourceType.PROFILES),
+                           (CREATE, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
+                           (CREATE, INSTANCE_B_CONFIG, ResourceType.INSTANCES),
+                           (START, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
+                           (START, INSTANCE_B_CONFIG, ResourceType.INSTANCES),
+                           (STOP, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
+                           (STOP, INSTANCE_B_CONFIG, ResourceType.INSTANCES),
+                           (DELETE, INSTANCE_A_CONFIG, ResourceType.INSTANCES),
                            (DELETE, INSTANCE_B_CONFIG, ResourceType.INSTANCES),
                            (DELETE, PROFILE_CONFIG, ResourceType.PROFILES),
                            (DELETE, NETWORK_CONFIG, ResourceType.NETWORKS),
                            (DELETE, STORAGE_POOL_CONFIG, ResourceType.STORAGE_POOLS)]
 
 
 def test_empty(client, mock_client):
```

