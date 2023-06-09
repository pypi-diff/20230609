# Comparing `tmp/fro_AI-0.8.4.tar.gz` & `tmp/fro_AI-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fro_AI-0.8.4.tar", last modified: Wed Aug  4 02:04:19 2021, max compression
+gzip compressed data, was "fro_AI-0.9.0.tar", last modified: Wed Aug  4 09:08:44 2021, max compression
```

## Comparing `fro_AI-0.8.4.tar` & `fro_AI-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.631606 fro_AI-0.8.4/
--rw-rw-rw-   0        0        0     1069 2020-12-17 01:10:12.000000 fro_AI-0.8.4/LICENSE
--rw-rw-rw-   0        0        0      465 2021-08-04 02:04:19.630629 fro_AI-0.8.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.330817 fro_AI-0.8.4/fro_AI/
--rw-rw-rw-   0        0        0     3084 2021-06-03 05:41:03.000000 fro_AI-0.8.4/fro_AI/Aruco.py
--rw-rw-rw-   0        0        0      217 2021-08-04 02:02:43.000000 fro_AI-0.8.4/fro_AI/__init__.py
--rw-rw-rw-   0        0        0     6303 2021-05-19 01:21:35.000000 fro_AI-0.8.4/fro_AI/classifier.py
--rw-rw-rw-   0        0        0     2974 2021-05-17 06:29:42.000000 fro_AI-0.8.4/fro_AI/color.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.353278 fro_AI-0.8.4/fro_AI/data/
--rw-rw-rw-   0        0        0    31565 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/data/imageNet_labels.txt
--rw-rw-rw-   0        0        0    14937 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face.py
--rw-rw-rw-   0        0        0     6002 2021-08-04 01:56:43.000000 fro_AI-0.8.4/fro_AI/face_detect.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.376716 fro_AI-0.8.4/fro_AI/face_evoLve/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.466562 fro_AI-0.8.4/fro_AI/face_evoLve/align/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/__init__.py
--rw-rw-rw-   0        0        0    10891 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/align_trans.py
--rw-rw-rw-   0        0        0     6926 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/box_utils.py
--rw-rw-rw-   0        0        0     4205 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/detector.py
--rw-rw-rw-   0        0        0     2901 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/face_align.py
--rw-rw-rw-   0        0        0     2609 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/face_resize.py
--rw-rw-rw-   0        0        0     3010 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/first_stage.py
--rw-rw-rw-   0        0        0     5145 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/get_nets.py
--rw-rw-rw-   0        0        0     8447 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/matlab_cp2tform.py
--rw-rw-rw-   0        0        0  2345483 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/onet.npy
--rw-rw-rw-   0        0        0    41271 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/pnet.npy
--rw-rw-rw-   0        0        0   604651 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/rnet.npy
--rw-rw-rw-   0        0        0      801 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/align/visualization_utils.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.482187 fro_AI-0.8.4/fro_AI/face_evoLve/backbone/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backbone/__init__.py
--rw-rw-rw-   0        0        0     7418 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backbone/model_irse.py
--rw-rw-rw-   0        0        0     5756 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backbone/model_resnet.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.527110 fro_AI-0.8.4/fro_AI/face_evoLve/backup/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/__init__.py
--rw-rw-rw-   0        0        0     1963 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/config.py
--rw-rw-rw-   0        0        0     1671 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/data_pipe.py
--rw-rw-rw-   0        0        0     9249 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/metrics.py
--rw-rw-rw-   0        0        0      670 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/prepare_data.py
--rw-rw-rw-   0        0        0    16788 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/train.py
--rw-rw-rw-   0        0        0     7584 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/backup/utils.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.533946 fro_AI-0.8.4/fro_AI/face_evoLve/balance/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/balance/__init__.py
--rw-rw-rw-   0        0        0      988 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/balance/remove_lowshot.py
--rw-rw-rw-   0        0        0     1942 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/config.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.541759 fro_AI-0.8.4/fro_AI/face_evoLve/head/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/head/__init__.py
--rw-rw-rw-   0        0        0    13954 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/head/metrics.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.548595 fro_AI-0.8.4/fro_AI/face_evoLve/loss/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/loss/__init__.py
--rw-rw-rw-   0        0        0      448 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/loss/focal.py
--rw-rw-rw-   0        0        0    13636 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/face_evoLve/train.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.579846 fro_AI-0.8.4/fro_AI/face_evoLve/util/
--rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/util/__init__.py
--rw-rw-rw-   0        0        0     3253 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/util/extract_feature_v1.py
--rw-rw-rw-   0        0        0     2206 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/util/extract_feature_v2.py
--rw-rw-rw-   0        0        0     8246 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/util/utils.py
--rw-rw-rw-   0        0        0     7781 2020-12-17 01:10:12.000000 fro_AI-0.8.4/fro_AI/face_evoLve/util/verification.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.619887 fro_AI-0.8.4/fro_AI/utils/
--rw-rw-rw-   0        0        0      120 2021-07-12 07:56:54.000000 fro_AI-0.8.4/fro_AI/utils/__init__.py
--rw-rw-rw-   0        0        0     1525 2021-05-19 07:12:06.000000 fro_AI-0.8.4/fro_AI/utils/camera.py
--rw-rw-rw-   0        0        0    10821 2021-05-18 03:05:15.000000 fro_AI-0.8.4/fro_AI/utils/data_utils.py
--rw-rw-rw-   0        0        0    11278 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/utils/generic_utils.py
--rw-rw-rw-   0        0        0     1352 2021-05-19 07:15:29.000000 fro_AI-0.8.4/fro_AI/utils/img_utils.py
--rw-rw-rw-   0        0        0     2767 2020-12-17 01:10:11.000000 fro_AI-0.8.4/fro_AI/utils/io_utils.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.628676 fro_AI-0.8.4/fro_AI/utils/templates/
--rw-rw-rw-   0        0        0      123 2021-07-12 08:01:05.000000 fro_AI-0.8.4/fro_AI/utils/templates/index.html
--rw-rw-rw-   0        0        0     1007 2021-05-19 08:31:51.000000 fro_AI-0.8.4/fro_AI/utils/usb_camera.py
--rw-rw-rw-   0        0        0     2537 2021-07-12 07:56:45.000000 fro_AI-0.8.4/fro_AI/utils/webstream.py
-drwxrwxrwx   0        0        0        0 2021-08-04 02:04:19.344489 fro_AI-0.8.4/fro_AI.egg-info/
--rw-rw-rw-   0        0        0      465 2021-08-04 02:04:19.000000 fro_AI-0.8.4/fro_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1952 2021-08-04 02:04:19.000000 fro_AI-0.8.4/fro_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-04 02:04:19.000000 fro_AI-0.8.4/fro_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2021-08-04 02:04:19.000000 fro_AI-0.8.4/fro_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-08-04 02:04:19.000000 fro_AI-0.8.4/fro_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-04 02:04:19.631606 fro_AI-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1343 2021-07-12 08:41:20.000000 fro_AI-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.121157 fro_AI-0.9.0/
+-rw-rw-rw-   0        0        0     1069 2020-12-17 01:10:12.000000 fro_AI-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      465 2021-08-04 09:08:44.120180 fro_AI-0.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.014708 fro_AI-0.9.0/fro_AI/
+-rw-rw-rw-   0        0        0     3084 2021-06-03 05:41:03.000000 fro_AI-0.9.0/fro_AI/Aruco.py
+-rw-rw-rw-   0        0        0       23 2021-08-04 09:08:02.000000 fro_AI-0.9.0/fro_AI/__init__.py
+-rw-rw-rw-   0        0        0     6303 2021-05-19 01:21:35.000000 fro_AI-0.9.0/fro_AI/classifier.py
+-rw-rw-rw-   0        0        0     2974 2021-05-17 06:29:42.000000 fro_AI-0.9.0/fro_AI/color.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.036193 fro_AI-0.9.0/fro_AI/data/
+-rw-rw-rw-   0        0        0    31565 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/data/imageNet_labels.txt
+-rw-rw-rw-   0        0        0    14937 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face.py
+-rw-rw-rw-   0        0        0     6002 2021-08-04 01:56:43.000000 fro_AI-0.9.0/fro_AI/face_detect.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.041077 fro_AI-0.9.0/fro_AI/face_evoLve/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/__init__.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.064514 fro_AI-0.9.0/fro_AI/face_evoLve/align/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/__init__.py
+-rw-rw-rw-   0        0        0    10891 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/align_trans.py
+-rw-rw-rw-   0        0        0     6926 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/box_utils.py
+-rw-rw-rw-   0        0        0     4205 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/detector.py
+-rw-rw-rw-   0        0        0     2901 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/face_align.py
+-rw-rw-rw-   0        0        0     2609 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/face_resize.py
+-rw-rw-rw-   0        0        0     3010 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/first_stage.py
+-rw-rw-rw-   0        0        0     5145 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/get_nets.py
+-rw-rw-rw-   0        0        0     8447 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/matlab_cp2tform.py
+-rw-rw-rw-   0        0        0  2345483 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/onet.npy
+-rw-rw-rw-   0        0        0    41271 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/pnet.npy
+-rw-rw-rw-   0        0        0   604651 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/rnet.npy
+-rw-rw-rw-   0        0        0      801 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/align/visualization_utils.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.070374 fro_AI-0.9.0/fro_AI/face_evoLve/backbone/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backbone/__init__.py
+-rw-rw-rw-   0        0        0     7418 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backbone/model_irse.py
+-rw-rw-rw-   0        0        0     5756 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backbone/model_resnet.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.080140 fro_AI-0.9.0/fro_AI/face_evoLve/backup/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/__init__.py
+-rw-rw-rw-   0        0        0     1963 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/config.py
+-rw-rw-rw-   0        0        0     1671 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/data_pipe.py
+-rw-rw-rw-   0        0        0     9249 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/metrics.py
+-rw-rw-rw-   0        0        0      670 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/prepare_data.py
+-rw-rw-rw-   0        0        0    16788 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/train.py
+-rw-rw-rw-   0        0        0     7584 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/backup/utils.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.083069 fro_AI-0.9.0/fro_AI/face_evoLve/balance/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/balance/__init__.py
+-rw-rw-rw-   0        0        0      988 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/balance/remove_lowshot.py
+-rw-rw-rw-   0        0        0     1942 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/config.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.085999 fro_AI-0.9.0/fro_AI/face_evoLve/head/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/head/__init__.py
+-rw-rw-rw-   0        0        0    13954 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/head/metrics.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.088929 fro_AI-0.9.0/fro_AI/face_evoLve/loss/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/loss/__init__.py
+-rw-rw-rw-   0        0        0      448 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/loss/focal.py
+-rw-rw-rw-   0        0        0    13636 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/face_evoLve/train.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.096742 fro_AI-0.9.0/fro_AI/face_evoLve/util/
+-rw-rw-rw-   0        0        0        1 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/util/__init__.py
+-rw-rw-rw-   0        0        0     3253 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/util/extract_feature_v1.py
+-rw-rw-rw-   0        0        0     2206 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/util/extract_feature_v2.py
+-rw-rw-rw-   0        0        0     8246 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/util/utils.py
+-rw-rw-rw-   0        0        0     7781 2020-12-17 01:10:12.000000 fro_AI-0.9.0/fro_AI/face_evoLve/util/verification.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.114320 fro_AI-0.9.0/fro_AI/utils/
+-rw-rw-rw-   0        0        0        0 2021-08-04 09:08:02.000000 fro_AI-0.9.0/fro_AI/utils/__init__.py
+-rw-rw-rw-   0        0        0     1525 2021-05-19 07:12:06.000000 fro_AI-0.9.0/fro_AI/utils/camera.py
+-rw-rw-rw-   0        0        0    10821 2021-05-18 03:05:15.000000 fro_AI-0.9.0/fro_AI/utils/data_utils.py
+-rw-rw-rw-   0        0        0    11278 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/utils/generic_utils.py
+-rw-rw-rw-   0        0        0     1352 2021-05-19 07:15:29.000000 fro_AI-0.9.0/fro_AI/utils/img_utils.py
+-rw-rw-rw-   0        0        0     2767 2020-12-17 01:10:11.000000 fro_AI-0.9.0/fro_AI/utils/io_utils.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.118227 fro_AI-0.9.0/fro_AI/utils/templates/
+-rw-rw-rw-   0        0        0      123 2021-07-12 08:01:05.000000 fro_AI-0.9.0/fro_AI/utils/templates/index.html
+-rw-rw-rw-   0        0        0     1007 2021-05-19 08:31:51.000000 fro_AI-0.9.0/fro_AI/utils/usb_camera.py
+-rw-rw-rw-   0        0        0     2537 2021-07-12 07:56:45.000000 fro_AI-0.9.0/fro_AI/utils/webstream.py
+drwxrwxrwx   0        0        0        0 2021-08-04 09:08:44.035217 fro_AI-0.9.0/fro_AI.egg-info/
+-rw-rw-rw-   0        0        0      465 2021-08-04 09:08:43.000000 fro_AI-0.9.0/fro_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1952 2021-08-04 09:08:43.000000 fro_AI-0.9.0/fro_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-04 09:08:43.000000 fro_AI-0.9.0/fro_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2021-08-04 09:08:43.000000 fro_AI-0.9.0/fro_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-08-04 09:08:43.000000 fro_AI-0.9.0/fro_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-08-04 09:08:44.121157 fro_AI-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2021-07-12 08:41:20.000000 fro_AI-0.9.0/setup.py
```

### Comparing `fro_AI-0.8.4/LICENSE` & `fro_AI-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/Aruco.py` & `fro_AI-0.9.0/fro_AI/Aruco.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/classifier.py` & `fro_AI-0.9.0/fro_AI/classifier.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/color.py` & `fro_AI-0.9.0/fro_AI/color.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/data/imageNet_labels.txt` & `fro_AI-0.9.0/fro_AI/data/imageNet_labels.txt`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face.py` & `fro_AI-0.9.0/fro_AI/face.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_detect.py` & `fro_AI-0.9.0/fro_AI/face_detect.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/align_trans.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/align_trans.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/box_utils.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/box_utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/detector.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/detector.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/face_align.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/face_align.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/face_resize.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/face_resize.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/first_stage.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/first_stage.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/get_nets.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/get_nets.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/matlab_cp2tform.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/onet.npy` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/onet.npy`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/pnet.npy` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/pnet.npy`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/rnet.npy` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/rnet.npy`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/align/visualization_utils.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/align/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backbone/model_irse.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backbone/model_irse.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backbone/model_resnet.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backbone/model_resnet.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backup/config.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backup/config.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backup/data_pipe.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backup/data_pipe.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backup/metrics.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backup/metrics.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backup/prepare_data.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backup/prepare_data.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backup/train.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backup/train.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/backup/utils.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/backup/utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/balance/remove_lowshot.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/balance/remove_lowshot.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/config.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/config.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/head/metrics.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/head/metrics.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/train.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/train.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/util/extract_feature_v1.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/util/extract_feature_v1.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/util/extract_feature_v2.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/util/extract_feature_v2.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/util/utils.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/util/utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/face_evoLve/util/verification.py` & `fro_AI-0.9.0/fro_AI/face_evoLve/util/verification.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/camera.py` & `fro_AI-0.9.0/fro_AI/utils/camera.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/data_utils.py` & `fro_AI-0.9.0/fro_AI/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/generic_utils.py` & `fro_AI-0.9.0/fro_AI/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/img_utils.py` & `fro_AI-0.9.0/fro_AI/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/io_utils.py` & `fro_AI-0.9.0/fro_AI/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/usb_camera.py` & `fro_AI-0.9.0/fro_AI/utils/usb_camera.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI/utils/webstream.py` & `fro_AI-0.9.0/fro_AI/utils/webstream.py`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/fro_AI.egg-info/SOURCES.txt` & `fro_AI-0.9.0/fro_AI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fro_AI-0.8.4/setup.py` & `fro_AI-0.9.0/setup.py`

 * *Files identical despite different names*

