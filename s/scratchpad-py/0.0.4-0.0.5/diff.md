# Comparing `tmp/scratchpad-py-0.0.4.tar.gz` & `tmp/scratchpad-py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchpad-py-0.0.4.tar", last modified: Wed Feb 22 07:11:26 2023, max compression
+gzip compressed data, was "scratchpad-py-0.0.5.tar", last modified: Fri Jun  9 09:04:22 2023, max compression
```

## Comparing `scratchpad-py-0.0.4.tar` & `scratchpad-py-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-22 07:11:26.461955 scratchpad-py-0.0.4/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-02-17 01:58:03.000000 scratchpad-py-0.0.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3333 2023-02-22 07:11:26.457054 scratchpad-py-0.0.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2884 2023-02-17 01:58:03.000000 scratchpad-py-0.0.4/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-22 07:11:26.422196 scratchpad-py-0.0.4/scratchpad/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-02-17 01:58:03.000000 scratchpad-py-0.0.4/scratchpad/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1414 2023-02-22 06:41:45.000000 scratchpad-py-0.0.4/scratchpad/composite_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      650 2023-02-22 06:42:20.000000 scratchpad-py-0.0.4/scratchpad/console_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      635 2023-02-22 06:42:57.000000 scratchpad-py-0.0.4/scratchpad/file_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1202 2023-02-22 07:02:55.000000 scratchpad-py-0.0.4/scratchpad/fluent_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-02-22 06:32:15.000000 scratchpad-py-0.0.4/scratchpad/jandi_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      835 2023-02-22 07:03:25.000000 scratchpad-py-0.0.4/scratchpad/line_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-02-22 07:03:59.000000 scratchpad-py-0.0.4/scratchpad/logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-02-22 03:08:03.000000 scratchpad-py-0.0.4/scratchpad/logger_impl.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2023-02-22 07:03:50.000000 scratchpad-py-0.0.4/scratchpad/logger_interface.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      260 2023-02-22 07:04:40.000000 scratchpad-py-0.0.4/scratchpad/memory_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      130 2023-02-22 07:04:47.000000 scratchpad-py-0.0.4/scratchpad/null_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       23 2023-02-17 01:58:03.000000 scratchpad-py-0.0.4/scratchpad/retry.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1703 2023-02-22 07:05:09.000000 scratchpad-py-0.0.4/scratchpad/scribe_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      941 2023-02-22 07:05:38.000000 scratchpad-py-0.0.4/scratchpad/telegram_logger.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-22 07:11:26.451933 scratchpad-py-0.0.4/scratchpad_py.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3333 2023-02-22 07:11:26.000000 scratchpad-py-0.0.4/scratchpad_py.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-02-22 07:11:26.000000 scratchpad-py-0.0.4/scratchpad_py.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-22 07:11:26.000000 scratchpad-py-0.0.4/scratchpad_py.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       80 2023-02-22 07:11:26.000000 scratchpad-py-0.0.4/scratchpad_py.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-02-22 07:11:26.000000 scratchpad-py-0.0.4/scratchpad_py.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-02-22 07:11:26.463358 scratchpad-py-0.0.4/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-02-22 06:38:38.000000 scratchpad-py-0.0.4/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-09 09:04:22.247809 scratchpad-py-0.0.5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3333 2023-06-09 09:04:22.246159 scratchpad-py-0.0.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2884 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-09 09:04:22.199780 scratchpad-py-0.0.5/scratchpad/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/scratchpad/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1433 2023-06-09 09:01:35.000000 scratchpad-py-0.0.5/scratchpad/composite_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      650 2023-02-22 06:42:20.000000 scratchpad-py-0.0.5/scratchpad/console_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      635 2023-02-22 06:42:57.000000 scratchpad-py-0.0.5/scratchpad/file_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1465 2023-06-09 09:01:35.000000 scratchpad-py-0.0.5/scratchpad/fluent_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-02-22 06:32:15.000000 scratchpad-py-0.0.5/scratchpad/jandi_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      835 2023-02-22 07:03:25.000000 scratchpad-py-0.0.5/scratchpad/line_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-02-22 07:03:59.000000 scratchpad-py-0.0.5/scratchpad/logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-02-22 03:08:03.000000 scratchpad-py-0.0.5/scratchpad/logger_impl.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2023-02-22 07:03:50.000000 scratchpad-py-0.0.5/scratchpad/logger_interface.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      260 2023-02-22 07:04:40.000000 scratchpad-py-0.0.5/scratchpad/memory_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      130 2023-02-22 07:04:47.000000 scratchpad-py-0.0.5/scratchpad/null_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       23 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/scratchpad/retry.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1703 2023-02-22 07:05:09.000000 scratchpad-py-0.0.5/scratchpad/scribe_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      941 2023-02-22 07:05:38.000000 scratchpad-py-0.0.5/scratchpad/telegram_logger.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-09 09:04:22.241278 scratchpad-py-0.0.5/scratchpad_py.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3333 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       80 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-09 09:04:22.248803 scratchpad-py-0.0.5/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-06-09 09:01:42.000000 scratchpad-py-0.0.5/setup.py
```

### Comparing `scratchpad-py-0.0.4/LICENSE` & `scratchpad-py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/PKG-INFO` & `scratchpad-py-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchpad-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: python logger libary
 Home-page: https://github.com/chirichidi/scratch-pad-py
 Author: chirichidi
 Author-email: tolessnoise@gmail.com
 Keywords: logger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scratchpad-py-0.0.4/README.md` & `scratchpad-py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/__init__.py` & `scratchpad-py-0.0.5/scratchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/composite_logger.py` & `scratchpad-py-0.0.5/scratchpad/composite_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             option = {}
 
         mergedMessage = {}
         if len(self.config["defaults"]) > 0:
             mergedMessage: dict = copy.deepcopy(self.config["defaults"])
             for k, v in mergedMessage.items():
                 if callable(v):
