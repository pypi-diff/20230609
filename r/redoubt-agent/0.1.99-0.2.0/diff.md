# Comparing `tmp/redoubt_agent-0.1.99.tar.gz` & `tmp/redoubt_agent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redoubt_agent-0.1.99.tar", last modified: Wed Jun  7 22:31:00 2023, max compression
+gzip compressed data, was "redoubt_agent-0.2.0.tar", last modified: Fri Jun  9 11:34:00 2023, max compression
```

## Comparing `redoubt_agent-0.1.99.tar` & `redoubt_agent-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:31:00.264026 redoubt_agent-0.1.99/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 22:30:50.000000 redoubt_agent-0.1.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-07 22:31:00.264026 redoubt_agent-0.1.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-07 22:30:50.000000 redoubt_agent-0.1.99/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 22:30:50.000000 redoubt_agent-0.1.99/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:31:00.264026 redoubt_agent-0.1.99/redoubt_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 22:30:50.000000 redoubt_agent-0.1.99/redoubt_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-07 22:30:50.000000 redoubt_agent-0.1.99/redoubt_agent/redoubt_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:31:00.264026 redoubt_agent-0.1.99/redoubt_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-07 22:31:00.000000 redoubt_agent-0.1.99/redoubt_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-07 22:31:00.000000 redoubt_agent-0.1.99/redoubt_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:31:00.000000 redoubt_agent-0.1.99/redoubt_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:31:00.000000 redoubt_agent-0.1.99/redoubt_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 22:31:00.000000 redoubt_agent-0.1.99/redoubt_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 22:31:00.000000 redoubt_agent-0.1.99/redoubt_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-07 22:31:00.268026 redoubt_agent-0.1.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 22:30:50.000000 redoubt_agent-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:34:00.233427 redoubt_agent-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 11:33:50.000000 redoubt_agent-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-09 11:34:00.233427 redoubt_agent-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 11:33:50.000000 redoubt_agent-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 11:33:50.000000 redoubt_agent-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:34:00.233427 redoubt_agent-0.2.0/redoubt_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 11:33:50.000000 redoubt_agent-0.2.0/redoubt_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-09 11:33:50.000000 redoubt_agent-0.2.0/redoubt_agent/redoubt_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:34:00.233427 redoubt_agent-0.2.0/redoubt_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-09 11:34:00.000000 redoubt_agent-0.2.0/redoubt_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 11:34:00.000000 redoubt_agent-0.2.0/redoubt_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:34:00.000000 redoubt_agent-0.2.0/redoubt_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:34:00.000000 redoubt_agent-0.2.0/redoubt_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 11:34:00.000000 redoubt_agent-0.2.0/redoubt_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 11:34:00.000000 redoubt_agent-0.2.0/redoubt_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-09 11:34:00.233427 redoubt_agent-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 11:33:50.000000 redoubt_agent-0.2.0/setup.py
```

### Comparing `redoubt_agent-0.1.99/LICENSE` & `redoubt_agent-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.99/PKG-INFO` & `redoubt_agent-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redoubt_agent
-Version: 0.1.99
+Version: 0.2.0
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
```

### Comparing `redoubt_agent-0.1.99/README.md` & `redoubt_agent-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.99/redoubt_agent/redoubt_sdk.py` & `redoubt_agent-0.2.0/redoubt_agent/redoubt_sdk.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,71 +8,70 @@
 
 from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.requests import RequestsHTTPTransport
 from gql.transport.websockets import WebsocketsTransport
 from loguru import logger
 
-DEFAULT_ENDPOINT = 'wss://graphql.redoubt.online/v1/graphql'
+DEFAULT_DATA_ENDPOINT = 'https://graphql.redoubt.online/v1/graphql'
+DEFAULT_EVENTS_ENDPOINT = 'wss://graphql.redoubt.online/events'
 
 
 class RedoubtEventsStream:
