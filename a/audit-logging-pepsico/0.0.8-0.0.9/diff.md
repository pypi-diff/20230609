# Comparing `tmp/audit_logging_pepsico-0.0.8.tar.gz` & `tmp/audit_logging_pepsico-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_logging_pepsico-0.0.8.tar", last modified: Fri Jun  9 13:00:40 2023, max compression
+gzip compressed data, was "audit_logging_pepsico-0.0.9.tar", last modified: Fri Jun  9 13:25:48 2023, max compression
```

## Comparing `audit_logging_pepsico-0.0.8.tar` & `audit_logging_pepsico-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:00:40.490443 audit_logging_pepsico-0.0.8/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.8/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:00:40.489405 audit_logging_pepsico-0.0.8/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.8/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:00:40.485904 audit_logging_pepsico-0.0.8/audit_logging_pepsico/
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/Kafka_log.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit_config.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/constants.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     5379 2023-06-09 12:59:55.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico/kafka_utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:00:40.488486 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-06-09 13:00:40.000000 audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-06-09 13:00:20.000000 audit_logging_pepsico-0.0.8/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-09 13:00:40.490827 audit_logging_pepsico-0.0.8/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:25:48.662654 audit_logging_pepsico-0.0.9/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.9/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:25:48.661945 audit_logging_pepsico-0.0.9/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.9/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:25:48.657523 audit_logging_pepsico-0.0.9/audit_logging_pepsico/
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/Kafka_log.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit_config.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/constants.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     5368 2023-06-09 13:25:10.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/kafka_utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:25:48.661061 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-06-09 13:25:33.000000 audit_logging_pepsico-0.0.9/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-09 13:25:48.663075 audit_logging_pepsico-0.0.9/setup.cfg
```

### Comparing `audit_logging_pepsico-0.0.8/LICENSE` & `audit_logging_pepsico-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.8/PKG-INFO` & `audit_logging_pepsico-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit_logging_pepsico
-Version: 0.0.8
+Version: 0.0.9
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.8/README.md` & `audit_logging_pepsico-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.8/audit_logging_pepsico/Kafka_log.py` & `audit_logging_pepsico-0.0.9/audit_logging_pepsico/Kafka_log.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit.py` & `audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.8/audit_logging_pepsico/audit_config.py` & `audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit_config.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.8/audit_logging_pepsico/kafka_utilities.py` & `audit_logging_pepsico-0.0.9/audit_logging_pepsico/kafka_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         logger.error('Exception while connecting Kafka')
         logger.error(str(ex))
         err = str(ex)
     finally:
         if err == "":
             return True, producer
         else:
-            return False, producer
+            return False, err
 
 
 def connect_kafka_consumer(kafka_consumer_config, logger):
     consumer = None
     err = ""
     try:
         consumer = Consumer(kafka_consumer_config)
@@ -39,15 +39,15 @@
         logger.error('Exception while connecting Kafka')
         logger.error(str(ex))
         err = str(ex)
     finally:
         if err == "":
             return True, consumer
         else:
-            return False, consumer
+            return False, err
 
 
 def delivery_callback(err, msg):
     if err:
         print('ERROR: Message failed delivery: {}'.format(err))
     else:
         print("Produced event to topic {topic}: value = {value:12}".format(
@@ -125,8 +125,7 @@
         except Exception as err:
             logger.error("Kafka Consumer Error: " + str(err))
             return False, "Exception: " + str(err)
         finally:
             kafka_consumer.close()
     else:
         return False, kafka_consumer
-
```

### Comparing `audit_logging_pepsico-0.0.8/audit_logging_pepsico.egg-info/PKG-INFO` & `audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit-logging-pepsico
-Version: 0.0.8
+Version: 0.0.9
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.8/pyproject.toml` & `audit_logging_pepsico-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audit_logging_pepsico"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "A logging package which allows users to log in pepsico format. Specially write logs for request and response."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["logging", "audit", "pepsico", "kafka", "couchbase"]
```

