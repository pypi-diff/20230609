# Comparing `tmp/osint-python-test-bed-adapter-2.2.4.tar.gz` & `tmp/osint-python-test-bed-adapter-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.2.4.tar", last modified: Wed Jun  7 20:38:14 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.2.5.tar", last modified: Fri Jun  9 13:41:43 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.2.4.tar` & `osint-python-test-bed-adapter-2.2.5.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.4/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1316 2023-04-06 23:36:33.000000 osint-python-test-bed-adapter-2.2.4/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-07 20:37:17.000000 osint-python-test-bed-adapter-2.2.4/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2413 2023-06-01 22:37:01.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2999 2023-06-07 19:48:38.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/http_server.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1064 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)     1873 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1409 2023-06-09 13:23:45.000000 osint-python-test-bed-adapter-2.2.5/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.317409 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1873 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      703 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       39 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       17 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)      758 2023-06-09 13:39:37.000000 osint-python-test-bed-adapter-2.2.5/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.317409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1361 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.327409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/
+-rw-r--r--   0 erik      (1000) erik      (1000)       68 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2246 2023-06-09 13:19:07.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1660 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2999 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2122 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.327409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/
+-rw-r--r--   0 erik      (1000) erik      (1000)       31 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3486 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/
+-rw-r--r--   0 erik      (1000) erik      (1000)       22 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      598 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1005 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.4/LICENSE` & `osint-python-test-bed-adapter-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/PKG-INFO` & `osint-python-test-bed-adapter-2.2.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-Metadata-Version: 2.1
-Name: osint-python-test-bed-adapter
-Version: 2.2.4
-Summary: Python adapter for Kafka
-Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
-Author: TimovdK
-Author-email: timo_kuil@hotmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# NAAS-PYTHON-KAFKA
 
-# naas-python-kafka
+This is the Kafka adapter for Python: it allows you to easily connect Python 
+services to Apache Kafka via Python.
 
-This is the kafka adapter for Python: it allows you to easily connect Python 
-services to Apache Kafka via Python. 
+The implementation is a wrapper around [Confluent-Kafka-Python](https://github.com/confluentinc/confluent-kafka-python):
 
-The implementation is a wrapper around [Confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python) 
-- AVRO schema's and messages: both key's and values should have a schema 
+- AVRO schema's and messages: both key's and values should have a schema.
 as explained [here](https://github.com/DRIVER-EU/avro-schemas).
 - Kafka consumer and producer for the test-bed topics.
 - Management
   - Heartbeat (topic: system-heartbeat), so you know which clients are online.
   Each time the test-bed-adapter is executed, it starts a heartbeat process to notify
   the its activity to other clients.
 
 ## Installation
-You need to install [Python 3+](https://www.python.org/). 
 
-To run the examples you will need to install the dependencies specified on the file [requirements.txt](https://github.com/DRIVER-EU/python-test-bed-adapter/blob/master/requirements.txt)
+You need to install [Python 3+](https://www.python.org/).
+
+To run the examples you will need to install the dependencies specified on the file [requirements.txt](https://github.com/DRIVER-EU/python-test-bed-adapter/blob/master/requirements.txt).
+
 For that, run
-```pip3 install -r requirements.txt```
+
+```bash
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -r requirements.txt # Or instead of `pip`, use `pip3`
+```
+
 from the project folder.
+
 ## Examples and usage
+
 - url_producer: creates a message with 4 URLs to RSS feeds on the topic ('system_rss_urls')
 - rss_producer: listens to url messages ('system_rss_urls') and produces RSS messages ('system_rss_urls')
 - rss_consumer: listens to RSS messages ('system_rss_urls') and prints them to console.
```

### Comparing `osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/PKG-INFO` & `osint-python-test-bed-adapter-2.2.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# naas-python-kafka
+# NAAS-PYTHON-KAFKA
 
-This is the kafka adapter for Python: it allows you to easily connect Python 
-services to Apache Kafka via Python. 
+This is the Kafka adapter for Python: it allows you to easily connect Python 
+services to Apache Kafka via Python.
 
-The implementation is a wrapper around [Confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python) 
-- AVRO schema's and messages: both key's and values should have a schema 
+The implementation is a wrapper around [Confluent-Kafka-Python](https://github.com/confluentinc/confluent-kafka-python):
+
+- AVRO schema's and messages: both key's and values should have a schema.
 as explained [here](https://github.com/DRIVER-EU/avro-schemas).
 - Kafka consumer and producer for the test-bed topics.
 - Management
   - Heartbeat (topic: system-heartbeat), so you know which clients are online.
   Each time the test-bed-adapter is executed, it starts a heartbeat process to notify
   the its activity to other clients.
 
 ## Installation
-You need to install [Python 3+](https://www.python.org/). 
 
-To run the examples you will need to install the dependencies specified on the file [requirements.txt](https://github.com/DRIVER-EU/python-test-bed-adapter/blob/master/requirements.txt)
+You need to install [Python 3+](https://www.python.org/).
+
+To run the examples you will need to install the dependencies specified on the file [requirements.txt](https://github.com/DRIVER-EU/python-test-bed-adapter/blob/master/requirements.txt).
+
 For that, run
-```pip3 install -r requirements.txt```
+
+```bash
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -r requirements.txt # Or instead of `pip`, use `pip3`
+```
+
 from the project folder.
+
 ## Examples and usage
+
 - url_producer: creates a message with 4 URLs to RSS feeds on the topic ('system_rss_urls')
 - rss_producer: listens to url messages ('system_rss_urls') and produces RSS messages ('system_rss_urls')
 - rss_consumer: listens to RSS messages ('system_rss_urls') and prints them to console.
+
+
```

### Comparing `osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,12 +10,10 @@
 test_bed_adapter/kafka/__init__.py
 test_bed_adapter/kafka/consumer_manager.py
 test_bed_adapter/kafka/heartbeat_manager.py
 test_bed_adapter/kafka/log_manager.py
 test_bed_adapter/kafka/producer_manager.py
 test_bed_adapter/options/__init__.py
 test_bed_adapter/options/test_bed_options.py
-test_bed_adapter/services/__init__.py
-test_bed_adapter/services/http_server.py
 test_bed_adapter/utils/__init__.py
 test_bed_adapter/utils/helpers.py
 test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.4/setup.py` & `osint-python-test-bed-adapter-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.2.4",
+    version="2.2.5",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
```

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/consumer_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,15 @@
         consumer_conf = {'bootstrap.servers': self.options.kafka_host,
                          'key.deserializer': self.avro_deserializer,
                          'value.deserializer': self.avro_deserializer,
                          'group.id': self.options.consumer_group,
                          'message.max.bytes': self.options.message_max_bytes,
                          'auto.offset.reset': self.options.offset_type}
         self.consumer = DeserializingConsumer(consumer_conf)
-        if self.options.offset_type == 'earliest':
-            self.consumer.assign([TopicPartition(topic=self.kafka_topic, partition=0, offset=0)])
-        else:
-            self.consumer.subscribe([kafka_topic])
+        self.consumer.subscribe([kafka_topic])
 
     def listen(self):
         _start_time = time.time()
         _latest_message = None
 
         # Ignore messages for a period of time
         while True and self.options.ignore_timeout:
```

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/log_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/producer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/test_bed_options.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

