# Comparing `tmp/audit_logging_pepsico-0.0.6.tar.gz` & `tmp/audit_logging_pepsico-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_logging_pepsico-0.0.6.tar", last modified: Sun May 21 21:14:09 2023, max compression
+gzip compressed data, was "audit_logging_pepsico-0.0.7.tar", last modified: Fri Jun  9 12:15:28 2023, max compression
```

## Comparing `audit_logging_pepsico-0.0.6.tar` & `audit_logging_pepsico-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-21 21:14:09.753518 audit_logging_pepsico-0.0.6/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.6/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-05-21 21:14:09.752870 audit_logging_pepsico-0.0.6/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.6/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-21 21:14:09.748998 audit_logging_pepsico-0.0.6/audit_logging_pepsico/
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/Kafka_log.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit_config.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/constants.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     4901 2023-05-18 10:09:56.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/kafka_utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-21 21:14:09.751963 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-05-21 21:11:33.000000 audit_logging_pepsico-0.0.6/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-21 21:14:09.753790 audit_logging_pepsico-0.0.6/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 12:15:28.211511 audit_logging_pepsico-0.0.7/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.7/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 12:15:28.211158 audit_logging_pepsico-0.0.7/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.7/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 12:15:28.207822 audit_logging_pepsico-0.0.7/audit_logging_pepsico/
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/Kafka_log.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit_config.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/constants.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     5219 2023-06-09 12:12:14.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico/kafka_utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 12:15:28.210345 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-06-09 12:15:28.000000 audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-06-09 12:15:13.000000 audit_logging_pepsico-0.0.7/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-09 12:15:28.211633 audit_logging_pepsico-0.0.7/setup.cfg
```

### Comparing `audit_logging_pepsico-0.0.6/LICENSE` & `audit_logging_pepsico-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.6/PKG-INFO` & `audit_logging_pepsico-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit_logging_pepsico
-Version: 0.0.6
+Version: 0.0.7
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.6/README.md` & `audit_logging_pepsico-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.6/audit_logging_pepsico/Kafka_log.py` & `audit_logging_pepsico-0.0.7/audit_logging_pepsico/Kafka_log.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit.py` & `audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit_config.py` & `audit_logging_pepsico-0.0.7/audit_logging_pepsico/audit_config.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.6/audit_logging_pepsico/kafka_utilities.py` & `audit_logging_pepsico-0.0.7/audit_logging_pepsico/kafka_utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,37 +7,39 @@
                                ClusterTimeoutOptions,
                                QueryOptions,
                                WaitUntilReadyOptions)
 from couchbase.auth import PasswordAuthenticator
 from datetime import timedelta
 from couchbase.diagnostics import ServiceType
 import base64
-import time 
+import time
 
 
 def connect_kafka_producer(kafka_producer_config, logger):
     producer = None
     try:
         producer = Producer(kafka_producer_config)
     except Exception as ex:
         logger.error('Exception while connecting Kafka')
         logger.error(str(ex))
+        return False, str(ex)
     finally:
-        return producer
+        return True, producer
 
 
 def connect_kafka_consumer(kafka_consumer_config, logger):
     consumer = None
     try:
         consumer = Consumer(kafka_consumer_config)
     except Exception as ex:
         logger.error('Exception while connecting Kafka')
         logger.error(str(ex))
+        return False, str(ex)
     finally:
-        return consumer
+        return True, consumer
 
 
 def delivery_callback(err, msg):
     if err:
         print('ERROR: Message failed delivery: {}'.format(err))
     else:
         print("Produced event to topic {topic}: value = {value:12}".format(
@@ -49,33 +51,32 @@
         kafka_producer.produce(kafka_topic, audit_log_str, callback=delivery_callback)
         kafka_producer.poll(10000)
         kafka_producer.flush()
         return True, "Kafka Audit logs produced successfully"
     except Exception as err:
         logger.info("Kafka Producer Error: " + str(err))
         return False, "Exception: " + str(err)
-    
 
 
 def couchbase_insert_logs(couchbase_config, doc, logger):
     try:
         key = doc["componentName"] + " " + doc["createdDate"]
         conn_str = couchbase_config["conn_str"]
         cb_username = couchbase_config["cb_username"]
         cb_password = couchbase_config["cb_password"]
         cb_password = base64.b64decode(cb_password.encode('utf-8')).decode('utf-8')
         bucket_name = couchbase_config["bucket_name"]
         auth = PasswordAuthenticator(cb_username, cb_password)
         timeout_opts = ClusterTimeoutOptions(connect_timeout=timedelta(seconds=20),
-                                         kv_timeout=timedelta(seconds=20))
+                                             kv_timeout=timedelta(seconds=20))
         options = ClusterOptions(auth, timeout_options=timeout_opts)
         # options = ClusterOptions(auth)
         cluster = Cluster.connect(conn_str, options)
         cluster.wait_until_ready(timedelta(seconds=10),
-             WaitUntilReadyOptions(service_types=[ServiceType.KeyValue, ServiceType.Query]))
+                                 WaitUntilReadyOptions(service_types=[ServiceType.KeyValue, ServiceType.Query]))
         logger.info("Cluster ==== \n" + str(cluster))
         bucket = cluster.bucket(bucket_name)
         logger.info("Bucket ==== " + str(bucket))
         coll = bucket.default_collection()
         logger.info("Colle === " + str(coll))
         res = coll.upsert(key, doc)
         logger.info("upsert res === " + str(res.cas))
