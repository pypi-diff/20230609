# Comparing `tmp/zhousf-lib-0.6.3.tar.gz` & `tmp/zhousf-lib-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.6.3.tar", last modified: Fri Jun  9 06:16:14 2023, max compression
+gzip compressed data, was "zhousf-lib-0.6.5.tar", last modified: Fri Jun  9 06:16:51 2023, max compression
```

## Comparing `zhousf-lib-0.6.3.tar` & `zhousf-lib-0.6.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.273000 zhousf-lib-0.6.3/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.6.3/LICENSE
--rw-rw-rw-   0        0        0      930 2023-06-09 06:16:14.273000 zhousf-lib-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 06:16:14.273974 zhousf-lib-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-06-09 06:14:27.000000 zhousf-lib-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.195992 zhousf-lib-0.6.3/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0      930 2023-06-09 06:16:14.000000 zhousf-lib-0.6.3/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-06-09 06:16:14.000000 zhousf-lib-0.6.3/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:16:14.000000 zhousf-lib-0.6.3/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 06:16:14.000000 zhousf-lib-0.6.3/zhousf_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 06:16:14.000000 zhousf-lib-0.6.3/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.197972 zhousf-lib-0.6.3/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.198972 zhousf-lib-0.6.3/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.6.3/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.200972 zhousf-lib-0.6.3/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     2937 2023-06-09 06:13:45.000000 zhousf-lib-0.6.3/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.206972 zhousf-lib-0.6.3/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5464 2023-06-07 07:56:06.000000 zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.212972 zhousf-lib-0.6.3/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.214972 zhousf-lib-0.6.3/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.6.3/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.216973 zhousf-lib-0.6.3/zhousflib/db/
--rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.6.3/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.6.3/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.219971 zhousf-lib-0.6.3/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.3/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.235002 zhousf-lib-0.6.3/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.6.3/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.6.3/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.6.3/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.236977 zhousf-lib-0.6.3/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1560 2023-06-08 02:34:30.000000 zhousf-lib-0.6.3/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.239007 zhousf-lib-0.6.3/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4611 2023-06-07 01:49:11.000000 zhousf-lib-0.6.3/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.241973 zhousf-lib-0.6.3/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.6.3/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.266972 zhousf-lib-0.6.3/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0      466 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/util/except_util.py
--rw-rw-rw-   0        0        0     1336 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0     1091 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/interceptor_util.py
--rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0      472 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.6.3/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4242 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.6.3/zhousflib/util/time_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:16:14.271973 zhousf-lib-0.6.3/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.6.3/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.6.3/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.376722 zhousf-lib-0.6.5/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0      930 2023-06-09 06:16:51.376722 zhousf-lib-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:16:51.377721 zhousf-lib-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-06-09 06:16:46.000000 zhousf-lib-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.300749 zhousf-lib-0.6.5/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-06-09 06:16:51.000000 zhousf-lib-0.6.5/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-06-09 06:16:51.000000 zhousf-lib-0.6.5/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:16:51.000000 zhousf-lib-0.6.5/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 06:16:51.000000 zhousf-lib-0.6.5/zhousf_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 06:16:51.000000 zhousf-lib-0.6.5/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.301734 zhousf-lib-0.6.5/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.302746 zhousf-lib-0.6.5/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.6.5/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.303722 zhousf-lib-0.6.5/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     2937 2023-06-09 06:13:45.000000 zhousf-lib-0.6.5/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.311752 zhousf-lib-0.6.5/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5464 2023-06-07 07:56:06.000000 zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.319723 zhousf-lib-0.6.5/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.321721 zhousf-lib-0.6.5/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.6.5/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.325748 zhousf-lib-0.6.5/zhousflib/db/
+-rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.6.5/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.6.5/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.327747 zhousf-lib-0.6.5/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.5/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.342751 zhousf-lib-0.6.5/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.6.5/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.6.5/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.6.5/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.344760 zhousf-lib-0.6.5/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1560 2023-06-08 02:34:30.000000 zhousf-lib-0.6.5/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.346750 zhousf-lib-0.6.5/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4611 2023-06-07 01:49:11.000000 zhousf-lib-0.6.5/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.349752 zhousf-lib-0.6.5/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.6.5/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.370721 zhousf-lib-0.6.5/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0      466 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/util/except_util.py
+-rw-rw-rw-   0        0        0     1336 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0     1091 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/interceptor_util.py
+-rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0      472 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.6.5/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4242 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.6.5/zhousflib/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:16:51.375722 zhousf-lib-0.6.5/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.6.5/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.6.5/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.6.3/LICENSE` & `zhousf-lib-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/PKG-INFO` & `zhousf-lib-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.6.3
+Version: 0.6.5
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.6.3/setup.py` & `zhousf-lib-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.6.3'
+VERSION = '0.6.5'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.6.3/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.6.5/zhousf_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.6.3
+Version: 0.6.5
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.6.3/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.6.5/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-0.6.5/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.6.5/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.6.5/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.6.5/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.6.5/zhousflib/db/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.6.5/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.6.5/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.6.5/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/font/__init__.py` & `zhousf-lib-0.6.5/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.6.5/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.6.5/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/pdf/export_image.py` & `zhousf-lib-0.6.5/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.6.5/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/calculater_util.py` & `zhousf-lib-0.6.5/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/cv_util.py` & `zhousf-lib-0.6.5/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.6.5/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/img_util.py` & `zhousf-lib-0.6.5/zhousflib/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/interceptor_util.py` & `zhousf-lib-0.6.5/zhousflib/util/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/iou_util.py` & `zhousf-lib-0.6.5/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/json_util.py` & `zhousf-lib-0.6.5/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/permission_util.py` & `zhousf-lib-0.6.5/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/poly_util.py` & `zhousf-lib-0.6.5/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/re_util.py` & `zhousf-lib-0.6.5/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/singleton.py` & `zhousf-lib-0.6.5/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/string_util.py` & `zhousf-lib-0.6.5/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/util/time_util.py` & `zhousf-lib-0.6.5/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/web/config.py` & `zhousf-lib-0.6.5/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/web/log_util.py` & `zhousf-lib-0.6.5/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/web/logger.py` & `zhousf-lib-0.6.5/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.3/zhousflib/web/response.py` & `zhousf-lib-0.6.5/zhousflib/web/response.py`

 * *Files identical despite different names*

