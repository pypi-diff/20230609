# Comparing `tmp/cove_unified_logs-0.1.6.tar.gz` & `tmp/cove_unified_logs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cove_unified_logs-0.1.6.tar", last modified: Thu Jun  8 21:32:08 2023, max compression
+gzip compressed data, was "cove_unified_logs-0.1.7.tar", last modified: Fri Jun  9 12:55:42 2023, max compression
```

## Comparing `cove_unified_logs-0.1.6.tar` & `cove_unified_logs-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 21:32:08.766795 cove_unified_logs-0.1.6/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.1.6/LICENSE
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 21:32:08.766685 cove_unified_logs-0.1.6/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.1.6/README.md
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 21:32:08.765748 cove_unified_logs-0.1.6/cove_unified_logs/
--rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 20:52:43.000000 cove_unified_logs-0.1.6/cove_unified_logs/__init__.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6059 2023-06-08 21:21:58.000000 cove_unified_logs-0.1.6/cove_unified_logs/cloud_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2204 2023-06-08 21:30:17.000000 cove_unified_logs-0.1.6/cove_unified_logs/console_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2219 2023-06-08 19:37:52.000000 cove_unified_logs-0.1.6/cove_unified_logs/log_consumer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2112 2023-06-08 20:15:13.000000 cove_unified_logs-0.1.6/cove_unified_logs/log_producer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.6/cove_unified_logs/middleware.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      247 2023-06-08 20:52:38.000000 cove_unified_logs-0.1.6/cove_unified_logs/singleton.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1583 2023-06-08 21:26:58.000000 cove_unified_logs-0.1.6/cove_unified_logs/unified_logger.py
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 21:32:08.766520 cove_unified_logs-0.1.6/cove_unified_logs.egg-info/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 21:32:08.000000 cove_unified_logs-0.1.6/cove_unified_logs.egg-info/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)      497 2023-06-08 21:32:08.000000 cove_unified_logs-0.1.6/cove_unified_logs.egg-info/SOURCES.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 21:32:08.000000 cove_unified_logs-0.1.6/cove_unified_logs.egg-info/dependency_links.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 21:32:08.000000 cove_unified_logs-0.1.6/cove_unified_logs.egg-info/requires.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 21:32:08.000000 cove_unified_logs-0.1.6/cove_unified_logs.egg-info/top_level.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 21:32:08.766834 cove_unified_logs-0.1.6/setup.cfg
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 21:31:42.000000 cove_unified_logs-0.1.6/setup.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-09 12:55:42.805212 cove_unified_logs-0.1.7/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.1.7/LICENSE
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-09 12:55:42.805068 cove_unified_logs-0.1.7/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.1.7/README.md
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-09 12:55:42.803863 cove_unified_logs-0.1.7/cove_unified_logs/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 20:52:43.000000 cove_unified_logs-0.1.7/cove_unified_logs/__init__.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6059 2023-06-08 21:21:58.000000 cove_unified_logs-0.1.7/cove_unified_logs/cloud_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2204 2023-06-08 21:30:17.000000 cove_unified_logs-0.1.7/cove_unified_logs/console_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2219 2023-06-08 19:37:52.000000 cove_unified_logs-0.1.7/cove_unified_logs/log_consumer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2112 2023-06-08 20:15:13.000000 cove_unified_logs-0.1.7/cove_unified_logs/log_producer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      884 2023-06-09 12:54:56.000000 cove_unified_logs-0.1.7/cove_unified_logs/middleware.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      247 2023-06-08 20:52:38.000000 cove_unified_logs-0.1.7/cove_unified_logs/singleton.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1583 2023-06-08 21:26:58.000000 cove_unified_logs-0.1.7/cove_unified_logs/unified_logger.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-09 12:55:42.804779 cove_unified_logs-0.1.7/cove_unified_logs.egg-info/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-09 12:55:42.000000 cove_unified_logs-0.1.7/cove_unified_logs.egg-info/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      497 2023-06-09 12:55:42.000000 cove_unified_logs-0.1.7/cove_unified_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-09 12:55:42.000000 cove_unified_logs-0.1.7/cove_unified_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-09 12:55:42.000000 cove_unified_logs-0.1.7/cove_unified_logs.egg-info/requires.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-09 12:55:42.000000 cove_unified_logs-0.1.7/cove_unified_logs.egg-info/top_level.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-09 12:55:42.805290 cove_unified_logs-0.1.7/setup.cfg
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-09 12:55:32.000000 cove_unified_logs-0.1.7/setup.py
```

### Comparing `cove_unified_logs-0.1.6/LICENSE` & `cove_unified_logs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/PKG-INFO` & `cove_unified_logs-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove_unified_logs
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.1.6/README.md` & `cove_unified_logs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs/cloud_logger.py` & `cove_unified_logs-0.1.7/cove_unified_logs/cloud_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs/console_logger.py` & `cove_unified_logs-0.1.7/cove_unified_logs/console_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs/log_consumer.py` & `cove_unified_logs-0.1.7/cove_unified_logs/log_consumer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs/log_producer.py` & `cove_unified_logs-0.1.7/cove_unified_logs/log_producer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs/middleware.py` & `cove_unified_logs-0.1.7/cove_unified_logs/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+# middleware.py
 from django.utils.deprecation import MiddlewareMixin
 from django.conf import settings
-from your_module import UnifiedLogger
 from django.apps import apps
-
+from .unified_logger import UnifiedLogger
 
 class LoggingMiddleware(MiddlewareMixin):
     def __init__(self, get_response):
         self.get_response = get_response
         self.app_name = apps.get_app_config(__package__.split('.')[0]).verbose_name
         self.logger = UnifiedLogger(self.app_name, config='all')
         self.logger.set_level(settings.LOG_LEVEL)
```

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs/unified_logger.py` & `cove_unified_logs-0.1.7/cove_unified_logs/unified_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.6/cove_unified_logs.egg-info/PKG-INFO` & `cove_unified_logs-0.1.7/cove_unified_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove-unified-logs
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.1.6/setup.py` & `cove_unified_logs-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cove_unified_logs',
-    version='0.1.6',
+    version='0.1.7',
     description='A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Coveidentity Tech Private Limited',
     author_email='sarvpriye.soni@coveidentity.com',
     url='https://github.com/Cove-Identity/cove-unified-logs',
     packages=['cove_unified_logs'],
```

