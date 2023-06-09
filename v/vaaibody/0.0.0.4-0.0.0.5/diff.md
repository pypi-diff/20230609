# Comparing `tmp/vaaibody-0.0.0.4.tar.gz` & `tmp/vaaibody-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaaibody-0.0.0.4.tar", last modified: Fri Jun  9 01:26:31 2023, max compression
+gzip compressed data, was "vaaibody-0.0.0.5.tar", last modified: Fri Jun  9 04:16:49 2023, max compression
```

## Comparing `vaaibody-0.0.0.4.tar` & `vaaibody-0.0.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      169 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/PKG-INFO
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       38 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/setup.cfg
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      687 2023-06-09 01:26:19.000000 vaaibody-0.0.0.4/setup.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:20:31.000000 vaaibody-0.0.0.4/source/vaaibody/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5622 2023-06-08 05:21:34.000000 vaaibody-0.0.0.4/source/vaaibody/audio_gest_player.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     6967 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/bvh_viewer.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody/core/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:13.000000 vaaibody-0.0.0.4/source/vaaibody/core/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12900 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/core/audio.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    22470 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/core/blending.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    28257 2023-06-08 06:32:22.000000 vaaibody-0.0.0.4/source/vaaibody/core/database.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    15988 2023-06-08 05:21:34.000000 vaaibody-0.0.0.4/source/vaaibody/core/feature.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1247 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/core/filter_frame.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    19598 2023-06-08 07:00:42.000000 vaaibody-0.0.0.4/source/vaaibody/core/frame.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    48881 2023-06-08 05:45:27.000000 vaaibody-0.0.0.4/source/vaaibody/core/gesture_matching.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      279 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/core/modAudio.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23410 2023-06-08 07:11:05.000000 vaaibody-0.0.0.4/source/vaaibody/core/motion.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9845 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/core/skeleton.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1488 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/decompressor.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4704 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/decompressor_savedb.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23724 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/decompressor_train.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9386 2023-06-08 05:21:34.000000 vaaibody-0.0.0.4/source/vaaibody/decompressor_util.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2680 2023-06-08 06:58:19.000000 vaaibody-0.0.0.4/source/vaaibody/dump_test.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3748 2023-06-08 05:33:24.000000 vaaibody-0.0.0.4/source/vaaibody/main.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3746 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/main_nn.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody/module/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:33.000000 vaaibody-0.0.0.4/source/vaaibody/module/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3951 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/module/idle_module.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12295 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/module/nontalking_control_module.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7487 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/module/tag_processing_module.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3440 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/module/transition_module.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody/parameter/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:26:25.000000 vaaibody-0.0.0.4/source/vaaibody/parameter/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1703 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/parameter/gesture_matching_parameter.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody/utilities/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:27:54.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8585 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/audio_motion_synch.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1310 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/audio_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14676 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/blending_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5318 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/exporter.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8788 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/filter.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    11238 2023-06-08 05:21:34.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/frame_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7150 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/motion_var_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9975 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/quat.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    16383 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/rendering_utils.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      890 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/timechecker.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1779 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/txform.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1641 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/utilities/utils.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody/viewer/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:28:52.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/__init__.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3294 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/camera.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1140 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/controller.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5603 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/double_bvh_viewer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8009 2023-06-08 05:21:34.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/gesture_result_viewer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    13925 2023-05-24 06:53:17.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/gui_viewer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1079 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/handler.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      795 2023-05-24 02:01:11.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/item_data.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4400 2023-06-08 05:10:08.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/item_drawer.py
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      412 2023-05-24 02:03:55.000000 vaaibody-0.0.0.4/source/vaaibody/viewer/obj_loader.py
-drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 01:26:31.879987 vaaibody-0.0.0.4/source/vaaibody.egg-info/
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      169 2023-06-09 01:26:31.000000 vaaibody-0.0.0.4/source/vaaibody.egg-info/PKG-INFO
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2102 2023-06-09 01:26:31.000000 vaaibody-0.0.0.4/source/vaaibody.egg-info/SOURCES.txt
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        1 2023-06-09 01:26:31.000000 vaaibody-0.0.0.4/source/vaaibody.egg-info/dependency_links.txt
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       27 2023-06-09 01:26:31.000000 vaaibody-0.0.0.4/source/vaaibody.egg-info/requires.txt
--rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        9 2023-06-09 01:26:31.000000 vaaibody-0.0.0.4/source/vaaibody.egg-info/top_level.txt
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      169 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/PKG-INFO
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       38 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/setup.cfg
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      687 2023-06-09 04:16:38.000000 vaaibody-0.0.0.5/setup.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:20:31.000000 vaaibody-0.0.0.5/source/vaaibody/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5718 2023-06-09 04:15:51.000000 vaaibody-0.0.0.5/source/vaaibody/audio_gest_player.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     6953 2023-06-09 04:15:51.000000 vaaibody-0.0.0.5/source/vaaibody/bvh_viewer.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/core/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:13.000000 vaaibody-0.0.0.5/source/vaaibody/core/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12912 2023-06-09 03:59:56.000000 vaaibody-0.0.0.5/source/vaaibody/core/audio.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23035 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/blending.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    28229 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/database.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    15953 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/feature.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1265 2023-06-09 04:05:38.000000 vaaibody-0.0.0.5/source/vaaibody/core/filter_frame.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    19689 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/core/frame.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    50321 2023-06-09 04:16:07.000000 vaaibody-0.0.0.5/source/vaaibody/core/gesture_matching.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      279 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/core/modAudio.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23436 2023-06-09 03:59:15.000000 vaaibody-0.0.0.5/source/vaaibody/core/motion.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9845 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/core/skeleton.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1488 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4740 2023-06-09 04:14:32.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor_savedb.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    23778 2023-06-09 04:14:42.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor_train.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9413 2023-06-09 04:14:48.000000 vaaibody-0.0.0.5/source/vaaibody/decompressor_util.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2734 2023-06-09 04:14:56.000000 vaaibody-0.0.0.5/source/vaaibody/dump_test.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3937 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/main.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3825 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/main_nn.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/module/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-08 08:19:33.000000 vaaibody-0.0.0.5/source/vaaibody/module/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4013 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/module/idle_module.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    12346 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/module/nontalking_control_module.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7487 2023-06-08 05:10:08.000000 vaaibody-0.0.0.5/source/vaaibody/module/tag_processing_module.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3445 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/module/transition_module.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/parameter/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:26:25.000000 vaaibody-0.0.0.5/source/vaaibody/parameter/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1703 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/parameter/gesture_matching_parameter.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/utilities/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:27:54.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8585 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/audio_motion_synch.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1310 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/audio_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14676 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/blending_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5318 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/exporter.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8788 2023-05-24 02:03:55.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/filter.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    11236 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/frame_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     7150 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/motion_var_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     9975 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/quat.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    16430 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/rendering_utils.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      890 2023-06-08 05:10:08.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/timechecker.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1779 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/txform.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1641 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/utilities/utils.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody/viewer/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 00:28:52.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/__init__.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     3294 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/camera.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1149 2023-06-09 04:02:53.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/controller.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     5648 2023-06-09 04:13:09.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/double_bvh_viewer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     8045 2023-06-09 04:13:26.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/gesture_result_viewer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)    14081 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/gui_viewer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     1079 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/handler.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      795 2023-05-24 02:01:11.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/item_data.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     4418 2023-06-09 04:03:09.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/item_drawer.py
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      527 2023-06-09 04:15:52.000000 vaaibody-0.0.0.5/source/vaaibody/viewer/obj_loader.py
+drwxrwxr-x   0 yoonhee   (1000) yoonhee   (1000)        0 2023-06-09 04:16:49.449629 vaaibody-0.0.0.5/source/vaaibody.egg-info/
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)      169 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/PKG-INFO
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)     2102 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        1 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)       27 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/requires.txt
+-rw-rw-r--   0 yoonhee   (1000) yoonhee   (1000)        9 2023-06-09 04:16:49.000000 vaaibody-0.0.0.5/source/vaaibody.egg-info/top_level.txt
```

### Comparing `vaaibody-0.0.0.4/setup.py` & `vaaibody-0.0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from os.path import basename, splitext
 from glob import glob
 
 setup(
     name='vaaibody', # 패키지 명
-    version='0.0.0.4',
+    version='0.0.0.5',
     description='VAAI-BODY gesture generation module',
     author='yoonhee',
     author_email='yhkim@ncsoft.com',
     py_modules=[splitext(basename(path))[0] for path in glob('source/*.py')],
     packages=find_packages(where='source', exclude=['*.depricated', 'depricated', '*.depricated.*', '*.testing']),
     python_requires='>=3.8',
     package_dir={'': 'source'},
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/audio_gest_player.py` & `vaaibody-0.0.0.5/source/vaaibody/audio_gest_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import imgui
 import simpleaudio as sa
 
-from core.audio import PlayAudioDatabase
-from core.modAudio import *
-from core.motion import MotionDatabase
-from core.skeleton import Skeleton
-from viewer.gui_viewer import MainWindow
-from viewer.item_drawer import *
+from vaaibody.core.audio import PlayAudioDatabase
+from vaaibody.core.modAudio import *
+from vaaibody.core.motion import MotionDatabase
+from vaaibody.core.skeleton import Skeleton
+from vaaibody.viewer.gui_viewer import MainWindow
+from vaaibody.viewer.item_drawer import *
 
 
 class MyWindow(MainWindow):
     def __init__(self, skeleton, db, audio_db):
         super().__init__()
         self.set_skeleton(skeleton)
         self.set_db(db)
@@ -149,12 +149,18 @@
         imgui.end_frame()
 
         self._imgui_renderer.render(imgui.get_draw_data())
 
 
 if __name__ == "__main__":
     skeleton = Skeleton(name="Gesture_Before")
-    skeleton.load_hierarchy_from_bvh("/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/bvh/VAAI_Free_01_02_M1.bvh")
-    db = MotionDatabase(skeleton, "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/bvh")
-    audio_db = PlayAudioDatabase("/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/wav")
+    skeleton.load_hierarchy_from_bvh(
+        "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/bvh/VAAI_Free_01_02_M1.bvh"
+    )
+    db = MotionDatabase(
+        skeleton, "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/bvh"
+    )
+    audio_db = PlayAudioDatabase(
+        "/home/yoonhee/Desktop/vaai-body/precessed_data/KTG/wav"
+    )
     main_window = MyWindow(skeleton, db, audio_db)
     main_window.loop()
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/bvh_viewer.py` & `vaaibody-0.0.0.5/source/vaaibody/bvh_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 import glfw
 import imgui
 
-from core.motion import MotionDatabase
-from core.skeleton import Skeleton
+from vaaibody.core.motion import MotionDatabase
+from vaaibody.core.skeleton import Skeleton
 import natsort
-from viewer.gui_viewer import MainWindow
-from viewer.item_drawer import *
-# from utilities.frame_utils import mirror_motion
+from vaaibody.viewer.gui_viewer import MainWindow
+from vaaibody.viewer.item_drawer import *
+
 
 class MyWindow(MainWindow):
     def __init__(self, skeleton, db):
         super().__init__()
         self.set_skeleton(skeleton)
         self.set_db(db)
         self.selected = 0
@@ -38,15 +38,14 @@
 
             if key == glfw.KEY_A:
                 pass
                 # current_motion = self._db.get_motion(self._current_motion_idx)
                 # new_motion = mirror_motion(current_motion)
                 # self._db.append_motion(new_motion)
 
-
     # 여기에 custom display 코드 작성
     def custom_display(
         self,
     ):
         imgui.new_frame()
         imgui.begin("custom window", True)
         if imgui.button("prev"):
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/audio.py` & `vaaibody-0.0.0.5/source/vaaibody/core/audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from copy import deepcopy
 
 import librosa
 import natsort
 import numpy as np
 import numpy.fft
 from tqdm import tqdm
-from utilities.utils import *
+from vaaibody.utilities.utils import get_data_stats
 
 
 def mel(f):
     return 2595.0 * numpy.log10(1.0 + f / 700.0)
 
 
 def melinv(m):
@@ -334,23 +334,23 @@
         self,
     ):
         start_time = time.time()
         print("Loading the Audio DB")
         if os.path.exists(self._dir_path):
             for file_path in natsort.natsorted(os.listdir(self._dir_path)):
                 if file_path.endswith(".pickle"):
