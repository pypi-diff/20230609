# Comparing `tmp/twitter-api-client-0.9.4.tar.gz` & `tmp/twitter-api-client-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.4.tar", last modified: Wed Jun  7 20:58:11 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.5.tar", last modified: Fri Jun  9 19:55:08 2023, max compression
```

## Comparing `twitter-api-client-0.9.4.tar` & `twitter-api-client-0.9.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.4/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-07 20:58:11.739655 twitter-api-client-0.9.4/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-07 20:57:15.000000 twitter-api-client-0.9.4/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.4/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23528 2023-06-07 19:13:05.000000 twitter-api-client-0.9.4/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28740 2023-06-07 20:57:15.000000 twitter-api-client-0.9.4/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.4/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    33428 2023-06-07 20:57:15.000000 twitter-api-client-0.9.4/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6127 2023-06-07 19:13:05.000000 twitter-api-client-0.9.4/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.4/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-09 19:55:08.049420 twitter-api-client-0.9.5/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.5/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-09 19:55:08.048420 twitter-api-client-0.9.5/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-09 19:55:08.049420 twitter-api-client-0.9.5/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-09 19:54:08.000000 twitter-api-client-0.9.5/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-09 19:55:08.048420 twitter-api-client-0.9.5/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.5/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23626 2023-06-09 19:50:48.000000 twitter-api-client-0.9.5/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28718 2023-06-09 19:44:07.000000 twitter-api-client-0.9.5/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.5/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    33526 2023-06-09 19:47:45.000000 twitter-api-client-0.9.5/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6225 2023-06-09 19:50:48.000000 twitter-api-client-0.9.5/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.5/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-09 19:55:08.048420 twitter-api-client-0.9.5/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.4/LICENSE` & `twitter-api-client-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.4/PKG-INFO` & `twitter-api-client-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.9.4/setup.py` & `twitter-api-client-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.4",
+    version="0.9.5",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.9.4/twitter/account.py` & `twitter-api-client-0.9.5/twitter/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,20 +559,23 @@
     @staticmethod
     def _init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
             logging.config.dictConfig(LOGGER_CONFIG)
 
-        # Set level of all other loggers to ERROR
+        # only support one logger
+        logger_name = list(LOGGER_CONFIG['loggers'].keys())[0]
+
+        # set level of all other loggers to ERROR
         for name in logging.root.manager.loggerDict:
-            if name != LOGGER_NAME:
+            if name != logger_name:
                 logging.getLogger(name).setLevel(logging.ERROR)
 
-        return logging.getLogger(LOGGER_NAME)
+        return logging.getLogger(logger_name)
 
     @staticmethod
     def _validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
```

### Comparing `twitter-api-client-0.9.4/twitter/constants.py` & `twitter-api-client-0.9.5/twitter/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 BLUE = '\x1b[34m'
 MAGENTA = '\x1b[35m'
 CYAN = '\x1b[36m'
 WHITE = '\x1b[37m'
 BOLD = '\x1b[1m'
 RESET = '\x1b[0m'
 
-LOGGER_NAME = 'twitter'
 LOGGER_CONFIG = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
             'format': '%(asctime)s.%(msecs)03d [%(levelname)s] :: %(message)s',
             'datefmt': '%Y-%m-%d %H:%M:%S'
@@ -36,20 +35,20 @@
             'formatter': 'standard',
             'stream': 'ext://sys.stdout',
         },
         'file': {
             'class': 'logging.FileHandler',
             'level': 'DEBUG',
             'formatter': 'standard',
-            'filename': 'log.log',
+            'filename': 'twitter.log',
             'mode': 'a',
         },
     },
     'loggers': {
-        LOGGER_NAME: {
+        'twitter': {
             'handlers': ['console', 'file'],
             'level': 'DEBUG',
         }
     }
 }
 
 ID_MAP = {
```

### Comparing `twitter-api-client-0.9.4/twitter/login.py` & `twitter-api-client-0.9.5/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.4/twitter/scraper.py` & `twitter-api-client-0.9.5/twitter/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -773,20 +773,23 @@
     @staticmethod
     def _init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
             logging.config.dictConfig(LOGGER_CONFIG)
 
-        # Set level of all other loggers to ERROR
+        # only support one logger
+        logger_name = list(LOGGER_CONFIG['loggers'].keys())[0]
+
+        # set level of all other loggers to ERROR
         for name in logging.root.manager.loggerDict:
-            if name != LOGGER_NAME:
+            if name != logger_name:
                 logging.getLogger(name).setLevel(logging.ERROR)
 
-        return logging.getLogger(LOGGER_NAME)
+        return logging.getLogger(logger_name)
 
     def _validate_session(self, *args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
         if not session:
```

### Comparing `twitter-api-client-0.9.4/twitter/search.py` & `twitter-api-client-0.9.5/twitter/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,20 +137,23 @@
     @staticmethod
     def _init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
             logging.config.dictConfig(LOGGER_CONFIG)
 
-        # Set level of all other loggers to ERROR
+        # only support one logger
+        logger_name = list(LOGGER_CONFIG['loggers'].keys())[0]
+
+        # set level of all other loggers to ERROR
         for name in logging.root.manager.loggerDict:
-            if name != LOGGER_NAME:
+            if name != logger_name:
                 logging.getLogger(name).setLevel(logging.ERROR)
 
-        return logging.getLogger(LOGGER_NAME)
+        return logging.getLogger(logger_name)
 
     @staticmethod
     def _validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
```

### Comparing `twitter-api-client-0.9.4/twitter/util.py` & `twitter-api-client-0.9.5/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.4/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.5/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

