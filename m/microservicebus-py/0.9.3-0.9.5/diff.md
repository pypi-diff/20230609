# Comparing `tmp/microservicebus-py-0.9.3.tar.gz` & `tmp/microservicebus-py-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.3.tar", last modified: Wed Jun  7 20:30:31 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.5.tar", last modified: Fri Jun  9 06:45:29 2023, max compression
```

## Comparing `microservicebus-py-0.9.3.tar` & `microservicebus-py-0.9.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-07 20:30:31.608461 microservicebus-py-0.9.3/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-07 20:30:31.597964 microservicebus-py-0.9.3/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.3/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-07 20:30:30.848069 microservicebus-py-0.9.3/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-07 20:30:30.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-07 20:30:31.611930 microservicebus-py-0.9.3/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.3/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-07 20:30:31.535830 microservicebus-py-0.9.3/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.3/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.3/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.3/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    30492 2023-06-07 20:25:29.000000 microservicebus-py-0.9.3/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.3/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.3/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.3/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.3/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.3/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.3/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.3/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.3/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-09 06:45:29.326264 microservicebus-py-0.9.5/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-09 06:45:29.317804 microservicebus-py-0.9.5/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.5/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-09 06:45:28.646693 microservicebus-py-0.9.5/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-09 06:45:28.000000 microservicebus-py-0.9.5/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-09 06:45:29.329259 microservicebus-py-0.9.5/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.5/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-09 06:45:29.260140 microservicebus-py-0.9.5/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.5/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.5/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1609 2023-06-08 22:01:37.000000 microservicebus-py-0.9.5/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    30523 2023-06-07 20:46:51.000000 microservicebus-py-0.9.5/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-06-09 06:40:37.000000 microservicebus-py-0.9.5/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.5/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.5/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.5/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.5/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.5/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.5/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.5/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.3/PKG-INFO` & `microservicebus-py-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.3
+Version: 0.9.5
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.3/README.md` & `microservicebus-py-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.5/microservicebus_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.3
+Version: 0.9.5
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.3/setup.py` & `microservicebus-py-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/axians.py` & `microservicebus-py-0.9.5/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/base_service.py` & `microservicebus-py-0.9.5/src/base_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/msb_handler.py` & `microservicebus-py-0.9.5/src/msb_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,16 @@
     async def _debug(self, message):
         if "nodeName" in self.settings and self._connected == True:
             self.connection.send("logMessage", [ self.settings["nodeName"], message.message[0], self.settings["organizationId"]])
 
     # endregion
     # region Private methods
     def debug_sync(self, message):
-        asyncio.run(self.Debug(message))
+        self.printf(message)
+        #asyncio.run(self.Debug(message))
 
     def get_settings(self):
         settings = {
             "hubUri": self.base_uri
         }
         # Check if directory exists
         if os.path.isdir(self.msb_dir) == False:
```

### Comparing `microservicebus-py-0.9.3/src/orchestrator_service.py` & `microservicebus-py-0.9.5/src/orchestrator_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         # region
         text = """\033[92m
            _               ____                  _          ____             
  _ __ ___ (_) ___ _ __ ___/ ___|  ___ _ ____   _(_) ___ ___| __ ) _   _ ___  
 | '_ ` _ \\| |/ __| '__/ _ \\___ \\ / _ \\ '__\\ \\ / / |/ __/ _ \\  _ \\| | | / __| 
 | | | | | | | (__| | | (_) |__) |  __/ |   \\ V /| | (_|  __/ |_) | |_| \\__ \\ 
 |_| |_| |_|_|\\___|_|  \\___/____/ \\___|_|    \\_/ |_|\\___\\___|____/ \\__,_|___/ \n\033[1mAXIANS IoT Operations - Python IoT agent\nfor more information visit https://microservicebus.com\n\033[0m"""
-        self.printf(text)
+        await self.Debug(text)
         # endregion
 
         await self.Debug("Started Python Node agent for microServicebus.com")
 
         while self.run:
             try:
                 msg = await self.queue.get()
```

### Comparing `microservicebus-py-0.9.3/src/rauc_handler.py` & `microservicebus-py-0.9.5/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/start.py` & `microservicebus-py-0.9.5/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/terminal_service.py` & `microservicebus-py-0.9.5/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/test.py` & `microservicebus-py-0.9.5/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/utils.py` & `microservicebus-py-0.9.5/src/utils.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.3/src/vpn_helper.py` & `microservicebus-py-0.9.5/src/vpn_helper.py`

 * *Files identical despite different names*

