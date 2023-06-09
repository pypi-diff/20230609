# Comparing `tmp/vaaibody-0.0.0.5.tar.gz` & `tmp/vaaibody-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaaibody-0.0.0.5.tar", last modified: Fri Jun  9 04:16:49 2023, max compression
+gzip compressed data, was "vaaibody-0.0.1.tar", last modified: Fri Jun  9 06:43:05 2023, max compression
```

## Comparing `vaaibody-0.0.0.5.tar` & `vaaibody-0.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      169 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/PKG-INFO
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       38 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/setup.cfg
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      687 2023-06-09 04:16:38.000000 vaaibody-0.0.0.5/setup.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:20:31.000000 vaaibody-0.0.0.5/source/vaaibody/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5718 2023-06-09 04:15:51.000000 vaaibody-0.0.0.5/source/vaaibody/audio_gest_player.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     6953 2023-06-09 04:15:51.000000 vaaibody-0.0.0.5/source/vaaibody/bvh_viewer.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/core/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:13.000000 vaaibody-0.0.0.5/source/vaaibody/core/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12912 2023-06-09 03:59:56.000000 vaaibody-0.0.0.5/source/vaaibody/core/audio.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23035 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/blending.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    28229 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/database.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    15953 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/feature.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1265 2023-06-09 04:05:38.000000 vaaibody-0.0.0.5/source/vaaibody/core/filter_frame.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    19689 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/frame.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    50321 2023-06-09 04:16:07.000000 vaaibody-0.0.0.5/source/vaaibody/core/gesture_matching.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      279 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/core/modAudio.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23436 2023-06-09 03:59:15.000000 vaaibody-0.0.0.5/source/vaaibody/core/motion.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9845 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/core/skeleton.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1488 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4740 2023-06-09 04:14:32.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor_savedb.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23778 2023-06-09 04:14:42.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor_train.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9413 2023-06-09 04:14:48.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor_util.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2734 2023-06-09 04:14:56.000000 vaaibody-0.0.0.5/source/vaaibody/dump_test.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3937 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/main.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3825 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/main_nn.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/module/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:33.000000 vaaibody-0.0.0.5/source/vaaibody/module/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4013 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/module/idle_module.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12346 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/module/nontalking_control_module.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7487 2023-06-08 05:10:08.000000 vaaibody-0.0.0.5/source/vaaibody/module/tag_processing_module.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3445 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/module/transition_module.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/parameter/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:26:25.000000 vaaibody-0.0.0.5/source/vaaibody/parameter/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1703 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/parameter/gesture_matching_parameter.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/utilities/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:27:54.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8585 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/audio_motion_synch.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1310 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/audio_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14676 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/blending_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5318 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/exporter.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8788 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/filter.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    11236 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/frame_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7150 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/motion_var_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9975 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/quat.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    16430 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/rendering_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      890 2023-06-08 05:10:08.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/timechecker.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1779 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/txform.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1641 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/utils.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/viewer/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:28:52.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3294 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/camera.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1149 2023-06-09 04:02:53.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/controller.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5648 2023-06-09 04:13:09.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/double_bvh_viewer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8045 2023-06-09 04:13:26.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/gesture_result_viewer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14081 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/gui_viewer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1079 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/handler.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      795 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/item_data.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4418 2023-06-09 04:03:09.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/item_drawer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      527 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/obj_loader.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody.egg-info/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      169 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/PKG-INFO
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2102 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/SOURCES.txt
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        1 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/dependency_links.txt
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       27 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/requires.txt
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        9 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/top_level.txt
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      167 2023-06-09 06:43:05.133366 vaaibody-0.0.1/PKG-INFO
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       38 2023-06-09 06:43:05.133366 vaaibody-0.0.1/setup.cfg
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      685 2023-06-09 06:42:41.000000 vaaibody-0.0.1/setup.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:20:31.000000 vaaibody-0.0.1/source/vaaibody/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5593 2023-06-09 05:25:34.000000 vaaibody-0.0.1/source/vaaibody/audio_gest_player.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     6953 2023-06-09 04:15:51.000000 vaaibody-0.0.1/source/vaaibody/bvh_viewer.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody/core/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:13.000000 vaaibody-0.0.1/source/vaaibody/core/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12912 2023-06-09 03:59:56.000000 vaaibody-0.0.1/source/vaaibody/core/audio.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23035 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/core/blending.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    28229 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/core/database.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    15953 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/core/feature.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1265 2023-06-09 04:05:38.000000 vaaibody-0.0.1/source/vaaibody/core/filter_frame.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    19109 2023-06-09 05:44:32.000000 vaaibody-0.0.1/source/vaaibody/core/frame.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    36600 2023-06-09 05:42:04.000000 vaaibody-0.0.1/source/vaaibody/core/gesture_matching.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      279 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/core/modAudio.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23436 2023-06-09 03:59:15.000000 vaaibody-0.0.1/source/vaaibody/core/motion.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9845 2023-05-24 02:03:55.000000 vaaibody-0.0.1/source/vaaibody/core/skeleton.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1488 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/decompressor.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4740 2023-06-09 04:14:32.000000 vaaibody-0.0.1/source/vaaibody/decompressor_savedb.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23778 2023-06-09 04:14:42.000000 vaaibody-0.0.1/source/vaaibody/decompressor_train.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9413 2023-06-09 04:14:48.000000 vaaibody-0.0.1/source/vaaibody/decompressor_util.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3007 2023-06-09 05:13:32.000000 vaaibody-0.0.1/source/vaaibody/dump_test.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3765 2023-06-09 05:46:29.000000 vaaibody-0.0.1/source/vaaibody/main.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3825 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/main_nn.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody/module/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:33.000000 vaaibody-0.0.1/source/vaaibody/module/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4013 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/module/idle_module.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12407 2023-06-09 05:44:48.000000 vaaibody-0.0.1/source/vaaibody/module/nontalking_control_module.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7514 2023-06-09 05:11:11.000000 vaaibody-0.0.1/source/vaaibody/module/tag_processing_module.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3489 2023-06-09 05:18:26.000000 vaaibody-0.0.1/source/vaaibody/module/transition_module.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody/parameter/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:26:25.000000 vaaibody-0.0.1/source/vaaibody/parameter/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1703 2023-05-24 02:03:55.000000 vaaibody-0.0.1/source/vaaibody/parameter/gesture_matching_parameter.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody/utilities/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:27:54.000000 vaaibody-0.0.1/source/vaaibody/utilities/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8585 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/utilities/audio_motion_synch.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1319 2023-06-09 05:11:51.000000 vaaibody-0.0.1/source/vaaibody/utilities/audio_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14703 2023-06-09 05:12:01.000000 vaaibody-0.0.1/source/vaaibody/utilities/blending_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5327 2023-06-09 05:12:04.000000 vaaibody-0.0.1/source/vaaibody/utilities/exporter.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8788 2023-05-24 02:03:55.000000 vaaibody-0.0.1/source/vaaibody/utilities/filter.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    11254 2023-06-09 05:12:17.000000 vaaibody-0.0.1/source/vaaibody/utilities/frame_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7168 2023-06-09 05:12:26.000000 vaaibody-0.0.1/source/vaaibody/utilities/motion_var_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9975 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/utilities/quat.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    16411 2023-06-09 05:12:34.000000 vaaibody-0.0.1/source/vaaibody/utilities/rendering_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      890 2023-06-08 05:10:08.000000 vaaibody-0.0.1/source/vaaibody/utilities/timechecker.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1779 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/utilities/txform.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1641 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/utilities/utils.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody/viewer/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:28:52.000000 vaaibody-0.0.1/source/vaaibody/viewer/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3294 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/viewer/camera.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1149 2023-06-09 04:02:53.000000 vaaibody-0.0.1/source/vaaibody/viewer/controller.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5648 2023-06-09 04:13:09.000000 vaaibody-0.0.1/source/vaaibody/viewer/double_bvh_viewer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5216 2023-06-09 05:48:27.000000 vaaibody-0.0.1/source/vaaibody/viewer/gesture_result_viewer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14081 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/viewer/gui_viewer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1079 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/viewer/handler.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      795 2023-05-24 02:01:11.000000 vaaibody-0.0.1/source/vaaibody/viewer/item_data.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4418 2023-06-09 04:03:09.000000 vaaibody-0.0.1/source/vaaibody/viewer/item_drawer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      527 2023-06-09 04:15:52.000000 vaaibody-0.0.1/source/vaaibody/viewer/obj_loader.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 06:43:05.133366 vaaibody-0.0.1/source/vaaibody.egg-info/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      167 2023-06-09 06:43:05.000000 vaaibody-0.0.1/source/vaaibody.egg-info/PKG-INFO
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2102 2023-06-09 06:43:05.000000 vaaibody-0.0.1/source/vaaibody.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        1 2023-06-09 06:43:05.000000 vaaibody-0.0.1/source/vaaibody.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       27 2023-06-09 06:43:05.000000 vaaibody-0.0.1/source/vaaibody.egg-info/requires.txt
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        9 2023-06-09 06:43:05.000000 vaaibody-0.0.1/source/vaaibody.egg-info/top_level.txt
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/audio_gest_player.py` & `vaaibody-0.0.1/source/vaaibody/audio_gest_player.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,18 +149,12 @@
         imgui.end_frame()
 
         self._imgui_renderer.render(imgui.get_draw_data())
 
 
 if __name__ == "__main__":
     skeleton = Skeleton(name="Gesture_Before")
