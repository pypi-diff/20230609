# Comparing `tmp/audit_logging_pepsico-0.0.7.tar.gz` & `tmp/audit_logging_pepsico-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_logging_pepsico-0.0.7.tar", last modified: Fri Jun  9 12:15:28 2023, max compression
+gzip compressed data, was "audit_logging_pepsico-0.0.8.tar", last modified: Fri Jun  9 13:00:40 2023, max compression
```

## Comparing `audit_logging_pepsico-0.0.7.tar` & `audit_logging_pepsico-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 12:15:28.211511 audit_logging_pepsico-0.0.7/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.7/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 12:15:28.211158 audit_logging_pepsico-0.0.7/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.7/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 12:15:28.207822 audit_logging_pepsico-0.0.7/audit_logging_pepsico/
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/Kafka_log.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit_config.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/constants.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     5219 2023-06-09 12:12:14.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/kafka_utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 12:15:28.210345 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-06-09 12:15:13.000000 audit_logging_pepsico-0.0.7/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-09 12:15:28.211633 audit_logging_pepsico-0.0.7/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:00:40.490443 audit_logging_pepsico-0.0.8/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.8/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:00:40.489405 audit_logging_pepsico-0.0.8/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.8/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:00:40.485904 audit_logging_pepsico-0.0.8/audit_logging_pepsico/
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/Kafka_log.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit_config.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/constants.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     5379 2023-06-09 12:59:55.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/kafka_utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:00:40.488486 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-06-09 13:00:20.000000 audit_logging_pepsico-0.0.8/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-09 13:00:40.490827 audit_logging_pepsico-0.0.8/setup.cfg
```

### Comparing `audit_logging_pepsico-0.0.7/LICENSE` & `audit_logging_pepsico-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.7/PKG-INFO` & `audit_logging_pepsico-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit_logging_pepsico
-Version: 0.0.7
+Version: 0.0.8
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.7/README.md` & `audit_logging_pepsico-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.7/audit_logging_pepsico/Kafka_log.py` & `audit_logging_pepsico-0.0.8/audit_logging_pepsico/Kafka_log.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit.py` & `audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit_config.py` & `audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit_config.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.7/audit_logging_pepsico/kafka_utilities.py` & `audit_logging_pepsico-0.0.8/audit_logging_pepsico/kafka_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,34 +12,42 @@
 from couchbase.diagnostics import ServiceType
 import base64
 import time
 
 
 def connect_kafka_producer(kafka_producer_config, logger):
     producer = None
+    err = ""
     try:
         producer = Producer(kafka_producer_config)
     except Exception as ex:
         logger.error('Exception while connecting Kafka')
         logger.error(str(ex))
-        return False, str(ex)
+        err = str(ex)
     finally:
-        return True, producer
+        if err == "":
+            return True, producer
+        else:
+            return False, producer
 
 
 def connect_kafka_consumer(kafka_consumer_config, logger):
     consumer = None
+    err = ""
     try:
         consumer = Consumer(kafka_consumer_config)
     except Exception as ex:
         logger.error('Exception while connecting Kafka')
         logger.error(str(ex))
-        return False, str(ex)
+        err = str(ex)
     finally:
-        return True, consumer
+        if err == "":
+            return True, consumer
+        else:
+            return False, consumer
 
 
 def delivery_callback(err, msg):
     if err:
         print('ERROR: Message failed delivery: {}'.format(err))
     else:
         print("Produced event to topic {topic}: value = {value:12}".format(
```

### Comparing `audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/PKG-INFO` & `audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit-logging-pepsico
-Version: 0.0.7
+Version: 0.0.8
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.7/pyproject.toml` & `audit_logging_pepsico-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audit_logging_pepsico"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "A logging package which allows users to log in pepsico format. Specially write logs for request and response."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["logging", "audit", "pepsico", "kafka", "couchbase"]
```

