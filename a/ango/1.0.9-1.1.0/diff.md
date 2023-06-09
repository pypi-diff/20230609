# Comparing `tmp/ango-1.0.9.tar.gz` & `tmp/ango-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.9.tar", last modified: Fri Jun  2 07:41:27 2023, max compression
+gzip compressed data, was "ango-1.1.0.tar", last modified: Fri Jun  9 07:30:29 2023, max compression
```

## Comparing `ango-1.0.9.tar` & `ango-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-02 07:41:27.094165 ango-1.0.9/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.9/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.9/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.9/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.9/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-05-30 11:15:47.000000 ango-1.0.9/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.9/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5446 2023-06-02 07:39:18.000000 ango-1.0.9/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14429 2023-06-01 20:58:42.000000 ango-1.0.9/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-02 07:41:26.000000 ango-1.0.9/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-02 07:41:27.000000 ango-1.0.9/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-02 07:41:26.000000 ango-1.0.9/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-06-02 07:41:27.000000 ango-1.0.9/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-02 07:41:27.000000 ango-1.0.9/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-02 07:41:27.094165 ango-1.0.9/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-06-02 07:22:27.000000 ango-1.0.9/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-09 07:30:29.560179 ango-1.1.0/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.0/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.1.0/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.1.0/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.1.0/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-09 07:29:48.000000 ango-1.1.0/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.1.0/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5511 2023-06-09 07:29:48.000000 ango-1.1.0/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-09 07:29:48.000000 ango-1.1.0/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-09 07:30:29.560179 ango-1.1.0/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-09 07:30:23.000000 ango-1.1.0/setup.py
```

### Comparing `ango-1.0.9/PKG-INFO` & `ango-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.9
+Version: 1.1.0
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.9/README.md` & `ango-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.9/ango/models/label_category.py` & `ango-1.1.0/ango/models/label_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Tool(enum.Enum):
     BoundingBox = "bounding-box"
     Segmentation = "segmentation"
     Polyline = "polyline"
     Polygon = "polygon"
-    RotatedBoundingBox = "rotated-bounding-box"
+    boundingBox = "rotated-bounding-box"
     Ner = "ner"
     Point = "point"
     Pdf = "pdf"
 
 
 class Classification(enum.Enum):
     Multi_dropdown = "multi-dropdown"
```

### Comparing `ango-1.0.9/ango/plugin_logger.py` & `ango-1.1.0/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.9/ango/plugins.py` & `ango-1.1.0/ango/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import datetime
 import logging
+import time
 from io import BytesIO
 from typing import Callable, Tuple
-import queue
+
 import requests
 import socketio
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
+from apscheduler.schedulers.background import BackgroundScheduler
 
 from ango.plugin_logger import PluginLogger
 from ango.sdk import SDK
 
 try:
     import asyncio
 except ImportError:
@@ -18,29 +20,31 @@
 
 class Plugin(socketio.ClientNamespace):
 
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__('/plugin')
         self.id = id
         self.secret = secret
-        scheduler = AsyncIOScheduler()
+        scheduler = BackgroundScheduler()
         scheduler.add_job(self.heartbeat, 'interval', seconds=60)
         scheduler.start()
         self.logger = logging.getLogger()
         self.callback = callback
+        self.loop = asyncio.get_event_loop()
 
     def on_connect(self):
-        self.heartbeat()
         self.logger.warning("Connected")
+        self.heartbeat()
 
     def on_disconnect(self):
         self.logger.warning("Disconnected")
 
     def heartbeat(self):
         self.emit('heartbeat', {"id": self.id, "secret": self.secret})
