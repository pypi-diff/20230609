# Comparing `tmp/utf-queue-client-1.9.4.tar.gz` & `tmp/utf-queue-client-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utf-queue-client-1.9.4.tar", last modified: Wed Jan 25 16:33:07 2023, max compression
+gzip compressed data, was "utf-queue-client-1.9.5.tar", last modified: Mon Mar  6 12:55:28 2023, max compression
```

## Comparing `utf-queue-client-1.9.4.tar` & `utf-queue-client-1.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.298243 utf-queue-client-1.9.4/
--rw-r--r--   0 dockerUser   (995)      995      278 2023-01-25 16:33:07.298243 utf-queue-client-1.9.4/PKG-INFO
--rw-r--r--   0 dockerUser   (995)      995        0 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/README.md
--rw-r--r--   0 dockerUser   (995)      995       69 2023-01-25 16:33:07.298243 utf-queue-client-1.9.4/setup.cfg
--rw-r--r--   0 dockerUser   (995)      995     1518 2023-01-25 16:30:58.000000 utf-queue-client-1.9.4/setup.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.290243 utf-queue-client-1.9.4/test/
--rw-r--r--   0 dockerUser   (995)      995      416 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_async_consumer.py
--rw-r--r--   0 dockerUser   (995)      995     1725 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_legacy_base_model.py
--rw-r--r--   0 dockerUser   (995)      995     3685 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_models.py
--rw-r--r--   0 dockerUser   (995)      995     5978 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_opentelemetry_data_producer.py
--rw-r--r--   0 dockerUser   (995)      995     4916 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_publish_test_results.py
--rw-r--r--   0 dockerUser   (995)      995     1321 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_sqa_test_result_producer.py
--rw-r--r--   0 dockerUser   (995)      995     2150 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_ubai_search.py
--rw-r--r--   0 dockerUser   (995)      995     3526 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/test/test_ubai_upload.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.290243 utf-queue-client-1.9.4/utf_queue_client/
--rw-r--r--   0 dockerUser   (995)      995       42 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/__init__.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.294243 utf-queue-client-1.9.4/utf_queue_client/clients/
--rw-r--r--   0 dockerUser   (995)      995     1257 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/clients/__init__.py
--rw-r--r--   0 dockerUser   (995)      995    21649 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/clients/async_consumer.py
--rw-r--r--   0 dockerUser   (995)      995     4737 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/clients/base_producer.py
--rw-r--r--   0 dockerUser   (995)      995     1878 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/clients/opentelemetry_data_producer.py
--rw-r--r--   0 dockerUser   (995)      995     4908 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/clients/sqa_test_result_producer.py
--rw-r--r--   0 dockerUser   (995)      995     4425 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/clients/ubai_artifact_upload_request_producer.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.294243 utf-queue-client-1.9.4/utf_queue_client/exceptions/
--rw-r--r--   0 dockerUser   (995)      995      735 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/exceptions/__init__.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.294243 utf-queue-client-1.9.4/utf_queue_client/models/
--rw-r--r--   0 dockerUser   (995)      995       71 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/models/__init__.py
--rw-r--r--   0 dockerUser   (995)      995     5501 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/models/base_model.py
--rw-r--r--   0 dockerUser   (995)      995      414 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/models/model_factory.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.294243 utf-queue-client-1.9.4/utf_queue_client/models/schemas/
--rw-r--r--   0 dockerUser   (995)      995      510 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/models/schemas/__init__.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.294243 utf-queue-client-1.9.4/utf_queue_client/scripts/
--rw-r--r--   0 dockerUser   (995)      995     3113 2023-01-25 16:30:58.000000 utf-queue-client-1.9.4/utf_queue_client/scripts/__init__.py
--rw-r--r--   0 dockerUser   (995)      995     5063 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/scripts/publish_test_results_cli.py
--rw-r--r--   0 dockerUser   (995)      995     2723 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/scripts/ubai_search_cli.py
--rw-r--r--   0 dockerUser   (995)      995     4178 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/scripts/ubai_upload_cli.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.294243 utf-queue-client-1.9.4/utf_queue_client/utils/
--rw-r--r--   0 dockerUser   (995)      995      603 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/utils/__init__.py
--rw-r--r--   0 dockerUser   (995)      995     2354 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/utils/queue_metrics_exporter.py
--rw-r--r--   0 dockerUser   (995)      995     2541 2023-01-25 16:08:40.000000 utf-queue-client-1.9.4/utf_queue_client/utils/queue_span_exporter.py
-drwxr-xr-x   0 dockerUser   (995)      995        0 2023-01-25 16:33:07.290243 utf-queue-client-1.9.4/utf_queue_client.egg-info/
--rw-r--r--   0 dockerUser   (995)      995      278 2023-01-25 16:33:07.000000 utf-queue-client-1.9.4/utf_queue_client.egg-info/PKG-INFO
--rw-r--r--   0 dockerUser   (995)      995     1345 2023-01-25 16:33:07.000000 utf-queue-client-1.9.4/utf_queue_client.egg-info/SOURCES.txt
--rw-r--r--   0 dockerUser   (995)      995        1 2023-01-25 16:33:07.000000 utf-queue-client-1.9.4/utf_queue_client.egg-info/dependency_links.txt
--rw-r--r--   0 dockerUser   (995)      995      259 2023-01-25 16:33:07.000000 utf-queue-client-1.9.4/utf_queue_client.egg-info/entry_points.txt
--rw-r--r--   0 dockerUser   (995)      995      223 2023-01-25 16:33:07.000000 utf-queue-client-1.9.4/utf_queue_client.egg-info/requires.txt
--rw-r--r--   0 dockerUser   (995)      995       17 2023-01-25 16:33:07.000000 utf-queue-client-1.9.4/utf_queue_client.egg-info/top_level.txt
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.212367 utf-queue-client-1.9.5/
+-rw-r--r--   0 dockerUser   (995)      995      278 2023-03-06 12:55:28.212367 utf-queue-client-1.9.5/PKG-INFO
+-rw-r--r--   0 dockerUser   (995)      995        0 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/README.md
+-rw-r--r--   0 dockerUser   (995)      995       69 2023-03-06 12:55:28.212367 utf-queue-client-1.9.5/setup.cfg
+-rw-r--r--   0 dockerUser   (995)      995     1518 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/setup.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/test/
+-rw-r--r--   0 dockerUser   (995)      995      416 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_async_consumer.py
+-rw-r--r--   0 dockerUser   (995)      995     1725 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_legacy_base_model.py
+-rw-r--r--   0 dockerUser   (995)      995     3685 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_models.py
+-rw-r--r--   0 dockerUser   (995)      995     5978 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_opentelemetry_data_producer.py
+-rw-r--r--   0 dockerUser   (995)      995     4984 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_publish_test_results.py
+-rw-r--r--   0 dockerUser   (995)      995     1321 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_sqa_test_result_producer.py
+-rw-r--r--   0 dockerUser   (995)      995     2150 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_ubai_search.py
+-rw-r--r--   0 dockerUser   (995)      995     3526 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/test/test_ubai_upload.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client/
+-rw-r--r--   0 dockerUser   (995)      995       42 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/__init__.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client/clients/
+-rw-r--r--   0 dockerUser   (995)      995     1257 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/clients/__init__.py
+-rw-r--r--   0 dockerUser   (995)      995    21649 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/clients/async_consumer.py
+-rw-r--r--   0 dockerUser   (995)      995     4737 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/clients/base_producer.py
+-rw-r--r--   0 dockerUser   (995)      995     1878 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/clients/opentelemetry_data_producer.py
+-rw-r--r--   0 dockerUser   (995)      995     4908 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/clients/sqa_test_result_producer.py
+-rw-r--r--   0 dockerUser   (995)      995     4425 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/clients/ubai_artifact_upload_request_producer.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client/exceptions/
+-rw-r--r--   0 dockerUser   (995)      995      735 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/exceptions/__init__.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client/models/
+-rw-r--r--   0 dockerUser   (995)      995       71 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/models/__init__.py
+-rw-r--r--   0 dockerUser   (995)      995     5501 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/models/base_model.py
+-rw-r--r--   0 dockerUser   (995)      995      414 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/models/model_factory.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client/models/schemas/
+-rw-r--r--   0 dockerUser   (995)      995      510 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/models/schemas/__init__.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client/scripts/
+-rw-r--r--   0 dockerUser   (995)      995     3113 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/scripts/__init__.py
+-rw-r--r--   0 dockerUser   (995)      995     5117 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/scripts/publish_test_results_cli.py
+-rw-r--r--   0 dockerUser   (995)      995     2723 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/scripts/ubai_search_cli.py
+-rw-r--r--   0 dockerUser   (995)      995     4178 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/scripts/ubai_upload_cli.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.212367 utf-queue-client-1.9.5/utf_queue_client/utils/
+-rw-r--r--   0 dockerUser   (995)      995      603 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/utils/__init__.py
+-rw-r--r--   0 dockerUser   (995)      995     2354 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/utils/queue_metrics_exporter.py
+-rw-r--r--   0 dockerUser   (995)      995     2541 2023-03-06 12:53:04.000000 utf-queue-client-1.9.5/utf_queue_client/utils/queue_span_exporter.py
+drwxr-xr-x   0 dockerUser   (995)      995        0 2023-03-06 12:55:28.208367 utf-queue-client-1.9.5/utf_queue_client.egg-info/
+-rw-r--r--   0 dockerUser   (995)      995      278 2023-03-06 12:55:28.000000 utf-queue-client-1.9.5/utf_queue_client.egg-info/PKG-INFO
+-rw-r--r--   0 dockerUser   (995)      995     1345 2023-03-06 12:55:28.000000 utf-queue-client-1.9.5/utf_queue_client.egg-info/SOURCES.txt
+-rw-r--r--   0 dockerUser   (995)      995        1 2023-03-06 12:55:28.000000 utf-queue-client-1.9.5/utf_queue_client.egg-info/dependency_links.txt
+-rw-r--r--   0 dockerUser   (995)      995      259 2023-03-06 12:55:28.000000 utf-queue-client-1.9.5/utf_queue_client.egg-info/entry_points.txt
+-rw-r--r--   0 dockerUser   (995)      995      223 2023-03-06 12:55:28.000000 utf-queue-client-1.9.5/utf_queue_client.egg-info/requires.txt
+-rw-r--r--   0 dockerUser   (995)      995       17 2023-03-06 12:55:28.000000 utf-queue-client-1.9.5/utf_queue_client.egg-info/top_level.txt
```

### Comparing `utf-queue-client-1.9.4/setup.py` & `utf-queue-client-1.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "utf-queue-client"
-VERSION = "1.9.4"
+VERSION = "1.9.5"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `utf-queue-client-1.9.4/test/test_legacy_base_model.py` & `utf-queue-client-1.9.5/test/test_legacy_base_model.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/test/test_models.py` & `utf-queue-client-1.9.5/test/test_models.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/test/test_opentelemetry_data_producer.py` & `utf-queue-client-1.9.5/test/test_opentelemetry_data_producer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/test/test_publish_test_results.py` & `utf-queue-client-1.9.5/test/test_publish_test_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         ("branchName", "release/22q3"),
         ("stackName", "WIFI"),
         ("SDKBuildNum", "1111"),
         ("jenkinsServerName", "LOCAL-RUN"),
         ("jenkinRunNum", "1111"),
         ("jenkinsJobName", "LOCAL-RUN"),
         ("jenkinsTestResultsUrl", "LOCAL-RUN"),
+        ("testFramework", "UTF"),
     ]
 
 
 @pytest.fixture
 def session_stop_data():
     yield [
         ("startTime", datetime.now().isoformat()),
@@ -43,14 +44,15 @@
         ("SKIP_cnt", "1"),
         ("BLOCK_cnt", "0"),
         ("jenkinsServerName", "LOCAL-RUN"),
         ("jenkinRunNum", "1111"),
         ("jenkinsJobName", "LOCAL-RUN"),
         ("jenkinsTestResultsUrl", "LOCAL-RUN"),
         ("traceId", "QWERTY12345"),
+        ("testFramework", "UTF"),
     ]
 
 
 @pytest.fixture
 def app_build_results_data():
     yield [
         ("app_name", "queue_client"),
```