-    skeleton.load_hierarchy_from_bvh(
-        "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/bvh/VAAI_Free_01_02_M1.bvh"
-    )
-    db = MotionDatabase(
-        skeleton, "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/bvh"
-    )
-    audio_db = PlayAudioDatabase(
-        "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/wav"
-    )
+    skeleton.load_hierarchy_from_bvh("data/motion/Gesture_Before/VAAI_Basic_01_01.bvh")
+    db = MotionDatabase(skeleton, "data/motion/Gesture_Before/")
+    audio_db = PlayAudioDatabase("data/audio/Gesture_Audio_Fin")
     main_window = MyWindow(skeleton, db, audio_db)
     main_window.loop()
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/bvh_viewer.py` & `vaaibody-0.0.1/source/vaaibody/bvh_viewer.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/audio.py` & `vaaibody-0.0.1/source/vaaibody/core/audio.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/blending.py` & `vaaibody-0.0.1/source/vaaibody/core/blending.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/database.py` & `vaaibody-0.0.1/source/vaaibody/core/database.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/feature.py` & `vaaibody-0.0.1/source/vaaibody/core/feature.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/filter_frame.py` & `vaaibody-0.0.1/source/vaaibody/core/filter_frame.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/frame.py` & `vaaibody-0.0.1/source/vaaibody/core/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,25 +91,14 @@
             self._skeleton,
             deepcopy(self._root_transform),
             deepcopy(self._local_transforms),
             scalar=self._is_scalar,
         )
         return new_frame
 
