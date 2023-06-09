# Comparing `tmp/RobertCommonIO-0.1.41.tar.gz` & `tmp/RobertCommonIO-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonIO-0.1.41.tar", last modified: Tue Jun  6 03:34:24 2023, max compression
+gzip compressed data, was "RobertCommonIO-0.1.42.tar", last modified: Fri Jun  9 09:56:56 2023, max compression
```

## Comparing `RobertCommonIO-0.1.41.tar` & `RobertCommonIO-0.1.42.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.088274 RobertCommonIO-0.1.41/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.41/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.41/MANIFEST.in
--rw-rw-rw-   0        0        0      878 2023-06-06 03:34:24.087273 RobertCommonIO-0.1.41/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-02 07:57:14.000000 RobertCommonIO-0.1.41/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.029368 RobertCommonIO-0.1.41/RobertCommonIO.egg-info/
--rw-rw-rw-   0        0        0      878 2023-06-06 03:34:23.000000 RobertCommonIO-0.1.41/RobertCommonIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2023-06-06 03:34:23.000000 RobertCommonIO-0.1.41/RobertCommonIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 03:34:23.000000 RobertCommonIO-0.1.41/RobertCommonIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-06-06 03:34:23.000000 RobertCommonIO-0.1.41/RobertCommonIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-06 03:34:23.000000 RobertCommonIO-0.1.41/RobertCommonIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      281 2023-05-25 09:15:35.000000 RobertCommonIO-0.1.41/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.031382 RobertCommonIO-0.1.41/robertcommonio/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.41/robertcommonio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.032398 RobertCommonIO-0.1.41/robertcommonio/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.41/robertcommonio/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.060436 RobertCommonIO-0.1.41/robertcommonio/system/io/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/__init__.py
--rw-rw-rw-   0        0        0    19281 2023-04-04 06:29:48.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/data_storage.py
--rw-rw-rw-   0        0        0     3336 2023-06-06 03:31:50.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/email.py
--rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/file.py
--rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/ftp.py
--rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/http.py
--rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/ini.py
--rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/license.py
--rw-rw-rw-   0        0        0    27197 2023-05-18 07:23:32.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/mongo.py
--rw-rw-rw-   0        0        0     6883 2023-05-16 09:34:00.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/mqtt.py
--rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/mysql.py
--rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/oss.py
--rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/rabitmq.py
--rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/redis.py
--rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/redis_cache.py
--rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/response.py
--rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/socket.py
--rw-rw-rw-   0        0        0     7249 2023-05-26 06:26:38.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/sqlalche.py
--rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/transport.py
--rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.41/robertcommonio/system/io/version.py
--rw-rw-rw-   0        0        0       42 2023-06-06 03:34:24.088274 RobertCommonIO-0.1.41/setup.cfg
--rw-rw-rw-   0        0        0     3869 2023-06-06 03:06:42.000000 RobertCommonIO-0.1.41/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.061471 RobertCommonIO-0.1.41/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.41/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.062477 RobertCommonIO-0.1.41/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.41/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:34:24.086275 RobertCommonIO-0.1.41/tests/test_system/test_io/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test.py
--rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_data_storage.py
--rw-rw-rw-   0        0        0    14345 2023-06-06 02:41:30.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_email.py
--rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_file.py
--rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_ftp.py
--rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_http.py
--rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_ini.py
--rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_license.py
--rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_mongo.py
--rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_mqtt.py
--rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_oracle.py
--rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_rabbitmq.py
--rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_socket.py
--rw-rw-rw-   0        0        0     3967 2023-06-02 08:41:38.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_sqlalche.py
--rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.41/tests/test_system/test_io/test_transport.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.698934 RobertCommonIO-0.1.42/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.42/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.42/MANIFEST.in
+-rw-rw-rw-   0        0        0      878 2023-06-09 09:56:56.698934 RobertCommonIO-0.1.42/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-06-02 07:57:14.000000 RobertCommonIO-0.1.42/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.653400 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/
+-rw-rw-rw-   0        0        0      878 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1703 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      250 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      275 2023-06-09 09:31:22.000000 RobertCommonIO-0.1.42/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.654400 RobertCommonIO-0.1.42/robertcommonio/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.42/robertcommonio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.655400 RobertCommonIO-0.1.42/robertcommonio/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.42/robertcommonio/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.676688 RobertCommonIO-0.1.42/robertcommonio/system/io/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/__init__.py
+-rw-rw-rw-   0        0        0    19281 2023-04-04 06:29:48.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/data_storage.py
+-rw-rw-rw-   0        0        0     3336 2023-06-06 03:31:50.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/email.py
+-rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/file.py
+-rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/ftp.py
+-rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/http.py
+-rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/ini.py
+-rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/license.py
+-rw-rw-rw-   0        0        0    27538 2023-06-08 15:33:06.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/mongo.py
+-rw-rw-rw-   0        0        0     6883 2023-05-16 09:34:00.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/mqtt.py
+-rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/mysql.py
+-rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/oss.py
+-rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/rabitmq.py
+-rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/redis.py
+-rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/redis_cache.py
+-rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/response.py
+-rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/socket.py
+-rw-rw-rw-   0        0        0     7249 2023-05-26 06:26:38.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/sqlalche.py
+-rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/transport.py
+-rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:56:56.698934 RobertCommonIO-0.1.42/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-06-09 09:33:34.000000 RobertCommonIO-0.1.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.678681 RobertCommonIO-0.1.42/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.42/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.678681 RobertCommonIO-0.1.42/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.42/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.696911 RobertCommonIO-0.1.42/tests/test_system/test_io/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test.py
+-rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_data_storage.py
+-rw-rw-rw-   0        0        0    14345 2023-06-06 02:41:30.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_email.py
+-rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_file.py
+-rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_ftp.py
+-rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_http.py
+-rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_ini.py
+-rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_license.py
+-rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_mongo.py
+-rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_mqtt.py
+-rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_oracle.py
+-rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_rabbitmq.py
+-rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_socket.py
+-rw-rw-rw-   0        0        0     3967 2023-06-02 08:41:38.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_sqlalche.py
+-rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_transport.py
```

### Comparing `RobertCommonIO-0.1.41/LICENSE` & `RobertCommonIO-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/PKG-INFO` & `RobertCommonIO-0.1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.41
+Version: 0.1.42
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.41/RobertCommonIO.egg-info/PKG-INFO` & `RobertCommonIO-0.1.42/RobertCommonIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.41
+Version: 0.1.42
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.41/RobertCommonIO.egg-info/SOURCES.txt` & `RobertCommonIO-0.1.42/RobertCommonIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/data_storage.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/email.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/file.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/ftp.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/http.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/http.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/ini.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/license.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/mongo.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,21 @@
             kwargs['sort'] = sort
         if session:
             kwargs['session'] = session
         with coll.find(filter=query, **kwargs) as cursor:
             for doc in cursor:
                 yield doc
 
