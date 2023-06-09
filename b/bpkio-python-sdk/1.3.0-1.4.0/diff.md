# Comparing `tmp/bpkio_python_sdk-1.3.0.tar.gz` & `tmp/bpkio_python_sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_python_sdk-1.3.0.tar", max compression
+gzip compressed data, was "bpkio_python_sdk-1.4.0.tar", max compression
```

## Comparing `bpkio_python_sdk-1.3.0.tar` & `bpkio_python_sdk-1.4.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.3.0/README.md
--rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.3.0/bpkio_api/__init__.py
--rw-r--r--   0        0        0     5766 2023-06-07 13:10:20.655016 bpkio_python_sdk-1.3.0/bpkio_api/api.py
--rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.3.0/bpkio_api/caching.py
--rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.3.0/bpkio_api/credential_provider.py
--rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.3.0/bpkio_api/defaults.py
--rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/__init__.py
--rw-r--r--   0        0        0     4521 2023-05-20 12:34:42.082005 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/categories.py
--rw-r--r--   0        0        0      700 2023-06-07 09:05:39.402150 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/consumption.py
--rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/enums.py
--rw-r--r--   0        0        0    21988 2023-05-20 12:34:42.083318 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/services.py
--rw-r--r--   0        0        0    21622 2023-05-20 12:34:42.084047 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/sources.py
--rw-r--r--   0        0        0     2675 2023-05-20 12:34:42.084780 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/tenants.py
--rw-r--r--   0        0        0     5972 2023-06-07 15:09:04.450220 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/transcoding_profiles.py
--rw-r--r--   0        0        0     2627 2023-05-20 12:34:42.085823 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/users.py
--rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.3.0/bpkio_api/exceptions.py
--rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.3.0/bpkio_api/helpers/codecstrings.py
--rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/__init__.py
--rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/dash.py
--rw-r--r--   0        0        0     3986 2023-06-07 12:31:03.185367 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/factory.py
--rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/generic.py
--rw-r--r--   0        0        0     4501 2023-06-06 15:17:48.082443 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/hls.py
--rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/jpeg.py
--rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/mp4.py
--rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/png.py
--rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vast.py
--rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vmap.py
--rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/xml.py
--rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.3.0/bpkio_api/helpers/list.py
--rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.3.0/bpkio_api/helpers/objects.py
--rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/__init__.py
--rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/analyser.py
--rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/dash.py
--rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/hls.py
--rw-r--r--   0        0        0     1587 2023-05-23 22:08:22.519293 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/profile_generator.py
--rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/__init__.py
--rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/curl.py
--rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/exporter.py
--rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/markdown.py
--rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/postman.py
--rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_items.py
--rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_recorder.py
--rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/text.py
--rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.3.0/bpkio_api/helpers/search.py
--rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.3.0/bpkio_api/helpers/source_type.py
--rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.3.0/bpkio_api/helpers/times.py
--rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.3.0/bpkio_api/mappings.py
--rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.3.0/bpkio_api/models/Categories.py
--rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.3.0/bpkio_api/models/Consumption.py
--rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.3.0/bpkio_api/models/Services.py
--rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.3.0/bpkio_api/models/Slots.py
--rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.3.0/bpkio_api/models/Sources.py
--rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.3.0/bpkio_api/models/Tenants.py
--rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.3.0/bpkio_api/models/TranscodingProfiles.py
--rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.3.0/bpkio_api/models/Users.py
--rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.3.0/bpkio_api/models/__init__.py
--rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.3.0/bpkio_api/models/common.py
--rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.3.0/bpkio_api/models/model_graph.py
--rw-r--r--   0        0        0     1941 2023-05-21 20:52:58.371698 bpkio_python_sdk-1.3.0/bpkio_api/response_handler.py
--rw-r--r--   0        0        0     1195 2023-06-07 15:37:33.376880 bpkio_python_sdk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.4.0/README.md
+-rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.4.0/bpkio_api/__init__.py
+-rw-r--r--   0        0        0     5794 2023-06-09 10:58:27.429762 bpkio_python_sdk-1.4.0/bpkio_api/api.py
+-rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.4.0/bpkio_api/caching.py
+-rw-r--r--   0        0        0      506 2023-06-09 11:08:00.617751 bpkio_python_sdk-1.4.0/bpkio_api/consumer.py
+-rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.4.0/bpkio_api/credential_provider.py
+-rw-r--r--   0        0        0      178 2023-06-09 11:21:14.279980 bpkio_python_sdk-1.4.0/bpkio_api/defaults.py
+-rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4563 2023-06-09 11:03:02.185931 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/categories.py
+-rw-r--r--   0        0        0      747 2023-06-09 11:03:16.109406 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/consumption.py
+-rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/enums.py
+-rw-r--r--   0        0        0    22070 2023-06-09 11:08:21.660390 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/services.py
+-rw-r--r--   0        0        0    21704 2023-06-09 11:08:38.030315 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/sources.py
+-rw-r--r--   0        0        0     2721 2023-06-09 11:05:03.964297 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/tenants.py
+-rw-r--r--   0        0        0     6014 2023-06-09 11:05:16.807277 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/transcoding_profiles.py
+-rw-r--r--   0        0        0     2673 2023-06-09 11:05:32.498036 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/users.py
+-rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.4.0/bpkio_api/exceptions.py
+-rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.4.0/bpkio_api/helpers/codecstrings.py
+-rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/__init__.py
+-rw-r--r--   0        0        0     4582 2023-06-09 11:40:34.918187 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/dash.py
+-rw-r--r--   0        0        0     3532 2023-06-09 12:34:36.766352 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/factory.py
+-rw-r--r--   0        0        0     2949 2023-06-09 14:49:36.436548 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/generic.py
+-rw-r--r--   0        0        0     4521 2023-06-09 11:38:49.325871 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/hls.py
+-rw-r--r--   0        0        0      446 2023-06-09 11:39:02.452951 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/jpeg.py
+-rw-r--r--   0        0        0      472 2023-06-09 11:40:16.383318 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/mp4.py
+-rw-r--r--   0        0        0      434 2023-06-09 11:40:11.132158 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/png.py
+-rw-r--r--   0        0        0     1976 2023-06-09 11:39:37.280020 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vast.py
+-rw-r--r--   0        0        0     2325 2023-06-09 11:39:46.049574 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vmap.py
+-rw-r--r--   0        0        0      580 2023-06-09 11:39:59.258206 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/xml.py
+-rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.4.0/bpkio_api/helpers/list.py
+-rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.4.0/bpkio_api/helpers/objects.py
+-rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/analyser.py
+-rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/dash.py
+-rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/hls.py
+-rw-r--r--   0        0        0     1587 2023-05-23 22:08:22.519293 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/profile_generator.py
+-rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/__init__.py
+-rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/curl.py
+-rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/exporter.py
+-rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/markdown.py
+-rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/postman.py
+-rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_items.py
+-rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_recorder.py
+-rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/text.py
+-rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.4.0/bpkio_api/helpers/search.py
+-rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.4.0/bpkio_api/helpers/source_type.py
+-rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.4.0/bpkio_api/helpers/times.py
+-rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.4.0/bpkio_api/mappings.py
+-rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.4.0/bpkio_api/models/Categories.py
+-rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.4.0/bpkio_api/models/Consumption.py
+-rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.4.0/bpkio_api/models/Services.py
+-rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.4.0/bpkio_api/models/Slots.py
+-rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.4.0/bpkio_api/models/Sources.py
+-rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.4.0/bpkio_api/models/Tenants.py
+-rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.4.0/bpkio_api/models/TranscodingProfiles.py
+-rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.4.0/bpkio_api/models/Users.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.4.0/bpkio_api/models/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.4.0/bpkio_api/models/common.py
+-rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.4.0/bpkio_api/models/model_graph.py
+-rw-r--r--   0        0        0     2152 2023-06-09 10:37:32.988041 bpkio_python_sdk-1.4.0/bpkio_api/response_handler.py
+-rw-r--r--   0        0        0     1195 2023-06-09 15:44:56.748527 bpkio_python_sdk-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.4.0/PKG-INFO
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/api.py` & `bpkio_python_sdk-1.4.0/bpkio_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import base64
 import json
 import os
 from typing import Optional
 from urllib.parse import urlparse
 