-    def fast_copy(
-        self,
-    ):
-        new_frame = Frame(
-            self._skeleton,
-            deepcopy(self._root_transform),
-            deepcopy(self._local_transforms),
-            scalar=self._is_scalar,
-        )
-        return new_frame
-
     def get_root_transform(self):
         return self._root_transform
 
     def get_inverse_root_transform(self):
         if self._root_transform_inv is None:
             self._root_transform_inv = self._root_transform.inverse()
         return self._root_transform_inv
@@ -258,21 +247,14 @@
 
     def set_dirty(self, joint_idx):
         joint_dict = self._skeleton.joint_dict
         self._component_dirty_flags[joint_idx] = True
         self._global_dirty_flags[joint_idx] = True
         self._body_global_dirty_flags[joint_idx] = True
 
-        # original version - traverse all joint idx
-        # for i in range(joint_idx, self._skeleton.num_joints()):
-        #     if self._skeleton.joints[i].parent is None:
-        #         continue
-        #     if self._dirty_flags[self._skeleton.joints[i].parent.idx]:
-        #         self._dirty_flags[i] = True
-
         # new version
         # traverse only child node
         visited = []
         need_to_visit = deque()
         need_to_visit.append(self._skeleton.joints[joint_idx])
 
         while need_to_visit:
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/gesture_matching.py` & `vaaibody-0.0.1/source/vaaibody/core/gesture_matching.py`

 * *Files 19% similar despite different names*

```diff
@@ -78,16 +78,15 @@
 
         # threshold
         self.is_speaking = True
         self.energy_term = 0.35
         self.thresh = 4.0
         self.angle_thresh_degree = 1000
         # self.thresh = 10
-        # self.max_onset = min(round(1.2 / self.frame_time), self.n_db_frame - 2)
-        self.max_onset = 60
+        self.max_onset = min(round(1.2 / self.frame_time), self.n_db_frame - 2)
         # self.max_onset = round(1. / self.frame_time)
         self.min_onset = round(0.25 / self.frame_time)
 
         # initialize
         self.tc = TC()
         self.init_feat()
         self.init_KD_tree()
@@ -179,308 +178,14 @@
                     seq_sil_rel_kd_tree = KDTree(
                         silent_release_feature[idx_motion][idx_seq, :, :],
                         metric="euclidean",
                     )
                     sil_rel_kd_tree.append(seq_sil_rel_kd_tree)
                 self.KDtree_sil_rel.append(sil_rel_kd_tree)
 