-                    v()
+                    mergedMessage[k] = v()
         
         mergedMessage.update(message)
 
         for loggerFilterParis in self.config["loggerFilterPairs"]:
             logger: LoggerInterface = loggerFilterParis["logger"]
             filter_ = loggerFilterParis["filter"]
```

### Comparing `scratchpad-py-0.0.4/scratchpad/console_logger.py` & `scratchpad-py-0.0.5/scratchpad/console_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/file_logger.py` & `scratchpad-py-0.0.5/scratchpad/file_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/fluent_logger.py` & `scratchpad-py-0.0.5/scratchpad/fluent_logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .logger_impl import LoggerImpl
-
+import socket
 
+from .logger_impl import LoggerImpl
 from fluent import sender
 
 class FluentLogger(LoggerImpl):
     def __init__(self, config: dict = None):
         if config is None:
             config = {}
 
@@ -15,35 +15,41 @@
             config["port"] = 24224
 
         if "tag" not in config:
             config["tag"] = "scratch-pad-python"
             
         self.config = config
         self.client = None
+        self.check_connection()
 
 
     def log(self, message: dict, option: dict = None):
         if option is None:
             option = {}
         if self.client is None:
             self.client = sender.FluentSender(self.config["tag"], host=self.config["host"], port=self.config["port"])
-        
-        if "label" not in option:
-            option["label"] = "test"
 
-        return self.client.emit(option["label"], message)
+        return self.client.emit(option.get("label"), message)
 
 
     def __del__(self):
         try:
             self.client.close()
             self.client = None
         except:
             pass
 
+    def check_connection(self):
+        try:
+            timeout = 5
+            socket.setdefaulttimeout(timeout)
+            socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect((self.config["host"], self.config["port"]))
+        except ConnectionRefusedError as e:
+            raise e
+
 
 if __name__ == "__main__":
     logger = FluentLogger()
 
     message = {
             "type": "fluent",
             "message": "hello world"
```

### Comparing `scratchpad-py-0.0.4/scratchpad/jandi_logger.py` & `scratchpad-py-0.0.5/scratchpad/jandi_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/line_logger.py` & `scratchpad-py-0.0.5/scratchpad/line_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/logger.py` & `scratchpad-py-0.0.5/scratchpad/logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/logger_impl.py` & `scratchpad-py-0.0.5/scratchpad/logger_impl.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/logger_interface.py` & `scratchpad-py-0.0.5/scratchpad/logger_interface.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/scribe_logger.py` & `scratchpad-py-0.0.5/scratchpad/scribe_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad/telegram_logger.py` & `scratchpad-py-0.0.5/scratchpad/telegram_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/scratchpad_py.egg-info/PKG-INFO` & `scratchpad-py-0.0.5/scratchpad_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchpad-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: python logger libary
 Home-page: https://github.com/chirichidi/scratch-pad-py
 Author: chirichidi
 Author-email: tolessnoise@gmail.com
 Keywords: logger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scratchpad-py-0.0.4/scratchpad_py.egg-info/SOURCES.txt` & `scratchpad-py-0.0.5/scratchpad_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.4/setup.py` & `scratchpad-py-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_descriprion = f.read()
 
 setuptools.setup(
     name             = 'scratchpad-py',
-    version          = '0.0.4',
+    version          = '0.0.5',
     description      = 'python logger libary',
     long_description = long_descriprion,
     long_description_content_type = "text/markdown",
     author           = 'chirichidi',
     author_email     = 'tolessnoise@gmail.com',
     url              = "https://github.com/chirichidi/scratch-pad-py",
     packages         = ["scratchpad"],
```