+        self.logger.warning("Heartbeat at %s" % str(time.time()))
 
     def on_plugin(self, data):
         data["logger"] = self._get_logger(data)
         data["batches"] = data.get('tags', [])
         response = {
             "response": self.callback(**data),
             "session": data.get("session", "")
@@ -50,22 +54,19 @@
     def _get_logger(self, data):
         org_id = data.get("orgId", "")
         run_by = data.get("runBy", "")
         session = data.get("session", "")
         logger = PluginLogger("logger", self.id, org_id, run_by, session, self)
         return logger
 
-    def start(self):
-        asyncio.get_event_loop().run_forever()
-
 
 class ExportPlugin(Plugin):
 
     def __init__(self, id: str, secret: str, callback: Callable[[str, dict], Tuple[str, BytesIO]],
-                 host="https://imeritapi.ango.ai"):
+                 host="https://api.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
 
     def on_plugin(self, data):
         """
         :param data: {project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime = None, tags: List[str] = None}
@@ -98,40 +99,32 @@
             "response": upload_url.split("?")[0],
             "session": data.get("session", "")
         }
         self.emit('response', response)
 
 
 class ModelPlugin(Plugin):
-    def __init__(self, id: str, secret: str, callback: Callable, host="https://imeritapi.ango.ai", concurrency=1):
+    def __init__(self, id: str, secret: str, callback: Callable, host="https://api.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
-        self.concurrency = concurrency
-        self.queue = queue.Queue()
-
-    async def work(self):
-        while True:
-            data = self.queue.get()
-            data["batches"] = data.get('tags', [])
-            api_key = data.get('apiKey')
-            task_id = data.get('taskId')
-            sdk = SDK(api_key=api_key, host=self.host)
-            answer = self.callback(**data)
-            sdk._annotate(task_id, answer.get("answer"))
 
     def on_plugin(self, data):
         workflow = data.get('workflow')
         if not workflow:
             return super().on_plugin(data)
-        self.queue.put(data)
-
-    def start(self):
-        tasks = [self.work() for i in range(self.concurrency)]
-        future = asyncio.gather(*tasks)
-        asyncio.get_event_loop().run_until_complete(future)
+        api_key = data.get('apiKey')
+        task_id = data.get('labeltask').get('_id')
+        sdk = SDK(api_key=api_key, host=self.host)
+        answer = self.callback(**data)
+        annotation = {
+            "tools": answer.get("answer").get("objects") + data.get('labeltask').get("answer").get("tools"),
+            "classifications": answer.get("answer").get("classifications") + data.get('labeltask').get("answer").get("classifications"),
+            "relations": answer.get("answer").get("relations") + data.get('labeltask').get("answer").get("relations")
+        }
+        return sdk._annotate(task_id, annotation);
 
 class FileExplorerPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
 class BatchModelPlugin(Plugin):
@@ -145,15 +138,15 @@
 
 
 class MarkdownPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
-def run(plugin, host="https://plugin.imerit.ango.ai"):
+def run(plugin, host="https://api.ango.ai"):
     sio = socketio.Client()
     sio.register_namespace(plugin)
     sio.connect(host, namespaces=["/plugin"], wait_timeout=100)
     try:
-        plugin.start()
+        asyncio.get_event_loop().run_forever()
     except (KeyboardInterrupt, SystemExit):
         logging.getLogger().warning("Plugin Stopped")
```

### Comparing `ango-1.0.9/ango/sdk.py` & `ango-1.1.0/ango/sdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import logging
 import mimetypes
 import urllib.request
 import uuid
 import zipfile
 from enum import Enum
 from typing import List
 
@@ -14,21 +13,18 @@
 
 from ango.models.enums import TaskStatus
 from ango.models.label_category import ToolCategory, ClassificationCategory, RelationCategory
 
 
 class SDK:
 
-    def __init__(self, api_key, host="https://imeritapi.ango.ai"):
+    def __init__(self, api_key, host="https://api.ango.ai"):
         self.api_key = api_key
         self.host = host
         self.session = requests.Session()
-        if host == 'https://api.ango.ai' or host == 'https://apibeta.ango.ai':
-            logging.getLogger().error("Please downgrade your version to < 1.0.0")
-        logging.getLogger().warning("Your host is %s" % host)
 
     def list_projects(self, page=1, limit=10):
         url = "%s/v2/listProjects?page=%s&limit=%s" % (self.host, page, limit)
 
         payload = {}
         headers = {
             'Content-Type': 'application/json',
@@ -45,24 +41,21 @@
             'Content-Type': 'application/json',
             'apikey': self.api_key
         }
 
         response = self.session.get(url, headers=headers, data=payload)
         return response.json()
 
-    def get_tasks(self, project_id: str, page: int = 1, limit: int = 10, status: str = None, stage: str = None,
-                  batches: List[str] = None):
+    def get_tasks(self, project_id: str, page: int = 1, limit: int = 10, status: str = None, batches: List[str] = None):
         url = "%s/v2/project/%s/tasks?page=%s&limit=%s" % (self.host, project_id, page, limit)
         if status:
             url += "&status[eq]=%s" % status
         if batches:
-            tags = self.__get_batches(project_id, batches)
-            url += "&batches=%s" % json.dumps(tags)
-        if stage:
-            url += "&stage=%s" % stage
+            tags = self.__getTags(project_id, batches)
+            url += "&tag=%s" % json.dumps(tags)
 
         payload = {}
         headers = {
             'Content-Type': 'application/json',
             'apikey': self.api_key
         }
         response = self.session.get(url, headers=headers, data=payload)
@@ -75,14 +68,27 @@
         headers = {
             'Content-Type': 'application/json',
             'apikey': self.api_key
         }
         response = self.session.get(url, headers=headers, data=payload)
         return response.json()
 
+    def set_task_status(self, task_id: str, status: TaskStatus):
+        url = "%s/v2/task/%s/status" % (self.host, task_id)
+
+        payload = {
+            'status': status.value
+        }
+        headers = {
+            'Content-Type': 'application/json',
+            'apikey': self.api_key
+        }
+        response = self.session.post(url, headers=headers, json=payload)
+        return response.json()
+
     def assign_task(self, task, userid=None, email=None):
         url = "%s/v2/task/assign" % self.host
 
         payload = {"task": task}
         if userid:
             payload["user"] = userid
         elif email:
@@ -103,39 +109,39 @@
         headers = {
             'apikey': self.api_key
         }
         r = self.session.get(url, headers=headers).json()
         url = r["data"]["uploadUrl"]
         return url
 
-    def __get_batches(self, project_id, batches):
+    def __getTags(self, project_id, tags):
         ptags = self.get_batches(project_id)
         resp = []
-        for t1 in batches:
-            batch_exist = False
+        for t1 in tags:
+            tag_exist = False
             for t2 in ptags:
                 if t1 == t2["_id"] or t1 == t2["name"]:
                     resp.append(t2["_id"])
-                    batch_exist = True
-            if not batch_exist:
+                    tag_exist = True
+            if not tag_exist:
                 raise Exception("Tag %s not found" % t1)
         return resp
 
-    def __check_storages(self, project_id, storage_id):
-        resp = self.get_storages(project_id)
-        storages_list = resp['data']['storages']
-        storage_exists = False
-        for t1 in storages_list:
-            if '_id' in t1 and t1['_id'] == storage_id:
-                storage_exists = True
-        return storage_exists
-
-    def upload_files(self, project_id: str, file_paths: List, storage_id: str = None, batches: List[str] = None):
-        if storage_id and not self.__check_storages(project_id, storage_id):
-            raise "Storage ID is Invalid!"
+    def __check_integration(self, project_id, integration_id):
+        resp = self.get_integrations(project_id)
+        integrations_list = resp['data']['integrations']
+        integration_exists = False
+        for t1 in integrations_list:
+            if '_id' in t1 and t1['_id'] == integration_id:
+                integration_exists = True
+        return integration_exists
+
+    def upload_files(self, project_id: str, file_paths: List, integration_id: str = None, batches: List[str] = None):
+        if integration_id and not self.__check_integration(project_id, integration_id):
+            raise "Integration ID is Invalid!"
         assets = []
         for path in tqdm(file_paths):
             uid = uuid.uuid4().hex
             data = ""
             external_id = ""
             if isinstance(path, str):
                 data = path
@@ -144,35 +150,35 @@
                 data = path.get("data")
                 external_id = path.get("externalId", uid)
             file = open(data, 'rb')
             fname = uid + '.' + file.name.split('.')[-1]
             url = self._get_upload_url(fname)
             requests.put(url, data=file.read())
             asset = {'data': url.split('?')[0], 'externalId': external_id}
-            if storage_id:
-                asset['storage'] = storage_id
+            if integration_id:
+                asset['storage'] = integration_id
             assets.append(asset)
 
         url = "%s/v2/project/%s/cloud" % (self.host, project_id)
         if batches:
-            tags = self.__get_batches(project_id, batches)
-            url += "?batches=%s" % json.dumps(tags)
+            tags = self.__getTags(project_id, batches)
+            url += "?tags=%s" % json.dumps(tags)
 
         payload = json.dumps({"assets": assets})
         headers = {
             'Content-Type': 'application/json',
             'apikey': self.api_key
         }
 
         response = self.session.post(url, headers=headers, data=payload)
         return response.json()
 
-    def upload_files_cloud(self, project_id: str, assets, storage_id: str = None, batches: List[str] = None):
-        if storage_id and not self.__check_storages(project_id, storage_id):
-            raise "Storage ID is Invalid!"
+    def upload_files_cloud(self, project_id: str, assets, integration_id: str = None, batches: List[str] = None):
+        if integration_id and not self.__check_integration(project_id, integration_id):
+            raise "Integration ID is Invalid!"
         url = "%s/v2/project/%s/cloud" % (self.host, project_id)
 
         tagMap = {}
         ptags = self.get_batches(project_id)
         for tag in ptags:
             tagMap[tag['name']] = tag['_id']
 
@@ -185,22 +191,22 @@
                         resp.append(t2["_id"])
                         tag_exist = True
                 if not tag_exist:
                     raise Exception("Tag %s not found" % t1)
             return resp
 
         for a in assets:
-            if storage_id:
-                a['storage'] = storage_id
+            if integration_id:
+                a['storage'] = integration_id
             if "batches" in a:
-                a['batches'] = switch_tags_names_with_ids(a['batches'])
+                a['tags'] = switch_tags_names_with_ids(a['batches'])
 
         if batches:
             tags = switch_tags_names_with_ids(batches)
-            url += "?batches=%s" % json.dumps(tags)
+            url += "?tags=%s" % json.dumps(tags)
 
         payload = json.dumps({"assets": assets})
         headers = {
             'Content-Type': 'application/json',
             'apikey': self.api_key
         }
 
@@ -221,24 +227,42 @@
 
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
     def get_assets(self, project_id, asset_id=None, external_id=None, page=1, limit=10):
         url = "%s/v2/project/%s/assets?page=%s&limit=%s" % (self.host, project_id, page, limit)
         if asset_id:
-            url += "&_id=%s" % asset_id
+            url += "?_id=" % asset_id
         if external_id:
-            url += "&externalId=%s" % external_id
+            url += "?externalId=" % external_id
 
         headers = {
             'apikey': self.api_key
         }
         response = self.session.get(url, headers=headers)
         return response.json()
 
+    def set_asset_priority(self, project_id: str, priority: int, external_id: str = None, asset_id: str = None):
+        if external_id is None and asset_id is None:
+            return Exception("External id or Assest Id should be provided!")
+
+        url = "%s/v2/priority/%s" % (self.host, project_id)
+
+        payload = {
+            "priority": priority,
+            "externalId": external_id,
+            "assetId": asset_id
+        }
+        headers = {
+            'apikey': self.api_key
+        }
+
+        response = self.session.post(url, headers=headers, json=payload)
+        return response.json()
+
     def create_attachment(self, project_id, attachments):
 
         url = "%s/v2/attachments" % self.host
 
         payload = {
             "project": project_id,
             "attachments": attachments
@@ -249,21 +273,22 @@
 
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
     def export(self, project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime] = None, batches: List[str] = None):
 
-        url = "%s/v2/export?project=%s&sendEmail=false&format=json&stage=[\"Complete\"]&" \
-              "includeMetadata=true&includeHistory=true&includeSegmentationPoints=true&doNotNotify=true"\
-              % (self.host, project_id)
+        url = "%s/v2/export?project=%s&labeledAt=true&reviewedAt=true&completion=true&totalDuration=true&skip=true" \
+              "&reviewConf=true&format=json&labelDuration=true&assetStatus=true&consensus=true&batches=true" \
+              "&updateInfo=true&issues=true&mask=true&boxImage=true&annotationMetadata=true&benchmark=true" \
+              "&labelStatus=true&segmentationPoints=true&sendEmail=false&doNotNotify=true" % (self.host, project_id)
         if type(assignees) == list and len(assignees) > 0:
             url += "&assignee=" + json.dumps(assignees)
         if type(batches) == list and len(batches) > 0:
-            url += "&batches=" + json.dumps(batches)
+            url += "&tag=" + json.dumps(batches)
         if type(completed_at) == list and len(completed_at) == 2:
             if completed_at[0] is not None:
                 url += "&completedAt[gt]=" + completed_at[0].isoformat()
             if completed_at[1] is not None:
                 url += "&completedAt[lt]=" + completed_at[1].isoformat()
         if type(updated_at) == list and len(updated_at) == 2:
             if updated_at[0] is not None:
@@ -313,57 +338,57 @@
             "project": project_id,
             "jsonContent": labels
         }
 
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
-    def get_storages(self, id: str = None):
-        url = "%s/v2/storages" % self.host
+    def get_integrations(self, id: str = None):
+        url = "%s/v2/integrations" % self.host
         headers = {
             'apikey': self.api_key
         }
         response = self.session.get(url, headers=headers)
         if id:
-            for i in response.json().get('data', {}).get("storages", []):
+            for i in response.json().get('data', {}).get("integrations", []):
                 if i["_id"] == id:
                     return i
         return response.json()
 
     def get_batches(self, project_id: str):
         p = self.get_project(project_id)
         if 'data' in p:
-            return p.get("data", {}).get("project", {}).get("batches", [])
+            return p.get("data", {}).get("project", {}).get("tags", [])
         else:
             raise Exception('Invalid Project Id!')
 
     def create_batch(self, project_id: str, batch_name: str):
         url = "%s/v2/batches/%s" % (self.host, project_id)
-        bacthes = self.get_batches(project_id)
+        tags = self.get_batches(project_id)
         headers = {
             'apikey': self.api_key
         }
-        bacthes.append({
+        tags.append({
             'name': batch_name
         })
         payload = {
-            "batches": bacthes,
+            "tags": tags,
         }
         response = self.session.post(url, headers=headers, json=payload)
-        return response.json().get("data", []).get("project", []).get("batches", [])
+        return response.json().get("data", []).get("project", []).get("tags", [])
 
     def assign_batches(self, project_id: str, asset_ids: List[str], batches: List[str]):
         url = "%s/v2/assignBatches" % self.host
-        batches = self.__get_batches(project_id, batches)
+        tags = self.__getTags(project_id, batches)
         headers = {
             'apikey': self.api_key
         }
         payload = {
             "assets": asset_ids,
-            "batches": batches,
+            "tags": tags,
         }
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
     def create_project(self, name, description=""):
         url = "%s/v2/project" % self.host
         headers = {
@@ -372,47 +397,32 @@
         payload = {
             "name": name,
             "description": description,
         }
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
-    def _annotate(self, task_id: str, answer: dict):
-        url = "%s/v2/annotate/%s?nextStage=true" % (self.host, task_id)
+    def create_webhook(self, webhook_url: str, project_id: str, secret: str, types: List[str]):
+        url = "%s/v2/webhook" % self.host
         headers = {
             'apikey': self.api_key
         }
         payload = {
-            "answer": answer,
-            "duration": 0
+            "url": webhook_url,
+            "types": types,
+            "secret": secret,
+            "project": project_id
         }
         response = self.session.post(url, headers=headers, json=payload)
-        return response.status_code == 200
-
-    def update_workflow_stages(self, project_id: str, stages: List[dict] = []):
+        return response.json()
 
-        url = "%s/v2/project/%s" % (self.host, project_id)
+    def _annotate(self, task_id: str, answer: dict):
+        url = "%s/v2/annotate/%s?nextStage=true" % (self.host, task_id)
         headers = {
             'apikey': self.api_key
         }
         payload = {
-            "stages": stages
+            "answer": answer,
+            "duration": 0
         }
-
         response = self.session.post(url, headers=headers, json=payload)
-        return response.json()
-
-    def get_task_history(self, id: str = None, task_id: str = None):
-
-        url = None
-        if id:
-            url = "%s/v2/taskHistory/%s" % (self.host, id)
-        elif task_id:
-            url = "%s/v2/task/%s/history" % (self.host, task_id)
-        else:
-            raise Exception("id or task_id should be specified!")
-
-        headers = {
-            'apikey': self.api_key
-        }
-        response = self.session.get(url, headers=headers)
-        return response.json()
+        return response.status_code == 200
```

### Comparing `ango-1.0.9/ango.egg-info/PKG-INFO` & `ango-1.1.0/ango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.9
+Version: 1.1.0
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.9/setup.py` & `ango-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.9",
+    version="1.1.0",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
-        "python-socketio~=5.8.0",
+        "python-socketio~=5.5.2",
         "APScheduler~=3.9.1",
         "websocket-client",
-        "flask-socketio",
+        "flask-socketio~=5.3.4",
         "requests~=2.27.1",
         "tqdm",
         "validators~=0.20.0",
         "boto3~=1.26.30",
     ],
     keywords=['ango', 'ango-hub', "ango sdk", "Ango", "Ango-hub"],
     classifiers=[
```