-    def test_new_metric(self, beat_test, mfcc_test, sil_hint):
-        pose_feature = self.pose_feature
-        beat_feature = self.beat_feature
-        lower_feature = self.lower_feature
-        silent_release_feature = self.silent_release_feature
-
-        AUDIO_SCALE_VALUE = 0.5
-        pose_beat_feature = []
-        test_pose_feature = []
-        lower_sliced_feature = []
-        silent_sliced_feature = []
-
-        time_stamp = []
-        for idx_clip in range(self._gesture_db._motion_db.num_motion()):
-            frame_num = self._gesture_db._motion_db.get_motion_len(idx_clip)
-            pose_beat_feature.append(
-                np.column_stack(
-                    [
-                        pose_feature[idx_clip][0][: -self.max_onset],
-                        AUDIO_SCALE_VALUE
-                        * beat_feature[idx_clip][0][: frame_num - self.max_onset],
-                    ]
-                )
-            )
-            if len(time_stamp) == 0:
-                time_stamp.append([0, frame_num - self.max_onset])
-            else:
-                time_stamp.append(
-                    [time_stamp[-1][0] + time_stamp[-1][1], frame_num - self.max_onset]
-                )
-
-        time_stamp_sil = []
-        for idx_clip_sil in range(self._silent_db._motion_db.num_motion()):
-            frame_num = self._silent_db._motion_db.get_motion_len(idx_clip_sil)
-            silent_sliced_feature.append(silent_release_feature[idx_clip_sil][0])
-            if len(time_stamp_sil) == 0:
-                time_stamp_sil.append([0, frame_num])
-            else:
-                time_stamp_sil.append(
-                    [time_stamp_sil[-1][0] + time_stamp_sil[-1][1], frame_num]
-                )
-
-        pose_beat_feature_concat = np.concatenate(pose_beat_feature, axis=0)
-        silent_feature_concat = np.concatenate(silent_sliced_feature, axis=0)
-
-        self.silent = sil_hint
-        n_frames = mfcc_test.shape[-1]
-        beat_test = np.concatenate(
-            (beat_test[:, 0:1], beat_test), axis=1
-        )  # 60, n_frame
-
-        pose_test = np.zeros(shape=(self.n_pose_feature, mfcc_test.shape[1]))
-        init_motion, init_seq, init_frm = self.init_frame(is_rand=False)
-        init_lower_motion, init_lower_seq, init_lower_frm = self.init_frame(
-            is_rand=False
-        )
-
-        lower_motion = init_lower_motion
-        lower_frm = init_lower_frm
-
-        pose_test[:, 0] = self.pose_feature[init_motion][init_seq, init_frm, :]
-        self.pred_motion_idx = []
-        self.pred_lower_idx = []
-        j = 1  # 입력 audio에 대해 현재 찾은 idx+1. 0이 아니라 1인 이유는 처음에 concat한 이유랑 같음.
-        loop_flag = True
-        start_time = time.time()
-
-        beat_score_aveg = []
-        pose_score_aveg = []
-
-        while loop_flag:
-            if self.silent is None:
-                self.step_size = self.slice_with_beat(beat_test, j)
-            else:
-                self.step_size = self.slice_with_beatNsil(beat_test, j)
-            if j + self.step_size >= n_frames:
-                self.step_size = n_frames - j - 1
-                loop_flag = False
-
-            if self.is_speaking:
-                pose_beat_feature_input = np.column_stack(
-                    [
-                        np.expand_dims(pose_test[:, j - 1], axis=0),
-                        np.expand_dims(AUDIO_SCALE_VALUE * beat_test[:, j], axis=0),
-                    ]
-                )
-                dist = pairwise_distances(
-                    pose_beat_feature_concat, pose_beat_feature_input
-                )
-            else:
-                pose_feature_input = np.expand_dims(pose_test[:, j - 1], axis=0)
-                dist = pairwise_distances(silent_feature_concat, pose_feature_input)
-
-            result_idx_list = np.argpartition(dist[:, 0], 2)
-            if dist[result_idx_list[0]] > 0:
-                result_idx = result_idx_list[0]
-            else:
-                result_idx = result_idx_list[1]
-
-            idx_pred_motion, idx_pred_frame = None, None
-            if not self.is_speaking:
-                time_seq_stamp = time_stamp_sil
-            else:
-                time_seq_stamp = time_stamp
-
-            for idx_time in range(len(time_seq_stamp)):
-                if idx_time < len(time_seq_stamp) - 1:
-                    if (
-                        result_idx >= time_seq_stamp[idx_time][0]
-                        and result_idx < time_seq_stamp[idx_time + 1][0]
-                    ):
-                        idx_pred_motion = idx_time
-                        idx_pred_frame = result_idx - time_seq_stamp[idx_time][0]
-                        break
-                else:
-                    if result_idx >= time_seq_stamp[idx_time][0]:
-                        idx_pred_motion = idx_time
-                        idx_pred_frame = result_idx - time_seq_stamp[idx_time][0]
-
-            if not self.is_speaking and idx_pred_motion is None:
-                idx_pred_motion, idx_pred_frame = 1, 0
-
-            # if self.is_speaking: #for test
-            #     print('score', dist[result_idx], idx_pred_motion, idx_pred_frame)
-            #     print('hamming', spatial.distance.hamming(beat_feature[idx_pred_motion][0][idx_pred_frame], beat_test[:, j]))
-            #     beat_score_aveg.append(spatial.distance.hamming(beat_feature[idx_pred_motion][0][idx_pred_frame], beat_test[:, j]))
-            #     pose_score_aveg.append(pairwise_distances(np.expand_dims(pose_feature[idx_pred_motion][0][idx_pred_frame],axis=0), np.expand_dims(pose_test[:, j - 1], axis=0)))
-
-            low_mo = self.play_motion_test(
-                lower_motion, lower_frm, lower_sliced_feature, time_seq_stamp
-            )
-            self.pred_lower_idx.append(low_mo)
-            lower_motion = low_mo[-1][0]
-            lower_frm = low_mo[-1][1]
-            if self.is_speaking:
-                pose_test[:, j : (j + self.step_size)] = pose_feature[idx_pred_motion][
-                    0
-                ][idx_pred_frame : (idx_pred_frame + self.step_size), :].transpose()
-            else:
-                res = (
-                    self.step_size
-                    - silent_release_feature[idx_pred_motion][0][
-                        idx_pred_frame : (idx_pred_frame + self.step_size), :
-                    ].shape[0]
-                )
-                if res > 0:
-                    pad_arr = np.array(
-                        res * [silent_release_feature[idx_pred_motion][0][-1, :]]
-                    )
-                    padded_feature = np.vstack(
-                        (
-                            silent_release_feature[idx_pred_motion][0][
-                                idx_pred_frame : (idx_pred_frame + self.step_size), :
-                            ],
-                            pad_arr,
-                        )
-                    )
-                    pose_test[:, j : (j + self.step_size)] = padded_feature.transpose()
-                else:
-                    pose_test[:, j : (j + self.step_size)] = silent_release_feature[
-                        idx_pred_motion
-                    ][0][
-                        idx_pred_frame : (idx_pred_frame + self.step_size), :
-                    ].transpose()
-
-            self.pred_motion_idx.append(
-                [idx_pred_motion, idx_pred_frame, self.step_size, self.is_speaking]
-            )
-            j += self.step_size
-
-        # print('a', sum(beat_score_aveg)/len(beat_score_aveg), len(beat_score_aveg))
-        # print('b', sum(pose_score_aveg)/len(pose_score_aveg), len(pose_score_aveg))
-        print("Matching takes {}seconds".format(time.time() - start_time))
-
-        start_blend = time.time()
-        self.blend_matched_test(init_lower_motion, False, apply_filter="lpf")
-        print("Blending takes {}seconds".format(time.time() - start_blend))
-
-    def blend_matched_test(
-        self,
-        init_lower_motion: int,
-        search_lower: bool = False,
-        apply_filter: str = None,
-    ):
-        """
-        Args:
-            init_lower_motion
-            search_lower
-            filter
-
-        Returns:
-            self.blended_frames
-        """
-
-        self.blended_frames = []
-        blend_dur = 90
-        root_offset = Transform(R.identity(), np.array([0, 0, 0]))
-        prev_motion = init_lower_motion
-        use_sil_real = False
-        pred_lower_idx_list = self.pred_lower_idx
-        blended_frames = self.blended_frames
-        print("Blending process")
-        use_sil_real = True
-
-        for i, motion_idx in enumerate(tqdm(self.pred_motion_idx)):
-            lower_list = pred_lower_idx_list[i]
-            is_speaking = motion_idx[3]
-            if i > 0:
-                first_motion, second_motion = (
-                    blended_frames[-2],
-                    self.blended_frames[-1],
-                )
-                if use_sil_real and not is_speaking:
-                    target_frame = self._silent_db.get_frame(
-                        motion_idx[0], motion_idx[1]
-                    ).copy()
-                else:
-                    target_frame = self._gesture_db.get_frame(
-                        motion_idx[0], motion_idx[1]
-                    ).copy()
-                # Implement add lower body to the target frame
-                if not search_lower:
-                    lower_idx = lower_list[0]
-
-                target_lower = self._gesture_db._motion_db.get_frame(
-                    lower_idx[0], lower_idx[1]
-                ).copy()
-                target_frame.set_root_transform(target_lower.get_root_transform())
-
-                for lower in self._gesture_db.lower_joints_matching:
-                    low_tar = target_lower.get_local_rotation_by_name(lower)
-                    target_frame.set_local_rotation_by_name(lower, low_tar)
-                new_root = target_frame.get_root_transform()
-                current_root = second_motion.get_root_transform()
-                root_offset = current_root * new_root.inverse()
-                target_frame.set_root_transform(
-                    root_offset * target_frame.get_root_transform()
-                )
-                blender = BlendingInertialization(
-                    second_motion,
-                    first_motion,
-                    target_frame,
-                    blend_dur,
-                    self.frame_time,
-                    is_frame=True,
-                )
-            for step_size in range(
-                motion_idx[2]
-            ):  # modion_cand - i, k, f, self.step_size
-                if use_sil_real and not is_speaking:
-                    try:
-                        current_frame = self._silent_db.get_frame(
-                            motion_idx[0], motion_idx[1] + step_size
-                        ).copy()
-                    except:
-                        current_frame = self._silent_db.get_frame(
-                            motion_idx[0], -1
-                        ).copy()
-                else:
-                    current_frame = self._gesture_db.get_frame(
-                        motion_idx[0], motion_idx[1] + step_size
-                    ).copy()
-                # Implement add lower body to the target frame
-                if not search_lower:
-                    lower_idx = lower_list[step_size]
-                    target_lower = self._gesture_db.get_frame(
-                        lower_idx[0], lower_idx[1]
-                    ).copy()
-                    if lower_idx[0] != prev_motion:
-                        new_root = target_lower.get_root_transform()
-                        current_root = self.blended_frames[-1].get_root_transform()
-                        root_offset = current_root * new_root.inverse()
-                        prev_motion = lower_idx[0]
-
-                # 하반신 덮어쓰기. 안그러면 발 미끌림
-                current_frame.set_root_transform(
-                    target_lower.get_root_transform()
-                )  # lower body의 root를 따르겠음
-                for lower in self._gesture_db.lower_joints_matching:  # 하반신 joint면
-                    low_tar = target_lower.get_local_rotation_by_name(lower)
-                    current_frame.set_local_rotation_by_name(
-                        lower, low_tar
-                    )  # local rotation == joint angle
-                if i > 0 and step_size < blend_dur:
-                    current_frame = blender.apply_frame_blending(
-                        current_frame, step_size + 1
-                    )
-
-                self.blended_frames.append(current_frame)
-
-        if apply_filter is not None:
-            self.blended_frames = filter_frames(self.blended_frames, apply_filter)
-        return self.blended_frames
-
     def verify_radius(
         self,
         index,
         feat,
     ):
         """
         radius
@@ -650,24 +355,14 @@
                 motion_cands.append([idx_motion, idx_seq, idx_frame, self.step_size])
                 pose_feature_cands.append(pose_feature_cand)
         pose_dist_cands = np.array(pose_dist_cands)
         motion_cands = np.array(motion_cands)
         pose_feature_cands = np.array(pose_feature_cands)
         return pose_dist_cands, motion_cands, pose_feature_cands
 
-    def play_motion_test(
-        self, lower_motion, lower_frm, lower_sliced_feature, time_stamp
-    ):
-        play_list = []
-        num_frame = self.n_db_frame[lower_motion]
-
-        for idx_step in range(1, self.step_size + 1):
-            play_list.append([lower_motion, idx_step + lower_frm])
-
-        return play_list
 
     def play_motion(self, lower_motion, lower_seq, lower_frm):
         play_list = []
         if lower_frm + self.step_size >= self.n_db_frame:
             for frm in range(lower_frm + 1, self.n_db_frame):
                 play_list.append([lower_motion, lower_seq, frm])
             res = lower_frm + self.step_size - self.n_db_frame + 1
@@ -693,14 +388,15 @@
                     play_list.append([motion, seq, frm + i])
         else:
             for i in range(1, self.step_size + 1):
                 play_list.append([lower_motion, lower_seq, lower_frm + i])
 
         return play_list
 
+
     def match_motion_with_silent(
         self,
         mfcc_test: np.ndarray,
         beat_test: np.ndarray,
         desired_k: int = 0,
         search_lower: bool = True,
         sil_hint: np.ndarray = None,
@@ -751,17 +447,14 @@
         else:
             lower_motion = init_lower_motion
             lower_seq = init_lower_seq
             lower_frm = init_lower_frm
         self.pred_motion_idx = []
         self.pred_lower_idx = []
 
-        beat_score_aveg = []
-        pose_score_aveg = []
-
         j = 1  # 입력 audio에 대해 현재 찾은 idx+1. 0이 아니라 1인 이유는 처음에 concat한 이유랑 같음.
         loop_flag = True
         start_time = time.time()
         while loop_flag:
             if self.silent is None:
                 self.step_size = self.slice_with_beat(beat_test, j)
             else:
@@ -787,27 +480,23 @@
                 ) = self.search_motion_only_cands_KD(
                     pose_test[:, j - 1], KD_type="silent_rel", max_query=20
                 )  # search pose from only motion (음성 없이)
             pose_score = np.array(pose_dist_cands).argsort().argsort()
 
             if self.is_speaking:
                 mfcc_score = self.sort_cosine_dist(mfcc_feature_cands, mfcc_test[:, j])
-                beat_score, beat_score_raw = self.sort_hamming_dist(
+                beat_score, _ = self.sort_hamming_dist(
                     beat_feature_cands, beat_test[:, j]
                 )
             total_score = pose_score
             if self.is_speaking:
-                # total_score += mfcc_score
+                total_score += mfcc_score
                 total_score += beat_score
             total_sorted_list = np.argsort(total_score).tolist()
-            # if self.is_speaking:
-            #     print(total_sorted_list[0], pose_dist_cands[total_sorted_list[0]], beat_score_raw[total_sorted_list[0]])
-            #     print('score sum', pose_dist_cands[total_sorted_list[0]] + beat_score_raw[total_sorted_list[0]])
-            #     beat_score_aveg.append(beat_score_raw[total_sorted_list[0]])
-            #     pose_score_aveg.append(pose_dist_cands[total_sorted_list[0]])
+
             pose_feature_cands = pose_feature_cands[total_sorted_list]
             motion_cands = motion_cands[total_sorted_list]  #
 
             if search_lower:
                 """
                 Search lower pose based on the pose difference
                 """
@@ -840,17 +529,14 @@
 
             pose_test[:, j : (j + self.step_size)] = pose_feature_cands[desired_k]
             self.pred_motion_idx.append(
                 [motion_cands[desired_k], self.is_speaking]
             )  # motion_cands[desired_k] 가 최종 결과물, is_speaking 까지 해서 db에서 찾아올 예정
             j += self.step_size
         print("Matching takes {}seconds".format(time.time() - start_time))
-        # print('a', sum(beat_score_aveg)/len(beat_score_aveg), len(beat_score_aveg))
-        # print('b', sum(pose_score_aveg)/len(pose_score_aveg), len(pose_score_aveg))
-
         start_blend = time.time()
         self.blend_matched(init_lower_motion, search_lower, apply_filter="lpf")
         print("Blending takes {}seconds".format(time.time() - start_blend))
 
     def blend_matched(
         self,
         init_lower_motion: int,
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/motion.py` & `vaaibody-0.0.1/source/vaaibody/core/motion.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/core/skeleton.py` & `vaaibody-0.0.1/source/vaaibody/core/skeleton.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/decompressor.py` & `vaaibody-0.0.1/source/vaaibody/decompressor.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/decompressor_savedb.py` & `vaaibody-0.0.1/source/vaaibody/decompressor_savedb.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/decompressor_train.py` & `vaaibody-0.0.1/source/vaaibody/decompressor_train.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/decompressor_util.py` & `vaaibody-0.0.1/source/vaaibody/decompressor_util.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/main.py` & `vaaibody-0.0.1/source/vaaibody/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import pathlib
 
 file_path = pathlib.Path(__file__).parent.resolve()
 data_path = file_path.parent.parent / "data"
 
 
 def match_gesture(
-    bvh_name="/home/yoonhee/Downloads/221123_Body_KSW/Gesture_Before/VAAI_Basic_01_03.bvh",
-    bvh_npz_path="data/matching_data/rhythm_motion_npz",
+    bvh_name="data/matching_data/rhythm_motion/VAAI_Short_01_02.bvh",
+    bvh_npz_path="data/matching_data/rhythm_motion_npz/",
     audio_db_path="data/matching_data/rhythm_audio",
     silent_db_path="data/matching_data/silent_release",
     test_audio_path="data/audio/Test/TTS.wav",
 ):
     """
     Init Database, parameters
     """
@@ -35,15 +35,15 @@
     fps = round(1.0 / motion_db.get_frame_time())
     frame_size = round(fps) * 2
     step_size = round(round(fps) * 0.5)
     audio_db = AudioDatabase(audio_db_path, fps, from_path=True)
     gdb = MotionAudioFeatureDatabase(
         motion_db,
         audio_db,
-        slice=False,
+        slice=True,
         frame_size=frame_size,
         db_path=data_path / "matching_data",
         db_file_name="wv_feature_no_sliced.pickle",
     )
 
     raw_silent_db = MotionDatabase(skeleton, silent_db_path, is_preload=True)
     silent_db = MotionFeatureDatabase(
@@ -59,24 +59,18 @@
     test_db = AudioFeatureDatabase(test_audio, fps)
     _, sil_hint = silent_detector(
         test_db.mfcc_feature, std_thresh=-0.2, duration=round(1.0 * fps)
     )
     """
     Search Motion with silence hint
     """
-    # gesture_matching.match_motion_with_silent(
-    #     test_db.mfcc_feature.transpose(),
-    #     test_db.beat_feature.transpose(),
-    #     search_lower=False,
-    #     sil_hint=sil_hint,
-    # )
-
-    gesture_matching.test_new_metric(
-        test_db.beat_feature.transpose(),
+    gesture_matching.match_motion_with_silent(
         test_db.mfcc_feature.transpose(),
+        test_db.beat_feature.transpose(),
+        search_lower=False,
         sil_hint=sil_hint,
     )
 
     # gesture_matching.matching_head(filter="lowpass")
     searched_motion = gesture_matching.convert_frames()
     """
     Export and return results
