# Comparing `tmp/sensory_cloud-1.0.3.tar.gz` & `tmp/sensory_cloud-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensory_cloud-1.0.3.tar", last modified: Tue May  2 13:35:40 2023, max compression
+gzip compressed data, was "sensory_cloud-1.2.2.tar", last modified: Fri Jun  9 16:26:02 2023, max compression
```

## Comparing `sensory_cloud-1.0.3.tar` & `sensory_cloud-1.2.2.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.036136 sensory_cloud-1.0.3/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    11357 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/LICENSE.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)       24 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/MANIFEST.in
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-05-02 13:35:40.035353 sensory_cloud-1.0.3/PKG-INFO
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      948 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/README.md
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/requirements.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)       38 2023-05-02 13:35:40.036548 sensory_cloud-1.0.3/setup.cfg
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      740 2023-05-02 12:48:44.000000 sensory_cloud-1.0.3/setup.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.978559 sensory_cloud-1.0.3/src/
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.989224 sensory_cloud-1.0.3/src/sensory_cloud/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2799 2023-05-02 13:20:01.000000 sensory_cloud-1.0.3/src/sensory_cloud/config.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.992920 sensory_cloud-1.0.3/src/sensory_cloud/generated/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/__init__.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.994446 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    59354 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/common_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/common_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.996389 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2976 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2592 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.998243 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    15147 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     8049 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.998940 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/__init__.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.001145 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     8671 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2827 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.003533 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)   125215 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    18777 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.005836 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    37387 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     8197 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.007820 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    24268 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     7750 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.011634 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    26140 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    13034 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    43642 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    18293 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.014717 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    52347 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     9870 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.017110 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)   113401 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/validate_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/validate_pb2_grpc.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    12350 2023-05-02 13:35:32.000000 sensory_cloud-1.0.3/src/sensory_cloud/initializer.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.024253 sensory_cloud-1.0.3/src/sensory_cloud/services/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    25738 2023-02-28 14:22:02.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/audio_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      642 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/crypto_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1253 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/health_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     6001 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/management_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     9735 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/oauth_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    11253 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/video_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2170 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/token_manager.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.992243 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/PKG-INFO
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2664 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        1 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/requires.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)       14 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.033724 sensory_cloud-1.0.3/test/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    23719 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_audio_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      638 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_crypto_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1450 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_health_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     6780 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_management_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    10159 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_oauth_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     3756 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_token_manager.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    10951 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_video_service.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:02.018498 sensory_cloud-1.2.2/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    11357 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/LICENSE.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)       24 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/MANIFEST.in
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-06-09 16:26:02.017667 sensory_cloud-1.2.2/PKG-INFO
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      948 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/README.md
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/requirements.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)       38 2023-06-09 16:26:02.019098 sensory_cloud-1.2.2/setup.cfg
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      740 2023-05-31 14:28:34.000000 sensory_cloud-1.2.2/setup.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.950183 sensory_cloud-1.2.2/src/
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.960571 sensory_cloud-1.2.2/src/sensory_cloud/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2799 2023-05-16 14:26:39.000000 sensory_cloud-1.2.2/src/sensory_cloud/config.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.964831 sensory_cloud-1.2.2/src/sensory_cloud/generated/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/__init__.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.966640 sensory_cloud-1.2.2/src/sensory_cloud/generated/common/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/common/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    59801 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/common/common_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/common/common_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.968635 sensory_cloud-1.2.2/src/sensory_cloud/generated/health/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/health/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2976 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/health/health_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2592 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/health/health_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.971031 sensory_cloud-1.2.2/src/sensory_cloud/generated/oauth/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/oauth/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    15147 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/oauth/oauth_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     8049 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.971947 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/__init__.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.974019 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/assistant/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/assistant/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     8671 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2827 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.976703 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/audio/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/audio/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)   126683 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/audio/audio_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    18777 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.980691 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/event/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/event/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    37849 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/event/event_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     8197 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.983174 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/file/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/file/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    24268 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/file/file_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     7750 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.987533 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    26140 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/device_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    13034 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    43642 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/enrollment_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    18293 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.989865 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/video/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/video/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    52347 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/video/video_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     9870 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.993744 sensory_cloud-1.2.2/src/sensory_cloud/generated/validate/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/validate/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)   113401 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/validate/validate_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-05-31 14:12:07.000000 sensory_cloud-1.2.2/src/sensory_cloud/generated/validate/validate_pb2_grpc.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    12350 2023-05-16 14:26:39.000000 sensory_cloud-1.2.2/src/sensory_cloud/initializer.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:02.004606 sensory_cloud-1.2.2/src/sensory_cloud/services/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2179 2023-06-01 15:01:18.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/assistant_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    26147 2023-06-09 16:11:47.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/audio_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      642 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/crypto_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1253 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/health_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     6001 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/management_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     9735 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/oauth_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    11253 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/services/video_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2170 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/src/sensory_cloud/token_manager.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:01.963967 sensory_cloud-1.2.2/src/sensory_cloud.egg-info/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-06-09 16:26:01.000000 sensory_cloud-1.2.2/src/sensory_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2712 2023-06-09 16:26:01.000000 sensory_cloud-1.2.2/src/sensory_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        1 2023-06-09 16:26:01.000000 sensory_cloud-1.2.2/src/sensory_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-06-09 16:26:01.000000 sensory_cloud-1.2.2/src/sensory_cloud.egg-info/requires.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)       14 2023-06-09 16:26:01.000000 sensory_cloud-1.2.2/src/sensory_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-06-09 16:26:02.015904 sensory_cloud-1.2.2/test/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    23719 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_audio_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      638 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_crypto_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1450 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_health_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     6780 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_management_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    10159 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_oauth_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     3756 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_token_manager.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    10951 2023-02-08 16:23:22.000000 sensory_cloud-1.2.2/test/test_video_service.py
```

### Comparing `sensory_cloud-1.0.3/LICENSE.txt` & `sensory_cloud-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/PKG-INFO` & `sensory_cloud-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensory_cloud
-Version: 1.0.3
+Version: 1.2.2
 Summary: Python SDK for Sensory Cloud
 Home-page: https://github.com/Sensory-Cloud/python-sdk
 Author: Jonathan Hersch
 Author-email: jhersch@sensoryinc.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `sensory_cloud-1.0.3/README.md` & `sensory_cloud-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/setup.py` & `sensory_cloud-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = requirements_txt.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sensory_cloud",
-    version="1.0.3",
+    version="1.2.2",
     description="Python SDK for Sensory Cloud",
     author="Jonathan Hersch",
     author_email="jhersch@sensoryinc.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=requirements,
     python_requires='>=3.6',
```

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/config.py` & `sensory_cloud-1.2.2/src/sensory_cloud/config.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/common/common_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/common/common_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='common/common.proto',
   package='sensory.api.common',
   syntax='proto3',
   serialized_options=b'\n\032ai.sensorycloud.api.commonB\025SensoryApiCommonProtoP\001Z8gitlab.com/sensory-cloud/server/titan.git/pkg/api/common\242\002\004SENG',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x13\x63ommon/common.proto\x12\x12sensory.api.common\x1a\x17validate/validate.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"U\n\x18\x43ompressionConfiguration\x12\x39\n\x0c\x63ompressions\x18\x01 \x03(\x0e\x32#.sensory.api.common.CompressionType\"Y\n\rTokenResponse\x12\x13\n\x0b\x61\x63\x63\x65ssToken\x18\x01 \x01(\t\x12\x11\n\texpiresIn\x18\x02 \x01(\x05\x12\r\n\x05keyId\x18\x03 \x01(\t\x12\x11\n\ttokenType\x18\x04 \x01(\t\"A\n\rServiceHealth\x12\x11\n\tisHealthy\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xc7\x01\n\x14ServerHealthResponse\x12\x11\n\tisHealthy\x18\x01 \x01(\x08\x12\x15\n\rserverVersion\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x33\n\x08services\x18\x04 \x03(\x0b\x32!.sensory.api.common.ServiceHealth\x12\x32\n\nserverType\x18\x05 \x01(\x0e\x32\x1e.sensory.api.common.ServerType\x12\x10\n\x08isLeader\x18\x06 \x01(\x08\"\x83\x01\n\rSystemSummary\x12\x35\n\x03\x63pu\x18\x01 \x01(\x0b\x32\x1e.sensory.api.common.CpuSummaryB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12;\n\x06memory\x18\x02 \x01(\x0b\x32!.sensory.api.common.MemorySummaryB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"\xa5\x01\n\nCpuSummary\x12\x0c\n\x04user\x18\x01 \x01(\x04\x12\x0c\n\x04nice\x18\x02 \x01(\x04\x12\x0e\n\x06system\x18\x03 \x01(\x04\x12\x0c\n\x04idle\x18\x04 \x01(\x04\x12\x0e\n\x06ioWait\x18\x05 \x01(\x04\x12\x0b\n\x03irq\x18\x06 \x01(\x04\x12\x0f\n\x07softIrq\x18\x07 \x01(\x04\x12\r\n\x05steal\x18\x08 \x01(\x04\x12\r\n\x05guest\x18\t \x01(\x04\x12\x11\n\tguestNice\x18\n \x01(\x04\"H\n\rMemorySummary\x12\x10\n\x08memTotal\x18\x01 \x01(\x04\x12\x0f\n\x07memFree\x18\x02 \x01(\x04\x12\x14\n\x0cmemAvailable\x18\x03 \x01(\x04\"D\n\rGenericClient\x12\x1a\n\x08\x63lientId\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01\x12\x17\n\x06secret\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\n\"\x88\x01\n\x0eTenantResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12-\n\tcreatedAt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tupdatedAt\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"]\n\x11PaginationOptions\x12\x10\n\x08ordering\x18\x01 \x01(\t\x12\x11\n\tdecending\x18\x02 \x01(\x08\x12\x11\n\tpageIndex\x18\x03 \x01(\x05\x12\x10\n\x08pageSize\x18\x04 \x01(\x05\"\xc2\x01\n\x12PaginationResponse\x12\x10\n\x08ordering\x18\x01 \x01(\t\x12\x11\n\tdecending\x18\x02 \x01(\x08\x12\x19\n\x11possibleOrderings\x18\x03 \x03(\t\x12\x12\n\ntotalCount\x18\x04 \x01(\x03\x12\x10\n\x08pageSize\x18\x05 \x01(\x05\x12\x15\n\rprevPageIndex\x18\x06 \x01(\x05\x12\x18\n\x10\x63urrentPageIndex\x18\x07 \x01(\x05\x12\x15\n\rnextPageIndex\x18\x08 \x01(\x05\"4\n\x0f\x45nrollmentToken\x12\r\n\x05token\x18\x01 \x01(\x0c\x12\x12\n\nexpiration\x18\x02 \x01(\x03\"\x86\x01\n\x10\x43reateKeyRequest\x12\x17\n\x04name\x18\x01 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x36\n\x07keyType\x18\x02 \x01(\x0e\x32\x1b.sensory.api.common.KeyTypeB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\r\n\x05value\x18\x03 \x01(\t\x12\x12\n\nexpiration\x18\x04 \x01(\x03\"\x8d\x01\n\x0bKeyResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12,\n\x07keyType\x18\x03 \x01(\x0e\x32\x1b.sensory.api.common.KeyType\x12\x12\n\nexpiration\x18\x04 \x01(\x03\x12\x10\n\x08tenantId\x18\x05 \x01(\t\x12\x10\n\x08\x64isabled\x18\x06 \x01(\x08*\x16\n\x04Void\x12\x0e\n\nVOID_VALUE\x10\x00*Q\n\x07KeyType\x12\x0e\n\nPUBLIC_KEY\x10\x00\x12\x16\n\x12PUBLIC_KEY_ED25519\x10\x01\x12\x11\n\rSHARED_SECRET\x10\x03\x12\x0b\n\x07\x41\x45S_256\x10\x04*4\n\x0b\x46\x65\x61tureFlag\x12\x0c\n\x08TSSV_ALL\x10\x00\x12\n\n\x06TS_ALL\x10\x01\x12\x0b\n\x07TNL_ALL\x10\x02*\xb9\x04\n\tModelType\x12\x0b\n\x07UNKNOWN\x10\x00\x12$\n VOICE_BIOMETRIC_TEXT_INDEPENDENT\x10\x01\x12\x1c\n\x18VOICE_BIOMETRIC_WAKEWORD\x10\x02\x12\x18\n\x14VOICE_EVENT_WAKEWORD\x10\x03\x12\x1c\n\x18VOICE_TRANSCRIBE_GRAMMAR\x10\x04\x12\'\n#VOICE_TRANSCRIBE_COMMAND_AND_SEARCH\x10\x05\x12(\n$VOICE_RECOGNITION_ACTIVITY_DETECTION\x10\x06\x12\x1b\n\x17VOICE_FEATURE_EXTRACTOR\x10\x07\x12\"\n\x1eVOICE_BIOMETRIC_LIVENESS_DIGIT\x10\x08\x12\"\n\x1eVOICE_BIOMETRIC_TEXT_DEPENDENT\x10\t\x12\x13\n\x0fVOICE_SYNTHESIS\x10\n\x12\x1a\n\x16SOUND_EVENT_ENROLLABLE\x10\x64\x12\x1c\n\x18SOUND_EVENT_REVALIDATION\x10\x65\x12\x15\n\x11SOUND_EVENT_FIXED\x10\x66\x12\x15\n\x11SOUND_SCENE_FIXED\x10g\x12\x13\n\x0e\x46\x41\x43\x45_BIOMETRIC\x10\xc9\x01\x12\x15\n\x10\x46\x41\x43\x45_RECOGNITION\x10\xca\x01\x12\x17\n\x12OBJECT_RECOGNITION\x10\xcb\x01\x12\x14\n\x0fIMAGE_TRANSFORM\x10\xcc\x01\x12\x13\n\x0e\x46\x41\x43\x45_EMBEDDING\x10\xcd\x01*X\n\x0eTechnologyType\x12\x0b\n\x07NOT_SET\x10\x00\x12\x08\n\x04TSSV\x10\x01\x12\x06\n\x02TS\x10\x02\x12\x07\n\x03TNL\x10\x03\x12\x07\n\x03STT\x10\x04\x12\x07\n\x03TTS\x10\x05\x12\x0c\n\x08SOUND_ID\x10\x06*&\n\x0f\x43ompressionType\x12\x13\n\x0fIMAGE_GRAYSCALE\x10\x00*|\n\nClientType\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06\x44\x45VICE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x08\n\x04USER\x10\x03\x12\x0e\n\nSUPER_USER\x10\x04\x12\x10\n\x0c\x42ILLING_USER\x10\x05\x12\x12\n\x0eREAD_ONLY_USER\x10\x06\x12\x08\n\x04ROOT\x10\x64*g\n\x0eUsageEventType\x12\x12\n\x0e\x41UTHENTICATION\x10\x00\x12\x0f\n\x0bRECOGNITION\x10\x01\x12\x0e\n\nENROLLMENT\x10\x02\x12\r\n\tSYNTHESIS\x10\x03\x12\x11\n\rTRANSCRIPTION\x10\x04*\x1f\n\nServerType\x12\t\n\x05TITAN\x10\x00\x12\x06\n\x02IO\x10\x01\x42v\n\x1a\x61i.sensorycloud.api.commonB\x15SensoryApiCommonProtoP\x01Z8gitlab.com/sensory-cloud/server/titan.git/pkg/api/common\xa2\x02\x04SENGb\x06proto3'
+  serialized_pb=b'\n\x13\x63ommon/common.proto\x12\x12sensory.api.common\x1a\x17validate/validate.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"U\n\x18\x43ompressionConfiguration\x12\x39\n\x0c\x63ompressions\x18\x01 \x03(\x0e\x32#.sensory.api.common.CompressionType\"Y\n\rTokenResponse\x12\x13\n\x0b\x61\x63\x63\x65ssToken\x18\x01 \x01(\t\x12\x11\n\texpiresIn\x18\x02 \x01(\x05\x12\r\n\x05keyId\x18\x03 \x01(\t\x12\x11\n\ttokenType\x18\x04 \x01(\t\"A\n\rServiceHealth\x12\x11\n\tisHealthy\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xc7\x01\n\x14ServerHealthResponse\x12\x11\n\tisHealthy\x18\x01 \x01(\x08\x12\x15\n\rserverVersion\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x33\n\x08services\x18\x04 \x03(\x0b\x32!.sensory.api.common.ServiceHealth\x12\x32\n\nserverType\x18\x05 \x01(\x0e\x32\x1e.sensory.api.common.ServerType\x12\x10\n\x08isLeader\x18\x06 \x01(\x08\"\x83\x01\n\rSystemSummary\x12\x35\n\x03\x63pu\x18\x01 \x01(\x0b\x32\x1e.sensory.api.common.CpuSummaryB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12;\n\x06memory\x18\x02 \x01(\x0b\x32!.sensory.api.common.MemorySummaryB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"\xa5\x01\n\nCpuSummary\x12\x0c\n\x04user\x18\x01 \x01(\x04\x12\x0c\n\x04nice\x18\x02 \x01(\x04\x12\x0e\n\x06system\x18\x03 \x01(\x04\x12\x0c\n\x04idle\x18\x04 \x01(\x04\x12\x0e\n\x06ioWait\x18\x05 \x01(\x04\x12\x0b\n\x03irq\x18\x06 \x01(\x04\x12\x0f\n\x07softIrq\x18\x07 \x01(\x04\x12\r\n\x05steal\x18\x08 \x01(\x04\x12\r\n\x05guest\x18\t \x01(\x04\x12\x11\n\tguestNice\x18\n \x01(\x04\"H\n\rMemorySummary\x12\x10\n\x08memTotal\x18\x01 \x01(\x04\x12\x0f\n\x07memFree\x18\x02 \x01(\x04\x12\x14\n\x0cmemAvailable\x18\x03 \x01(\x04\"D\n\rGenericClient\x12\x1a\n\x08\x63lientId\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01\x12\x17\n\x06secret\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\n\"\x88\x01\n\x0eTenantResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12-\n\tcreatedAt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tupdatedAt\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"]\n\x11PaginationOptions\x12\x10\n\x08ordering\x18\x01 \x01(\t\x12\x11\n\tdecending\x18\x02 \x01(\x08\x12\x11\n\tpageIndex\x18\x03 \x01(\x05\x12\x10\n\x08pageSize\x18\x04 \x01(\x05\"\xc2\x01\n\x12PaginationResponse\x12\x10\n\x08ordering\x18\x01 \x01(\t\x12\x11\n\tdecending\x18\x02 \x01(\x08\x12\x19\n\x11possibleOrderings\x18\x03 \x03(\t\x12\x12\n\ntotalCount\x18\x04 \x01(\x03\x12\x10\n\x08pageSize\x18\x05 \x01(\x05\x12\x15\n\rprevPageIndex\x18\x06 \x01(\x05\x12\x18\n\x10\x63urrentPageIndex\x18\x07 \x01(\x05\x12\x15\n\rnextPageIndex\x18\x08 \x01(\x05\"4\n\x0f\x45nrollmentToken\x12\r\n\x05token\x18\x01 \x01(\x0c\x12\x12\n\nexpiration\x18\x02 \x01(\x03\"\x86\x01\n\x10\x43reateKeyRequest\x12\x17\n\x04name\x18\x01 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x36\n\x07keyType\x18\x02 \x01(\x0e\x32\x1b.sensory.api.common.KeyTypeB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\r\n\x05value\x18\x03 \x01(\t\x12\x12\n\nexpiration\x18\x04 \x01(\x03\"\x8d\x01\n\x0bKeyResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12,\n\x07keyType\x18\x03 \x01(\x0e\x32\x1b.sensory.api.common.KeyType\x12\x12\n\nexpiration\x18\x04 \x01(\x03\x12\x10\n\x08tenantId\x18\x05 \x01(\t\x12\x10\n\x08\x64isabled\x18\x06 \x01(\x08*\x16\n\x04Void\x12\x0e\n\nVOID_VALUE\x10\x00*Q\n\x07KeyType\x12\x0e\n\nPUBLIC_KEY\x10\x00\x12\x16\n\x12PUBLIC_KEY_ED25519\x10\x01\x12\x11\n\rSHARED_SECRET\x10\x03\x12\x0b\n\x07\x41\x45S_256\x10\x04*4\n\x0b\x46\x65\x61tureFlag\x12\x0c\n\x08TSSV_ALL\x10\x00\x12\n\n\x06TS_ALL\x10\x01\x12\x0b\n\x07TNL_ALL\x10\x02*\xcb\x04\n\tModelType\x12\x0b\n\x07UNKNOWN\x10\x00\x12$\n VOICE_BIOMETRIC_TEXT_INDEPENDENT\x10\x01\x12\x1c\n\x18VOICE_BIOMETRIC_WAKEWORD\x10\x02\x12\x18\n\x14VOICE_EVENT_WAKEWORD\x10\x03\x12\x1c\n\x18VOICE_TRANSCRIBE_GRAMMAR\x10\x04\x12\'\n#VOICE_TRANSCRIBE_COMMAND_AND_SEARCH\x10\x05\x12(\n$VOICE_RECOGNITION_ACTIVITY_DETECTION\x10\x06\x12\x1b\n\x17VOICE_FEATURE_EXTRACTOR\x10\x07\x12\"\n\x1eVOICE_BIOMETRIC_LIVENESS_DIGIT\x10\x08\x12\"\n\x1eVOICE_BIOMETRIC_TEXT_DEPENDENT\x10\t\x12\x13\n\x0fVOICE_SYNTHESIS\x10\n\x12\x1a\n\x16SOUND_EVENT_ENROLLABLE\x10\x64\x12\x1c\n\x18SOUND_EVENT_REVALIDATION\x10\x65\x12\x15\n\x11SOUND_EVENT_FIXED\x10\x66\x12\x15\n\x11SOUND_SCENE_FIXED\x10g\x12\x13\n\x0e\x46\x41\x43\x45_BIOMETRIC\x10\xc9\x01\x12\x15\n\x10\x46\x41\x43\x45_RECOGNITION\x10\xca\x01\x12\x17\n\x12OBJECT_RECOGNITION\x10\xcb\x01\x12\x14\n\x0fIMAGE_TRANSFORM\x10\xcc\x01\x12\x13\n\x0e\x46\x41\x43\x45_EMBEDDING\x10\xcd\x01\x12\x10\n\x0bLLM_GPT_3_5\x10\xad\x02*X\n\x0eTechnologyType\x12\x0b\n\x07NOT_SET\x10\x00\x12\x08\n\x04TSSV\x10\x01\x12\x06\n\x02TS\x10\x02\x12\x07\n\x03TNL\x10\x03\x12\x07\n\x03STT\x10\x04\x12\x07\n\x03TTS\x10\x05\x12\x0c\n\x08SOUND_ID\x10\x06*&\n\x0f\x43ompressionType\x12\x13\n\x0fIMAGE_GRAYSCALE\x10\x00*|\n\nClientType\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06\x44\x45VICE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x08\n\x04USER\x10\x03\x12\x0e\n\nSUPER_USER\x10\x04\x12\x10\n\x0c\x42ILLING_USER\x10\x05\x12\x12\n\x0eREAD_ONLY_USER\x10\x06\x12\x08\n\x04ROOT\x10\x64*p\n\x0eUsageEventType\x12\x12\n\x0e\x41UTHENTICATION\x10\x00\x12\x0f\n\x0bRECOGNITION\x10\x01\x12\x0e\n\nENROLLMENT\x10\x02\x12\r\n\tSYNTHESIS\x10\x03\x12\x11\n\rTRANSCRIPTION\x10\x04\x12\x07\n\x03LLM\x10\x05*\x1f\n\nServerType\x12\t\n\x05TITAN\x10\x00\x12\x06\n\x02IO\x10\x01\x42v\n\x1a\x61i.sensorycloud.api.commonB\x15SensoryApiCommonProtoP\x01Z8gitlab.com/sensory-cloud/server/titan.git/pkg/api/common\xa2\x02\x04SENGb\x06proto3'
   ,
   dependencies=[validate_dot_validate__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 _VOID = _descriptor.EnumDescriptor(
   name='Void',
   full_name='sensory.api.common.Void',
   filename=None,
@@ -217,19 +217,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='FACE_EMBEDDING', index=19, number=205,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='LLM_GPT_3_5', index=20, number=301,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=1922,
-  serialized_end=2491,
+  serialized_end=2509,
 )
 _sym_db.RegisterEnumDescriptor(_MODELTYPE)
 
 ModelType = enum_type_wrapper.EnumTypeWrapper(_MODELTYPE)
 _TECHNOLOGYTYPE = _descriptor.EnumDescriptor(
   name='TechnologyType',
   full_name='sensory.api.common.TechnologyType',
@@ -271,16 +276,16 @@
       name='SOUND_ID', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2493,
-  serialized_end=2581,
+  serialized_start=2511,
+  serialized_end=2599,
 )
 _sym_db.RegisterEnumDescriptor(_TECHNOLOGYTYPE)
 
 TechnologyType = enum_type_wrapper.EnumTypeWrapper(_TECHNOLOGYTYPE)
 _COMPRESSIONTYPE = _descriptor.EnumDescriptor(
   name='CompressionType',
   full_name='sensory.api.common.CompressionType',
@@ -292,16 +297,16 @@
       name='IMAGE_GRAYSCALE', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2583,
-  serialized_end=2621,
+  serialized_start=2601,
+  serialized_end=2639,
 )
 _sym_db.RegisterEnumDescriptor(_COMPRESSIONTYPE)
 
 CompressionType = enum_type_wrapper.EnumTypeWrapper(_COMPRESSIONTYPE)
 _CLIENTTYPE = _descriptor.EnumDescriptor(
   name='ClientType',
   full_name='sensory.api.common.ClientType',
@@ -348,16 +353,16 @@
       name='ROOT', index=7, number=100,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2623,
-  serialized_end=2747,
+  serialized_start=2641,
+  serialized_end=2765,
 )
 _sym_db.RegisterEnumDescriptor(_CLIENTTYPE)
 
 ClientType = enum_type_wrapper.EnumTypeWrapper(_CLIENTTYPE)
 _USAGEEVENTTYPE = _descriptor.EnumDescriptor(
   name='UsageEventType',
   full_name='sensory.api.common.UsageEventType',
@@ -386,19 +391,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='TRANSCRIPTION', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='LLM', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2749,
-  serialized_end=2852,
+  serialized_start=2767,
+  serialized_end=2879,
 )
 _sym_db.RegisterEnumDescriptor(_USAGEEVENTTYPE)
 
 UsageEventType = enum_type_wrapper.EnumTypeWrapper(_USAGEEVENTTYPE)
 _SERVERTYPE = _descriptor.EnumDescriptor(
   name='ServerType',
   full_name='sensory.api.common.ServerType',
@@ -415,16 +425,16 @@
       name='IO', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2854,
-  serialized_end=2885,
+  serialized_start=2881,
+  serialized_end=2912,
 )
 _sym_db.RegisterEnumDescriptor(_SERVERTYPE)
 
 ServerType = enum_type_wrapper.EnumTypeWrapper(_SERVERTYPE)
 VOID_VALUE = 0
 PUBLIC_KEY = 0
 PUBLIC_KEY_ED25519 = 1
@@ -449,14 +459,15 @@
 SOUND_EVENT_FIXED = 102
 SOUND_SCENE_FIXED = 103
 FACE_BIOMETRIC = 201
 FACE_RECOGNITION = 202
 OBJECT_RECOGNITION = 203
 IMAGE_TRANSFORM = 204
 FACE_EMBEDDING = 205
+LLM_GPT_3_5 = 301
 NOT_SET = 0
 TSSV = 1
 TS = 2
 TNL = 3
 STT = 4
 TTS = 5
 SOUND_ID = 6
@@ -470,14 +481,15 @@
 READ_ONLY_USER = 6
 ROOT = 100
 AUTHENTICATION = 0
 RECOGNITION = 1
 ENROLLMENT = 2
 SYNTHESIS = 3
 TRANSCRIPTION = 4
+LLM = 5
 TITAN = 0
 IO = 1
 
 
 
 _COMPRESSIONCONFIGURATION = _descriptor.Descriptor(
   name='CompressionConfiguration',
```

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/health/health_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/health/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/oauth/oauth_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/audio/audio_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='v1/audio/audio.proto',
   package='sensory.api.v1.audio',
   syntax='proto3',
   serialized_options=b'\n\034ai.sensorycloud.api.v1.audioB\026SensoryApiV1AudioProtoP\001Z:gitlab.com/sensory-cloud/server/titan.git/pkg/api/v1/audio\242\002\005SENGA',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x14v1/audio/audio.proto\x12\x14sensory.api.v1.audio\x1a\x17validate/validate.proto\x1a\x13\x63ommon/common.proto\"\x12\n\x10GetModelsRequest\"\xf2\x01\n\nAudioModel\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cisEnrollable\x18\x02 \x01(\x08\x12\x30\n\tmodelType\x18\x03 \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\x13\n\x0b\x66ixedPhrase\x18\x04 \x01(\t\x12\x12\n\nsampleRate\x18\x05 \x01(\x05\x12\x10\n\x08versions\x18\x06 \x03(\t\x12\x36\n\ntechnology\x18\x07 \x01(\x0e\x32\".sensory.api.common.TechnologyType\x12\x1b\n\x13isLivenessSupported\x18\x08 \x01(\x08\"\x7f\n AudioRequestPostProcessingAction\x12\x10\n\x08\x61\x63tionId\x18\x01 \x01(\t\x12I\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32/.sensory.api.v1.audio.AudioPostProcessingActionB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"\x80\x01\n!AudioResponsePostProcessingAction\x12\x10\n\x08\x61\x63tionId\x18\x01 \x01(\t\x12I\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32/.sensory.api.v1.audio.AudioPostProcessingActionB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"E\n\x11GetModelsResponse\x12\x30\n\x06models\x18\x01 \x03(\x0b\x32 .sensory.api.v1.audio.AudioModel\"\x8a\x01\n\x17\x43reateEnrollmentRequest\x12>\n\x06\x63onfig\x18\x01 \x01(\x0b\x32,.sensory.api.v1.audio.CreateEnrollmentConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\x82\x01\n\x13\x41uthenticateRequest\x12:\n\x06\x63onfig\x18\x01 \x01(\x0b\x32(.sensory.api.v1.audio.AuthenticateConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\xe8\x01\n\x14ValidateEventRequest\x12;\n\x06\x63onfig\x18\x01 \x01(\x0b\x32).sensory.api.v1.audio.ValidateEventConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x12\x0c\n\x04topN\x18\x03 \x01(\x05\x12T\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x36.sensory.api.v1.audio.AudioRequestPostProcessingActionB\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\x92\x01\n\x1a\x43reateEnrolledEventRequest\x12\x43\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x31.sensory.api.v1.audio.CreateEnrollmentEventConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\x94\x01\n\x1cValidateEnrolledEventRequest\x12\x43\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x31.sensory.api.v1.audio.ValidateEnrolledEventConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\xd4\x01\n\x11TranscribeRequest\x12\x38\n\x06\x63onfig\x18\x01 \x01(\x0b\x32&.sensory.api.v1.audio.TranscribeConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x12T\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x36.sensory.api.v1.audio.AudioRequestPostProcessingActionB\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"e\n\x17SynthesizeSpeechRequest\x12\x0e\n\x06phrase\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x02 \x01(\x0b\x32*.sensory.api.v1.audio.VoiceSynthesisConfig\"\xfa\x01\n\x18\x43reateEnrollmentResponse\x12\x17\n\x0fpercentComplete\x18\x01 \x01(\x03\x12\x13\n\x0b\x61udioEnergy\x18\x02 \x01(\x02\x12\x14\n\x0c\x65nrollmentId\x18\x03 \x01(\t\x12\x11\n\tmodelName\x18\x04 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x05 \x01(\t\x12\x13\n\x0bmodelPrompt\x18\x06 \x01(\t\x12\x1e\n\x16percentSegmentComplete\x18\x07 \x01(\x03\x12<\n\x0f\x65nrollmentToken\x18\x08 \x01(\x0b\x32#.sensory.api.common.EnrollmentToken\"\xc9\x01\n\x14\x41uthenticateResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x05token\x18\x03 \x01(\x0b\x32!.sensory.api.common.TokenResponse\x12\x0e\n\x06userId\x18\x04 \x01(\t\x12\x14\n\x0c\x65nrollmentId\x18\x05 \x01(\t\x12\x13\n\x0bmodelPrompt\x18\x06 \x01(\t\x12\x1e\n\x16percentSegmentComplete\x18\x07 \x01(\x03\"U\n\x13SoundIdTopNResponse\x12\x10\n\x08resultId\x18\x01 \x01(\t\x12\x12\n\nlogitScore\x18\x02 \x01(\x02\x12\x18\n\x10probabilityScore\x18\x03 \x01(\x02\"\xf6\x01\n\x15ValidateEventResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x10\n\x08resultId\x18\x03 \x01(\t\x12\r\n\x05score\x18\x04 \x01(\x02\x12?\n\x0ctopNResponse\x18\x05 \x03(\x0b\x32).sensory.api.v1.audio.SoundIdTopNResponse\x12U\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x37.sensory.api.v1.audio.AudioResponsePostProcessingAction\"\x80\x01\n\x1dValidateEnrolledEventResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x14\n\x0c\x65nrollmentId\x18\x03 \x01(\t\x12\x0e\n\x06userId\x18\x04 \x01(\t\x12\x13\n\x0bmodelPrompt\x18\x05 \x01(\t\"\xa1\x01\n\x0eTranscribeWord\x12\x13\n\x0b\x62\x65gintimeMs\x18\x01 \x01(\x04\x12\x11\n\tendtimeMs\x18\x02 \x01(\x04\x12\x12\n\nconfidence\x18\x03 \x01(\x02\x12\x32\n\twordState\x18\x04 \x01(\x0e\x32\x1f.sensory.api.v1.audio.WordState\x12\x11\n\twordIndex\x18\x05 \x01(\x04\x12\x0c\n\x04word\x18\x06 \x01(\t\"|\n\x16TranscribeWordResponse\x12\x33\n\x05words\x18\x01 \x03(\x0b\x32$.sensory.api.v1.audio.TranscribeWord\x12\x16\n\x0e\x66irstWordIndex\x18\x02 \x01(\x04\x12\x15\n\rlastWordIndex\x18\x03 \x01(\x04\"\xda\x01\n\x12TranscribeResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12>\n\x08wordList\x18\x04 \x01(\x0b\x32,.sensory.api.v1.audio.TranscribeWordResponse\x12\x18\n\x10hasVoiceActivity\x18\x05 \x01(\x08\x12U\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x37.sensory.api.v1.audio.AudioResponsePostProcessingAction\"|\n\x18SynthesizeSpeechResponse\x12\x33\n\x06\x63onfig\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x13\n\x11streamingResponse\"\xa0\x03\n\x16\x43reateEnrollmentConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x19\n\x06userId\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x1b\n\x08\x64\x65viceId\x18\x03 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x1d\n\tmodelName\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x1d\n\x0b\x64\x65scription\x18\x05 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xff\x07\x12\x19\n\x11isLivenessEnabled\x18\x06 \x01(\x08\x12,\n\x17\x65nrollmentNumUtterances\x18\x07 \x01(\rB\t\xfa\x42\x06*\x04\x18\n(\x00H\x00\x12-\n\x12\x65nrollmentDuration\x18\x08 \x01(\x02\x42\x0f\xfa\x42\x0c\n\n\x1d\x00\x00pA-\x00\x00\x00\x00H\x00\x12\x1c\n\x0breferenceId\x18\t \x01(\tB\x07\xfa\x42\x04r\x02\x18\x7f\x12.\n&disableServerEnrollmentTemplateStorage\x18\n \x01(\x08\x42\x0e\n\x0c\x65nrollLength\"\xb5\x03\n\x12\x41uthenticateConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12 \n\x0c\x65nrollmentId\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x12\x1b\n\x11\x65nrollmentGroupId\x18\x03 \x01(\tH\x00\x12\x16\n\x0e\x64oIncludeToken\x18\x04 \x01(\x08\x12I\n\x0bsensitivity\x18\x05 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12V\n\x08security\x18\x06 \x01(\x0e\x32:.sensory.api.v1.audio.AuthenticateConfig.ThresholdSecurityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x19\n\x11isLivenessEnabled\x18\x07 \x01(\x08\x12\x17\n\x0f\x65nrollmentToken\x18\x08 \x01(\x0c\"&\n\x11ThresholdSecurity\x12\x08\n\x04HIGH\x10\x00\x12\x07\n\x03LOW\x10\x01\x42\r\n\x06\x61uthId\x12\x03\xf8\x42\x01\"\xd6\x01\n\x13ValidateEventConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x1d\n\tmodelName\x18\x02 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x19\n\x06userId\x18\x03 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12I\n\x0bsensitivity\x18\x04 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"\xbd\x02\n\x1b\x43reateEnrollmentEventConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x19\n\x06userId\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x1d\n\tmodelName\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x1d\n\x0b\x64\x65scription\x18\x04 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xff\x07\x12,\n\x17\x65nrollmentNumUtterances\x18\x05 \x01(\rB\t\xfa\x42\x06*\x04\x18\n(\x00H\x00\x12-\n\x12\x65nrollmentDuration\x18\x06 \x01(\x02\x42\x0f\xfa\x42\x0c\n\n\x1d\x00\x00pA-\x00\x00\x00\x00H\x00\x12\x1c\n\x0breferenceId\x18\x07 \x01(\tB\x07\xfa\x42\x04r\x02\x18\x7f\x42\x0e\n\x0c\x65nrollLength\"\x8b\x02\n\x1bValidateEnrolledEventConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12 \n\x0c\x65nrollmentId\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x12\x1b\n\x11\x65nrollmentGroupId\x18\x03 \x01(\tH\x00\x12I\n\x0bsensitivity\x18\x04 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x17\n\x0f\x65nrollmentToken\x18\x05 \x01(\x0c\x42\r\n\x06\x61uthId\x12\x03\xf8\x42\x01\"2\n\x15\x43ustomVocabularyWords\x12\x19\n\x05words\x18\x01 \x03(\tB\n\xfa\x42\x07\x92\x01\x04\x08\x01\x10\x64\"\x81\x01\n\x15TranscribeEventConfig\x12\x1d\n\tmodelName\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12I\n\x0bsensitivity\x18\x02 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"\x9b\x04\n\x10TranscribeConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x1d\n\tmodelName\x18\x02 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x19\n\x06userId\x18\x03 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\'\n\x1f\x65nablePunctuationCapitalization\x18\x04 \x01(\x08\x12\x19\n\x11\x64oSingleUtterance\x18\x05 \x01(\x08\x12\x42\n\x0evadSensitivity\x18\x06 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivity\x12\x13\n\x0bvadDuration\x18\x07 \x01(\x02\x12N\n\x1a\x63ustomVocabRewardThreshold\x18\x08 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivity\x12\x1a\n\x12\x63ustomVocabularyId\x18\t \x01(\t\x12\x43\n\x0e\x63ustomWordList\x18\n \x01(\x0b\x32+.sensory.api.v1.audio.CustomVocabularyWords\x12\x43\n\x0ewakeWordConfig\x18\x0b \x01(\x0b\x32+.sensory.api.v1.audio.TranscribeEventConfig\"\xeb\x01\n\x0b\x41udioConfig\x12K\n\x08\x65ncoding\x18\x01 \x01(\x0e\x32/.sensory.api.v1.audio.AudioConfig.AudioEncodingB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12!\n\x0fsampleRateHertz\x18\x02 \x01(\x05\x42\x08\xfa\x42\x05\x1a\x03(\xc0>\x12\"\n\x11\x61udioChannelCount\x18\x03 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02 \x00\x12\x14\n\x0clanguageCode\x18\x04 \x01(\t\"2\n\rAudioEncoding\x12\x0c\n\x08LINEAR16\x10\x00\x12\x08\n\x04\x46LAC\x10\x01\x12\t\n\x05MULAW\x10\x02\"b\n\x14VoiceSynthesisConfig\x12\x1d\n\tmodelName\x18\x02 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12%\n\x0fsampleRateHertz\x18\x03 \x01(\x05\x42\x0c\xfa\x42\t\x1a\x07\x18\x80\xee\x05(\xc0>J\x04\x08\x01\x10\x02*I\n\x19\x41udioPostProcessingAction\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x46LUSH\x10\x01\x12\t\n\x05RESET\x10\x02\x12\t\n\x05\x46INAL\x10\x03*7\n\tWordState\x12\x15\n\x11WORDSTATE_PENDING\x10\x00\x12\x13\n\x0fWORDSTATE_FINAL\x10\x01*N\n\x14ThresholdSensitivity\x12\n\n\x06LOWEST\x10\x00\x12\x07\n\x03LOW\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x08\n\x04HIGH\x10\x03\x12\x0b\n\x07HIGHEST\x10\x04\x32m\n\x0b\x41udioModels\x12^\n\tGetModels\x12&.sensory.api.v1.audio.GetModelsRequest\x1a\'.sensory.api.v1.audio.GetModelsResponse\"\x00\x32\xf7\x01\n\x0f\x41udioBiometrics\x12w\n\x10\x43reateEnrollment\x12-.sensory.api.v1.audio.CreateEnrollmentRequest\x1a..sensory.api.v1.audio.CreateEnrollmentResponse\"\x00(\x01\x30\x01\x12k\n\x0c\x41uthenticate\x12).sensory.api.v1.audio.AuthenticateRequest\x1a*.sensory.api.v1.audio.AuthenticateResponse\"\x00(\x01\x30\x01\x32\x85\x03\n\x0b\x41udioEvents\x12n\n\rValidateEvent\x12*.sensory.api.v1.audio.ValidateEventRequest\x1a+.sensory.api.v1.audio.ValidateEventResponse\"\x00(\x01\x30\x01\x12}\n\x13\x43reateEnrolledEvent\x12\x30.sensory.api.v1.audio.CreateEnrolledEventRequest\x1a..sensory.api.v1.audio.CreateEnrollmentResponse\"\x00(\x01\x30\x01\x12\x86\x01\n\x15ValidateEnrolledEvent\x12\x32.sensory.api.v1.audio.ValidateEnrolledEventRequest\x1a\x33.sensory.api.v1.audio.ValidateEnrolledEventResponse\"\x00(\x01\x30\x01\x32|\n\x13\x41udioTranscriptions\x12\x65\n\nTranscribe\x12\'.sensory.api.v1.audio.TranscribeRequest\x1a(.sensory.api.v1.audio.TranscribeResponse\"\x00(\x01\x30\x01\x32\x87\x01\n\x0e\x41udioSynthesis\x12u\n\x10SynthesizeSpeech\x12-.sensory.api.v1.audio.SynthesizeSpeechRequest\x1a..sensory.api.v1.audio.SynthesizeSpeechResponse\"\x00\x30\x01\x42|\n\x1c\x61i.sensorycloud.api.v1.audioB\x16SensoryApiV1AudioProtoP\x01Z:gitlab.com/sensory-cloud/server/titan.git/pkg/api/v1/audio\xa2\x02\x05SENGAb\x06proto3'
+  serialized_pb=b'\n\x14v1/audio/audio.proto\x12\x14sensory.api.v1.audio\x1a\x17validate/validate.proto\x1a\x13\x63ommon/common.proto\"\x12\n\x10GetModelsRequest\"\xf2\x01\n\nAudioModel\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cisEnrollable\x18\x02 \x01(\x08\x12\x30\n\tmodelType\x18\x03 \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\x13\n\x0b\x66ixedPhrase\x18\x04 \x01(\t\x12\x12\n\nsampleRate\x18\x05 \x01(\x05\x12\x10\n\x08versions\x18\x06 \x03(\t\x12\x36\n\ntechnology\x18\x07 \x01(\x0e\x32\".sensory.api.common.TechnologyType\x12\x1b\n\x13isLivenessSupported\x18\x08 \x01(\x08\"\x7f\n AudioRequestPostProcessingAction\x12\x10\n\x08\x61\x63tionId\x18\x01 \x01(\t\x12I\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32/.sensory.api.v1.audio.AudioPostProcessingActionB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"\x80\x01\n!AudioResponsePostProcessingAction\x12\x10\n\x08\x61\x63tionId\x18\x01 \x01(\t\x12I\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32/.sensory.api.v1.audio.AudioPostProcessingActionB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"E\n\x11GetModelsResponse\x12\x30\n\x06models\x18\x01 \x03(\x0b\x32 .sensory.api.v1.audio.AudioModel\"\x8a\x01\n\x17\x43reateEnrollmentRequest\x12>\n\x06\x63onfig\x18\x01 \x01(\x0b\x32,.sensory.api.v1.audio.CreateEnrollmentConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\x82\x01\n\x13\x41uthenticateRequest\x12:\n\x06\x63onfig\x18\x01 \x01(\x0b\x32(.sensory.api.v1.audio.AuthenticateConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\xda\x01\n\x14ValidateEventRequest\x12;\n\x06\x63onfig\x18\x01 \x01(\x0b\x32).sensory.api.v1.audio.ValidateEventConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x12T\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x36.sensory.api.v1.audio.AudioRequestPostProcessingActionB\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\x92\x01\n\x1a\x43reateEnrolledEventRequest\x12\x43\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x31.sensory.api.v1.audio.CreateEnrollmentEventConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\x94\x01\n\x1cValidateEnrolledEventRequest\x12\x43\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x31.sensory.api.v1.audio.ValidateEnrolledEventConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"\xd4\x01\n\x11TranscribeRequest\x12\x38\n\x06\x63onfig\x18\x01 \x01(\x0b\x32&.sensory.api.v1.audio.TranscribeConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x12T\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x36.sensory.api.v1.audio.AudioRequestPostProcessingActionB\x17\n\x10streamingRequest\x12\x03\xf8\x42\x01\"e\n\x17SynthesizeSpeechRequest\x12\x0e\n\x06phrase\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x02 \x01(\x0b\x32*.sensory.api.v1.audio.VoiceSynthesisConfig\"\xfa\x01\n\x18\x43reateEnrollmentResponse\x12\x17\n\x0fpercentComplete\x18\x01 \x01(\x03\x12\x13\n\x0b\x61udioEnergy\x18\x02 \x01(\x02\x12\x14\n\x0c\x65nrollmentId\x18\x03 \x01(\t\x12\x11\n\tmodelName\x18\x04 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x05 \x01(\t\x12\x13\n\x0bmodelPrompt\x18\x06 \x01(\t\x12\x1e\n\x16percentSegmentComplete\x18\x07 \x01(\x03\x12<\n\x0f\x65nrollmentToken\x18\x08 \x01(\x0b\x32#.sensory.api.common.EnrollmentToken\"\xc9\x01\n\x14\x41uthenticateResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x05token\x18\x03 \x01(\x0b\x32!.sensory.api.common.TokenResponse\x12\x0e\n\x06userId\x18\x04 \x01(\t\x12\x14\n\x0c\x65nrollmentId\x18\x05 \x01(\t\x12\x13\n\x0bmodelPrompt\x18\x06 \x01(\t\x12\x1e\n\x16percentSegmentComplete\x18\x07 \x01(\x03\"U\n\x13SoundIdTopNResponse\x12\x10\n\x08resultId\x18\x01 \x01(\t\x12\x12\n\nlogitScore\x18\x02 \x01(\x02\x12\x18\n\x10probabilityScore\x18\x03 \x01(\x02\"\xa6\x02\n\x15ValidateEventResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x10\n\x08resultId\x18\x03 \x01(\t\x12\r\n\x05score\x18\x04 \x01(\x02\x12?\n\x0ctopNResponse\x18\x05 \x03(\x0b\x32).sensory.api.v1.audio.SoundIdTopNResponse\x12\x17\n\x0fResultStartTime\x18\x06 \x01(\x02\x12\x15\n\rResultEndTime\x18\x07 \x01(\x02\x12U\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x37.sensory.api.v1.audio.AudioResponsePostProcessingAction\"\x80\x01\n\x1dValidateEnrolledEventResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x14\n\x0c\x65nrollmentId\x18\x03 \x01(\t\x12\x0e\n\x06userId\x18\x04 \x01(\t\x12\x13\n\x0bmodelPrompt\x18\x05 \x01(\t\"\xa1\x01\n\x0eTranscribeWord\x12\x13\n\x0b\x62\x65gintimeMs\x18\x01 \x01(\x04\x12\x11\n\tendtimeMs\x18\x02 \x01(\x04\x12\x12\n\nconfidence\x18\x03 \x01(\x02\x12\x32\n\twordState\x18\x04 \x01(\x0e\x32\x1f.sensory.api.v1.audio.WordState\x12\x11\n\twordIndex\x18\x05 \x01(\x04\x12\x0c\n\x04word\x18\x06 \x01(\t\"|\n\x16TranscribeWordResponse\x12\x33\n\x05words\x18\x01 \x03(\x0b\x32$.sensory.api.v1.audio.TranscribeWord\x12\x16\n\x0e\x66irstWordIndex\x18\x02 \x01(\x04\x12\x15\n\rlastWordIndex\x18\x03 \x01(\x04\"\xda\x01\n\x12TranscribeResponse\x12\x13\n\x0b\x61udioEnergy\x18\x01 \x01(\x02\x12>\n\x08wordList\x18\x04 \x01(\x0b\x32,.sensory.api.v1.audio.TranscribeWordResponse\x12\x18\n\x10hasVoiceActivity\x18\x05 \x01(\x08\x12U\n\x14postProcessingAction\x18\n \x01(\x0b\x32\x37.sensory.api.v1.audio.AudioResponsePostProcessingAction\"|\n\x18SynthesizeSpeechResponse\x12\x33\n\x06\x63onfig\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigH\x00\x12\x16\n\x0c\x61udioContent\x18\x02 \x01(\x0cH\x00\x42\x13\n\x11streamingResponse\"\xa0\x03\n\x16\x43reateEnrollmentConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x19\n\x06userId\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x1b\n\x08\x64\x65viceId\x18\x03 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x1d\n\tmodelName\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x1d\n\x0b\x64\x65scription\x18\x05 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xff\x07\x12\x19\n\x11isLivenessEnabled\x18\x06 \x01(\x08\x12,\n\x17\x65nrollmentNumUtterances\x18\x07 \x01(\rB\t\xfa\x42\x06*\x04\x18\n(\x00H\x00\x12-\n\x12\x65nrollmentDuration\x18\x08 \x01(\x02\x42\x0f\xfa\x42\x0c\n\n\x1d\x00\x00pA-\x00\x00\x00\x00H\x00\x12\x1c\n\x0breferenceId\x18\t \x01(\tB\x07\xfa\x42\x04r\x02\x18\x7f\x12.\n&disableServerEnrollmentTemplateStorage\x18\n \x01(\x08\x42\x0e\n\x0c\x65nrollLength\"\xb5\x03\n\x12\x41uthenticateConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12 \n\x0c\x65nrollmentId\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x12\x1b\n\x11\x65nrollmentGroupId\x18\x03 \x01(\tH\x00\x12\x16\n\x0e\x64oIncludeToken\x18\x04 \x01(\x08\x12I\n\x0bsensitivity\x18\x05 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12V\n\x08security\x18\x06 \x01(\x0e\x32:.sensory.api.v1.audio.AuthenticateConfig.ThresholdSecurityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x19\n\x11isLivenessEnabled\x18\x07 \x01(\x08\x12\x17\n\x0f\x65nrollmentToken\x18\x08 \x01(\x0c\"&\n\x11ThresholdSecurity\x12\x08\n\x04HIGH\x10\x00\x12\x07\n\x03LOW\x10\x01\x42\r\n\x06\x61uthId\x12\x03\xf8\x42\x01\"\xe4\x01\n\x13ValidateEventConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x1d\n\tmodelName\x18\x02 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x19\n\x06userId\x18\x03 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12I\n\x0bsensitivity\x18\x04 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x0c\n\x04topN\x18\x05 \x01(\x05\"\xbd\x02\n\x1b\x43reateEnrollmentEventConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x19\n\x06userId\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\x1d\n\tmodelName\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x1d\n\x0b\x64\x65scription\x18\x04 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xff\x07\x12,\n\x17\x65nrollmentNumUtterances\x18\x05 \x01(\rB\t\xfa\x42\x06*\x04\x18\n(\x00H\x00\x12-\n\x12\x65nrollmentDuration\x18\x06 \x01(\x02\x42\x0f\xfa\x42\x0c\n\n\x1d\x00\x00pA-\x00\x00\x00\x00H\x00\x12\x1c\n\x0breferenceId\x18\x07 \x01(\tB\x07\xfa\x42\x04r\x02\x18\x7f\x42\x0e\n\x0c\x65nrollLength\"\x8b\x02\n\x1bValidateEnrolledEventConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12 \n\x0c\x65nrollmentId\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x12\x1b\n\x11\x65nrollmentGroupId\x18\x03 \x01(\tH\x00\x12I\n\x0bsensitivity\x18\x04 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x17\n\x0f\x65nrollmentToken\x18\x05 \x01(\x0c\x42\r\n\x06\x61uthId\x12\x03\xf8\x42\x01\"2\n\x15\x43ustomVocabularyWords\x12\x19\n\x05words\x18\x01 \x03(\tB\n\xfa\x42\x07\x92\x01\x04\x08\x01\x10\x64\"\x81\x01\n\x15TranscribeEventConfig\x12\x1d\n\tmodelName\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12I\n\x0bsensitivity\x18\x02 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivityB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\"\xb2\x04\n\x10TranscribeConfig\x12:\n\x05\x61udio\x18\x01 \x01(\x0b\x32!.sensory.api.v1.audio.AudioConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x1d\n\tmodelName\x18\x02 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12\x19\n\x06userId\x18\x03 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12\'\n\x1f\x65nablePunctuationCapitalization\x18\x04 \x01(\x08\x12\x19\n\x11\x64oSingleUtterance\x18\x05 \x01(\x08\x12\x42\n\x0evadSensitivity\x18\x06 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivity\x12\x13\n\x0bvadDuration\x18\x07 \x01(\x02\x12N\n\x1a\x63ustomVocabRewardThreshold\x18\x08 \x01(\x0e\x32*.sensory.api.v1.audio.ThresholdSensitivity\x12\x1a\n\x12\x63ustomVocabularyId\x18\t \x01(\t\x12\x43\n\x0e\x63ustomWordList\x18\n \x01(\x0b\x32+.sensory.api.v1.audio.CustomVocabularyWords\x12\x15\n\rdoOfflineMode\x18\x0b \x01(\x08\x12\x43\n\x0ewakeWordConfig\x18\x0c \x01(\x0b\x32+.sensory.api.v1.audio.TranscribeEventConfig\"\xeb\x01\n\x0b\x41udioConfig\x12K\n\x08\x65ncoding\x18\x01 \x01(\x0e\x32/.sensory.api.v1.audio.AudioConfig.AudioEncodingB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12!\n\x0fsampleRateHertz\x18\x02 \x01(\x05\x42\x08\xfa\x42\x05\x1a\x03(\xc0>\x12\"\n\x11\x61udioChannelCount\x18\x03 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02 \x00\x12\x14\n\x0clanguageCode\x18\x04 \x01(\t\"2\n\rAudioEncoding\x12\x0c\n\x08LINEAR16\x10\x00\x12\x08\n\x04\x46LAC\x10\x01\x12\t\n\x05MULAW\x10\x02\"b\n\x14VoiceSynthesisConfig\x12\x1d\n\tmodelName\x18\x02 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x01\x12%\n\x0fsampleRateHertz\x18\x03 \x01(\x05\x42\x0c\xfa\x42\t\x1a\x07\x18\x80\xee\x05(\xc0>J\x04\x08\x01\x10\x02*I\n\x19\x41udioPostProcessingAction\x12\x0b\n\x07NOT_SET\x10\x00\x12\t\n\x05\x46LUSH\x10\x01\x12\t\n\x05RESET\x10\x02\x12\t\n\x05\x46INAL\x10\x03*7\n\tWordState\x12\x15\n\x11WORDSTATE_PENDING\x10\x00\x12\x13\n\x0fWORDSTATE_FINAL\x10\x01*N\n\x14ThresholdSensitivity\x12\n\n\x06LOWEST\x10\x00\x12\x07\n\x03LOW\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x08\n\x04HIGH\x10\x03\x12\x0b\n\x07HIGHEST\x10\x04\x32m\n\x0b\x41udioModels\x12^\n\tGetModels\x12&.sensory.api.v1.audio.GetModelsRequest\x1a\'.sensory.api.v1.audio.GetModelsResponse\"\x00\x32\xf7\x01\n\x0f\x41udioBiometrics\x12w\n\x10\x43reateEnrollment\x12-.sensory.api.v1.audio.CreateEnrollmentRequest\x1a..sensory.api.v1.audio.CreateEnrollmentResponse\"\x00(\x01\x30\x01\x12k\n\x0c\x41uthenticate\x12).sensory.api.v1.audio.AuthenticateRequest\x1a*.sensory.api.v1.audio.AuthenticateResponse\"\x00(\x01\x30\x01\x32\x85\x03\n\x0b\x41udioEvents\x12n\n\rValidateEvent\x12*.sensory.api.v1.audio.ValidateEventRequest\x1a+.sensory.api.v1.audio.ValidateEventResponse\"\x00(\x01\x30\x01\x12}\n\x13\x43reateEnrolledEvent\x12\x30.sensory.api.v1.audio.CreateEnrolledEventRequest\x1a..sensory.api.v1.audio.CreateEnrollmentResponse\"\x00(\x01\x30\x01\x12\x86\x01\n\x15ValidateEnrolledEvent\x12\x32.sensory.api.v1.audio.ValidateEnrolledEventRequest\x1a\x33.sensory.api.v1.audio.ValidateEnrolledEventResponse\"\x00(\x01\x30\x01\x32|\n\x13\x41udioTranscriptions\x12\x65\n\nTranscribe\x12\'.sensory.api.v1.audio.TranscribeRequest\x1a(.sensory.api.v1.audio.TranscribeResponse\"\x00(\x01\x30\x01\x32\x87\x01\n\x0e\x41udioSynthesis\x12u\n\x10SynthesizeSpeech\x12-.sensory.api.v1.audio.SynthesizeSpeechRequest\x1a..sensory.api.v1.audio.SynthesizeSpeechResponse\"\x00\x30\x01\x42|\n\x1c\x61i.sensorycloud.api.v1.audioB\x16SensoryApiV1AudioProtoP\x01Z:gitlab.com/sensory-cloud/server/titan.git/pkg/api/v1/audio\xa2\x02\x05SENGAb\x06proto3'
   ,
   dependencies=[validate_dot_validate__pb2.DESCRIPTOR,common_dot_common__pb2.DESCRIPTOR,])
 
 _AUDIOPOSTPROCESSINGACTION = _descriptor.EnumDescriptor(
   name='AudioPostProcessingAction',
   full_name='sensory.api.v1.audio.AudioPostProcessingAction',
   filename=None,
@@ -52,16 +52,16 @@
       name='FINAL', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6106,
-  serialized_end=6179,
+  serialized_start=6177,
+  serialized_end=6250,
 )
 _sym_db.RegisterEnumDescriptor(_AUDIOPOSTPROCESSINGACTION)
 
 AudioPostProcessingAction = enum_type_wrapper.EnumTypeWrapper(_AUDIOPOSTPROCESSINGACTION)
 _WORDSTATE = _descriptor.EnumDescriptor(
   name='WordState',
   full_name='sensory.api.v1.audio.WordState',
@@ -78,16 +78,16 @@
       name='WORDSTATE_FINAL', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6181,
-  serialized_end=6236,
+  serialized_start=6252,
+  serialized_end=6307,
 )
 _sym_db.RegisterEnumDescriptor(_WORDSTATE)
 
 WordState = enum_type_wrapper.EnumTypeWrapper(_WORDSTATE)
 _THRESHOLDSENSITIVITY = _descriptor.EnumDescriptor(
   name='ThresholdSensitivity',
   full_name='sensory.api.v1.audio.ThresholdSensitivity',
@@ -119,16 +119,16 @@
       name='HIGHEST', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6238,
-  serialized_end=6316,
+  serialized_start=6309,
+  serialized_end=6387,
 )
 _sym_db.RegisterEnumDescriptor(_THRESHOLDSENSITIVITY)
 
 ThresholdSensitivity = enum_type_wrapper.EnumTypeWrapper(_THRESHOLDSENSITIVITY)
 NOT_SET = 0
 FLUSH = 1
 RESET = 2
@@ -158,16 +158,16 @@
       name='LOW', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=4180,
-  serialized_end=4218,
+  serialized_start=4214,
+  serialized_end=4252,
 )
 _sym_db.RegisterEnumDescriptor(_AUTHENTICATECONFIG_THRESHOLDSECURITY)
 
 _AUDIOCONFIG_AUDIOENCODING = _descriptor.EnumDescriptor(
   name='AudioEncoding',
   full_name='sensory.api.v1.audio.AudioConfig.AudioEncoding',
   filename=None,
@@ -188,16 +188,16 @@
       name='MULAW', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5954,
-  serialized_end=6004,
+  serialized_start=6025,
+  serialized_end=6075,
 )
 _sym_db.RegisterEnumDescriptor(_AUDIOCONFIG_AUDIOENCODING)
 
 
 _GETMODELSREQUEST = _descriptor.Descriptor(
   name='GetModelsRequest',
   full_name='sensory.api.v1.audio.GetModelsRequest',
@@ -521,22 +521,15 @@
       name='audioContent', full_name='sensory.api.v1.audio.ValidateEventRequest.audioContent', index=1,
       number=2, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='topN', full_name='sensory.api.v1.audio.ValidateEventRequest.topN', index=2,
-      number=3, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='postProcessingAction', full_name='sensory.api.v1.audio.ValidateEventRequest.postProcessingAction', index=3,
+      name='postProcessingAction', full_name='sensory.api.v1.audio.ValidateEventRequest.postProcessingAction', index=2,
       number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -552,15 +545,15 @@
     _descriptor.OneofDescriptor(
       name='streamingRequest', full_name='sensory.api.v1.audio.ValidateEventRequest.streamingRequest',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\370B\001'),
   ],
   serialized_start=963,
-  serialized_end=1195,
+  serialized_end=1181,
 )
 
 
 _CREATEENROLLEDEVENTREQUEST = _descriptor.Descriptor(
   name='CreateEnrolledEventRequest',
   full_name='sensory.api.v1.audio.CreateEnrolledEventRequest',
   filename=None,
@@ -595,16 +588,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='streamingRequest', full_name='sensory.api.v1.audio.CreateEnrolledEventRequest.streamingRequest',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\370B\001'),
   ],
-  serialized_start=1198,
-  serialized_end=1344,
+  serialized_start=1184,
+  serialized_end=1330,
 )
 
 
 _VALIDATEENROLLEDEVENTREQUEST = _descriptor.Descriptor(
   name='ValidateEnrolledEventRequest',
   full_name='sensory.api.v1.audio.ValidateEnrolledEventRequest',
   filename=None,
@@ -639,16 +632,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='streamingRequest', full_name='sensory.api.v1.audio.ValidateEnrolledEventRequest.streamingRequest',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\370B\001'),
   ],
-  serialized_start=1347,
-  serialized_end=1495,
+  serialized_start=1333,
+  serialized_end=1481,
 )
 
 
 _TRANSCRIBEREQUEST = _descriptor.Descriptor(
   name='TranscribeRequest',
   full_name='sensory.api.v1.audio.TranscribeRequest',
   filename=None,
@@ -690,16 +683,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='streamingRequest', full_name='sensory.api.v1.audio.TranscribeRequest.streamingRequest',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\370B\001'),
   ],
-  serialized_start=1498,
-  serialized_end=1710,
+  serialized_start=1484,
+  serialized_end=1696,
 )
 
 
 _SYNTHESIZESPEECHREQUEST = _descriptor.Descriptor(
   name='SynthesizeSpeechRequest',
   full_name='sensory.api.v1.audio.SynthesizeSpeechRequest',
   filename=None,
@@ -729,16 +722,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1712,
-  serialized_end=1813,
+  serialized_start=1698,
+  serialized_end=1799,
 )
 
 
 _CREATEENROLLMENTRESPONSE = _descriptor.Descriptor(
   name='CreateEnrollmentResponse',
   full_name='sensory.api.v1.audio.CreateEnrollmentResponse',
   filename=None,
@@ -810,16 +803,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1816,
-  serialized_end=2066,
+  serialized_start=1802,
+  serialized_end=2052,
 )
 
 
 _AUTHENTICATERESPONSE = _descriptor.Descriptor(
   name='AuthenticateResponse',
   full_name='sensory.api.v1.audio.AuthenticateResponse',
   filename=None,
@@ -884,16 +877,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2069,
-  serialized_end=2270,
+  serialized_start=2055,
+  serialized_end=2256,
 )
 
 
 _SOUNDIDTOPNRESPONSE = _descriptor.Descriptor(
   name='SoundIdTopNResponse',
   full_name='sensory.api.v1.audio.SoundIdTopNResponse',
   filename=None,
@@ -930,16 +923,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2272,
-  serialized_end=2357,
+  serialized_start=2258,
+  serialized_end=2343,
 )
 
 
 _VALIDATEEVENTRESPONSE = _descriptor.Descriptor(
   name='ValidateEventResponse',
   full_name='sensory.api.v1.audio.ValidateEventResponse',
   filename=None,
@@ -979,15 +972,29 @@
       name='topNResponse', full_name='sensory.api.v1.audio.ValidateEventResponse.topNResponse', index=4,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='postProcessingAction', full_name='sensory.api.v1.audio.ValidateEventResponse.postProcessingAction', index=5,
+      name='ResultStartTime', full_name='sensory.api.v1.audio.ValidateEventResponse.ResultStartTime', index=5,
+      number=6, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='ResultEndTime', full_name='sensory.api.v1.audio.ValidateEventResponse.ResultEndTime', index=6,
+      number=7, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='postProcessingAction', full_name='sensory.api.v1.audio.ValidateEventResponse.postProcessingAction', index=7,
       number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -997,16 +1004,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2360,
-  serialized_end=2606,
+  serialized_start=2346,
+  serialized_end=2640,
 )
 
 
 _VALIDATEENROLLEDEVENTRESPONSE = _descriptor.Descriptor(
   name='ValidateEnrolledEventResponse',
   full_name='sensory.api.v1.audio.ValidateEnrolledEventResponse',
   filename=None,
@@ -1057,16 +1064,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2609,
-  serialized_end=2737,
+  serialized_start=2643,
+  serialized_end=2771,
 )
 
 
 _TRANSCRIBEWORD = _descriptor.Descriptor(
   name='TranscribeWord',
   full_name='sensory.api.v1.audio.TranscribeWord',
   filename=None,
@@ -1124,16 +1131,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2740,
-  serialized_end=2901,
+  serialized_start=2774,
+  serialized_end=2935,
 )
 
 
 _TRANSCRIBEWORDRESPONSE = _descriptor.Descriptor(
   name='TranscribeWordResponse',
   full_name='sensory.api.v1.audio.TranscribeWordResponse',
   filename=None,
@@ -1170,16 +1177,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2903,
-  serialized_end=3027,
+  serialized_start=2937,
+  serialized_end=3061,
 )
 
 
 _TRANSCRIBERESPONSE = _descriptor.Descriptor(
   name='TranscribeResponse',
   full_name='sensory.api.v1.audio.TranscribeResponse',
   filename=None,
@@ -1223,16 +1230,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3030,
-  serialized_end=3248,
+  serialized_start=3064,
+  serialized_end=3282,
 )
 
 
 _SYNTHESIZESPEECHRESPONSE = _descriptor.Descriptor(
   name='SynthesizeSpeechResponse',
   full_name='sensory.api.v1.audio.SynthesizeSpeechResponse',
   filename=None,
@@ -1267,16 +1274,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='streamingResponse', full_name='sensory.api.v1.audio.SynthesizeSpeechResponse.streamingResponse',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3250,
-  serialized_end=3374,
+  serialized_start=3284,
+  serialized_end=3408,
 )
 
 
 _CREATEENROLLMENTCONFIG = _descriptor.Descriptor(
   name='CreateEnrollmentConfig',
   full_name='sensory.api.v1.audio.CreateEnrollmentConfig',
   filename=None,
@@ -1367,16 +1374,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='enrollLength', full_name='sensory.api.v1.audio.CreateEnrollmentConfig.enrollLength',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3377,
-  serialized_end=3793,
+  serialized_start=3411,
+  serialized_end=3827,
 )
 
 
 _AUTHENTICATECONFIG = _descriptor.Descriptor(
   name='AuthenticateConfig',
   full_name='sensory.api.v1.audio.AuthenticateConfig',
   filename=None,
@@ -1454,16 +1461,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='authId', full_name='sensory.api.v1.audio.AuthenticateConfig.authId',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\370B\001'),
   ],
-  serialized_start=3796,
-  serialized_end=4233,
+  serialized_start=3830,
+  serialized_end=4267,
 )
 
 
 _VALIDATEEVENTCONFIG = _descriptor.Descriptor(
   name='ValidateEventConfig',
   full_name='sensory.api.v1.audio.ValidateEventConfig',
   filename=None,
@@ -1495,28 +1502,35 @@
     _descriptor.FieldDescriptor(
       name='sensitivity', full_name='sensory.api.v1.audio.ValidateEventConfig.sensitivity', index=3,
       number=4, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=b'\372B\005\202\001\002\020\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='topN', full_name='sensory.api.v1.audio.ValidateEventConfig.topN', index=4,
+      number=5, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4236,
-  serialized_end=4450,
+  serialized_start=4270,
+  serialized_end=4498,
 )
 
 
 _CREATEENROLLMENTEVENTCONFIG = _descriptor.Descriptor(
   name='CreateEnrollmentEventConfig',
   full_name='sensory.api.v1.audio.CreateEnrollmentEventConfig',
   filename=None,
@@ -1586,16 +1600,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='enrollLength', full_name='sensory.api.v1.audio.CreateEnrollmentEventConfig.enrollLength',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=4453,
-  serialized_end=4770,
+  serialized_start=4501,
+  serialized_end=4818,
 )
 
 
 _VALIDATEENROLLEDEVENTCONFIG = _descriptor.Descriptor(
   name='ValidateEnrolledEventConfig',
   full_name='sensory.api.v1.audio.ValidateEnrolledEventConfig',
   filename=None,
@@ -1651,16 +1665,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='authId', full_name='sensory.api.v1.audio.ValidateEnrolledEventConfig.authId',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\370B\001'),
   ],
-  serialized_start=4773,
-  serialized_end=5040,
+  serialized_start=4821,
+  serialized_end=5088,
 )
 
 
 _CUSTOMVOCABULARYWORDS = _descriptor.Descriptor(
   name='CustomVocabularyWords',
   full_name='sensory.api.v1.audio.CustomVocabularyWords',
   filename=None,
@@ -1683,16 +1697,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5042,
-  serialized_end=5092,
+  serialized_start=5090,
+  serialized_end=5140,
 )
 
 
 _TRANSCRIBEEVENTCONFIG = _descriptor.Descriptor(
   name='TranscribeEventConfig',
   full_name='sensory.api.v1.audio.TranscribeEventConfig',
   filename=None,
@@ -1722,16 +1736,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5095,
-  serialized_end=5224,
+  serialized_start=5143,
+  serialized_end=5272,
 )
 
 
 _TRANSCRIBECONFIG = _descriptor.Descriptor(
   name='TranscribeConfig',
   full_name='sensory.api.v1.audio.TranscribeConfig',
   filename=None,
@@ -1806,16 +1820,23 @@
       name='customWordList', full_name='sensory.api.v1.audio.TranscribeConfig.customWordList', index=9,
       number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='wakeWordConfig', full_name='sensory.api.v1.audio.TranscribeConfig.wakeWordConfig', index=10,
-      number=11, type=11, cpp_type=10, label=1,
+      name='doOfflineMode', full_name='sensory.api.v1.audio.TranscribeConfig.doOfflineMode', index=10,
+      number=11, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='wakeWordConfig', full_name='sensory.api.v1.audio.TranscribeConfig.wakeWordConfig', index=11,
+      number=12, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -1824,16 +1845,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5227,
-  serialized_end=5766,
+  serialized_start=5275,
+  serialized_end=5837,
 )
 
 
 _AUDIOCONFIG = _descriptor.Descriptor(
   name='AudioConfig',
   full_name='sensory.api.v1.audio.AudioConfig',
   filename=None,
@@ -1878,16 +1899,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5769,
-  serialized_end=6004,
+  serialized_start=5840,
+  serialized_end=6075,
 )
 
 
 _VOICESYNTHESISCONFIG = _descriptor.Descriptor(
   name='VoiceSynthesisConfig',
   full_name='sensory.api.v1.audio.VoiceSynthesisConfig',
   filename=None,
@@ -1917,16 +1938,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6006,
-  serialized_end=6104,
+  serialized_start=6077,
+  serialized_end=6175,
 )
 
 _AUDIOMODEL.fields_by_name['modelType'].enum_type = common_dot_common__pb2._MODELTYPE
 _AUDIOMODEL.fields_by_name['technology'].enum_type = common_dot_common__pb2._TECHNOLOGYTYPE
 _AUDIOREQUESTPOSTPROCESSINGACTION.fields_by_name['action'].enum_type = _AUDIOPOSTPROCESSINGACTION
 _AUDIORESPONSEPOSTPROCESSINGACTION.fields_by_name['action'].enum_type = _AUDIOPOSTPROCESSINGACTION
 _GETMODELSRESPONSE.fields_by_name['models'].message_type = _AUDIOMODEL
@@ -2338,16 +2359,16 @@
 _AUDIOMODELS = _descriptor.ServiceDescriptor(
   name='AudioModels',
   full_name='sensory.api.v1.audio.AudioModels',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=6318,
-  serialized_end=6427,
+  serialized_start=6389,
+  serialized_end=6498,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetModels',
     full_name='sensory.api.v1.audio.AudioModels.GetModels',
     index=0,
     containing_service=None,
     input_type=_GETMODELSREQUEST,
@@ -2364,16 +2385,16 @@
 _AUDIOBIOMETRICS = _descriptor.ServiceDescriptor(
   name='AudioBiometrics',
   full_name='sensory.api.v1.audio.AudioBiometrics',
   file=DESCRIPTOR,
   index=1,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=6430,
-  serialized_end=6677,
+  serialized_start=6501,
+  serialized_end=6748,
   methods=[
   _descriptor.MethodDescriptor(
     name='CreateEnrollment',
     full_name='sensory.api.v1.audio.AudioBiometrics.CreateEnrollment',
     index=0,
     containing_service=None,
     input_type=_CREATEENROLLMENTREQUEST,
@@ -2400,16 +2421,16 @@
 _AUDIOEVENTS = _descriptor.ServiceDescriptor(
   name='AudioEvents',
   full_name='sensory.api.v1.audio.AudioEvents',
   file=DESCRIPTOR,
   index=2,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=6680,
-  serialized_end=7069,
+  serialized_start=6751,
+  serialized_end=7140,
   methods=[
   _descriptor.MethodDescriptor(
     name='ValidateEvent',
     full_name='sensory.api.v1.audio.AudioEvents.ValidateEvent',
     index=0,
     containing_service=None,
     input_type=_VALIDATEEVENTREQUEST,
@@ -2446,16 +2467,16 @@
 _AUDIOTRANSCRIPTIONS = _descriptor.ServiceDescriptor(
   name='AudioTranscriptions',
   full_name='sensory.api.v1.audio.AudioTranscriptions',
   file=DESCRIPTOR,
   index=3,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=7071,
-  serialized_end=7195,
+  serialized_start=7142,
+  serialized_end=7266,
   methods=[
   _descriptor.MethodDescriptor(
     name='Transcribe',
     full_name='sensory.api.v1.audio.AudioTranscriptions.Transcribe',
     index=0,
     containing_service=None,
     input_type=_TRANSCRIBEREQUEST,
@@ -2472,16 +2493,16 @@
 _AUDIOSYNTHESIS = _descriptor.ServiceDescriptor(
   name='AudioSynthesis',
   full_name='sensory.api.v1.audio.AudioSynthesis',
   file=DESCRIPTOR,
   index=4,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=7198,
-  serialized_end=7333,
+  serialized_start=7269,
+  serialized_end=7404,
   methods=[
   _descriptor.MethodDescriptor(
     name='SynthesizeSpeech',
     full_name='sensory.api.v1.audio.AudioSynthesis.SynthesizeSpeech',
     index=0,
     containing_service=None,
     input_type=_SYNTHESIZESPEECHREQUEST,
```

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/event/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='v1/event/event.proto',
   package='sensory.api.v1.event',
   syntax='proto3',
   serialized_options=b'\n\034ai.sensorycloud.api.v1.eventB\026SensoryApiV1EventProtoP\001Z:gitlab.com/sensory-cloud/server/titan.git/pkg/api/v1/event\242\002\004SENG',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x14v1/event/event.proto\x12\x14sensory.api.v1.event\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x13\x63ommon/common.proto\"M\n\x19PublishUsageEventsRequest\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32 .sensory.api.v1.event.UsageEvent\"\xb1\x03\n\nUsageEvent\x12\x37\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x01\x12\x19\n\x08\x64uration\x18\x02 \x01(\x03\x42\x07\xfa\x42\x04\"\x02(\x00\x12\x14\n\x02id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01\x12\x1b\n\x08\x63lientId\x18\x04 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12:\n\x04type\x18\x05 \x01(\x0e\x32\".sensory.api.common.UsageEventTypeB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x19\n\x05route\x18\x06 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x03\x12\x38\n\x0ctechnologies\x18\x07 \x03(\x0e\x32\".sensory.api.common.TechnologyType\x12\x0e\n\x06models\x18\x08 \x03(\t\x12\x17\n\x0f\x61udioDurationMs\x18\t \x01(\x03\x12\x17\n\x0fvideoFrameCount\x18\n \x01(\x03\x12\x10\n\x08tenantId\x18\x0b \x01(\t\x12\x37\n\x10\x62illableFunction\x18\x0c \x01(\x0e\x32\x1d.sensory.api.common.ModelType\"\xc6\x03\n\x12UsageEventResponse\x12\x37\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x01\x12\x19\n\x08\x64uration\x18\x02 \x01(\x03\x42\x07\xfa\x42\x04\"\x02(\x00\x12\x14\n\x02id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01\x12\x1b\n\x08\x63lientId\x18\x04 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12:\n\x04type\x18\x05 \x01(\x0e\x32\".sensory.api.common.UsageEventTypeB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x19\n\x05route\x18\x06 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x03\x12\x38\n\x0ctechnologies\x18\x07 \x03(\x0e\x32\".sensory.api.common.TechnologyType\x12\x0e\n\x06models\x18\x08 \x03(\t\x12\x15\n\rbillableValue\x18\t \x01(\x03\x12\x15\n\rbillableUnits\x18\n \x01(\t\x12\x10\n\x08tenantId\x18\x0b \x01(\t\x12\x37\n\x10\x62illableFunction\x18\x0c \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\x0f\n\x07\x63redits\x18\r \x01(\x01\"\xf5\x01\n\x15UsageEventListRequest\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x39\n\npagination\x18\x02 \x01(\x0b\x32%.sensory.api.common.PaginationOptions\x12)\n\x05\x61\x66ter\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x11\x62illableFunctions\x18\x05 \x03(\x0e\x32\x1d.sensory.api.common.ModelType\"\x8e\x01\n\x16UsageEventListResponse\x12\x38\n\x06\x65vents\x18\x01 \x03(\x0b\x32(.sensory.api.v1.event.UsageEventResponse\x12:\n\npagination\x18\x02 \x01(\x0b\x32&.sensory.api.common.PaginationResponse\"\xbd\x01\n\x19GlobalEventSummaryRequest\x12\x0f\n\x07tenants\x18\x01 \x03(\t\x12)\n\x05\x61\x66ter\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x11\x62illableFunctions\x18\x05 \x03(\x0e\x32\x1d.sensory.api.common.ModelType\"T\n\x11UsageEventSummary\x12?\n\tsummaries\x18\x01 \x03(\x0b\x32,.sensory.api.v1.event.UsageEventModelSummary\"\xa1\x01\n\x16UsageEventModelSummary\x12\x37\n\x10\x62illableFunction\x18\x01 \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\r\n\x05units\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x03\x12\r\n\x05\x63ount\x18\x04 \x01(\x03\x12\x0f\n\x07\x63redits\x18\x05 \x01(\x01\x12\x10\n\x08tenantId\x18\x06 \x01(\t\"\x1c\n\x1aPublishUsageEventsResponse2\xe0\x03\n\x0c\x45ventService\x12y\n\x12PublishUsageEvents\x12/.sensory.api.v1.event.PublishUsageEventsRequest\x1a\x30.sensory.api.v1.event.PublishUsageEventsResponse\"\x00\x12p\n\x11GetUsageEventList\x12+.sensory.api.v1.event.UsageEventListRequest\x1a,.sensory.api.v1.event.UsageEventListResponse\"\x00\x12n\n\x14GetUsageEventSummary\x12+.sensory.api.v1.event.UsageEventListRequest\x1a\'.sensory.api.v1.event.UsageEventSummary\"\x00\x12s\n\x15GetGlobalUsageSummary\x12/.sensory.api.v1.event.GlobalEventSummaryRequest\x1a\'.sensory.api.v1.event.UsageEventSummary\"\x00\x42{\n\x1c\x61i.sensorycloud.api.v1.eventB\x16SensoryApiV1EventProtoP\x01Z:gitlab.com/sensory-cloud/server/titan.git/pkg/api/v1/event\xa2\x02\x04SENGb\x06proto3'
+  serialized_pb=b'\n\x14v1/event/event.proto\x12\x14sensory.api.v1.event\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x13\x63ommon/common.proto\"M\n\x19PublishUsageEventsRequest\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32 .sensory.api.v1.event.UsageEvent\"\xc5\x03\n\nUsageEvent\x12\x37\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x01\x12\x19\n\x08\x64uration\x18\x02 \x01(\x03\x42\x07\xfa\x42\x04\"\x02(\x00\x12\x14\n\x02id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01\x12\x1b\n\x08\x63lientId\x18\x04 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12:\n\x04type\x18\x05 \x01(\x0e\x32\".sensory.api.common.UsageEventTypeB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x19\n\x05route\x18\x06 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x03\x12\x38\n\x0ctechnologies\x18\x07 \x03(\x0e\x32\".sensory.api.common.TechnologyType\x12\x0e\n\x06models\x18\x08 \x03(\t\x12\x17\n\x0f\x61udioDurationMs\x18\t \x01(\x03\x12\x17\n\x0fvideoFrameCount\x18\n \x01(\x03\x12\x10\n\x08tenantId\x18\x0b \x01(\t\x12\x37\n\x10\x62illableFunction\x18\x0c \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\x12\n\ntokenCount\x18\r \x01(\x03\"\xc6\x03\n\x12UsageEventResponse\x12\x37\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x01\x12\x19\n\x08\x64uration\x18\x02 \x01(\x03\x42\x07\xfa\x42\x04\"\x02(\x00\x12\x14\n\x02id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01\x12\x1b\n\x08\x63lientId\x18\x04 \x01(\tB\t\xfa\x42\x06r\x04\x10\x01\x18\x7f\x12:\n\x04type\x18\x05 \x01(\x0e\x32\".sensory.api.common.UsageEventTypeB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x19\n\x05route\x18\x06 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xff\x03\x12\x38\n\x0ctechnologies\x18\x07 \x03(\x0e\x32\".sensory.api.common.TechnologyType\x12\x0e\n\x06models\x18\x08 \x03(\t\x12\x15\n\rbillableValue\x18\t \x01(\x03\x12\x15\n\rbillableUnits\x18\n \x01(\t\x12\x10\n\x08tenantId\x18\x0b \x01(\t\x12\x37\n\x10\x62illableFunction\x18\x0c \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\x0f\n\x07\x63redits\x18\r \x01(\x01\"\xf5\x01\n\x15UsageEventListRequest\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x39\n\npagination\x18\x02 \x01(\x0b\x32%.sensory.api.common.PaginationOptions\x12)\n\x05\x61\x66ter\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x11\x62illableFunctions\x18\x05 \x03(\x0e\x32\x1d.sensory.api.common.ModelType\"\x8e\x01\n\x16UsageEventListResponse\x12\x38\n\x06\x65vents\x18\x01 \x03(\x0b\x32(.sensory.api.v1.event.UsageEventResponse\x12:\n\npagination\x18\x02 \x01(\x0b\x32&.sensory.api.common.PaginationResponse\"\xbd\x01\n\x19GlobalEventSummaryRequest\x12\x0f\n\x07tenants\x18\x01 \x03(\t\x12)\n\x05\x61\x66ter\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x62\x65\x66ore\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x11\x62illableFunctions\x18\x05 \x03(\x0e\x32\x1d.sensory.api.common.ModelType\"T\n\x11UsageEventSummary\x12?\n\tsummaries\x18\x01 \x03(\x0b\x32,.sensory.api.v1.event.UsageEventModelSummary\"\xa1\x01\n\x16UsageEventModelSummary\x12\x37\n\x10\x62illableFunction\x18\x01 \x01(\x0e\x32\x1d.sensory.api.common.ModelType\x12\r\n\x05units\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x03\x12\r\n\x05\x63ount\x18\x04 \x01(\x03\x12\x0f\n\x07\x63redits\x18\x05 \x01(\x01\x12\x10\n\x08tenantId\x18\x06 \x01(\t\"\x1c\n\x1aPublishUsageEventsResponse2\xe0\x03\n\x0c\x45ventService\x12y\n\x12PublishUsageEvents\x12/.sensory.api.v1.event.PublishUsageEventsRequest\x1a\x30.sensory.api.v1.event.PublishUsageEventsResponse\"\x00\x12p\n\x11GetUsageEventList\x12+.sensory.api.v1.event.UsageEventListRequest\x1a,.sensory.api.v1.event.UsageEventListResponse\"\x00\x12n\n\x14GetUsageEventSummary\x12+.sensory.api.v1.event.UsageEventListRequest\x1a\'.sensory.api.v1.event.UsageEventSummary\"\x00\x12s\n\x15GetGlobalUsageSummary\x12/.sensory.api.v1.event.GlobalEventSummaryRequest\x1a\'.sensory.api.v1.event.UsageEventSummary\"\x00\x42{\n\x1c\x61i.sensorycloud.api.v1.eventB\x16SensoryApiV1EventProtoP\x01Z:gitlab.com/sensory-cloud/server/titan.git/pkg/api/v1/event\xa2\x02\x04SENGb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,validate_dot_validate__pb2.DESCRIPTOR,common_dot_common__pb2.DESCRIPTOR,])
 
 
 
 
 _PUBLISHUSAGEEVENTSREQUEST = _descriptor.Descriptor(
@@ -149,28 +149,35 @@
     _descriptor.FieldDescriptor(
       name='billableFunction', full_name='sensory.api.v1.event.UsageEvent.billableFunction', index=11,
       number=12, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='tokenCount', full_name='sensory.api.v1.event.UsageEvent.tokenCount', index=12,
+      number=13, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=205,
-  serialized_end=638,
+  serialized_end=658,
 )
 
 
 _USAGEEVENTRESPONSE = _descriptor.Descriptor(
   name='UsageEventResponse',
   full_name='sensory.api.v1.event.UsageEventResponse',
   filename=None,
@@ -277,16 +284,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=641,
-  serialized_end=1095,
+  serialized_start=661,
+  serialized_end=1115,
 )
 
 
 _USAGEEVENTLISTREQUEST = _descriptor.Descriptor(
   name='UsageEventListRequest',
   full_name='sensory.api.v1.event.UsageEventListRequest',
   filename=None,
@@ -337,16 +344,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1098,
-  serialized_end=1343,
+  serialized_start=1118,
+  serialized_end=1363,
 )
 
 
 _USAGEEVENTLISTRESPONSE = _descriptor.Descriptor(
   name='UsageEventListResponse',
   full_name='sensory.api.v1.event.UsageEventListResponse',
   filename=None,
@@ -376,16 +383,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1346,
-  serialized_end=1488,
+  serialized_start=1366,
+  serialized_end=1508,
 )
 
 
 _GLOBALEVENTSUMMARYREQUEST = _descriptor.Descriptor(
   name='GlobalEventSummaryRequest',
   full_name='sensory.api.v1.event.GlobalEventSummaryRequest',
   filename=None,
@@ -429,16 +436,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1491,
-  serialized_end=1680,
+  serialized_start=1511,
+  serialized_end=1700,
 )
 
 
 _USAGEEVENTSUMMARY = _descriptor.Descriptor(
   name='UsageEventSummary',
   full_name='sensory.api.v1.event.UsageEventSummary',
   filename=None,
@@ -461,16 +468,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1682,
-  serialized_end=1766,
+  serialized_start=1702,
+  serialized_end=1786,
 )
 
 
 _USAGEEVENTMODELSUMMARY = _descriptor.Descriptor(
   name='UsageEventModelSummary',
   full_name='sensory.api.v1.event.UsageEventModelSummary',
   filename=None,
@@ -528,16 +535,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1769,
-  serialized_end=1930,
+  serialized_start=1789,
+  serialized_end=1950,
 )
 
 
 _PUBLISHUSAGEEVENTSRESPONSE = _descriptor.Descriptor(
   name='PublishUsageEventsResponse',
   full_name='sensory.api.v1.event.PublishUsageEventsResponse',
   filename=None,
@@ -553,16 +560,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1932,
-  serialized_end=1960,
+  serialized_start=1952,
+  serialized_end=1980,
 )
 
 _PUBLISHUSAGEEVENTSREQUEST.fields_by_name['events'].message_type = _USAGEEVENT
 _USAGEEVENT.fields_by_name['timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _USAGEEVENT.fields_by_name['type'].enum_type = common_dot_common__pb2._USAGEEVENTTYPE
 _USAGEEVENT.fields_by_name['technologies'].enum_type = common_dot_common__pb2._TECHNOLOGYTYPE
 _USAGEEVENT.fields_by_name['billableFunction'].enum_type = common_dot_common__pb2._MODELTYPE
@@ -673,16 +680,16 @@
 _EVENTSERVICE = _descriptor.ServiceDescriptor(
   name='EventService',
   full_name='sensory.api.v1.event.EventService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1963,
-  serialized_end=2443,
+  serialized_start=1983,
+  serialized_end=2463,
   methods=[
   _descriptor.MethodDescriptor(
     name='PublishUsageEvents',
     full_name='sensory.api.v1.event.EventService.PublishUsageEvents',
     index=0,
     containing_service=None,
     input_type=_PUBLISHUSAGEEVENTSREQUEST,
```

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/device_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/enrollment_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/video/video_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/validate_pb2.py` & `sensory_cloud-1.2.2/src/sensory_cloud/generated/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/initializer.py` & `sensory_cloud-1.2.2/src/sensory_cloud/initializer.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/services/audio_service.py` & `sensory_cloud-1.2.2/src/sensory_cloud/services/audio_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,35 +351,39 @@
         audio_config: audio_pb2.AudioConfig,
         user_id: str,
         model_name: str,
         audio_stream_iterator: typing.Iterable[bytes],
         sensitivity: audio_pb2.ThresholdSensitivity = audio_pb2.ThresholdSensitivity.Value(
             "MEDIUM"
         ),
+        topN: int = 5,
     ) -> typing.Iterable[audio_pb2.ValidateEventResponse]:
         """
         Stream audio to Sensory Cloud in order to recognize a specific phrase or sound
 
         Arguments:
             audio_config: AudioConfig object
             user_id: String containing the user id
             model_name: String containing the name of the model to be used
             audio_stream_iterator: Iterator of audio bytes
             sensitivity: ThresholdSensitivity enum that sets the sensitivity level of the authentication
                 default = ThresholdSensitivity.Value("MEDIUM")
+            topN: Integer indicating how many sounds to return when using the sound_id_topn model
+                default = 5
 
         Returns:
             An iterator of ValidateEventResponse objects
         """
 
         config = audio_pb2.ValidateEventConfig(
             audio=audio_config,
             modelName=model_name,
             userId=user_id,
             sensitivity=sensitivity,
+            topN=topN,
         )
 
         request_iterator: RequestIterator = RequestIterator(
             audio_request=audio_pb2.ValidateEventRequest,
             request_config=config,
             audio_stream_iterator=audio_stream_iterator,
         )
@@ -541,23 +545,26 @@
         enable_punctuation_capitalization: bool = False,
         do_single_utterance: bool = False,
         vad_sensitivity: audio_pb2.ThresholdSensitivity = None,
         vad_duration: float = None,
         custom_vocab_reward_threshold: audio_pb2.ThresholdSensitivity = None,
         custom_vocabulary_id: str = None,
         custom_word_list: typing.List[str] = None,
+        do_offline_mode: bool = False,
     ) -> typing.Iterable[audio_pb2.TranscribeResponse]:
         """
         Stream audio to Sensory Cloud in order to transcribe spoken words
 
         Arguments:
             audio_config: AudioConfig object
             user_id: String containing the user id
             model_name: String containing the name of the model to be used
             audio_stream_iterator: Iterator of audio bytes
+            enable_punctuation_capitalization: Boolean indicating whether or 
+                not the transcript should use punctuation and capitalization
 
         Returns:
             An iterator of TranscribeResponse objects
         """
 
         custom_vocab = (
             audio_pb2.CustomVocabularyWords(words=custom_word_list)
@@ -572,14 +579,15 @@
             enablePunctuationCapitalization=enable_punctuation_capitalization,
             doSingleUtterance=do_single_utterance,
             vadSensitivity=vad_sensitivity,
             vadDuration=vad_duration,
             customVocabRewardThreshold=custom_vocab_reward_threshold,
             customVocabularyId=custom_vocabulary_id,
             customWordList=custom_vocab,
+            doOfflineMode=do_offline_mode,
         )
 
         request_iterator: RequestIterator = RequestIterator(
             audio_request=audio_pb2.TranscribeRequest,
             request_config=config,
             audio_stream_iterator=audio_stream_iterator,
         )
```

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/services/crypto_service.py` & `sensory_cloud-1.2.2/src/sensory_cloud/services/crypto_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/services/health_service.py` & `sensory_cloud-1.2.2/src/sensory_cloud/services/health_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/services/management_service.py` & `sensory_cloud-1.2.2/src/sensory_cloud/services/management_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/services/oauth_service.py` & `sensory_cloud-1.2.2/src/sensory_cloud/services/oauth_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/services/video_service.py` & `sensory_cloud-1.2.2/src/sensory_cloud/services/video_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud/token_manager.py` & `sensory_cloud-1.2.2/src/sensory_cloud/token_manager.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud.egg-info/PKG-INFO` & `sensory_cloud-1.2.2/src/sensory_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensory-cloud
-Version: 1.0.3
+Version: 1.2.2
 Summary: Python SDK for Sensory Cloud
 Home-page: https://github.com/Sensory-Cloud/python-sdk
 Author: Jonathan Hersch
 Author-email: jhersch@sensoryinc.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `sensory_cloud-1.0.3/src/sensory_cloud.egg-info/SOURCES.txt` & `sensory_cloud-1.2.2/src/sensory_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 src/sensory_cloud/generated/v1/video/__init__.py
 src/sensory_cloud/generated/v1/video/video_pb2.py
 src/sensory_cloud/generated/v1/video/video_pb2_grpc.py
 src/sensory_cloud/generated/validate/__init__.py
 src/sensory_cloud/generated/validate/validate_pb2.py
 src/sensory_cloud/generated/validate/validate_pb2_grpc.py
 src/sensory_cloud/services/__init__.py
+src/sensory_cloud/services/assistant_service.py
 src/sensory_cloud/services/audio_service.py
 src/sensory_cloud/services/crypto_service.py
 src/sensory_cloud/services/health_service.py
 src/sensory_cloud/services/management_service.py
 src/sensory_cloud/services/oauth_service.py
 src/sensory_cloud/services/video_service.py
 test/test_audio_service.py
```

### Comparing `sensory_cloud-1.0.3/test/test_audio_service.py` & `sensory_cloud-1.2.2/test/test_audio_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/test/test_crypto_service.py` & `sensory_cloud-1.2.2/test/test_crypto_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/test/test_health_service.py` & `sensory_cloud-1.2.2/test/test_health_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/test/test_management_service.py` & `sensory_cloud-1.2.2/test/test_management_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/test/test_oauth_service.py` & `sensory_cloud-1.2.2/test/test_oauth_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/test/test_token_manager.py` & `sensory_cloud-1.2.2/test/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.3/test/test_video_service.py` & `sensory_cloud-1.2.2/test/test_video_service.py`

 * *Files identical despite different names*

