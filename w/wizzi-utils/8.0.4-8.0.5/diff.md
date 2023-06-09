# Comparing `tmp/wizzi_utils-8.0.4.tar.gz` & `tmp/wizzi_utils-8.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wizzi_utils-8.0.4.tar", last modified: Fri Jun  9 13:23:41 2023, max compression
+gzip compressed data, was "dist\wizzi_utils-8.0.5.tar", last modified: Fri Jun  9 13:36:53 2023, max compression
```

## Comparing `wizzi_utils-8.0.4.tar` & `wizzi_utils-8.0.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.784065 wizzi_utils-8.0.4/
--rw-rw-rw-   0        0        0     1077 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     6839 2023-06-09 13:23:41.784065 wizzi_utils-8.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6003 2023-05-26 18:32:12.000000 wizzi_utils-8.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-06-09 13:23:41.784065 wizzi_utils-8.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2721 2023-06-09 13:19:39.000000 wizzi_utils-8.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.740213 wizzi_utils-8.0.4/wizzi_utils/
--rw-rw-rw-   0        0        0     2215 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.745195 wizzi_utils-8.0.4/wizzi_utils/google/
--rw-rw-rw-   0        0        0      140 2023-05-18 12:28:31.000000 wizzi_utils-8.0.4/wizzi_utils/google/__init__.py
--rw-rw-rw-   0        0        0    29127 2023-05-18 12:36:17.000000 wizzi_utils-8.0.4/wizzi_utils/google/google_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.746192 wizzi_utils-8.0.4/wizzi_utils/google/test/
--rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/google/test/__init__.py
--rw-rw-rw-   0        0        0    12539 2023-05-18 12:32:45.000000 wizzi_utils-8.0.4/wizzi_utils/google/test/test_google_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.747189 wizzi_utils-8.0.4/wizzi_utils/json/
--rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/json/__init__.py
--rw-rw-rw-   0        0        0     3035 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/json/json_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.749182 wizzi_utils-8.0.4/wizzi_utils/json/test/
--rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/json/test/__init__.py
--rw-rw-rw-   0        0        0     1815 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/json/test/test_json_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.750179 wizzi_utils-8.0.4/wizzi_utils/misc/
--rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/misc/__init__.py
--rw-rw-rw-   0        0        0    93477 2023-06-09 13:20:15.000000 wizzi_utils-8.0.4/wizzi_utils/misc/misc_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.751176 wizzi_utils-8.0.4/wizzi_utils/misc/test/
--rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/misc/test/__init__.py
--rw-rw-rw-   0        0        0    41133 2023-05-18 11:21:37.000000 wizzi_utils-8.0.4/wizzi_utils/misc/test/test_misc_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.754166 wizzi_utils-8.0.4/wizzi_utils/models/
--rw-rw-rw-   0        0        0      316 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/__init__.py
--rw-rw-rw-   0        0        0    32920 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/base_models.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.757159 wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/
--rw-rw-rw-   0        0        0      447 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/__init__.py
--rw-rw-rw-   0        0        0    11967 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/object_detection.py
--rw-rw-rw-   0        0        0    30085 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/pose_detection.py
--rw-rw-rw-   0        0        0    13099 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/tracking.py
--rw-rw-rw-   0        0        0    41515 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/labels_bank.py
--rw-rw-rw-   0        0        0    53088 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/models_configs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.762139 wizzi_utils-8.0.4/wizzi_utils/models/test/
--rw-rw-rw-   0        0        0      201 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/__init__.py
--rw-rw-rw-   0        0        0     9974 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/shared_code_for_tests.py
--rw-rw-rw-   0        0        0     3796 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/test_cv2_od.py
--rw-rw-rw-   0        0        0     4868 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/test_cv2_pd.py
--rw-rw-rw-   0        0        0     5884 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/test_cv2_tracking.py
--rw-rw-rw-   0        0        0     1916 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/test_models.py
--rw-rw-rw-   0        0        0     3683 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/test_tflite_od.py
--rw-rw-rw-   0        0        0     4392 2023-05-18 13:12:36.000000 wizzi_utils-8.0.4/wizzi_utils/models/test/test_tflite_pd.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.764132 wizzi_utils-8.0.4/wizzi_utils/models/tflite_models/
--rw-rw-rw-   0        0        0      308 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/tflite_models/__init__.py
--rw-rw-rw-   0        0        0    12906 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/tflite_models/object_detection.py
--rw-rw-rw-   0        0        0    19806 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/models/tflite_models/pose_detection.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.766126 wizzi_utils-8.0.4/wizzi_utils/open_cv/
--rw-rw-rw-   0        0        0      143 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/open_cv/__init__.py
--rw-rw-rw-   0        0        0    53198 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/open_cv/open_cv_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.767122 wizzi_utils-8.0.4/wizzi_utils/open_cv/test/
--rw-rw-rw-   0        0        0      113 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/open_cv/test/__init__.py
--rw-rw-rw-   0        0        0    40649 2023-05-18 12:57:14.000000 wizzi_utils-8.0.4/wizzi_utils/open_cv/test/test_open_cv_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.768119 wizzi_utils-8.0.4/wizzi_utils/pyplot/
--rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/pyplot/__init__.py
--rw-rw-rw-   0        0        0    67007 2023-06-09 13:22:11.000000 wizzi_utils-8.0.4/wizzi_utils/pyplot/pyplot_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.769116 wizzi_utils-8.0.4/wizzi_utils/pyplot/test/
--rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/pyplot/test/__init__.py
--rw-rw-rw-   0        0        0    38480 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/pyplot/test/test_pyplot_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.770112 wizzi_utils-8.0.4/wizzi_utils/socket/
--rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/socket/__init__.py
--rw-rw-rw-   0        0        0    24353 2023-05-18 11:25:24.000000 wizzi_utils-8.0.4/wizzi_utils/socket/socket_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.771109 wizzi_utils-8.0.4/wizzi_utils/socket/test/
--rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/socket/test/__init__.py
--rw-rw-rw-   0        0        0    10494 2023-05-18 11:29:49.000000 wizzi_utils-8.0.4/wizzi_utils/socket/test/test_socket_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.772106 wizzi_utils-8.0.4/wizzi_utils/tflite/
--rw-rw-rw-   0        0        0      264 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/tflite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.774099 wizzi_utils-8.0.4/wizzi_utils/tflite/test/
--rw-rw-rw-   0        0        0      105 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/tflite/test/__init__.py
--rw-rw-rw-   0        0        0      403 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/tflite/test/test_tflite.py
--rw-rw-rw-   0        0        0     2952 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/tflite/tflite_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.775096 wizzi_utils-8.0.4/wizzi_utils/torch/
--rw-rw-rw-   0        0        0      636 2023-05-26 18:23:15.000000 wizzi_utils-8.0.4/wizzi_utils/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.776092 wizzi_utils-8.0.4/wizzi_utils/torch/test/
--rw-rw-rw-   0        0        0      109 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/torch/test/__init__.py
--rw-rw-rw-   0        0        0    16354 2023-05-18 13:15:33.000000 wizzi_utils-8.0.4/wizzi_utils/torch/test/test_torch_tools.py
--rw-rw-rw-   0        0        0    26441 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/torch/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.777089 wizzi_utils-8.0.4/wizzi_utils/tts/
--rw-rw-rw-   0        0        0      125 2023-05-18 13:05:38.000000 wizzi_utils-8.0.4/wizzi_utils/tts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.778086 wizzi_utils-8.0.4/wizzi_utils/tts/test/
--rw-rw-rw-   0        0        0       99 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/tts/test/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 08:10:35.000000 wizzi_utils-8.0.4/wizzi_utils/tts/test/test_tts.py
--rw-rw-rw-   0        0        0    21592 2023-05-18 13:17:11.000000 wizzi_utils-8.0.4/wizzi_utils/tts/tts.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:23:41.743202 wizzi_utils-8.0.4/wizzi_utils.egg-info/
--rw-rw-rw-   0        0        0     6839 2023-06-09 13:23:41.000000 wizzi_utils-8.0.4/wizzi_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4360 2023-06-09 13:23:41.000000 wizzi_utils-8.0.4/wizzi_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:23:41.000000 wizzi_utils-8.0.4/wizzi_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-09 13:23:41.000000 wizzi_utils-8.0.4/wizzi_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0      491 2023-06-09 13:23:41.000000 wizzi_utils-8.0.4/wizzi_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.135202 wizzi_utils-8.0.5/
+-rw-rw-rw-   0        0        0     1077 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     6839 2023-06-09 13:36:53.135202 wizzi_utils-8.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6003 2023-05-26 18:32:12.000000 wizzi_utils-8.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-09 13:36:53.136199 wizzi_utils-8.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2721 2023-06-09 13:35:15.000000 wizzi_utils-8.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.098326 wizzi_utils-8.0.5/wizzi_utils/
+-rw-rw-rw-   0        0        0     2215 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.102313 wizzi_utils-8.0.5/wizzi_utils/google/
+-rw-rw-rw-   0        0        0      140 2023-05-18 12:28:31.000000 wizzi_utils-8.0.5/wizzi_utils/google/__init__.py
+-rw-rw-rw-   0        0        0    29127 2023-05-18 12:36:17.000000 wizzi_utils-8.0.5/wizzi_utils/google/google_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.103309 wizzi_utils-8.0.5/wizzi_utils/google/test/
+-rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/google/test/__init__.py
+-rw-rw-rw-   0        0        0    12539 2023-05-18 12:32:45.000000 wizzi_utils-8.0.5/wizzi_utils/google/test/test_google_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.105302 wizzi_utils-8.0.5/wizzi_utils/json/
+-rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/__init__.py
+-rw-rw-rw-   0        0        0     3035 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/json_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.106299 wizzi_utils-8.0.5/wizzi_utils/json/test/
+-rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/test/__init__.py
+-rw-rw-rw-   0        0        0     1815 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/test/test_json_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.106299 wizzi_utils-8.0.5/wizzi_utils/misc/
+-rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/misc/__init__.py
+-rw-rw-rw-   0        0        0    93477 2023-06-09 13:35:19.000000 wizzi_utils-8.0.5/wizzi_utils/misc/misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.108292 wizzi_utils-8.0.5/wizzi_utils/misc/test/
+-rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/misc/test/__init__.py
+-rw-rw-rw-   0        0        0    41133 2023-05-18 11:21:37.000000 wizzi_utils-8.0.5/wizzi_utils/misc/test/test_misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.110286 wizzi_utils-8.0.5/wizzi_utils/models/
+-rw-rw-rw-   0        0        0      316 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/__init__.py
+-rw-rw-rw-   0        0        0    32920 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/base_models.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.112279 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/
+-rw-rw-rw-   0        0        0      447 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/__init__.py
+-rw-rw-rw-   0        0        0    11967 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/object_detection.py
+-rw-rw-rw-   0        0        0    30085 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/pose_detection.py
+-rw-rw-rw-   0        0        0    13099 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/tracking.py
+-rw-rw-rw-   0        0        0    41515 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/labels_bank.py
+-rw-rw-rw-   0        0        0    53088 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/models_configs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.116266 wizzi_utils-8.0.5/wizzi_utils/models/test/
+-rw-rw-rw-   0        0        0      201 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/__init__.py
+-rw-rw-rw-   0        0        0     9974 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/shared_code_for_tests.py
+-rw-rw-rw-   0        0        0     3796 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_od.py
+-rw-rw-rw-   0        0        0     4868 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_pd.py
+-rw-rw-rw-   0        0        0     5884 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_tracking.py
+-rw-rw-rw-   0        0        0     1916 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_models.py
+-rw-rw-rw-   0        0        0     3683 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_od.py
+-rw-rw-rw-   0        0        0     4392 2023-05-18 13:12:36.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_pd.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.118259 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/
+-rw-rw-rw-   0        0        0      308 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/__init__.py
+-rw-rw-rw-   0        0        0    12906 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/object_detection.py
+-rw-rw-rw-   0        0        0    19806 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/pose_detection.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.119255 wizzi_utils-8.0.5/wizzi_utils/open_cv/
+-rw-rw-rw-   0        0        0      143 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/__init__.py
+-rw-rw-rw-   0        0        0    53198 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/open_cv_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.120252 wizzi_utils-8.0.5/wizzi_utils/open_cv/test/
+-rw-rw-rw-   0        0        0      113 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/test/__init__.py
+-rw-rw-rw-   0        0        0    40649 2023-05-18 12:57:14.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/test/test_open_cv_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.121249 wizzi_utils-8.0.5/wizzi_utils/pyplot/
+-rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/__init__.py
+-rw-rw-rw-   0        0        0    67007 2023-06-09 13:22:11.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/pyplot_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.122245 wizzi_utils-8.0.5/wizzi_utils/pyplot/test/
+-rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/test/__init__.py
+-rw-rw-rw-   0        0        0    38480 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/test/test_pyplot_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.123242 wizzi_utils-8.0.5/wizzi_utils/socket/
+-rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/socket/__init__.py
+-rw-rw-rw-   0        0        0    24353 2023-05-18 11:25:24.000000 wizzi_utils-8.0.5/wizzi_utils/socket/socket_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.124239 wizzi_utils-8.0.5/wizzi_utils/socket/test/
+-rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/socket/test/__init__.py
+-rw-rw-rw-   0        0        0    10494 2023-05-18 11:29:49.000000 wizzi_utils-8.0.5/wizzi_utils/socket/test/test_socket_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.125235 wizzi_utils-8.0.5/wizzi_utils/tflite/
+-rw-rw-rw-   0        0        0      264 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.125235 wizzi_utils-8.0.5/wizzi_utils/tflite/test/
+-rw-rw-rw-   0        0        0      105 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/test/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/test/test_tflite.py
+-rw-rw-rw-   0        0        0     2952 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/tflite_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.126232 wizzi_utils-8.0.5/wizzi_utils/torch/
+-rw-rw-rw-   0        0        0      636 2023-05-26 18:23:15.000000 wizzi_utils-8.0.5/wizzi_utils/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.127229 wizzi_utils-8.0.5/wizzi_utils/torch/test/
+-rw-rw-rw-   0        0        0      109 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/torch/test/__init__.py
+-rw-rw-rw-   0        0        0    16354 2023-05-18 13:15:33.000000 wizzi_utils-8.0.5/wizzi_utils/torch/test/test_torch_tools.py
+-rw-rw-rw-   0        0        0    26441 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/torch/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.128225 wizzi_utils-8.0.5/wizzi_utils/tts/
+-rw-rw-rw-   0        0        0      125 2023-05-18 13:05:38.000000 wizzi_utils-8.0.5/wizzi_utils/tts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.129222 wizzi_utils-8.0.5/wizzi_utils/tts/test/
+-rw-rw-rw-   0        0        0       99 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tts/test/__init__.py
+-rw-rw-rw-   0        0        0     3309 2023-06-09 13:28:53.000000 wizzi_utils-8.0.5/wizzi_utils/tts/test/test_tts.py
+-rw-rw-rw-   0        0        0    21600 2023-06-09 13:31:50.000000 wizzi_utils-8.0.5/wizzi_utils/tts/tts.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.101315 wizzi_utils-8.0.5/wizzi_utils.egg-info/
+-rw-rw-rw-   0        0        0     6839 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4360 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      491 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/top_level.txt
```

### Comparing `wizzi_utils-8.0.4/LICENSE.txt` & `wizzi_utils-8.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/PKG-INFO` & `wizzi_utils-8.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wizzi_utils
-Version: 8.0.4
+Version: 8.0.5
 Summary: Debugging tools and fast coding
 Home-page: https://github.com/2easy4wizzi/wizzi_utils_pypi
 Author: Gilad Eini
 Author-email: giladEini@gmail.com
 License: MIT
-Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.4.tar.gz
+Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.5.tar.gz
 Keywords: debugging tools,json,open cv,pyplot,socket,torch,tf lite
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wizzi_utils-8.0.4/README.md` & `wizzi_utils-8.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/setup.py` & `wizzi_utils-8.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
         'wizzi_utils/tts',
         'wizzi_utils/tts/test',
         'wizzi_utils/models',
         'wizzi_utils/models/cv2_models',
         'wizzi_utils/models/tflite_models',
         'wizzi_utils/models/test',
     ],
-    version='8.0.4',
+    version='8.0.5',
     license='MIT',  # https://help.github.com/articles/licensing-a-repository
     description='Debugging tools and fast coding',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Gilad Eini',
     author_email='giladEini@gmail.com',
     url='https://github.com/2easy4wizzi/wizzi_utils_pypi',  # link to github
-    download_url='https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.4.tar.gz',
+    download_url='https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.5.tar.gz',
     keywords=[  # Keywords that define your package best
         'debugging tools',
         'json',
         'open cv',
         'pyplot',
         'socket',
         'torch',
```

### Comparing `wizzi_utils-8.0.4/wizzi_utils/__init__.py` & `wizzi_utils-8.0.5/wizzi_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/google/google_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/google/google_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/google/test/test_google_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/google/test/test_google_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/json/json_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/json/json_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/json/test/test_json_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/json/test/test_json_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/misc/misc_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/misc/misc_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
 
 
 def version() -> str:
     """
     :return:
     """
     # v = pkg_resources.require("wizzi_utils")[0].version
-    v = '8.0.4'
+    v = '8.0.5'
     return v
 
 
 def is_windows() -> bool:
     """
     :return:
     see os_test() - tested
```

### Comparing `wizzi_utils-8.0.4/wizzi_utils/misc/test/test_misc_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/misc/test/test_misc_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/base_models.py` & `wizzi_utils-8.0.5/wizzi_utils/models/base_models.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/object_detection.py` & `wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/object_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/pose_detection.py` & `wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/pose_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/cv2_models/tracking.py` & `wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/tracking.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/labels_bank.py` & `wizzi_utils-8.0.5/wizzi_utils/models/labels_bank.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/models_configs.py` & `wizzi_utils-8.0.5/wizzi_utils/models/models_configs.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/shared_code_for_tests.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/shared_code_for_tests.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/test_cv2_od.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_od.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/test_cv2_pd.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_pd.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/test_cv2_tracking.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_tracking.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/test_models.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/test_models.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/test_tflite_od.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_od.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/test/test_tflite_pd.py` & `wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_pd.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/tflite_models/object_detection.py` & `wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/object_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/models/tflite_models/pose_detection.py` & `wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/pose_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/open_cv/open_cv_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/open_cv/open_cv_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/open_cv/test/test_open_cv_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/open_cv/test/test_open_cv_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/pyplot/pyplot_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/pyplot/pyplot_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/pyplot/test/test_pyplot_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/pyplot/test/test_pyplot_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/socket/socket_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/socket/socket_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/socket/test/test_socket_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/socket/test/test_socket_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/tflite/tflite_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/tflite/tflite_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/torch/__init__.py` & `wizzi_utils-8.0.5/wizzi_utils/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/torch/test/test_torch_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/torch/test/test_torch_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/torch/torch_tools.py` & `wizzi_utils-8.0.5/wizzi_utils/torch/torch_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.4/wizzi_utils/tts/test/test_tts.py` & `wizzi_utils-8.0.5/wizzi_utils/tts/test/test_tts.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,16 +86,18 @@
         cs = [
             'I say this a lot of times',
             'what\'s cooking good looking'
         ]
         run_machine_buddy_gui(voice_idx=0, rate=150, volume=90, loc='tl', common_sentences=cs)
     except ImportError as e:
         mt.exception_error(e, real_exception=True)
-        mt.exception_error('try pip install PyQt5')
-        mt.exception_error('or pip install matplotlib')
+        mt.exception_error('try: pip install PyQt5')
+        mt.exception_error('pip install PyQt5')
+        mt.exception_error('pip install matplotlib')
+        mt.exception_error('python -m pip install --upgrade --force-reinstall PyQt5')
     return
 
 
 def test_all():
     print('{}{}:'.format('-' * 5, mt.get_base_file_and_function_name(depth=1)))
     str_test()
     instance_test()
```

### Comparing `wizzi_utils-8.0.4/wizzi_utils/tts/tts.py` & `wizzi_utils-8.0.5/wizzi_utils/tts/tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
             common_say = self.common_combo.currentText()
             if common_say:
                 print('common say {}'.format(common_say))
                 self.machine_buddy.say(text=common_say)
             return
 
         @staticmethod
-        def keyPressEvent(event: QtGui.QKeyEvent):
+        def keyPressEvent(event: QtGui.QKeyEvent):  # noqa
             if event.key() in [QtCore.Qt.Key_Escape]:
                 print('keyPressEvent(): Qt plot: Esc was clicked. Terminating...')
                 MachineBuddyGui.get_qt_app().quit()
 
         @staticmethod
         def get_qt_app() -> QtWidgets.QApplication:
             app = QtWidgets.QApplication.instance()  # main app must init before creating GLViewWidget
```

### Comparing `wizzi_utils-8.0.4/wizzi_utils.egg-info/PKG-INFO` & `wizzi_utils-8.0.5/wizzi_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wizzi-utils
-Version: 8.0.4
+Version: 8.0.5
 Summary: Debugging tools and fast coding
 Home-page: https://github.com/2easy4wizzi/wizzi_utils_pypi
 Author: Gilad Eini
 Author-email: giladEini@gmail.com
 License: MIT
-Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.4.tar.gz
+Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.5.tar.gz
 Keywords: debugging tools,json,open cv,pyplot,socket,torch,tf lite
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wizzi_utils-8.0.4/wizzi_utils.egg-info/SOURCES.txt` & `wizzi_utils-8.0.5/wizzi_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