@@ -90,15 +84,18 @@
     exporter.init_export(len(searched_motion))
     exporter.export_motion(searched_motion, DOF_6=True)
     return skeleton, searched_motion, test_audio, sil_hint
 
 
 if __name__ == "__main__":
     skel, searched_motion, test_audio, sil_hint = match_gesture(
-        bvh_name="/home/yoonhee/Downloads/221123_Body_KSW/Gesture_Before/VAAI_Basic_01_01.bvh",
+        bvh_name=data_path
+        / "matching_data"
+        / "Gesture_Before"
+        / "VAAI_Basic_01_01.bvh",
         bvh_npz_path=data_path / "matching_data" / "rhythm_motion_npz",
         audio_db_path=data_path / "matching_data" / "rhythm_audio",
         silent_db_path=data_path / "matching_data" / "silent_release",
         test_audio_path=data_path / "audio" / "Test" / "TTS_Travel.wav",
     )
     print("Audio length: ", test_audio.audio().shape[0] / test_audio.sr())
     visualize = True
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/main_nn.py` & `vaaibody-0.0.1/source/vaaibody/main_nn.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/module/idle_module.py` & `vaaibody-0.0.1/source/vaaibody/module/idle_module.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/module/nontalking_control_module.py` & `vaaibody-0.0.1/source/vaaibody/module/nontalking_control_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections import deque
 import numpy as np
 import string