### Comparing `utf-queue-client-1.9.4/test/test_sqa_test_result_producer.py` & `utf-queue-client-1.9.5/test/test_sqa_test_result_producer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/test/test_ubai_search.py` & `utf-queue-client-1.9.5/test/test_ubai_search.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/test/test_ubai_upload.py` & `utf-queue-client-1.9.5/test/test_ubai_upload.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/clients/__init__.py` & `utf-queue-client-1.9.5/utf_queue_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/clients/async_consumer.py` & `utf-queue-client-1.9.5/utf_queue_client/clients/async_consumer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/clients/base_producer.py` & `utf-queue-client-1.9.5/utf_queue_client/clients/base_producer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/clients/opentelemetry_data_producer.py` & `utf-queue-client-1.9.5/utf_queue_client/clients/opentelemetry_data_producer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/clients/sqa_test_result_producer.py` & `utf-queue-client-1.9.5/utf_queue_client/clients/sqa_test_result_producer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/clients/ubai_artifact_upload_request_producer.py` & `utf-queue-client-1.9.5/utf_queue_client/clients/ubai_artifact_upload_request_producer.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/exceptions/__init__.py` & `utf-queue-client-1.9.5/utf_queue_client/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/models/base_model.py` & `utf-queue-client-1.9.5/utf_queue_client/models/base_model.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/scripts/__init__.py` & `utf-queue-client-1.9.5/utf_queue_client/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/scripts/publish_test_results_cli.py` & `utf-queue-client-1.9.5/utf_queue_client/scripts/publish_test_results_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,12 +132,13 @@
         FAIL_cnt=data_dict.get("FAIL_cnt"),
         SKIP_cnt=data_dict.get("SKIP_cnt"),
         jenkinsServerName=data_dict.get("jenkinsServerName"),
         jenkinRunNum=data_dict.get("jenkinRunNum"),
         jenkinsJobName=data_dict.get("jenkinsJobName"),
         jenkinsTestResultsUrl=data_dict.get("jenkinsTestResultsUrl"),
         traceId=data_dict.get("traceId"),
+        testFramework=data_dict.get("testFramework"),
     )
 
 
 if __name__ == "__main__":
     cli_entrypoint()
```

### Comparing `utf-queue-client-1.9.4/utf_queue_client/scripts/ubai_search_cli.py` & `utf-queue-client-1.9.5/utf_queue_client/scripts/ubai_search_cli.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/scripts/ubai_upload_cli.py` & `utf-queue-client-1.9.5/utf_queue_client/scripts/ubai_upload_cli.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/utils/__init__.py` & `utf-queue-client-1.9.5/utf_queue_client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/utils/queue_metrics_exporter.py` & `utf-queue-client-1.9.5/utf_queue_client/utils/queue_metrics_exporter.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client/utils/queue_span_exporter.py` & `utf-queue-client-1.9.5/utf_queue_client/utils/queue_span_exporter.py`

 * *Files identical despite different names*

### Comparing `utf-queue-client-1.9.4/utf_queue_client.egg-info/SOURCES.txt` & `utf-queue-client-1.9.5/utf_queue_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

