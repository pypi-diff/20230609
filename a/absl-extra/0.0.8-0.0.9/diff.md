# Comparing `tmp/absl_extra-0.0.8.tar.gz` & `tmp/absl_extra-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.8.tar", last modified: Sat May  6 22:23:13 2023, max compression
+gzip compressed data, was "absl_extra-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.8.tar` & `absl_extra-0.0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1299 2023-05-06 22:23:04.204153 absl_extra-0.0.8/Readme.md
--rw-r--r--   0        0        0     6326 2023-05-06 22:23:04.204153 absl_extra-0.0.8/absl_extra.py
--rw-r--r--   0        0        0      689 2023-05-06 22:23:04.204153 absl_extra-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 absl_extra-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1253 2023-05-29 17:58:37.926290 absl_extra-0.0.9/Readme.md
+-rw-r--r--   0        0        0     6322 2023-05-29 17:58:37.926290 absl_extra-0.0.9/absl_extra.py
+-rw-r--r--   0        0        0      689 2023-05-29 17:58:37.926290 absl_extra-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1941 1970-01-01 00:00:00.000000 absl_extra-0.0.9/PKG-INFO
```

### Comparing `absl_extra-0.0.8/Readme.md` & `absl_extra-0.0.9/Readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 Minimal example
 
 ```python
 import os
 from pymongo.collection import Collection
 from ml_collections import ConfigDict
 from absl import logging
-from absl_extra import register_task, SlackBaseNotifier, MongoConfig, run
+from absl_extra import register_task, SlackNotifier, MongoConfig, run
 
 
 @register_task
 def main(config: ConfigDict, db: Collection) -> None:
-    logging.info("Doing some heavy lifting...")
+  logging.info("Doing some heavy lifting...")
 
 
 if __name__ == "__main__":
-    run(
-        config_file="config.py",
-        mongo_config=MongoConfig(
-            uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
-        ),
-        notifier=SlackBaseNotifier(
-            slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
-        ),
-    )
+  run(
+    config_file="config.py",
+    mongo_config=MongoConfig(
+      uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
+    ),
+    notifier=SlackNotifier(
+      slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+    ),
+  )
 ```
```

### Comparing `absl_extra-0.0.8/absl_extra.py` & `absl_extra-0.0.9/absl_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def notify_job_failed(self, name: str, exception: Exception):
         logging.fatal(f"Job {name} failed", exc_info=exception)
 
 
 if util.find_spec("slack_sdk"):
     import slack_sdk
 
-    class SlackBaseNotifier(BaseNotifier):
+    class SlackNotifier(BaseNotifier):
         def __init__(self, slack_token: str, channel_id: str):
             self.slack_token = slack_token
             self.channel_id = channel_id
 
         def notify_job_started(self, name: str):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
```

### Comparing `absl_extra-0.0.8/pyproject.toml` & `absl_extra-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.8"
+version = "0.0.9"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.8/PKG-INFO` & `absl_extra-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.8
+Version: 0.0.9
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
@@ -33,27 +33,27 @@
 Minimal example
 
 ```python
 import os
 from pymongo.collection import Collection
 from ml_collections import ConfigDict
 from absl import logging
-from absl_extra import register_task, SlackBaseNotifier, MongoConfig, run
+from absl_extra import register_task, SlackNotifier, MongoConfig, run
 
 
 @register_task
 def main(config: ConfigDict, db: Collection) -> None:
-    logging.info("Doing some heavy lifting...")
+  logging.info("Doing some heavy lifting...")
 
 
 if __name__ == "__main__":
-    run(
-        config_file="config.py",
-        mongo_config=MongoConfig(
-            uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
-        ),
-        notifier=SlackBaseNotifier(
-            slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
-        ),
-    )
+  run(
+    config_file="config.py",
+    mongo_config=MongoConfig(
+      uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
+    ),
+    notifier=SlackNotifier(
+      slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+    ),
+  )
 ```
```