-from core.database import MotionDatabase, DefaultMotionFeatureDatabase
-from core.skeleton import Transform
-from core.frame import Frame
-from core.feature import NonTalkingPoseFeature, NonTalkingHistoryFeature
-from module.idle_module import IdleModule
-from module.transition_module import TransitionModule
-from module.tag_processing_module import TagProcessingModule
-from utilities.timechecker import TimeChecker as TC
-from utilities.frame_utils import shift_root, find_single_cut_idx
+from vaaibody.core.database import MotionDatabase, DefaultMotionFeatureDatabase
+from vaaibody.core.skeleton import Transform
+from vaaibody.core.frame import Frame
+from vaaibody.core.feature import NonTalkingPoseFeature, NonTalkingHistoryFeature
+from vaaibody.module.idle_module import IdleModule
+from vaaibody.module.transition_module import TransitionModule
+from vaaibody.module.tag_processing_module import TagProcessingModule
+from vaaibody.utilities.timechecker import TimeChecker as TC
+from vaaibody.utilities.frame_utils import shift_root, find_single_cut_idx
 
 
 class NonTalkingModule(object):
     def __init__(
         self,
         db: MotionDatabase,
         idle_file="./data/idle_HSO.csv",
@@ -150,26 +150,26 @@
     """
 
     def get_next_frame(
         self,
     ):
         if self.current_play_state == "transition":
             frame, is_end_blending = self.transition_module.get_transition_frame(
-                self.current_motion[self.idx_current].fast_copy()
+                self.current_motion[self.idx_current].copy()
             )
             self.idx_current = (
                 self.idx_current + 1
                 if self.transition_module.moving_blend_flag
                 else self.idx_current
             )
             if is_end_blending:
                 self.current_play_state = "play"
         elif self.current_play_state == "play":
             frame = shift_root(
-                self.current_motion[self.idx_current].fast_copy(),
+                self.current_motion[self.idx_current].copy(),
                 self.translation_offset,
             )
             self.idx_current += 1
             if self.current_motion_state == "duration_tag":
                 if self.idx_current >= self.tag_processing_module.hold_end:
                     self.tag_processing_module.reset()
                     self.switch_to_retract(frame)
@@ -303,13 +303,13 @@
             and self.tag_processing_module.loop_len >= 15
         ):
             """
             Put looping motion
             """
             idx_hold_loop = self.tag_processing_module.idx_loop_start + loop_cnt
             frame = self.transition_module.get_loop_frame(
-                self.current_motion[idx_hold_loop].fast_copy()
+                self.current_motion[idx_hold_loop].copy()
             )
             self.tag_processing_module.loop_motion.append(frame)
         return self.tag_processing_module.loop_motion[
             loop_cnt % self.tag_processing_module.loop_len
-        ].fast_copy()
+        ].copy()
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/module/tag_processing_module.py` & `vaaibody-0.0.1/source/vaaibody/module/tag_processing_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import deque
 import pandas as pd
 import numpy as np
 import string
-from core.frame import Frame
-from utilities.frame_utils import find_single_cut_idx
-from utilities.timechecker import TimeChecker as TC
+from vaaibody.core.frame import Frame
+from vaaibody.utilities.frame_utils import find_single_cut_idx
+from vaaibody.utilities.timechecker import TimeChecker as TC
 
 
 class PhaseInformation:
     def __init__(self, db, phase_file) -> None:
         self.phase_info = pd.read_csv(phase_file)
         self.idx_phase_list = []
         self.tag_names = []
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/module/transition_module.py` & `vaaibody-0.0.1/source/vaaibody/module/transition_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from core.blending import BlendingInertialization, RootBlender, RootInertialization
-from core.frame import Frame
-from core.motion import Motion
+from vaaibody.core.blending import (
+    BlendingInertialization,
+    RootBlender,
+    RootInertialization,
+)
+from vaaibody.core.frame import Frame
+from vaaibody.core.motion import Motion
 
 
 class TransitionModule(object):
     def __init__(self, frame_time: float) -> None:
         self.frame_time = frame_time
         self.blend_dur = 60
         self.reset_transition_info()
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/parameter/gesture_matching_parameter.py` & `vaaibody-0.0.1/source/vaaibody/parameter/gesture_matching_parameter.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/audio_motion_synch.py` & `vaaibody-0.0.1/source/vaaibody/utilities/audio_motion_synch.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/audio_utils.py` & `vaaibody-0.0.1/source/vaaibody/utilities/audio_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Tuple
-from core.audio import Audio
+from vaaibody.core.audio import Audio
 import numpy as np
 
 
 def cut_audio(original_audio: Audio, st_time=0, end_time=-1):
     if end_time == -1:
         end_frm = original_audio.audio().shape[0]
     else:
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/blending_utils.py` & `vaaibody-0.0.1/source/vaaibody/utilities/blending_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from core.blending import *
-from core.frame import Frame
-from core.motion import Motion
+from vaaibody.core.blending import *
+from vaaibody.core.frame import Frame
+from vaaibody.core.motion import Motion
 
 
 def brute_add(motion1: Motion, motion2: Motion, path=None):
     brute_motion = motion1.copy()
     if path is not None:
         brute_motion._file_path = path
     brute_motion.append(motion2.copy())
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/exporter.py` & `vaaibody-0.0.1/source/vaaibody/utilities/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from core.motion import Motion
+from vaaibody.core.motion import Motion
 from tqdm import tqdm
 
 
 class Exporter:
     def __init__(self, sample, path=None, file_name=None):
         self.sample_bvh = sample
         if path is not None and file_name is not None:
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/filter.py` & `vaaibody-0.0.1/source/vaaibody/utilities/filter.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/frame_utils.py` & `vaaibody-0.0.1/source/vaaibody/utilities/frame_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.signal import butter, filtfilt, savgol_filter
 from scipy.spatial.transform import Rotation as R
-from core.skeleton import Transform
-from core.motion import Motion
+from vaaibody.core.skeleton import Transform
+from vaaibody.core.motion import Motion
 
 # def spin_180(rotation:R):
 #     mirror_rot = np.array([[-1,-1,1],[1,1,-1],[1,1,-1]])
 #     return mirror_rot * rotation.as_matrix()
 
 
 def shift_root(frame, translation_offset):
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/motion_var_utils.py` & `vaaibody-0.0.1/source/vaaibody/utilities/motion_var_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from core.motion import Motion
-from core.skeleton import Transform
+from vaaibody.core.motion import Motion
+from vaaibody.core.skeleton import Transform
 from scipy.spatial.transform import Rotation as R
 
 
 def append_end_motion(motion, count):
     frames = []
     for i in range(len(motion)):
         frame = motion[i].copy()
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/quat.py` & `vaaibody-0.0.1/source/vaaibody/utilities/quat.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/rendering_utils.py` & `vaaibody-0.0.1/source/vaaibody/utilities/rendering_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import numpy as np
 from OpenGL.GL import *
 from OpenGL.GLU import *
 from vaaibody.viewer.obj_loader import HEAD_OBJ, HEAD_OBJ_SIZE, HEAD_BOX
 
 import math
-import numpy as np
 
 quad_obj = gluNewQuadric()
 
 
 class Color:
     colors = []
     colors.append([0.3, 0.3, 0.3])
```

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/timechecker.py` & `vaaibody-0.0.1/source/vaaibody/utilities/timechecker.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/txform.py` & `vaaibody-0.0.1/source/vaaibody/utilities/txform.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/utilities/utils.py` & `vaaibody-0.0.1/source/vaaibody/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/camera.py` & `vaaibody-0.0.1/source/vaaibody/viewer/camera.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/controller.py` & `vaaibody-0.0.1/source/vaaibody/viewer/controller.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/double_bvh_viewer.py` & `vaaibody-0.0.1/source/vaaibody/viewer/double_bvh_viewer.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/gui_viewer.py` & `vaaibody-0.0.1/source/vaaibody/viewer/gui_viewer.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/handler.py` & `vaaibody-0.0.1/source/vaaibody/viewer/handler.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/item_data.py` & `vaaibody-0.0.1/source/vaaibody/viewer/item_data.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/item_drawer.py` & `vaaibody-0.0.1/source/vaaibody/viewer/item_drawer.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody/viewer/obj_loader.py` & `vaaibody-0.0.1/source/vaaibody/viewer/obj_loader.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.5/source/vaaibody.egg-info/SOURCES.txt` & `vaaibody-0.0.1/source/vaaibody.egg-info/SOURCES.txt`

 * *Files identical despite different names*