@@ -84,37 +85,40 @@
         return True, res
     except Exception as err:
         logger.error("Exception in couchbase: " + str(err))
         return False, "Exception: " + str(err)
 
 
 def kafka_consume_logs(kafka_consumer_config, kafka_topic, couchbase_config, logger, duration):
-    kafka_consumer = connect_kafka_consumer(kafka_consumer_config, logger)
-    kafka_consumer.subscribe([kafka_topic])
-    try:
-        t_end = time.time() + duration
-        while time.time() < t_end:
-            msg = kafka_consumer.poll(1.0)
-            logger.info("Consumer Message: " + str(msg))
-            if msg is not None and msg.error() is None:
-                logger.info("Kafka Topic: " + str(msg.topic()))
-                logger.info("Kafka Message Value: " + str(json.loads(msg.value())))
-                msg_value = json.loads(msg.value())
-                couchbase_resp_status, coucbase_resp_msg = couchbase_insert_logs(couchbase_config, msg_value, logger)
-                if couchbase_resp_status:
-                    logger.info("Kafka Log is consumed and inserted in Couchbase")
-                else:
-                    logger.error(coucbase_resp_msg)
-                    return False, coucbase_resp_msg
-            elif msg is not None and msg.error() is not None:
-                logger.error("Kafka Consumer Error: " + str(msg.error()))
-                return False, "Error: " + str(msg.error())
-        return True, "Kafka Audit Logs Consumed Successfully"
-    except KeyboardInterrupt:
-        kafka_consumer.close()
-        return True, "Kafka Consumer Stopped Successfully"
-    except Exception as err:
-        logger.error("Kafka Consumer Error: " + str(err))
-        return False, "Exception: " + str(err)
-    finally:
-        kafka_consumer.close()
+    kafka_consumer_connect_status, kafka_consumer = connect_kafka_consumer(kafka_consumer_config, logger)
+    if kafka_consumer_connect_status:
+        kafka_consumer.subscribe([kafka_topic])
+        try:
+            t_end = time.time() + duration
+            while time.time() < t_end:
+                msg = kafka_consumer.poll(1.0)
+                logger.info("Consumer Message: " + str(msg))
+                if msg is not None and msg.error() is None:
+                    logger.info("Kafka Topic: " + str(msg.topic()))
+                    logger.info("Kafka Message Value: " + str(json.loads(msg.value())))
+                    msg_value = json.loads(msg.value())
+                    couchbase_resp_status, coucbase_resp_msg = couchbase_insert_logs(couchbase_config, msg_value, logger)
+                    if couchbase_resp_status:
+                        logger.info("Kafka Log is consumed and inserted in Couchbase")
+                    else:
+                        logger.error(coucbase_resp_msg)
+                        return False, coucbase_resp_msg
+                elif msg is not None and msg.error() is not None:
+                    logger.error("Kafka Consumer Error: " + str(msg.error()))
+                    return False, "Error: " + str(msg.error())
+            return True, "Kafka Audit Logs Consumed Successfully"
+        except KeyboardInterrupt:
+            kafka_consumer.close()
+            return True, "Kafka Consumer Stopped Successfully"
+        except Exception as err:
+            logger.error("Kafka Consumer Error: " + str(err))
+            return False, "Exception: " + str(err)
+        finally:
+            kafka_consumer.close()
+    else:
+        return False, kafka_consumer
```

### Comparing `audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/PKG-INFO` & `audit_logging_pepsico-0.0.7/audit_logging_pepsico.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit-logging-pepsico
-Version: 0.0.6
+Version: 0.0.7
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.6/pyproject.toml` & `audit_logging_pepsico-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audit_logging_pepsico"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "A logging package which allows users to log in pepsico format. Specially write logs for request and response."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["logging", "audit", "pepsico", "kafka", "couchbase"]
```