-                    path = "{}/{}".format(self._dir_path, file_path)
+                    path = self._dir_path / file_path
                     with open(path, "rb") as fr:
                         db = pickle.load(fr)
                     self._audio_db = []
                     beat_class = None
                     n_db = len(db["audio"])
                     mfcc_all = np.zeros((0, self._ncep + 1))
                     for i in range(n_db):
-                        path = self._dir_path + db["name"][i] + ".wav"
+                        path = self._dir_path / str(db["name"][i] + ".wav")
                         self._audio_db.append(
                             Audio(
                                 db["audio"][i],
                                 db["sr"][i],
                                 db["beat"][i],
                                 db["mfcc"][i],
                                 db["mfcc_der"][i],
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/blending.py` & `vaaibody-0.0.0.5/source/vaaibody/core/blending.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 from scipy.spatial.transform import Slerp
 
-from core.skeleton import Transform
+from vaaibody.core.skeleton import Transform
 
 # Here we need root blending code
 
 
 class RootBlender:
     def __init__(self, src, dst, dur_cnt, is_moving=False):
         self.dur_cnt = dur_cnt
         self.src_transform = src.get_root_transform()
         self.dst_transform = dst.get_root_transform()
         self.moving_flag = is_moving
-        left_foot = (src.get_component_translation_by_name("LeftToe") -  dst.get_component_translation_by_name("LeftToe"))/2
-        right_foot = (src.get_component_translation_by_name("RightToe") -  dst.get_component_translation_by_name("RightToe"))/2
-        self.transl_int = np.matmul(src.get_root_transform().rotation_np, (left_foot + right_foot))
+        left_foot = (
+            src.get_component_translation_by_name("LeftToe")
+            - dst.get_component_translation_by_name("LeftToe")
+        ) / 2
+        right_foot = (
+            src.get_component_translation_by_name("RightToe")
+            - dst.get_component_translation_by_name("RightToe")
+        ) / 2
+        self.transl_int = np.matmul(
+            src.get_root_transform().rotation_np, (left_foot + right_foot)
+        )
         self.transl_offset = (
-            self.src_transform.translation - self.dst_transform.translation 
+            self.src_transform.translation
+            - self.dst_transform.translation
             + self.transl_int
         )
 
         R_concat = R.concatenate(
             [self.src_transform.rotation, self.dst_transform.rotation]
         )
         st_end = [0, dur_cnt]
@@ -49,22 +58,26 @@
         translate = (
             self.src_transform.translation * (self.dur_cnt - cnt)
             + self.dst_transform.translation * cnt
         )
         translate /= self.dur_cnt
         return translate
 
-    def root_transl_off(
-        self, cnt
-    ):
-        translate = self.src_transform.translation + self.transl_int * cnt / self.dur_cnt
+    def root_transl_off(self, cnt):
+        translate = (
+            self.src_transform.translation + self.transl_int * cnt / self.dur_cnt
+        )
         return translate
 
     def root_moving_off(self, frame, cnt):
-        return frame.get_root_transform().translation + (self.transl_offset - self.transl_int)  + self.transl_int * cnt / self.dur_cnt
+        return (
+            frame.get_root_transform().translation
+            + (self.transl_offset - self.transl_int)
+            + self.transl_int * cnt / self.dur_cnt
+        )
 
     def root_blending(self, frame, cnt):
         if cnt < self.dur_cnt:
             if self.moving_flag:
                 root_ori = self.linear_ori_blending(frame, cnt)[0]
                 transl = self.root_moving_off(frame, cnt)
             else:
@@ -92,38 +105,62 @@
         ori_blendings = self.linear_ori_blending(frame, cnt)
         root_ori = ori_blendings[0]
         trans = frame.get_root_transform().translation
         new_root = Transform(root_ori, trans)
         frame.set_root_transform(new_root)
         return frame
 
+
 class RootInertialization:
     def __init__(
         self,
         source_first,
         source_second,
         target,
         blend_len,
-        is_moving = False,
+        is_moving=False,
         frame_time=1 / 60,
     ):
         self._blend_len = blend_len
         self._frame_time = frame_time
         self.moving_flag = is_moving
 
-        self._q0 = target.get_root_transform().inverse() * source_first.get_root_transform()
-        self._qp = target.get_root_transform().inverse() * source_second.get_root_transform()
+        self._q0 = (
+            target.get_root_transform().inverse() * source_first.get_root_transform()
+        )
+        self._qp = (
+            target.get_root_transform().inverse() * source_second.get_root_transform()
+        )
 
-        self.default_transl_offset = source_first.get_root_transform().translation - target.get_root_transform().translation
-        left_foot0 = (source_first.get_component_translation_by_name("LeftToe") -  target.get_component_translation_by_name("LeftToe"))/2
-        right_foot0 = (source_first.get_component_translation_by_name("RightToe") -  target.get_component_translation_by_name("RightToe"))/2
-        self.transl0 = np.matmul(source_first.get_root_transform().rotation_np, (left_foot0 + right_foot0))
-        left_footp = (source_second.get_component_translation_by_name("LeftToe") -  target.get_component_translation_by_name("LeftToe"))/2
-        right_footp = (source_second.get_component_translation_by_name("RightToe") -  target.get_component_translation_by_name("RightToe"))/2
-        translp = np.matmul(source_second.get_root_transform().rotation_np, (left_footp + right_footp))
+        self.default_transl_offset = (
+            source_first.get_root_transform().translation
+            - target.get_root_transform().translation
+        )
+        left_foot0 = (
+            source_first.get_component_translation_by_name("LeftToe")
+            - target.get_component_translation_by_name("LeftToe")
+        ) / 2
+        right_foot0 = (
+            source_first.get_component_translation_by_name("RightToe")
+            - target.get_component_translation_by_name("RightToe")
+        ) / 2
+        self.transl0 = np.matmul(
+            source_first.get_root_transform().rotation_np, (left_foot0 + right_foot0)
+        )
+        left_footp = (
+            source_second.get_component_translation_by_name("LeftToe")
+            - target.get_component_translation_by_name("LeftToe")
+        ) / 2
+        right_footp = (
+            source_second.get_component_translation_by_name("RightToe")
+            - target.get_component_translation_by_name("RightToe")
+        ) / 2
+        translp = np.matmul(
+            source_second.get_root_transform().rotation_np, (left_footp + right_footp)
+        )
         self.transl_offset = self.default_transl_offset + self.transl0
 
         self._x0 = np.array([self._q0.rotation.as_rotvec()])
         self._x0[np.linalg.norm(self._x0, axis=1) == 0, :] = 0.00000001
         self._x0_u = self._x0 / np.linalg.norm(self._x0, axis=1, keepdims=True)
         self._x0_u[np.isnan(self._x0_u)] = 0.0
         self._x0 = np.linalg.norm(self._x0, axis=1)
@@ -182,22 +219,31 @@
         xt_t = xt[joint_num:]
         return R.from_rotvec(xt_r), xt_t
 
     def root_blending(self, frame, count):
         xt_r, xt_t = self.get_xt(count)
         if count < self._blend_len:
             root_ori = xt_r[0] * frame.get_root_transform().rotation
-            transl = frame.get_root_transform().translation + self.default_transl_offset + (self.transl0 - xt_t)[0]
+            transl = (
+                frame.get_root_transform().translation
+                + self.default_transl_offset
+                + (self.transl0 - xt_t)[0]
+            )
         else:
             root_ori = frame.get_root_transform().rotation
-            transl = frame.get_root_transform().translation + self.default_transl_offset + self.transl0
+            transl = (
+                frame.get_root_transform().translation
+                + self.default_transl_offset
+                + self.transl0
+            )
         new_root = Transform(root_ori, transl)
         frame.set_root_transform(new_root)
         return frame
 
+
 class BlendingInertialization:
     def __init__(
         self,
         source_first,
         source_second,
         target,
         blend_len,
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/database.py` & `vaaibody-0.0.0.5/source/vaaibody/core/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 import time
 from pathlib import Path
 from typing import Optional
 
 import numpy as np
 from parameter.gesture_matching_parameter import MCS_LOWER_BLENDING
 from tqdm import tqdm
-from utilities.utils import get_data_stats, normalize_data
+from vaaibody.utilities.utils import get_data_stats, normalize_data
 
-from core.audio import Audio, AudioDatabase
-from core.feature import (AudioFeature, HeadPoseFeature, LowerPoseFeature,
-                          NonTalkingPoseFeature, WeightedUpperVelFeature)
-from core.motion import MotionDatabase
+from vaaibody.core.audio import Audio, AudioDatabase
+from vaaibody.core.feature import (
+    AudioFeature,
+    HeadPoseFeature,
+    LowerPoseFeature,
+    NonTalkingPoseFeature,
+    WeightedUpperVelFeature,
+)
+from vaaibody.core.motion import MotionDatabase
 
 
 class AudioFeatureDatabase:
     def __init__(self, audio: Audio, fps):
         start_time = time.time()
         self._audio = audio
         self._is_loaded = False
@@ -108,28 +113,27 @@
         self._control_weight = weights.pop("control")
         self._pose_feature.set_weights(weights)
 
     def preprocess_from_pickle_file(
         self,
     ):
         if os.path.exists(self._db_path):
-            path = "{}/{}".format(self._db_path, self.db_file_name)
+            path = self._db_path / self.db_file_name
             if os.path.exists(path):
                 with open(path, "rb") as fr:
                     db = pickle.load(fr)
                     self.idx_motion_list = db["idx_motion_list"]
                     n_feature = len(db["pose_feature"])
                     for idx_feature in range(n_feature):
                         self.pose_feature.append(db["pose_feature"][idx_feature])
                         self.lower_feature.append(db["lower_feature"][idx_feature])
                         self.head_feature.append(db["head_feature"][idx_feature])
             else:
                 return False
         self.calc_nums()
-
         return True
 
     def preprocess_from_scratch(
         self,
     ):
         _pose_feature = WeightedUpperVelFeature(look_ahead=self.motion_look_ahead)
         _head_feature = HeadPoseFeature(look_ahead=self.motion_look_ahead)
@@ -168,15 +172,15 @@
         }
 
         for idx_feature in range(len(self.pose_feature)):
             db_dict["pose_feature"].append(self.pose_feature[idx_feature])
             db_dict["lower_feature"].append(self.lower_feature[idx_feature])
             db_dict["head_feature"].append(self.head_feature[idx_feature])
         db_dict["idx_motion_list"] = self.idx_motion_list
-        save_filename = "{}/{}".format(self._db_path, self.db_file_name)
+        save_filename = self._db_path / self.db_file_name
         with open(save_filename, "wb") as fw:
             pickle.dump(db_dict, fw)
 
     def calc_nums(
         self,
     ):
         self._num_motion = len(self.pose_feature)
@@ -495,15 +499,15 @@
             db_dict["pose_feature"].append(self.pose_feature[idx_feature])
             db_dict["lower_feature"].append(self.lower_feature[idx_feature])
             db_dict["head_feature"].append(self.head_feature[idx_feature])
             db_dict["mfcc_feature"].append(self.mfcc_feature[idx_feature])
             db_dict["beat_feature"].append(self.beat_feature[idx_feature])
         db_dict["idx_motion_list"] = self.idx_motion_list
         db_dict["motion_name_list"] = self.motion_name_list
-        save_filename = "{}/{}".format(self._db_path, self.db_file_name)
+        save_filename = self._db_path / self.db_file_name
         with open(save_filename, "wb") as fw:
             pickle.dump(db_dict, fw)
         print("DB saved")
 
     def calc_nums(
         self,
     ):
@@ -648,15 +652,15 @@
 
     def preprocess_from_db(
         self,
     ):
         print("Load data from preprocess_from_scratched file:", self.db_file_name)
         self._gesture_feature_DB = []
         if os.path.exists(self._db_path):
-            path = "{}/{}".format(self._db_path, self.db_file_name)
+            path = self._db_path / self.db_file_name
             if os.path.exists(path):
                 with open(path, "rb") as fr:
                     db = pickle.load(fr)
                     self.motion_idx_list = db["motion_idx_list"]
                     n_db = len(db["pose_feature"])
                     for i in range(n_db):
                         self._gesture_feature_DB.append([db["pose_feature"][i]])
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/feature.py` & `vaaibody-0.0.0.5/source/vaaibody/core/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from collections import deque
 
 import numpy as np
-from parameter.gesture_matching_parameter import (MCS_LOWER,
-                                                  MCS_LOWER_BLENDING, MCS_NON,
-                                                  MCS_SPINES, MCS_UPPER,
-                                                  MCS_UPPER_2)
-from utilities.frame_utils import get_position_vel
+from parameter.gesture_matching_parameter import (
+    MCS_LOWER,
+    MCS_LOWER_BLENDING,
+    MCS_NON,
+    MCS_SPINES,
+    MCS_UPPER,
+    MCS_UPPER_2,
+)
+from vaaibody.utilities.frame_utils import get_position_vel
 
 """"
 Here, we define the pose feature and the audio feature
 We first define the upper body pose feature and then move on to the full body
 The upper body pose features are the relative positions of below body parts to the root.
 - Both side elbow, wrist, index_base, little_base. (Total 8 joints)
 """
@@ -180,14 +184,15 @@
             post_pad = np.zeros((idx, 3))
             body_feat[:, i, :] = np.concatenate(
                 (single_feat[idx:, :], post_pad), axis=0
             )
         body_feat = body_feat.reshape((m_num, -1))
         return body_feat
 
+
 class WeightedUpperPoseFeature(JointFeature):
     def __init__(
         self,
         look_ahead: list = [0],
         weight: float = 1,
         min_cost: float = 0,
         max_cost=None,
@@ -321,28 +326,31 @@
 
     def compute_feature(self, motion):
         m_num = motion.num_frame()
         single_feat = np.zeros((m_num, len(self._joints) * 3))
         for idx_frame in range(m_num):
             single_feat[idx_frame, :] = np.concatenate(
                 [
-                    motion._frames[idx_frame].get_component_transform_by_name(j).translation
+                    motion._frames[idx_frame]
+                    .get_component_transform_by_name(j)
+                    .translation
                     for j in self._joints
                 ],
                 axis=-1,
             )
         body_feat = np.zeros((m_num, len(self._look_ahead), len(self._joints) * 3))
         for i, idx in enumerate(self._look_ahead):
             post_pad = np.zeros((idx, len(self._joints) * 3))
             body_feat[:, i, :] = np.concatenate(
                 (single_feat[idx:, :], post_pad), axis=0
             )
         body_feat = body_feat.reshape((m_num, -1))
         return body_feat
 
+
 class NonTalkingPoseFeature(JointFeature):
     def __init__(
         self,
         look_ahead: list = [0],
         weight: float = 1,
         min_cost: float = 0,
         max_cost=None,
@@ -360,15 +368,17 @@
     def compute_feature(self, motion):
         joint_dict = motion._skeleton.joint_dict
         m_num = motion.num_frame()
         single_feat = np.zeros((m_num, len(self._joints) * 3))
         for idx_frame in range(m_num):
             single_feat[idx_frame, :] = np.concatenate(
                 [
-                    motion._frames[idx_frame].get_component_transform_by_name(j).translation
+                    motion._frames[idx_frame]
+                    .get_component_transform_by_name(j)
+                    .translation
                     for j in self._joints
                 ],
                 axis=-1,
             )
         body_feat = np.zeros((m_num, len(self._look_ahead), len(self._joints) * 3))
         for i, idx in enumerate(self._look_ahead):
             post_pad = np.zeros((idx, len(self._joints) * 3))
@@ -434,15 +444,15 @@
         max_cost=None,
     ):
         self.joints = MCS_NON
         self._look_behind = look_behind
         super().__init__(self.joints, weight, min_cost, max_cost)
 
     def update_look_behind(self, look_behind):
-        self._look_behind= look_behind
+        self._look_behind = look_behind
 
     def compute_dof(self):
         return len(self._joints) * len(self._look_behind) * 3
 
     def compute_feature(self, motion):
         m_num = motion.num_frame()
         single_feat = np.zeros((m_num, len(self._joints) * 3))
@@ -455,15 +465,15 @@
                 [
                     motion._frames[i].get_component_transform_by_name(j).translation
                     for j in self._joints
                 ],
                 axis=-1,
             )
         body_feat = np.zeros((m_num, len(self._look_behind), len(self._joints) * 3))
-        
+
         """
         이 부분이 history로 패딩하는 코드이다.
         """
         for i, idx in enumerate(self._look_behind):
             if idx == 0:
                 body_feat[:, i, :] = single_feat
                 continue
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/filter_frame.py` & `vaaibody-0.0.0.5/source/vaaibody/core/filter_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from utilities.filter import *
-from utilities.frame_utils import *
+from vaaibody.utilities.filter import *
+from vaaibody.utilities.frame_utils import *
 
 """
 TO DO
 Make it compatable for action
 """
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/frame.py` & `vaaibody-0.0.0.5/source/vaaibody/core/frame.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from copy import deepcopy
 from typing import List, Optional
 
 import numpy as np
-from collections import deque # deque 패키지 불러오기
+from collections import deque  # deque 패키지 불러오기
 
 import scipy as sp
 from scipy.spatial.transform import Rotation as R
-from utilities.timechecker import TimeChecker as TC
-
-from .skeleton import Skeleton, Transform
 
+from vaaibody.core.skeleton import Skeleton, Transform
 
 
 class Frame:
     __slots__ = (
         "_skeleton",
         "_root_transform",
         "_root_transform_inv",
@@ -46,16 +44,20 @@
         self._global_transforms = global_transforms
         self._component_transforms = component_transforms
         self._body_global_transforms = body_global_transforms
         self._is_scalar = scalar
 
         self._rot = self._skeleton._rot
         self._global_dirty_flags = [False for _ in range(self._skeleton.num_joints())]
-        self._component_dirty_flags = [False for _ in range(self._skeleton.num_joints())]
-        self._body_global_dirty_flags = [False for _ in range(self._skeleton.num_joints())]
+        self._component_dirty_flags = [
+            False for _ in range(self._skeleton.num_joints())
+        ]
+        self._body_global_dirty_flags = [
+            False for _ in range(self._skeleton.num_joints())
+        ]
 
         if global_transforms is None:
             self._global_transforms = [None] * self._skeleton.num_joints()
         if component_transforms is None:
             self._body_global_transforms = [None] * self._skeleton.num_joints()
         if body_global_transforms is None:
             self._component_transforms = [None] * self._skeleton.num_joints()
@@ -133,24 +135,30 @@
     def get_local_translation(self, joint_idx):
         return self._local_transforms[joint_idx].translation
 
     def get_local_translation_by_name(self, joint_name):
         return self.get_local_translation(self._skeleton.joint_dict[joint_name])
 
     def get_body_global_transform(self, joint_idx):
-        if self._body_global_dirty_flags[joint_idx] or self._body_global_transforms[joint_idx] is None:
-            self.update_transforms(joint_idx, update_type='body_global')
+        if (
+            self._body_global_dirty_flags[joint_idx]
+            or self._body_global_transforms[joint_idx] is None
+        ):
+            self.update_transforms(joint_idx, update_type="body_global")
         return self._body_global_transforms[joint_idx]
 
     def get_body_global_transform_by_name(self, joint_name):
         return self.get_body_global_transform(self._skeleton.joint_dict[joint_name])
 
     def get_global_transform(self, joint_idx):
-        if self._global_dirty_flags[joint_idx] or self._global_transforms[joint_idx] is None:
-            self.update_transforms(joint_idx, update_type='global')
+        if (
+            self._global_dirty_flags[joint_idx]
+            or self._global_transforms[joint_idx] is None
+        ):
+            self.update_transforms(joint_idx, update_type="global")
         return self._global_transforms[joint_idx]
 
     def get_relative_translation_by_name(self, joint1, joint2):
         diff = self.get_global_translation_by_name(
             joint1
         ) - self.get_global_translation_by_name(joint2)
         norm_diff = np.matmul(
@@ -177,16 +185,19 @@
     def get_global_translation(self, joint_idx):
         return self.get_global_transform(joint_idx).translation
 
     def get_global_translation_by_name(self, joint_name):
         return self.get_global_translation(self._skeleton.joint_dict[joint_name])
 
     def get_component_transform(self, joint_idx):
-        if self._component_dirty_flags[joint_idx] or self._component_dirty_flags[joint_idx] is None:
-            self.update_transforms(joint_idx, update_type='component')
+        if (
+            self._component_dirty_flags[joint_idx]
+            or self._component_dirty_flags[joint_idx] is None
+        ):
+            self.update_transforms(joint_idx, update_type="component")
         return self._component_transforms[joint_idx]
 
     def get_component_transform_by_name(self, joint_name):
         if joint_name[-2:] == "_e":
             joint_idx = self._skeleton.joint_dict[joint_name[:-2]]
             joint_comp = self.get_component_transform(joint_idx)
             end_local_transform = self._skeleton.joints[joint_idx]._end_site_transform
@@ -199,31 +210,29 @@
 
     def get_component_translation_by_name(self, joint_name):
         return self.get_component_transform_by_name(joint_name).translation
 
     def set_root_transform(self, new_transform):
         self._root_transform = new_transform
         self._root_transform_inv = self._root_transform.inverse()
-        self.set_dirty(0) 
+        self.set_dirty(0)
 
     def set_by_raw_rotations(self, raw_rotations):
         for idx in range(1, self.num_joints()):
             current_rotation = R.from_euler(
                 self._rot, raw_rotations[3 * (idx + 1) : 3 * (idx + 2)], degrees=True
             )
             self.set_local_rotation(joint_idx=idx, new_rotation=current_rotation)
 
     def set_local_transforms(self, new_transforms):
         for idx in range(self.num_joints()):
             self.set_local_transform(idx, new_transforms[idx])
 
     def set_local_transform_by_name(self, joint_name, new_transform):
-        self.set_local_transform(
-            self._skeleton.joint_dict[joint_name], new_transform
-        )
+        self.set_local_transform(self._skeleton.joint_dict[joint_name], new_transform)
 
     def set_local_transform(self, joint_idx, new_transform):
         self._local_transforms[joint_idx] = new_transform
         self.set_dirty(joint_idx)
 
     def set_local_translation(self, joint_idx, new_translation):
         self._local_transforms[joint_idx].translation = new_translation
@@ -272,15 +281,15 @@
             if visit_joint_idx not in visited:
                 self._component_dirty_flags[visit_joint_idx] = True
                 self._global_dirty_flags[visit_joint_idx] = True
                 self._body_global_dirty_flags[visit_joint_idx] = True
                 visited.append(visit_joint_idx)
                 need_to_visit.extend(node._children)
 
-    def update_transforms(self, joint_idx, update_type='global'):
+    def update_transforms(self, joint_idx, update_type="global"):
         joint = self._skeleton.joints[joint_idx]
         parent = joint.parent
 
         if self._global_dirty_flags[joint_idx]:
             if parent is not None:
                 self._global_transforms[joint_idx] = (
                     self.get_global_transform(parent.idx)
@@ -288,21 +297,21 @@
                 )
             else:
                 self._global_transforms[joint_idx] = (
                     self._root_transform * self._local_transforms[joint_idx]
                 )
             self._global_dirty_flags[joint_idx] = False
 
-        if update_type == 'body_global' and self._body_global_dirty_flags[joint_idx]:
+        if update_type == "body_global" and self._body_global_dirty_flags[joint_idx]:
             self._body_global_transforms[joint_idx] = (
                 self._global_transforms[joint_idx] * joint.body_transform
             )
             self._body_global_dirty_flags[joint_idx] = False
 
-        elif update_type == 'component' and self._component_dirty_flags[joint_idx]:
+        elif update_type == "component" and self._component_dirty_flags[joint_idx]:
             self._component_transforms[joint_idx] = (
                 self.get_inverse_root_transform() * self._global_transforms[joint_idx]
             )
             self._component_dirty_flags[joint_idx] = False
 
     def scale(self, scale, method="vector"):
         if method == "vector":
@@ -483,8 +492,8 @@
         # new_root_transform.translation = self.get_root_transform().translation - base_frame.get_root_transform().translation
         new_local_transforms = [
             base_frame.get_local_transform(j).inverse() * self.get_local_transform(j)
             for j in range(self.num_joints())
         ]
         return Frame(
             self._skeleton, new_root_transform, new_local_transforms, scalar=False
-        )
+        )
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/gesture_matching.py` & `vaaibody-0.0.0.5/source/vaaibody/core/gesture_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from sklearn.metrics import pairwise_distances
 
 # from decompressor_util import get_local_transform_from_posrot
 from parameter.gesture_matching_parameter import MCS_SPINES
 from scipy import spatial
 from sklearn.neighbors import KDTree
 from tqdm import tqdm
-from utilities import quat
-from utilities.frame_utils import filter_frames
-from utilities.timechecker import TimeChecker as TC
-from utilities.utils import angle_between_two_vectors
+from vaaibody.utilities import quat
+from vaaibody.utilities.frame_utils import filter_frames
+from vaaibody.utilities.timechecker import TimeChecker as TC
+from vaaibody.utilities.utils import angle_between_two_vectors
 
-from core.blending import BlendingInertialization, JointBlendingInertialization
-from core.database import (
+from vaaibody.core.blending import BlendingInertialization, JointBlendingInertialization
+from vaaibody.core.database import (
     LatentFeatureDatabase,
     MotionAudioFeatureDatabase,
     MotionFeatureDatabase,
 )
-from core.motion import Motion
-from core.skeleton import *
+from vaaibody.core.motion import Motion
+from vaaibody.core.skeleton import *
 
 
 class GestureMatching(object):
     def __init__(
         self,
         gesture_db: MotionAudioFeatureDatabase,
         step_size=48,
@@ -194,42 +194,55 @@
         test_pose_feature = []
         lower_sliced_feature = []
         silent_sliced_feature = []
 
         time_stamp = []
         for idx_clip in range(self._gesture_db._motion_db.num_motion()):
             frame_num = self._gesture_db._motion_db.get_motion_len(idx_clip)
-            pose_beat_feature.append(np.column_stack([pose_feature[idx_clip][0][:-self.max_onset], 
-            AUDIO_SCALE_VALUE * beat_feature[idx_clip][0][:frame_num-self.max_onset]]))
+            pose_beat_feature.append(
+                np.column_stack(
+                    [
+                        pose_feature[idx_clip][0][: -self.max_onset],
+                        AUDIO_SCALE_VALUE
+                        * beat_feature[idx_clip][0][: frame_num - self.max_onset],
+                    ]
+                )
+            )
             if len(time_stamp) == 0:
-                time_stamp.append([0, frame_num-self.max_onset])
+                time_stamp.append([0, frame_num - self.max_onset])
             else:
-                time_stamp.append([time_stamp[-1][0] + time_stamp[-1][1], frame_num-self.max_onset])
+                time_stamp.append(
+                    [time_stamp[-1][0] + time_stamp[-1][1], frame_num - self.max_onset]
+                )
 
         time_stamp_sil = []
         for idx_clip_sil in range(self._silent_db._motion_db.num_motion()):
             frame_num = self._silent_db._motion_db.get_motion_len(idx_clip_sil)
             silent_sliced_feature.append(silent_release_feature[idx_clip_sil][0])
             if len(time_stamp_sil) == 0:
                 time_stamp_sil.append([0, frame_num])
             else:
-                time_stamp_sil.append([time_stamp_sil[-1][0] + time_stamp_sil[-1][1], frame_num])
+                time_stamp_sil.append(
+                    [time_stamp_sil[-1][0] + time_stamp_sil[-1][1], frame_num]
+                )
 
         pose_beat_feature_concat = np.concatenate(pose_beat_feature, axis=0)
         silent_feature_concat = np.concatenate(silent_sliced_feature, axis=0)
- 
+
         self.silent = sil_hint
         n_frames = mfcc_test.shape[-1]
         beat_test = np.concatenate(
             (beat_test[:, 0:1], beat_test), axis=1
         )  # 60, n_frame
-        
+
         pose_test = np.zeros(shape=(self.n_pose_feature, mfcc_test.shape[1]))
         init_motion, init_seq, init_frm = self.init_frame(is_rand=False)
-        init_lower_motion, init_lower_seq, init_lower_frm = self.init_frame(is_rand=False)
+        init_lower_motion, init_lower_seq, init_lower_frm = self.init_frame(
+            is_rand=False
+        )
 
         lower_motion = init_lower_motion
         lower_frm = init_lower_frm
 
         pose_test[:, 0] = self.pose_feature[init_motion][init_seq, init_frm, :]
         self.pred_motion_idx = []
         self.pred_lower_idx = []
@@ -244,72 +257,104 @@
             if self.silent is None:
                 self.step_size = self.slice_with_beat(beat_test, j)
             else:
                 self.step_size = self.slice_with_beatNsil(beat_test, j)
             if j + self.step_size >= n_frames:
                 self.step_size = n_frames - j - 1
                 loop_flag = False
-            
+
             if self.is_speaking:
-                pose_beat_feature_input = np.column_stack([np.expand_dims(pose_test[:, j - 1], axis=0), 
-                np.expand_dims(AUDIO_SCALE_VALUE * beat_test[:, j], axis=0)])
-                dist = pairwise_distances(pose_beat_feature_concat, pose_beat_feature_input)
+                pose_beat_feature_input = np.column_stack(
+                    [
+                        np.expand_dims(pose_test[:, j - 1], axis=0),
+                        np.expand_dims(AUDIO_SCALE_VALUE * beat_test[:, j], axis=0),
+                    ]
+                )
+                dist = pairwise_distances(
+                    pose_beat_feature_concat, pose_beat_feature_input
+                )
             else:
                 pose_feature_input = np.expand_dims(pose_test[:, j - 1], axis=0)
                 dist = pairwise_distances(silent_feature_concat, pose_feature_input)
 
             result_idx_list = np.argpartition(dist[:, 0], 2)
             if dist[result_idx_list[0]] > 0:
                 result_idx = result_idx_list[0]
             else:
                 result_idx = result_idx_list[1]
 
-
             idx_pred_motion, idx_pred_frame = None, None
             if not self.is_speaking:
                 time_seq_stamp = time_stamp_sil
             else:
                 time_seq_stamp = time_stamp
 
             for idx_time in range(len(time_seq_stamp)):
-                if idx_time < len(time_seq_stamp)-1:
-                    if result_idx >= time_seq_stamp[idx_time][0] and result_idx < time_seq_stamp[idx_time+1][0]:
+                if idx_time < len(time_seq_stamp) - 1:
+                    if (
+                        result_idx >= time_seq_stamp[idx_time][0]
+                        and result_idx < time_seq_stamp[idx_time + 1][0]
+                    ):
                         idx_pred_motion = idx_time
                         idx_pred_frame = result_idx - time_seq_stamp[idx_time][0]
                         break
                 else:
                     if result_idx >= time_seq_stamp[idx_time][0]:
                         idx_pred_motion = idx_time
                         idx_pred_frame = result_idx - time_seq_stamp[idx_time][0]
 
             if not self.is_speaking and idx_pred_motion is None:
-                idx_pred_motion, idx_pred_frame = 1,0
+                idx_pred_motion, idx_pred_frame = 1, 0
 
             # if self.is_speaking: #for test
             #     print('score', dist[result_idx], idx_pred_motion, idx_pred_frame)
             #     print('hamming', spatial.distance.hamming(beat_feature[idx_pred_motion][0][idx_pred_frame], beat_test[:, j]))
             #     beat_score_aveg.append(spatial.distance.hamming(beat_feature[idx_pred_motion][0][idx_pred_frame], beat_test[:, j]))
             #     pose_score_aveg.append(pairwise_distances(np.expand_dims(pose_feature[idx_pred_motion][0][idx_pred_frame],axis=0), np.expand_dims(pose_test[:, j - 1], axis=0)))
-    
-            low_mo = self.play_motion_test(lower_motion, lower_frm, lower_sliced_feature, time_seq_stamp)
+
+            low_mo = self.play_motion_test(
+                lower_motion, lower_frm, lower_sliced_feature, time_seq_stamp
+            )
             self.pred_lower_idx.append(low_mo)
             lower_motion = low_mo[-1][0]
             lower_frm = low_mo[-1][1]
             if self.is_speaking:
-                pose_test[:, j : (j + self.step_size)] = pose_feature[idx_pred_motion][0][idx_pred_frame : (idx_pred_frame + self.step_size), :].transpose()
-            else:
-                res = self.step_size - silent_release_feature[idx_pred_motion][0][idx_pred_frame : (idx_pred_frame + self.step_size), :].shape[0] 
+                pose_test[:, j : (j + self.step_size)] = pose_feature[idx_pred_motion][
+                    0
+                ][idx_pred_frame : (idx_pred_frame + self.step_size), :].transpose()
+            else:
+                res = (
+                    self.step_size
+                    - silent_release_feature[idx_pred_motion][0][
+                        idx_pred_frame : (idx_pred_frame + self.step_size), :
+                    ].shape[0]
+                )
                 if res > 0:
-                    pad_arr = np.array(res*[silent_release_feature[idx_pred_motion][0][-1, :]])
-                    padded_feature = np.vstack((silent_release_feature[idx_pred_motion][0][idx_pred_frame : (idx_pred_frame + self.step_size), :], pad_arr))
+                    pad_arr = np.array(
+                        res * [silent_release_feature[idx_pred_motion][0][-1, :]]
+                    )
+                    padded_feature = np.vstack(
+                        (
+                            silent_release_feature[idx_pred_motion][0][
+                                idx_pred_frame : (idx_pred_frame + self.step_size), :
+                            ],
+                            pad_arr,
+                        )
+                    )
                     pose_test[:, j : (j + self.step_size)] = padded_feature.transpose()
                 else:
-                    pose_test[:, j : (j + self.step_size)] = silent_release_feature[idx_pred_motion][0][idx_pred_frame : (idx_pred_frame + self.step_size), :].transpose()
-            
-            self.pred_motion_idx.append([idx_pred_motion, idx_pred_frame, self.step_size, self.is_speaking])
+                    pose_test[:, j : (j + self.step_size)] = silent_release_feature[
+                        idx_pred_motion
+                    ][0][
+                        idx_pred_frame : (idx_pred_frame + self.step_size), :
+                    ].transpose()
+
+            self.pred_motion_idx.append(
+                [idx_pred_motion, idx_pred_frame, self.step_size, self.is_speaking]
+            )
             j += self.step_size
 
         # print('a', sum(beat_score_aveg)/len(beat_score_aveg), len(beat_score_aveg))
         # print('b', sum(pose_score_aveg)/len(pose_score_aveg), len(pose_score_aveg))
         print("Matching takes {}seconds".format(time.time() - start_time))
 
         start_blend = time.time()
@@ -347,22 +392,28 @@
             is_speaking = motion_idx[3]
             if i > 0:
                 first_motion, second_motion = (
                     blended_frames[-2],
                     self.blended_frames[-1],
                 )
                 if use_sil_real and not is_speaking:
-                    target_frame = self._silent_db.get_frame(motion_idx[0], motion_idx[1]).copy()
+                    target_frame = self._silent_db.get_frame(
+                        motion_idx[0], motion_idx[1]
+                    ).copy()
                 else:
-                    target_frame = self._gesture_db.get_frame(motion_idx[0], motion_idx[1]).copy()
+                    target_frame = self._gesture_db.get_frame(
+                        motion_idx[0], motion_idx[1]
+                    ).copy()
                 # Implement add lower body to the target frame
                 if not search_lower:
                     lower_idx = lower_list[0]
 
-                target_lower = self._gesture_db._motion_db.get_frame(lower_idx[0], lower_idx[1]).copy()
+                target_lower = self._gesture_db._motion_db.get_frame(
+                    lower_idx[0], lower_idx[1]
+                ).copy()
                 target_frame.set_root_transform(target_lower.get_root_transform())
 
                 for lower in self._gesture_db.lower_joints_matching:
                     low_tar = target_lower.get_local_rotation_by_name(lower)
                     target_frame.set_local_rotation_by_name(lower, low_tar)
                 new_root = target_frame.get_root_transform()
                 current_root = second_motion.get_root_transform()
@@ -374,26 +425,36 @@
                     second_motion,
                     first_motion,
                     target_frame,
                     blend_dur,
                     self.frame_time,
                     is_frame=True,
                 )
-            for step_size in range(motion_idx[2]):  # modion_cand - i, k, f, self.step_size
+            for step_size in range(
+                motion_idx[2]
+            ):  # modion_cand - i, k, f, self.step_size
                 if use_sil_real and not is_speaking:
                     try:
-                        current_frame = self._silent_db.get_frame(motion_idx[0], motion_idx[1]+step_size).copy()
+                        current_frame = self._silent_db.get_frame(
+                            motion_idx[0], motion_idx[1] + step_size
+                        ).copy()
                     except:
-                        current_frame = self._silent_db.get_frame(motion_idx[0], -1).copy()
+                        current_frame = self._silent_db.get_frame(
+                            motion_idx[0], -1
+                        ).copy()
                 else:
-                    current_frame = self._gesture_db.get_frame(motion_idx[0], motion_idx[1]+step_size).copy()
+                    current_frame = self._gesture_db.get_frame(
+                        motion_idx[0], motion_idx[1] + step_size
+                    ).copy()
                 # Implement add lower body to the target frame
                 if not search_lower:
                     lower_idx = lower_list[step_size]
-                    target_lower = self._gesture_db.get_frame(lower_idx[0], lower_idx[1]).copy()
+                    target_lower = self._gesture_db.get_frame(
+                        lower_idx[0], lower_idx[1]
+                    ).copy()
                     if lower_idx[0] != prev_motion:
                         new_root = target_lower.get_root_transform()
                         current_root = self.blended_frames[-1].get_root_transform()
                         root_offset = current_root * new_root.inverse()
                         prev_motion = lower_idx[0]
 
                 # 하반신 덮어쓰기. 안그러면 발 미끌림
@@ -588,16 +649,18 @@
                 pose_dist_cands.append(d)
                 motion_cands.append([idx_motion, idx_seq, idx_frame, self.step_size])
                 pose_feature_cands.append(pose_feature_cand)
         pose_dist_cands = np.array(pose_dist_cands)
         motion_cands = np.array(motion_cands)
         pose_feature_cands = np.array(pose_feature_cands)
         return pose_dist_cands, motion_cands, pose_feature_cands
-    
-    def play_motion_test(self, lower_motion, lower_frm, lower_sliced_feature, time_stamp):
+
+    def play_motion_test(
+        self, lower_motion, lower_frm, lower_sliced_feature, time_stamp
+    ):
         play_list = []
         num_frame = self.n_db_frame[lower_motion]
 
         for idx_step in range(1, self.step_size + 1):
             play_list.append([lower_motion, idx_step + lower_frm])
 
         return play_list
@@ -688,15 +751,15 @@
         else:
             lower_motion = init_lower_motion
             lower_seq = init_lower_seq
             lower_frm = init_lower_frm
         self.pred_motion_idx = []
         self.pred_lower_idx = []
 
-        beat_score_aveg = [] 
+        beat_score_aveg = []
         pose_score_aveg = []
 
         j = 1  # 입력 audio에 대해 현재 찾은 idx+1. 0이 아니라 1인 이유는 처음에 concat한 이유랑 같음.
         loop_flag = True
         start_time = time.time()
         while loop_flag:
             if self.silent is None:
@@ -720,19 +783,21 @@
                 (
                     pose_dist_cands,
                     motion_cands,
                     pose_feature_cands,
                 ) = self.search_motion_only_cands_KD(
                     pose_test[:, j - 1], KD_type="silent_rel", max_query=20
                 )  # search pose from only motion (음성 없이)
-            pose_score = np.array(pose_dist_cands).argsort().argsort()  
+            pose_score = np.array(pose_dist_cands).argsort().argsort()
 
             if self.is_speaking:
                 mfcc_score = self.sort_cosine_dist(mfcc_feature_cands, mfcc_test[:, j])
-                beat_score, beat_score_raw = self.sort_hamming_dist(beat_feature_cands, beat_test[:, j])
+                beat_score, beat_score_raw = self.sort_hamming_dist(
+                    beat_feature_cands, beat_test[:, j]
+                )
             total_score = pose_score
             if self.is_speaking:
                 # total_score += mfcc_score
                 total_score += beat_score
             total_sorted_list = np.argsort(total_score).tolist()
             # if self.is_speaking:
             #     print(total_sorted_list[0], pose_dist_cands[total_sorted_list[0]], beat_score_raw[total_sorted_list[0]])
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/motion.py` & `vaaibody-0.0.0.5/source/vaaibody/core/motion.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from copy import deepcopy
 from pathlib import Path
 
 import natsort
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 
-from .frame import Frame
-from .skeleton import Skeleton, Transform
+from vaaibody.core.frame import Frame
+from vaaibody.core.skeleton import Skeleton, Transform
 
 
 def load_frame_from_bvh(file_path, idx, default_lines):
     """
     idx에 해당하는 frame line load
     """
     line = linecache.getline(file_path, idx + default_lines)
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/core/skeleton.py` & `vaaibody-0.0.0.5/source/vaaibody/core/skeleton.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/decompressor.py` & `vaaibody-0.0.0.5/source/vaaibody/decompressor.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/decompressor_savedb.py` & `vaaibody-0.0.0.5/source/vaaibody/decompressor_savedb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from scipy.spatial.transform import Rotation as R
 from torch.utils.tensorboard import SummaryWriter
 
-from core.database import MotionDatabase, MotionFeatureDatabase
-from core.skeleton import Skeleton
+from vaaibody.core.database import MotionDatabase, MotionFeatureDatabase
+from vaaibody.core.skeleton import Skeleton
 from decompressor import Compressor, Decompressor
 from decompressor_util import *
-from utilities import quat, txform
-from utilities.exporter import Exporter
+from vaaibody.utilities import quat, txform
+from vaaibody.utilities.exporter import Exporter
 
 # Load
 bvh_name = "data/matching_data/rhythm_motion/VAAI_Short_01_02.bvh"
 bvh_npz_path = "data/matching_data/rhythm_motion_npz/"
 audio_db_path = "data/matching_data/rhythm_audio"
 silent_db_path = "data/matching_data/silent_release"
 # silent_db_path = "data/motion/Gesture_Before"
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/decompressor_train.py` & `vaaibody-0.0.0.5/source/vaaibody/decompressor_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import argparse
 import sys
 
 import numpy as np
 import torch
 from torch.utils.tensorboard import SummaryWriter
 
-from core.database import MotionDatabase, MotionFeatureDatabase
-from core.frame import Frame
-from core.motion import Motion
-from core.skeleton import Skeleton
+from vaaibody.core.database import MotionDatabase, MotionFeatureDatabase
+from vaaibody.core.frame import Frame
+from vaaibody.core.motion import Motion
+from vaaibody.core.skeleton import Skeleton
 from decompressor import Compressor, Decompressor
 from decompressor_util import *
-from utilities import quat, txform
-from utilities.exporter import Exporter
+from vaaibody.utilities import quat, txform
+from vaaibody.utilities.exporter import Exporter
 
 
 def main(args):
     # Path
     bvh_name = args.bvh_name
     bvh_npz_path = args.bvh_npz_path
     audio_db_path = args.audio_db_path
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/decompressor_util.py` & `vaaibody-0.0.0.5/source/vaaibody/decompressor_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import torch
 from scipy.spatial.transform import Rotation as R
 
-from core.motion import Motion
-from core.skeleton import Transform
-from utilities.frame_utils import get_angular_vel, get_position_vel
+from vaaibody.core.motion import Motion
+from vaaibody.core.skeleton import Transform
+from vaaibody.utilities.frame_utils import get_angular_vel, get_position_vel
 
 
 def get_positions_from_motion(motion: Motion):
     skel = motion.skeleton
     n_joint = skel.num_joints()
     frm_time = motion.frame_time
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/dump_test.py` & `vaaibody-0.0.0.5/source/vaaibody/dump_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from core.audio import *
-from core.skeleton import *
-from core.motion import MotionDatabase
+from vaaibody.core.audio import *
+from vaaibody.core.skeleton import *
+from vaaibody.core.motion import MotionDatabase
 from module.nontalking_control_module import NonTalkingModule
-from testing.motion_tester import *
-from testing.blending_test_vis import TestWindow
-from testing.convAI_viewer_test import ConvAIWindow
+from vaaibody.testing.motion_tester import *
+from vaaibody.testing.blending_test_vis import TestWindow
+from vaaibody.testing.convAI_viewer_test import ConvAIWindow
 
 """
 여기에 testing 파일을 덤프하여 테스트해본다.
 """
 
 """
 Test 1. diff character test
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/main.py` & `vaaibody-0.0.0.5/source/vaaibody/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import time
 
-from core.audio import AudioDatabase, load_audio_from_wav
-from core.database import (
+from vaaibody.core.audio import AudioDatabase, load_audio_from_wav
+from vaaibody.core.database import (
     AudioFeatureDatabase,
     MotionAudioFeatureDatabase,
     MotionFeatureDatabase,
 )
-from core.gesture_matching import GestureMatching
-from core.motion import MotionDatabase
-from core.skeleton import Skeleton
-from core.frame import Frame
-from utilities.exporter import Exporter
-from utilities.audio_utils import silent_detector
-from utilities.timechecker import TimeChecker
-from viewer.gesture_result_viewer import GestureWindow
+from vaaibody.core.gesture_matching import GestureMatching
+from vaaibody.core.motion import MotionDatabase
+from vaaibody.core.skeleton import Skeleton
+from vaaibody.utilities.exporter import Exporter
+from vaaibody.utilities.audio_utils import silent_detector
+from vaaibody.viewer.gesture_result_viewer import GestureWindow
+import pathlib
+
+file_path = pathlib.Path(__file__).parent.resolve()
+data_path = file_path.parent.parent / "data"
 
 
 def match_gesture(
     bvh_name="/home/yoonhee/Downloads/221123_Body_KSW/Gesture_Before/VAAI_Basic_01_03.bvh",
     bvh_npz_path="data/matching_data/rhythm_motion_npz",
     audio_db_path="data/matching_data/rhythm_audio",
     silent_db_path="data/matching_data/silent_release",
@@ -35,22 +37,22 @@
     step_size = round(round(fps) * 0.5)
     audio_db = AudioDatabase(audio_db_path, fps, from_path=True)
     gdb = MotionAudioFeatureDatabase(
         motion_db,
         audio_db,
         slice=False,
         frame_size=frame_size,
-        db_path="data/matching_data",
+        db_path=data_path / "matching_data",
         db_file_name="wv_feature_no_sliced.pickle",
     )
 
     raw_silent_db = MotionDatabase(skeleton, silent_db_path, is_preload=True)
     silent_db = MotionFeatureDatabase(
         raw_silent_db,
-        db_path="data/matching_data",
+        db_path=data_path / "matching_data",
         db_file_name="wv_silent_release.pickle",
     )
     """
     Gesture matching
     """
     gesture_matching = GestureMatching(gdb, step_size=step_size, silent_db=silent_db)
     test_audio = load_audio_from_wav(test_audio_path, frate=fps)
@@ -64,41 +66,42 @@
     # gesture_matching.match_motion_with_silent(
     #     test_db.mfcc_feature.transpose(),
     #     test_db.beat_feature.transpose(),
     #     search_lower=False,
     #     sil_hint=sil_hint,
     # )
 
-    gesture_matching.test_new_metric(        
+    gesture_matching.test_new_metric(
         test_db.beat_feature.transpose(),
         test_db.mfcc_feature.transpose(),
-        sil_hint=sil_hint)
+        sil_hint=sil_hint,
+    )
 
     # gesture_matching.matching_head(filter="lowpass")
     searched_motion = gesture_matching.convert_frames()
     """
     Export and return results
     """
     timestr = time.strftime("%m%d_%H%M%S")
     # exporter = Exporter("data/matching_data/rhythm_motion/VAAI_Short_01_02.bvh", "data/matching_result/", "matching_result_" + timestr + ".bvh")
     exporter = Exporter(
-        bvh_name, "data/matching_result/", "matching_result_" + timestr + ".bvh"
+        bvh_name,
+        data_path / "matching_result" / str("matching_result_" + timestr + ".bvh"),
     )
     exporter.init_export(len(searched_motion))
     exporter.export_motion(searched_motion, DOF_6=True)
     return skeleton, searched_motion, test_audio, sil_hint
 
 
 if __name__ == "__main__":
     skel, searched_motion, test_audio, sil_hint = match_gesture(
         bvh_name="/home/yoonhee/Downloads/221123_Body_KSW/Gesture_Before/VAAI_Basic_01_01.bvh",
-        bvh_npz_path="data/matching_data/rhythm_motion_npz/",
-        audio_db_path="data/matching_data/rhythm_audio",
-        silent_db_path="data/matching_data/silent_release",
-        test_audio_path="data/audio/Test/TTS_Travel.wav",
+        bvh_npz_path=data_path / "matching_data" / "rhythm_motion_npz",
+        audio_db_path=data_path / "matching_data" / "rhythm_audio",
+        silent_db_path=data_path / "matching_data" / "silent_release",
+        test_audio_path=data_path / "audio" / "Test" / "TTS_Travel.wav",
     )
     print("Audio length: ", test_audio.audio().shape[0] / test_audio.sr())
     visualize = True
     if visualize:
         main_window = GestureWindow(skel, searched_motion, test_audio, sil_hint)
         main_window.loop()
-
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/main_nn.py` & `vaaibody-0.0.0.5/source/vaaibody/main_nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import time
 
 import torch
 
-from core.audio import *
-from core.database import *
-from core.gesture_matching import *
-from core.motion import MotionDatabase
-from core.skeleton import Skeleton
-from utilities.audio_utils import silent_detector
-from utilities.exporter import Exporter
-from viewer.gesture_result_viewer import GestureWindow
+from vaaibody.core.audio import *
+from vaaibody.core.database import *
+from vaaibody.core.gesture_matching import *
+from vaaibody.core.motion import MotionDatabase
+from vaaibody.core.skeleton import Skeleton
+from vaaibody.utilities.audio_utils import silent_detector
+import pathlib
+from vaaibody.utilities.exporter import Exporter
+from vaaibody.viewer.gesture_result_viewer import GestureWindow
+
+file_path = pathlib.Path(__file__).parent.resolve()
+data_path = file_path.parent.parent / "data"
 
 
 def match_gesture(
     bvh_name="data/matching_data/rhythm_motion/VAAI_Short_01_02.bvh",
     bvh_npz_path="data/matching_data/rhythm_motion_npz/",
     audio_db_path="data/matching_data/rhythm_audio",
     silent_db_path="data/matching_data/silent_release",
@@ -35,15 +39,17 @@
         audio_db,
         slice=True,
         frame_size=frame_size,
         db_path="data/matching_data",
         db_file_name="wv_feature_no_aug.pickle",
     )
     raw_silent_db = MotionDatabase(skeleton, silent_db_path, is_preload=True)
-    silent_db = MotionFeatureDatabase(raw_silent_db, db_path="data/matching_data")
+    silent_db = MotionFeatureDatabase(
+        raw_silent_db, db_path=data_path / "matching_data"
+    )
 
     ## NN
     # neural network
     n_features = gdb._pose_feature_size
     n_latent = 64
     latent_feature_db = LatentFeatureDatabase(
         path="latentFeature.pickle", slice=True, frame_size=30
@@ -54,15 +60,14 @@
     decompressor_mean_out = np.load("decompressor_mean_out.npy")
     decompressor_std_out = np.load("decompressor_std_out.npy")
 
     network_decompressor = Decompressor(
         n_features + n_latent, len(decompressor_mean_out)
     )
     network_decompressor.load_state_dict(torch.load("decompressor.pt"))
-
     network_decompressor.eval()
 
     gesture_matching = GestureMatching(
         gdb,
         step_size=step_size,
         silent_db=silent_db,
         latent_db=latent_feature_db,
@@ -92,17 +97,17 @@
     # gesture_matching.matching_head(filter="lowpass")
     searched_motion = gesture_matching.convert_frames()
 
     """
     Export and return results
     """
     timestr = time.strftime("%m%d_%H%M%S")
-    # exporter = Exporter("data/matching_data/rhythm_motion/VAAI_Short_01_02.bvh", "data/matching_result/", "matching_result_" + timestr + ".bvh")
     exporter = Exporter(
-        bvh_name, "data/matching_result/", "matching_result_" + timestr + ".bvh"
+        bvh_name,
+        data_path / "matching_result" / str("matching_result_" + timestr + ".bvh"),
     )
     exporter.init_export(len(searched_motion))
     exporter.export_motion(searched_motion, DOF_6=True)
 
     return skeleton, searched_motion, test_audio, sil_hint
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/module/idle_module.py` & `vaaibody-0.0.0.5/source/vaaibody/module/idle_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import deque
 import pandas as pd
 import random
 
+
 class IdleModule(object):
     def __init__(self, db, idle_file) -> None:
         """
         Idle motion을 초기화
         Current 와 Next를 만들어야 하기 때문에 두 번 만든다.
         """
         self.idle_info = pd.read_csv(idle_file)
@@ -17,30 +18,33 @@
         self.motion_dict_manip = {}
         self.hold_manip = {}
         self.idle_dict = {}
         self.n_idle_played = 0
         for file_name in self.idle_info["File"]:
             current_info = self.idle_info.loc[self.idle_info["File"] == file_name]
             tag = current_info["Tag"].iloc[0]
-            if  tag == "idle":
+            if tag == "idle":
                 idx_idle, motion_idle = db.get_idx_motion_by_name(file_name)
-                idx_st =  int(current_info["Start"].iloc[0])
-                idx_end =  int(current_info["End"].iloc[0])
+                idx_st = int(current_info["Start"].iloc[0])
+                idx_end = int(current_info["End"].iloc[0])
                 idx_end = None if idx_end == -1 else idx_end
                 motion_idle.cut_frame(idx_st, idx_end)
                 self.idx_list_idle.append(idx_idle)
                 self.motion_dict_idle[idx_idle] = motion_idle
                 self.idle_dict[idx_idle] = file_name
-                trans_diff = motion_idle[-1].get_root_transform().translation - motion_idle[0].get_root_transform().translation
-                # print(idx_idle, trans_diff) 
+                trans_diff = (
+                    motion_idle[-1].get_root_transform().translation
+                    - motion_idle[0].get_root_transform().translation
+                )
+                # print(idx_idle, trans_diff)
             elif tag == "manipulator":
                 idx_manip, motion_manip = db.get_idx_motion_by_name(file_name)
                 # mirror_motion(motion_manip)
-                idx_st =  int(current_info["Start"].iloc[0])
-                idx_end =  int(current_info["End"].iloc[0])
+                idx_st = int(current_info["Start"].iloc[0])
+                idx_end = int(current_info["End"].iloc[0])
                 idx_end = None if idx_end == -1 else idx_end
                 motion_manip.cut_frame(idx_st, idx_end)
                 self.idx_list_manip.append(idx_manip)
                 self.hold_manip[idx_manip] = int(current_info["Hold1"].iloc[0])
                 self.motion_dict_manip[idx_manip] = motion_manip
 
         self.variety = 0.3
@@ -57,32 +61,34 @@
         """
         To do: Idle motion 생성 알고리즘 
         1. Idle to Idle
         2. KNN 랜덤 idle 넘어가는거 추가하기 
         3. 스트레칭 등의 랜덤 모션 추가
         """
         if not is_first:
-            num =  random.random()
+            num = random.random()
             if num < self.variety and self.is_idle:
                 self.generate_next_manipulator()
                 return
         if len(self.idx_list_idle) < self.n_idle_played:
             self.idx_list_idle.append(self.idx_used_idle.popleft())
-        idx_selected = random.randint(0, len(self.idx_list_idle) -1)
+        idx_selected = random.randint(0, len(self.idx_list_idle) - 1)
         self.idx_next_motion = self.idx_list_idle.pop(idx_selected)
         self.next_motion = self.motion_dict_idle[self.idx_next_motion]
         self.idx_used_idle.append(self.idx_next_motion)
-        
+
         self.is_idle = True
 
         if is_first:
             self.generate_next_idle_motion()
 
-    def generate_next_manipulator(self, ):
+    def generate_next_manipulator(
+        self,
+    ):
         if len(self.idx_list_manip) < self.n_manip_played:
             self.idx_list_manip.append(self.idx_used_manip.popleft())
-        idx_selected = random.randint(0, len(self.idx_list_manip) -1)
+        idx_selected = random.randint(0, len(self.idx_list_manip) - 1)
         self.idx_next_motion = self.idx_list_manip.pop(idx_selected)
         self.next_motion = self.motion_dict_manip[self.idx_next_motion]
         self.frm_hold = self.hold_manip[self.idx_next_motion]
         self.idx_used_manip.append(self.idx_next_motion)
-        self.is_idle = False
+        self.is_idle = False
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/module/nontalking_control_module.py` & `vaaibody-0.0.0.5/source/vaaibody/module/nontalking_control_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         )
         self.idle_module = IdleModule(db, idle_file)
         self.transition_module = TransitionModule(db.get_frame_time())
         self.tag_processing_module = TagProcessingModule(
             db, phase_file, self.pose_feature, self.feature_db
         )
         self.pose_feature.update_look_ahead(self.future_look_ahead)
-        history = NonTalkingHistoryFeature(look_behind=[0,5,10,15,20,25])
+        history = NonTalkingHistoryFeature(look_behind=[0, 5, 10, 15, 20, 25])
 
         """
         Init parameters
         """
         self.translation_offset = np.zeros(3)
         self.play_state_list = ["play", "transition", "loop"]
         self.motion_state_list = ["normal_tag", "duration_tag", "idle"]
@@ -208,29 +208,33 @@
         current_motion_feature = (
             self.pose_feature.compute_single_frame_feature_from_frame(motion_future)
         )
         target_motion_feature = self.feature_db._gesture_feature_DB[idx_next_motion][0][
             0
         ]
         self.len_motion = len(target_motion)
-        idx_find_range = self.len_motion // 3 if self.idle_module.is_idle else self.idle_module.frm_hold
+        idx_find_range = (
+            self.len_motion // 3
+            if self.idle_module.is_idle
+            else self.idle_module.frm_hold
+        )
 
         idx_target_motion_cut, _ = find_single_cut_idx(
             current_motion_feature=current_motion_feature,
             target_motion_feature=target_motion_feature,
-            idx_feat_end= idx_find_range
+            idx_feat_end=idx_find_range,
         )
 
         self.transition_module.init_motion_transition(
             front_first_frame=self.past_pose,
             front_second_frame=current_frame,
             target_motion=target_motion,
             idx_target_motion_cut=idx_target_motion_cut,
             blend_dur=self.idle_transition_duration,
-            is_moving= False,
+            is_moving=False,
         )
         self.current_motion = target_motion
         self.translation_offset = self.transition_module.root_blender.transl_offset
         self.current_play_state = "transition"
         self.current_motion_state = "idle"
         self.idx_current = idx_target_motion_cut
         self.idle_module.generate_next_idle_motion()
@@ -241,15 +245,15 @@
             motion_future.append(self.get_pseudo_future(idx_future))
 
         searched_info = self.tag_processing_module.search_tagged_motion(
             motion_future,
             motion_tag="Untagged",
             start_feature="Retract",
             end_feature="End",
-            blend_duration= self.retract_transition_duration
+            blend_duration=self.retract_transition_duration,
         )
         processed_tag_info = self.tag_processing_module.process_matching_profile(
             *searched_info,
             blend_duration=self.retract_transition_duration,
             duration_tag=-1
         )
         target_motion = processed_tag_info[0]
@@ -283,15 +287,15 @@
         self.transition_module.init_motion_transition(
             front_first_frame=self.current_motion[loop_end - 1],
             front_second_frame=self.current_motion[loop_end],
             target_motion=self.current_motion,
             idx_target_motion_cut=loop_start,
             blend_dur=blend_dur,
             is_moving=False,
-            is_loop = True
+            is_loop=True,
         )
 
     def get_loop_motion(
         self,
     ):
         loop_cnt = self.idx_current - self.tag_processing_module.idx_retract_start
         if (
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/module/tag_processing_module.py` & `vaaibody-0.0.0.5/source/vaaibody/module/tag_processing_module.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/module/transition_module.py` & `vaaibody-0.0.0.5/source/vaaibody/module/transition_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self,
         front_first_frame: Frame,
         front_second_frame: Frame,
         target_motion: Motion,
         idx_target_motion_cut: int,
         blend_dur: int,
         is_moving: bool = False,
-        is_loop:bool = False
+        is_loop: bool = False,
     ):
         """
         Motion Transition을 Inertialization을 이용하여 초기화함
         Args
             front_first_frame: 지금 모션의 직전 frame, root가 보정되어 있어야 한다.
             front_second_frame: 지금 모션의 지금 frame, root가 보정되어 있어야 한다.
             blend_dur: duration
@@ -52,24 +52,24 @@
             vel_reducer=vel_reducer,
         )
         if is_loop:
             self.root_blender = RootBlender(
                 front_second_frame,
                 target_motion[idx_target_motion_cut],
                 blend_dur,
-                is_moving
+                is_moving,
             )
         else:
             self.root_blender = RootInertialization(
                 front_second_frame,
                 front_first_frame,
                 back_target_frame,
                 blend_dur,
                 is_moving,
-                self.frame_time
+                self.frame_time,
             )
         self.moving_blend_flag = is_moving
         self.blend_dur = blend_dur
         self.blending_cnt = 0
 
     def reset_transition_info(
         self,
@@ -83,15 +83,15 @@
         """
         self.blender = None
         self.moving_blend_flag = False
         self.blending_cnt = 0
 
     def get_transition_frame(self, current_pose):
         self.blender.apply_frame_blending(current_pose, self.blending_cnt)
-        self.root_blender.root_blending(current_pose,self.blending_cnt)
+        self.root_blender.root_blending(current_pose, self.blending_cnt)
         self.blending_cnt += 1
 
         return current_pose, self.blending_cnt >= self.blend_dur
 
     def get_loop_frame(self, current_pose):
         self.blender.apply_frame_blending(current_pose, self.blending_cnt)
         self.root_blender.root_loop_blending(current_pose, self.blending_cnt)
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/parameter/gesture_matching_parameter.py` & `vaaibody-0.0.0.5/source/vaaibody/parameter/gesture_matching_parameter.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/audio_motion_synch.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/audio_motion_synch.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/audio_utils.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/audio_utils.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/blending_utils.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/blending_utils.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/exporter.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/exporter.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/filter.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/filter.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/frame_utils.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/frame_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from scipy.spatial.transform import Rotation as R
 from core.skeleton import Transform
 from core.motion import Motion
 
 # def spin_180(rotation:R):
 #     mirror_rot = np.array([[-1,-1,1],[1,1,-1],[1,1,-1]])
 #     return mirror_rot * rotation.as_matrix()
-    
+
+
 def shift_root(frame, translation_offset):
     root_ori = frame.get_root_transform().rotation
     transl = frame.get_root_transform().translation + translation_offset
     new_root = Transform(root_ori, transl)
     frame.set_root_transform(new_root)
     return frame
 
@@ -219,14 +220,15 @@
                 vel = dev / frm_time
             else:
                 vel = dev / (2 * frm_time)
             i_vel[3 * joint_idx : 3 * (joint_idx + 1)] = vel
         pose_vel.append(i_vel)
     return np.array(pose_vel, dtype="f")
 
+
 def plot_position_vel(motion):
     plt.close("all")
     vel = get_position_vel(motion).transpose()
     j_dict = motion.skeleton.joint_dict
     dt = motion.frame_time
     t = np.arange(0, motion.num_frame())
     # t = np.arange(0, motion.num_frame()) * dt
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/motion_var_utils.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/motion_var_utils.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/quat.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/quat.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/rendering_utils.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/rendering_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from re import L
 
 import numpy as np
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from viewer.obj_loader import HEAD_OBJ, HEAD_OBJ_SIZE, HEAD_BOX
+from vaaibody.viewer.obj_loader import HEAD_OBJ, HEAD_OBJ_SIZE, HEAD_BOX
 
 import math
 import numpy as np
 
 quad_obj = gluNewQuadric()
 
 
@@ -84,15 +84,17 @@
                     current_frame.get_global_transform(idx).translation + end_trans / 2
                 )
                 # glColor3f(1.0, 0, 0)
                 x_axis = np.matmul(
                     current_frame.get_global_transform(idx).rotation_np,
                     np.array([0, 0, 0.1]),
                 )
-                euler = current_frame.get_global_transform(idx).rotation.as_euler("ZXY", degrees = True)
+                euler = current_frame.get_global_transform(idx).rotation.as_euler(
+                    "ZXY", degrees=True
+                )
                 # draw_arrow(head, head + x_axis, 0.01)
                 draw_head(head, euler)
 
     else:
         for idx, j in enumerate(skel.joints):
             body_pose = current_frame.get_body_global_transform(idx)
             # body_pose = current_frame.get_global_transform(idx) * skel.joints[idx].body_transform
@@ -157,18 +159,17 @@
 
     glColor4f(0.7, 0.2, 0.2, 0.25)
     # scene_trans +
     glPushMatrix()
     glScalef(*scene_scale)
     glTranslatef(*scene_trans)
     glTranslatef(*scene_trans_offset)
-    glRotatef(euler[0],0,0, 1)    
-    glRotatef(euler[1],1,0,0)
-    glRotatef(euler[2],0,1, 0)
-
+    glRotatef(euler[0], 0, 0, 1)
+    glRotatef(euler[1], 1, 0, 0)
+    glRotatef(euler[2], 0, 1, 0)
 
     glRotatef(-90, 0, 1, 0)
     glRotatef(180, 1, 0, 0)
     glRotatef(10, 0, 0, 1)
 
     for mesh in HEAD_OBJ.mesh_list:
         glBegin(GL_TRIANGLES)
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/timechecker.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/timechecker.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/txform.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/txform.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/utilities/utils.py` & `vaaibody-0.0.0.5/source/vaaibody/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/camera.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/camera.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/controller.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from viewer.camera import FreeCamera, TargetCamera
+from vaaibody.viewer.camera import FreeCamera, TargetCamera
 
 
 class Controller:
     def __init__(self, owner):
         self._param_class = None
         self._owner = owner
         self._name = "Controller"
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/double_bvh_viewer.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/double_bvh_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import imgui, glfw
-from core.skeleton import *
-from core.frame import Frame
-from core.database import MotionDatabase
+from vaaibody.core.skeleton import *
+from vaaibody.core.frame import Frame
+from vaaibody.core.database import MotionDatabase
 import natsort
-from viewer.gui_viewer import MainWindow
-from viewer.item_drawer import *
+from vaaibody.viewer.gui_viewer import MainWindow
+from vaaibody.viewer.item_drawer import *
 
 
 class DoubleViewer(MainWindow):
     def __init__(
         self,
         skeleton_main: Skeleton,
         db_main: MotionDatabase,
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/gesture_result_viewer.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/gesture_result_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 
 import glfw
 import imgui
 import numpy as np
 import simpleaudio as sa
-from core.modAudio import *
+from vaaibody.core.modAudio import *
 from scipy.spatial.transform import Rotation as R
-from utilities.frame_utils import *
+from vaaibody.utilities.frame_utils import *
 
-from viewer.gui_viewer import MainWindow
-from viewer.item_drawer import *
+from vaaibody.viewer.gui_viewer import MainWindow
+from vaaibody.viewer.item_drawer import *
 
 
 class GestureWindow(MainWindow):
     def __init__(self, skel, searched_motion, test_audio, sil_hint):
         super().__init__()
         self.set_skeleton(skel)
         self.set_motion(searched_motion)
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/gui_viewer.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/gui_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import time
 
 import glfw
 import imgui
 import numpy as np
-from core.frame import Frame
+from vaaibody.core.frame import Frame
 from imgui.integrations.glfw import GlfwRenderer
 from OpenGL.GL.shaders import *
 from OpenGL.GLU import *
 
-from viewer.controller import Controller
-from viewer.handler import *
-from viewer.item_drawer import *
+import pathlib
+from vaaibody.viewer.controller import Controller
+from vaaibody.viewer.handler import *
+from vaaibody.viewer.item_drawer import *
+
+data_path = pathlib.Path(__file__).parent.resolve().parent.parent.parent / "data"
 
 
 class MainWindow(
     KeyEventHandler,
     MouseButtonEventHandler,
     ScrollEventHandler,
     CursorPosEventHandler,
@@ -57,18 +60,18 @@
 
         glfw.set_key_callback(self._window, self.event_key)
         glfw.set_mouse_button_callback(self._window, self.event_mouse_button)
         glfw.set_scroll_callback(self._window, self.event_scroll)
         glfw.set_cursor_pos_callback(self._window, self.event_cursor_pos)
         glfw.set_window_size_callback(self._window, self.event_window_size)
 
-        file = open("data/shader/shader_vert.txt")
+        file = open(data_path / "shader" / "shader_vert.txt")
         vertex_shader_src = file.read()
         file.close()
-        file = open("data/shader/shader_frag.txt")
+        file = open(data_path / "shader" / "shader_frag.txt")
         frag_shader_src = file.read()
         file.close()
 
         self._shader = glCreateProgram()
         vertex_shader = compileShader(vertex_shader_src, GL_VERTEX_SHADER)
         frag_shader = compileShader(frag_shader_src, GL_FRAGMENT_SHADER)
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/handler.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/handler.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/item_data.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/item_data.py`

 * *Files identical despite different names*

### Comparing `vaaibody-0.0.0.4/source/vaaibody/viewer/item_drawer.py` & `vaaibody-0.0.0.5/source/vaaibody/viewer/item_drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from builtins import *
 from copy import deepcopy
 
 import numpy as np
-import utilities.rendering_utils as ru
+import vaaibody.utilities.rendering_utils as ru
 from OpenGL.GL import *
 from OpenGL.GL.shaders import *
 from OpenGL.GLU import *
 
-from viewer.item_data import *
+from vaaibody.viewer.item_data import *
 
 
 class ItemDrawer:
     def handling_class(self) -> object:
         """return handling class of this drawer"""
         pass
```

### Comparing `vaaibody-0.0.0.4/source/vaaibody.egg-info/SOURCES.txt` & `vaaibody-0.0.0.5/source/vaaibody.egg-info/SOURCES.txt`

 * *Files identical despite different names*