+    def count(self, coll_name: str, query: dict, projection: Optional[dict] = None, tz_info: Optional[str] = None) -> Iterator[dict]:
+        coll = self._get_coll(coll_name, tz_info)
+        kwargs = {}
+        if projection:
+            kwargs['projection'] = projection
+        return coll.count_documents(filter=query, **kwargs)
+
     def aggr(self, coll_name: str, pipeline: List, allow_disk_use: bool = False, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> Iterator[dict]:
         coll = self._get_coll(coll_name, tz_info)
         with coll.aggregate(pipeline, allowDiskUse=allow_disk_use, session=session) as cursor:
             for doc in cursor:
                 yield doc
 
     def insert_many(self, coll_name: str, docs: List[dict], session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> InsertManyResult:
```

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/mqtt.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/mysql.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/mysql.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/oss.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/oss.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/rabitmq.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/rabitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/redis.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/redis.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/redis_cache.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/redis_cache.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/response.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/response.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/socket.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/sqlalche.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/transport.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/transport.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/robertcommonio/system/io/version.py` & `RobertCommonIO-0.1.42/robertcommonio/system/io/version.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/setup.py` & `RobertCommonIO-0.1.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonIO'
 DESCRIPTION = 'Robert Common IO Library'
 URL = 'https://github.com/hun0423/RobertCommonIO'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.41'
-DATE = '2023-06-06'
+VERSION = '0.1.42'
+DATE = '2023-06-09'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_data_storage.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_email.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_file.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_ftp.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_license.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_mongo.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_mongo.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_mqtt.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_oracle.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_oracle.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_rabbitmq.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_socket.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_sqlalche.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.41/tests/test_system/test_io/test_transport.py` & `RobertCommonIO-0.1.42/tests/test_system/test_io/test_transport.py`

 * *Files identical despite different names*