-from uplink import Consumer
 from uplink.auth import BearerToken
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import init_cache
 from bpkio_api.credential_provider import TenantProfile, TenantProfileProvider
 from bpkio_api.defaults import DEFAULT_FQDN
 from bpkio_api.endpoints import (
     CategoriesApi,
     ConsumptionApi,
     ServicesApi,
@@ -21,15 +21,15 @@
 )
 from bpkio_api.exceptions import InvalidApiKeyFormat
 from bpkio_api.helpers.recorder import SessionRecorder
 from bpkio_api.mappings import model_to_endpoint
 from bpkio_api.models import Tenant
 
 
-class BroadpeakIoApi(Consumer):
+class BroadpeakIoApi(BpkioSdkConsumer):
     def __init__(
         self,
         *,
         tenant: Optional[str] = None,
         api_key: Optional[str] = None,
         fqdn: str = DEFAULT_FQDN,
         use_cache: bool = True,
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/caching.py` & `bpkio_python_sdk-1.4.0/bpkio_api/caching.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/credential_provider.py` & `bpkio_python_sdk-1.4.0/bpkio_api/credential_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/categories.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/categories.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Any, List, Tuple
 
 from uplink import (
     Body,
-    Consumer,
     Query,
     delete,
     get,
     json,
     post,
     put,
     response_handler,
     returns,
 )
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import cache_api_results
 from bpkio_api.exceptions import ResourceExistsError
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.Categories import Category, CategoryIn
 from bpkio_api.response_handler import postprocess_response
 
 from .enums import UpsertOperationType
 
 
 @response_handler(postprocess_response)
-class CategoriesApi(Consumer):
+class CategoriesApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json(List[Category])
     @get("categories")
     def get_page(self, offset: Query = 0, limit: Query = 5) -> List[Category]:  # type: ignore
         """Get a (partial) list of categories"""
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/consumption.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/consumption.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from datetime import datetime
 
-from uplink import Consumer, Query, get, response_handler, returns
+from uplink import Query, get, response_handler, returns
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.models.Consumption import ConsumptionData
 from bpkio_api.response_handler import postprocess_response
 
 
 @response_handler(postprocess_response)
-class ConsumptionApi(Consumer):
+class ConsumptionApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("consumption")
     def retrieve(
         self,
         start_time: Query("start-time"),  # type: ignore
         end_time: Query("end-time"),  # type: ignore
-        tenant: Query("tenantId")
+        tenant: Query("tenantId"),
     ) -> ConsumptionData:  # type: ignore
         """Get the consumption data between 2 dates"""
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/services.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from datetime import datetime
 from typing import Any, List, Tuple
 
 from uplink import (
     Body,
-    Consumer,
     Query,
     delete,
     get,
     json,
     params,
     post,
     put,
     response_handler,
     returns,
 )
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import cache_api_results
 from bpkio_api.exceptions import BroadpeakIoHelperError, ResourceExistsError
 from bpkio_api.helpers.list import collect_from_ids, get_all_with_pagination
 from bpkio_api.helpers.objects import find_duplicates_of
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models import ContentReplacementSlot
 from bpkio_api.models import Services as Svc
 from bpkio_api.models import VirtualChannelSlot, VirtualChannelSlotIn
 from bpkio_api.response_handler import postprocess_response, return_count
 
 from .enums import UpsertOperationType
 
 
 @response_handler(postprocess_response)
-class ServicesApi(Consumer):
+class ServicesApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
         self.virtual_channel = VirtualChannelServiceApi(
             parent_api=self, base_url=base_url, **kwargs
         )
         self.content_replacement = ContentReplacementServiceApi(
@@ -256,15 +256,15 @@
                         return (updated_resource, UpsertOperationType.UPDATED)
 
 
 # === CONTENT-REPLACEMENT SERVICES ===
 
 
 @response_handler(postprocess_response)
-class ContentReplacementServiceApi(Consumer):
+class ContentReplacementServiceApi(BpkioSdkConsumer):
     def __init__(self, parent_api: ServicesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
         self.slots = ContentReplacementServiceSlotsApi(base_url, **kwargs)
 
     @returns.json(Svc.ContentReplacementService)
@@ -320,15 +320,15 @@
             filters = [(value, field, method)]
 
         services = self.list()
         return search_array_with_filters(services, filters=filters)
 
 
 @response_handler(postprocess_response)
-class ContentReplacementServiceSlotsApi(Consumer):
+class ContentReplacementServiceSlotsApi(BpkioSdkConsumer):
     @returns.json()
     @get("services/content-replacement/{service_id}/slots")
     def get_page(
         self,
         service_id,
         offset: Query = 0,
         limit: Query = 50,
@@ -395,15 +395,15 @@
         )
 
 
 # === VIRTUAL-CHANNEL SERVICES ===
 
 
 @response_handler(postprocess_response)
-class VirtualChannelServiceApi(Consumer):
+class VirtualChannelServiceApi(BpkioSdkConsumer):
     def __init__(self, parent_api: ServicesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
         self.slots = VirtualChannelServiceSlotsApi(base_url, **kwargs)
 
     @returns.json(Svc.VirtualChannelService)
@@ -457,15 +457,15 @@
             filters = [(value, field, method)]
 
         services = self.list()
         return search_array_with_filters(services, filters=filters)
 
 
 @response_handler(postprocess_response)
-class VirtualChannelServiceSlotsApi(Consumer):
+class VirtualChannelServiceSlotsApi(BpkioSdkConsumer):
     @returns.json()
     @get("services/virtual-channel/{service_id}/slots")
     def get_page(
         self,
         service_id,
         offset: Query = 0,
         limit: Query = 50,
@@ -540,15 +540,15 @@
         )
 
 
 # === AD-INSERTION SERVICES ===
 
 
 @response_handler(postprocess_response)
-class AdInsertionServiceApi(Consumer):
+class AdInsertionServiceApi(BpkioSdkConsumer):
     def __init__(self, parent_api: ServicesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(Svc.AdInsertionService)
     @get("services/ad-insertion/{service_id}")
     def retrieve(self, service_id):
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/sources.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, List, Tuple
 from urllib.parse import urlparse, urlunparse
 
 from uplink import (
     Body,
-    Consumer,
     Query,
     delete,
     get,
     json,
     post,
     put,
     response_handler,
     returns,
 )
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import cache_api_results
 from bpkio_api.exceptions import BroadpeakIoHelperError, ResourceExistsError
 from bpkio_api.helpers.list import collect_from_ids, get_all_with_pagination
 from bpkio_api.helpers.objects import find_duplicates_of
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models import Sources as S
 from bpkio_api.response_handler import postprocess_response
 
 from .enums import UpsertOperationType
 
 
 @response_handler(postprocess_response)
-class SourcesApi(Consumer):
+class SourcesApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
         self.asset = AssetSourcesApi(parent_api=self, base_url=base_url, **kwargs)
         self.live = LiveSourcesApi(parent_api=self, base_url=base_url, **kwargs)
         self.asset_catalog = AssetCatalogSourcesApi(
             parent_api=self, base_url=base_url, **kwargs
@@ -267,15 +267,15 @@
             return self.check(type=source.type, url=url)
 
 
 # === ASSET SOURCES ===
 
 
 @response_handler(postprocess_response)
-class AssetSourcesApi(Consumer):
+class AssetSourcesApi(BpkioSdkConsumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.AssetSource)
     @get("sources/asset/{source_id}")
     def retrieve(self, source_id):
@@ -330,15 +330,15 @@
         return search_array_with_filters(sources, filters=filters)
 
 
 # === LIVE SOURCES ===
 
 
 @response_handler(postprocess_response)
-class LiveSourcesApi(Consumer):
+class LiveSourcesApi(BpkioSdkConsumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.LiveSource)
     @get("sources/live/{source_id}")
     def retrieve(self, source_id):
@@ -393,15 +393,15 @@
         return search_array_with_filters(sources, filters=filters)
 
 
 # === ASSET CATALOG SOURCES ===
 
 
 @response_handler(postprocess_response)
-class AssetCatalogSourcesApi(Consumer):
+class AssetCatalogSourcesApi(BpkioSdkConsumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.AssetCatalogSource)
     @get("sources/asset-catalog/{source_id}")
     def retrieve(self, source_id):
@@ -456,15 +456,15 @@
         return search_array_with_filters(sources, filters=filters)
 
 
 # === AD SERVER SOURCES ===
 
 
 @response_handler(postprocess_response)
-class AdServerSourcesApi(Consumer):
+class AdServerSourcesApi(BpkioSdkConsumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.AdServerSource)
     @get("sources/ad-server/{source_id}")
     def retrieve(self, source_id):
@@ -547,15 +547,15 @@
         return search_array_with_filters(sources, filters=filters)
 
 
 # === SLATE SOURCES ===
 
 
 @response_handler(postprocess_response)
-class SlateSourcesApi(Consumer):
+class SlateSourcesApi(BpkioSdkConsumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.SlateSource)
     @get("sources/slate/{source_id}")
     def retrieve(self, source_id):
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/tenants.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/tenants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Any, List, Tuple
 
-from uplink import Consumer, Query, get, response_handler, returns
+from uplink import Query, get, response_handler, returns
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import cache_api_results
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.Tenants import Tenant
 from bpkio_api.response_handler import postprocess_response
 
 
 @response_handler(postprocess_response)
-class TenantsApi(Consumer):
+class TenantsApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json(List[Tenant])
     @get("tenants")
     def get_page(self, offset: Query = 0, limit: Query = 5) -> List[Tenant]:  # type: ignore
         """List all tenants"""
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/transcoding_profiles.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/transcoding_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, List, Optional, Tuple
 
 from uplink import (
     Body,
-    Consumer,
     Query,
     delete,
     get,
     json,
     post,
     put,
     response_handler,
     returns,
 )
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import cache_api_results
 from bpkio_api.exceptions import ResourceExistsError
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.objects import find_duplicates_of
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.TranscodingProfiles import (
     TranscodingProfile,
@@ -24,15 +24,15 @@
 )
 from bpkio_api.response_handler import postprocess_response
 
 from .enums import UpsertOperationType
 
 
 @response_handler(postprocess_response)
-class TranscodingProfilesApi(Consumer):
+class TranscodingProfilesApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("transcoding-profiles")
     def get_page(
         self, offset: Query = 0, limit: Query = 50, tenant_id: Query("tenantId") = None
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/users.py` & `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Any, List, Tuple
 
-from uplink import Consumer, Query, get, response_handler, returns
+from uplink import Query, get, response_handler, returns
 
+from bpkio_api.consumer import BpkioSdkConsumer
 from bpkio_api.caching import cache_api_results
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.Users import User
 from bpkio_api.response_handler import postprocess_response
 
 
 @response_handler(postprocess_response)
-class UsersApi(Consumer):
+class UsersApi(BpkioSdkConsumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("users")
     def get_page(self, offset: Query = 0, limit: Query = 5) -> List[User]:  # type: ignore
         """List all users"""
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/exceptions.py` & `bpkio_python_sdk-1.4.0/bpkio_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/codecstrings.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/codecstrings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/dash.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/dash.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 class DASHHandler(XMLHandler):
     content_types = ["application/dash+xml"]
     file_extensions = [".mpd", ".dash"]
 
     uri_attributes = ["initialization", "media"]
     uri_elements = ["BaseURL"]
 
-    def __init__(self, url, content: bytes | None = None):
-        super().__init__(url, content)
+    def __init__(self, url, content: bytes | None = None, **kwargs):
+        super().__init__(url, content, **kwargs)
         self._document: MPD = None
 
     @property
     def document(self) -> MPD:
         # if not self._document:
         #    self._document = Parser.from_string(self.content.decode())
         # return self._document
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/factory.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import re
 from urllib.parse import urlparse
 
 import requests
 
-from bpkio_api import __version__
+from bpkio_api.defaults import USER_AGENT_FOR_HANDLERS
 from bpkio_api.exceptions import BroadpeakIoHelperError
 
 # Imports not used in the file, but necessary to ensure all handlers are loaded
 from .dash import DASHHandler
 from .generic import ContentHandler
 from .hls import HLSHandler
 from .jpeg import JPEGHandler
@@ -18,16 +18,14 @@
 from .vast import VASTHandler
 from .vmap import VMAPHandler
 from .xml import XMLHandler
 
 # Registry for subclasses
 _registry = {}
 
-# Main headers
-headers = {"User-Agent": f"bpkio-python-sdk/{__version__}"}
 
 # Timeout for HEAD
 timeout = 2
 
 logger = logging.getLogger(__name__)
 
 
@@ -40,32 +38,17 @@
 for handler_cls in all_subclasses(ContentHandler):
     for content_type in handler_cls.content_types:
         _registry[content_type] = handler_cls
     for extension in handler_cls.file_extensions:
         _registry[extension] = handler_cls
 
 
-def fetch_content_with_size_limit(url, size_limit, enforce_limit=True):
-    response = requests.get(url, stream=True, headers=headers)
-    if response.status_code != 200:
-        raise BroadpeakIoHelperError(
-            status_code=response.status_code,
-            message=f"Unable to fetch content - server response {response.status_code} for url {url}",
-            original_message="",
-        )
-
-    content = b""
-    for chunk in response.iter_content(chunk_size=1024):
-        content += chunk
-        if len(content) > size_limit:
-            raise Exception("Content too long to be parseable efficiently")
-    return content
-
+def create_handler(url, get_full_content=False, from_url_only=False, user_agent=None):
+    headers = {"User-Agent": user_agent or USER_AGENT_FOR_HANDLERS}
 
-def create_handler(url, get_full_content=False, from_url_only=False):
     try:
         content_type = ""
         if not from_url_only:
             try:
                 response = requests.head(
                     url, allow_redirects=True, headers=headers, timeout=timeout
                 )
@@ -87,16 +70,20 @@
         if handler_cls is None:
             if from_url_only:
                 raise ValueError(
                     "No information available in the URL to determine content type: "
                     f"{content_type} / {file_extension}"
                 )
 
-            content = fetch_content_with_size_limit(
-                url, 100 * 1024, enforce_limit=(not get_full_content)
+            content = ContentHandler.fetch_content_with_size_limit(
+                url=url,
+                size_limit=100 * 1024,
+                headers=headers,
+                enforce_limit=(not get_full_content),
+                timeout=timeout
             )
 
             # Fallback: analyze content if handler is not found by content-type
             # or file extension
             if content:
                 for handler in all_subclasses(ContentHandler):
                     if handler.is_supported_content(content):
@@ -105,15 +92,15 @@
 
         if handler_cls is None:
             raise ValueError(
                 "Could not determine content type from content-type, file extension, or content of URL: "
                 f"- TYPE: {content_type} \n- EXTENSION: {file_extension} \n- CONTENT: {content}"
             )
 
-        return handler_cls(url, content)
+        return handler_cls(url, content, user_agent=user_agent)
 
     except Exception as e:
         raise BroadpeakIoHelperError(
             status_code=400,
             message=f"Unable to determine a usable handler for url {url}",
             original_message=e.args[0]
             if len(e.args)
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/generic.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,87 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import Dict, List
+from typing import Dict, List, Optional
 from urllib.parse import parse_qs, urlparse
 
 import requests
 
-from bpkio_api import __version__
-
-headers = {"User-Agent": f"bpkio-python-sdk/{__version__}"}
+from bpkio_api.defaults import USER_AGENT_FOR_HANDLERS
+from bpkio_api.exceptions import BroadpeakIoHelperError
 
 
 class ContentHandler(ABC):
     content_types = []
     file_extensions = []
 
     document = None
 
     @abstractmethod
-    def __init__(self, url, content: bytes | None = None):
-        self.logger = logging.getLogger(self.__class__.__name__)
+    def __init__(
+        self, url, content: Optional[bytes] = None, user_agent: Optional[str] = None
+    ):
+        self.logger = logging.getLogger("bpkio_api.content_handler")
 
         self.url = url
         self.original_url = url
         if content:
             self._content = content
         else:
             self._content = None
 
+        self.headers = {"User-Agent": user_agent or USER_AGENT_FOR_HANDLERS}
+
         # broadpeak session id (in case handler is for a bpk sessionservice)
         self.session_id = None
 
     @property
     def content(self):
         if self._content is None:
             self._fetch_content()
         return self._content
 
     def _fetch_content(self) -> bytes:
-        self.logger.debug(f"Fetching content from {self.url}")
-        response = requests.get(self.url, headers=headers)
+        self.logger.debug(
+            f"Fetching content from {self.url} with headers {self.headers}"
+        )
+        response = requests.get(self.url, headers=self.headers)
         self._content = response.content
 
         # overwrite the URL, in case of redirect
         self.url = response.url
 
         # check if a broadpeak.io session was started
         params = parse_qs(
             urlparse(self.url).query, keep_blank_values=True, strict_parsing=False
         )
         if "sessionid" in params:
             self.session_id = params["sessionid"][0]
 
         return self._content
 
+    @staticmethod
+    def fetch_content_with_size_limit(
+        url, size_limit, headers, enforce_limit=True, timeout=5
+    ):
+        response = requests.get(url, stream=True, headers=headers)  # , timeout=timeout)
+        if response.status_code != 200:
+            raise BroadpeakIoHelperError(
+                status_code=response.status_code,
+                message="Unable to fetch content - "
+                + f"server response {response.status_code} for url {url}",
+                original_message="",
+            )
+
+        content = b""
+        for chunk in response.iter_content(chunk_size=1024):
+            content += chunk
+            if len(content) > size_limit:
+                raise Exception("Content too long to be parseable efficiently")
+        return content
+
     def reload(self):
         self._fetch_content()
 
     @staticmethod
     @abstractmethod
     def is_supported_content(content) -> bool:
         pass
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/hls.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/hls.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from .generic import ContentHandler
 
 
 class HLSHandler(ContentHandler):
     content_types = ["application/x-mpegurl", "application/vnd.apple.mpegurl"]
     file_extensions = [".m3u8", ".hls"]
 
-    def __init__(self, url, content: bytes | None = None):
-        super().__init__(url, content)
+    def __init__(self, url, content: bytes | None = None, **kwargs):
+        super().__init__(url, content, **kwargs)
         self._document: m3u8.M3U8 = None
 
     @property
     def document(self) -> m3u8.M3U8:
         if not self._document:
             self._document = m3u8.loads(content=self.content.decode(), uri=self.url)
         return self._document
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vast.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vast.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class VASTHandler(XMLHandler):
     content_types = []
     file_extensions = [".vast"]
 
     uri_elements = ["MediaFile"]
 
-    def __init__(self, url, content: bytes | None = None):
-        super().__init__(url, content)
+    def __init__(self, url, content: bytes | None = None, **kwargs):
+        super().__init__(url, content, **kwargs)
         self._document: etree._Element = None
 
     @property
     def document(self) -> etree._Element:
         if not self._document:
             self._document = etree.fromstring(self.content)
         return self._document
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vmap.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 class VMAPHandler(XMLHandler):
     content_types = []
     file_extensions = [".vmap"]
 
     uri_elements = ["vmap:AdTagURI"]
 
-    def __init__(self, url, content: bytes | None = None):
-        super().__init__(url, content)
+    def __init__(self, url, content: bytes | None = None, **kwargs):
+        super().__init__(url, content, **kwargs)
         self._document: etree._Element = None
 
     @property
     def document(self) -> etree._Element:
         if self._document is None:
             self._document = etree.fromstring(self.content)
         return self._document
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/xml.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/xml.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class XMLHandler(ContentHandler):
     content_types = []
     file_extensions = []
 
     uri_attributes = []
     uri_elements = []
 
-    def __init__(self, url, content: bytes | None = None):
-        super().__init__(url, content)
+    def __init__(self, url, content: bytes | None = None, **kwargs):
+        super().__init__(url, content, **kwargs)
 
     def read(self):
         return "Handling XML file."
 
     @staticmethod
     def is_supported_content(content) -> bool:
         return False
```

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/list.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/dash.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/hls.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/profile_generator.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/profile_generator.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/curl.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/curl.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/exporter.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/exporter.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/markdown.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/markdown.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/postman.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/postman.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_items.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_items.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_recorder.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/text.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/text.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/search.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/source_type.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/source_type.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/helpers/times.py` & `bpkio_python_sdk-1.4.0/bpkio_api/helpers/times.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/mappings.py` & `bpkio_python_sdk-1.4.0/bpkio_api/mappings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/models/Services.py` & `bpkio_python_sdk-1.4.0/bpkio_api/models/Services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/models/Slots.py` & `bpkio_python_sdk-1.4.0/bpkio_api/models/Slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/models/Sources.py` & `bpkio_python_sdk-1.4.0/bpkio_api/models/Sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/models/__init__.py` & `bpkio_python_sdk-1.4.0/bpkio_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/models/common.py` & `bpkio_python_sdk-1.4.0/bpkio_api/models/common.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/models/model_graph.py` & `bpkio_python_sdk-1.4.0/bpkio_api/models/model_graph.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.3.0/bpkio_api/response_handler.py` & `bpkio_python_sdk-1.4.0/bpkio_api/response_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 
 logger = logging.getLogger("bpkio_api.response_handler")
 
 
 def postprocess_response(response):
     """Checks whether or not the response was successful."""
 
+    headers = response.request.headers
+    if "Authorization" in headers:
+        auth = headers.get("Authorization")
+        headers["Authorization"] = auth[0:10] + "*****" + auth[-5:]
+
     logger.debug(response.request.method + " " + response.request.url)
-    logger.debug(f" ({response.status_code}) -> {response.text}")
+    logger.debug(headers)
+    logger.debug(f"> ({response.status_code}) -> {response.text}")
 
     # Record into the session
     SessionRecorder.record(response)
 
     if 200 <= response.status_code < 300:
         # invalidate cache for operations that change lists of resources
         if response.request.method in ("PUT", "DELETE", "POST"):
@@ -57,10 +63,7 @@
             message=response_payload["message"],
             reason=response.reason,
         )
 
 
 def return_count(response):
     return int(response.headers["x-pagination-total-count"])
-
-
-
```

### Comparing `bpkio_python_sdk-1.3.0/pyproject.toml` & `bpkio_python_sdk-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-python-sdk"
-version = "1.3.0"
+version = "1.4.0"
 description = "An (opinionated) Python SDK for the broadpeak.io REST APIs"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bpkio_python_sdk-1.3.0/PKG-INFO` & `bpkio_python_sdk-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-python-sdk
-Version: 1.3.0
+Version: 1.4.0
 Summary: An (opinionated) Python SDK for the broadpeak.io REST APIs
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