-    def __init__(self, api_key=None, endpoint=DEFAULT_ENDPOINT):
+    def __init__(self, api_key=None, data_endpoint=DEFAULT_DATA_ENDPOINT, events_endpoint=DEFAULT_EVENTS_ENDPOINT):
         if api_key is None:
             api_key = os.environ.get('REDOUBT_API_KEY', None)
         assert api_key is not None, "API key not found"
-        self.transport = WebsocketsTransport(
-            url=endpoint, ping_interval=1, pong_timeout=1, headers={
+        self.events_transport = WebsocketsTransport(
+            url=events_endpoint, ping_interval=1, pong_timeout=1, headers={
+                'X-API-Key': api_key
+            }
+        )
+        self.data_transport = AIOHTTPTransport(
+            url=data_endpoint, headers={
                 'X-API-Key': api_key
             }
         )
 
     async def execute(self, query):
-        async with Client(transport=self.transport, fetch_schema_from_transport=False) as session:
+        async with Client(transport=self.data_transport, fetch_schema_from_transport=False) as session:
             return await session.execute(gql(query))
 
     async def subscribe(self, handler, scope=None, event_type=None, event_target=None):
-        now = datetime.now().astimezone(timezone.utc).strftime(
-            "%Y-%m-%d %H:%M:%S")  # "2023-05-29 12:10:16.051"# int(time.time())
-        logger.info(f"Starting from cursor {now}")
+        logger.info(f"Starting streaming events for filter scope={scope}, type={event_type}, target={event_target}")
         filters = []
         if scope is not None:
-            filters.append("""{event_scope: {_eq: "%s"}}""" % scope)
+            filters.append("""event_scope: "%s" """ % scope)
         if event_type is not None:
-            filters.append("""{event_type: {_eq: "%s"}}""" % event_type)
+            filters.append("""event_type: "%s" """ % event_type)
         if event_target is not None:
-            filters.append("""{event_target: {_eq: "%s"}}""" % event_target)
+            filters.append("""event_target: "%s" """ % event_target)
         if len(filters) == 0:
             filters = ""
         else:
-            filters = "," + ",".join(filters)
+            filters = ",".join(filters)
 
         subscription = gql("""
-            subscription GetEventsStreamStreamingSubscription {
-                redoubt_events (
-                    where: {_and: [
-                        {time: {_gte: "%s"}}
-                        %s
-                    ]}
+            subscription GetEvents {
+                events (%s
                     ) {
+                    data
                     event_id
                     event_scope
                     event_target
                     finding_type
                     event_type
                     severity
-                    data
-                    time
                 }
             }
-        """ % (now, filters))
-        async with Client(transport=self.transport, fetch_schema_from_transport=False) as session:
+        """ % (filters))
+        async with Client(transport=self.events_transport, fetch_schema_from_transport=False) as session:
             async for result in session.subscribe(subscription):
-                for event in result['redoubt_events']:
-                    if event_type is not None and event['event_type'] != event_type:
-                        logger.info(event_type)
-                        continue
-                    event['data'] = json.loads(event['data'])
-                    if inspect.iscoroutinefunction(handler):
-                        await handler(event, session)
-                    else:
-                        handler(event, session)
+                event = result['events']
+                if event_type is not None and event['event_type'] != event_type:
+                    logger.info(event_type)
+                    continue
+                event['data'] = json.loads(event['data'])
+                if inspect.iscoroutinefunction(handler):
+                    await handler(event)
+                else:
+                    handler(event)
```

### Comparing `redoubt_agent-0.1.99/redoubt_agent.egg-info/PKG-INFO` & `redoubt_agent-0.2.0/redoubt_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redoubt-agent
-Version: 0.1.99
+Version: 0.2.0
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
```

### Comparing `redoubt_agent-0.1.99/setup.cfg` & `redoubt_agent-0.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = redoubt_agent
-version = 0.1.99
+version = 0.2.0
 description = re:doubt Bot Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.redoubt.online/
 keywords = TON, redoubt, sdk
 license = Apache 2.0
 classifiers =
```

