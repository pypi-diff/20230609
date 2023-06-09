# Comparing `tmp/pancollection-0.2a0.tar.gz` & `tmp/pancollection-0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pancollection-0.2a0.tar", last modified: Fri Jun  9 06:06:42 2023, max compression
+gzip compressed data, was "dist\pancollection-0.2b0.tar", last modified: Fri Jun  9 06:53:33 2023, max compression
```

## Comparing `pancollection-0.2a0.tar` & `pancollection-0.2b0.tar`

### file list

```diff
@@ -1,108 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/
--rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 pancollection-0.2a0/LICENSE
--rw-rw-rw-   0        0        0     5824 2023-06-09 06:06:42.000000 pancollection-0.2a0/PKG-INFO
--rw-rw-rw-   0        0        0     5293 2023-06-07 04:18:18.000000 pancollection-0.2a0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/
--rw-rw-rw-   0        0        0      229 2023-06-06 18:32:01.000000 pancollection-0.2a0/pancollection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/common/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/common/__init__.py
--rw-rw-rw-   0        0        0      697 2023-06-09 05:15:41.000000 pancollection-0.2a0/pancollection/common/builder.py
--rw-rw-rw-   0        0        0    14450 2023-06-09 05:14:41.000000 pancollection-0.2a0/pancollection/common/dataset.py
--rw-rw-rw-   0        0        0     2238 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/common/dataset_hp.py
--rw-rw-rw-   0        0        0    16414 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/common/evaluate.py
--rw-rw-rw-   0        0        0     7163 2023-06-06 18:38:21.000000 pancollection-0.2a0/pancollection/common/psdata.py
--rw-rw-rw-   0        0        0     4847 2023-03-30 10:19:53.000000 pancollection-0.2a0/pancollection/common/test_panloader.py
--rw-rw-rw-   0        0        0     3965 2023-06-06 18:38:37.000000 pancollection-0.2a0/pancollection/common/train_panloader.py
--rw-rw-rw-   0        0        0     3958 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/common/valid_panloader.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/configs/
--rw-rw-rw-   0        0        0      336 2023-06-06 18:33:33.000000 pancollection-0.2a0/pancollection/configs/__init__.py
--rw-rw-rw-   0        0        0     1151 2023-06-09 05:08:57.000000 pancollection-0.2a0/pancollection/configs/configs.py
--rw-rw-rw-   0        0        0      824 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/configs/hook_configs.py
--rw-rw-rw-   0        0        0     3078 2023-06-06 18:51:23.000000 pancollection-0.2a0/pancollection/configs/option_DCFNet.py
--rw-rw-rw-   0        0        0     2927 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_LAGNet.py
--rw-rw-rw-   0        0        0     2896 2023-06-06 18:51:14.000000 pancollection-0.2a0/pancollection/configs/option_bdpn.py
--rw-rw-rw-   0        0        0     2811 2023-06-06 18:51:32.000000 pancollection-0.2a0/pancollection/configs/option_dicnn.py
--rw-rw-rw-   0        0        0     2878 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_drpnn.py
--rw-rw-rw-   0        0        0     3220 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_fusionnet.py
--rw-rw-rw-   0        0        0     2921 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_msdcnn.py
--rw-rw-rw-   0        0        0     3087 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_pannet.py
--rw-rw-rw-   0        0        0     2865 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_pnn.py
--rw-rw-rw-   0        0        0      703 2023-06-09 05:02:24.000000 pancollection-0.2a0/pancollection/hug_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/ADKNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:55:31.000000 pancollection-0.2a0/pancollection/models/ADKNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/
--rw-rw-rw-   0        0        0       18 2023-03-22 11:48:22.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/__init__.py
--rw-rw-rw-   0        0        0    11638 2023-03-22 11:48:22.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/ddf.py
--rw-rw-rw-   0        0        0     2289 2023-03-22 11:48:22.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/BDPN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/BDPN/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-06-06 18:36:55.000000 pancollection-0.2a0/pancollection/models/BDPN/bdpn_main.py
--rw-rw-rw-   0        0        0     7813 2023-06-09 05:15:23.000000 pancollection-0.2a0/pancollection/models/BDPN/model_bdpn.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DCFNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DCFNet/__init__.py
--rw-rw-rw-   0        0        0    32420 2023-06-09 05:14:16.000000 pancollection-0.2a0/pancollection/models/DCFNet/model_fcc_dense_head.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DHIFNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DHIFNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DRPNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DRPNN/__init__.py
--rw-rw-rw-   0        0        0     3849 2023-06-06 18:36:22.000000 pancollection-0.2a0/pancollection/models/DRPNN/drpnn_main.py
--rw-rw-rw-   0        0        0     5302 2023-06-09 05:15:15.000000 pancollection-0.2a0/pancollection/models/DRPNN/model_drpnn.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DiCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DiCNN/__init__.py
--rw-rw-rw-   0        0        0     3840 2023-06-06 18:35:36.000000 pancollection-0.2a0/pancollection/models/DiCNN/dicnn_main.py
--rw-rw-rw-   0        0        0     3768 2023-06-09 05:14:16.000000 pancollection-0.2a0/pancollection/models/DiCNN/model_dicnn.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/FusionNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/FusionNet/__init__.py
--rw-rw-rw-   0        0        0     3501 2023-06-06 18:35:47.000000 pancollection-0.2a0/pancollection/models/FusionNet/fusionnet_main.py
--rw-rw-rw-   0        0        0     5615 2023-06-09 05:14:50.000000 pancollection-0.2a0/pancollection/models/FusionNet/model_fusionnet.py
--rw-rw-rw-   0        0        0      518 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/FusionNet/run_fusionnet.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/GPPNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/GPPNN/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/GPPNN/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/GPPNN/models/
--rw-rw-rw-   0        0        0     4902 2023-06-09 06:05:48.000000 pancollection-0.2a0/pancollection/models/GPPNN/models/GPPNN.py
--rw-rw-rw-   0        0        0      686 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/GPPNN/models/__init__.py
--rw-rw-rw-   0        0        0    38742 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/GPPNN/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/LAGConv/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/LAGConv/__init__.py
--rw-rw-rw-   0        0        0     2254 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/LAGConv/data.py
--rw-rw-rw-   0        0        0     6962 2023-06-09 06:05:48.000000 pancollection-0.2a0/pancollection/models/LAGConv/model.py
--rw-rw-rw-   0        0        0     1990 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/LAGConv/test.py
--rw-rw-rw-   0        0        0     7423 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/LAGConv/train.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/MSDCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/MSDCNN/__init__.py
--rw-rw-rw-   0        0        0     5864 2023-06-09 06:05:48.000000 pancollection-0.2a0/pancollection/models/MSDCNN/model_msdcnn.py
--rw-rw-rw-   0        0        0     3845 2023-06-06 18:37:05.000000 pancollection-0.2a0/pancollection/models/MSDCNN/msdcnn_main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/MUCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/MUCNN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/
--rw-rw-rw-   0        0        0       81 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/__init__.py
--rw-rw-rw-   0        0        0      940 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/data.py
--rw-rw-rw-   0        0        0     3897 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/datasets.py
--rw-rw-rw-   0        0        0     5410 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/evaluate.py
--rw-rw-rw-   0        0        0     3027 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/model.py
--rw-rw-rw-   0        0        0     1328 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/utils.py
--rw-rw-rw-   0        0        0     3395 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/MUCNN/main_test_multi.py
--rw-rw-rw-   0        0        0     2670 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/MUCNN/main_test_single.py
--rw-rw-rw-   0        0        0     8936 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/MUCNN/train.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/PNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/PNN/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-06-09 05:14:58.000000 pancollection-0.2a0/pancollection/models/PNN/model_pnn.py
--rw-rw-rw-   0        0        0     4390 2023-06-06 18:35:57.000000 pancollection-0.2a0/pancollection/models/PNN/pnn_main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/PanNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/PanNet/__init__.py
--rw-rw-rw-   0        0        0     4917 2023-06-09 05:15:07.000000 pancollection-0.2a0/pancollection/models/PanNet/model_pannet.py
--rw-rw-rw-   0        0        0     3813 2023-06-06 18:36:06.000000 pancollection-0.2a0/pancollection/models/PanNet/pannet_main.py
--rw-rw-rw-   0        0        0      508 2023-06-09 05:14:16.000000 pancollection-0.2a0/pancollection/models/__init__.py
--rw-rw-rw-   0        0        0     3123 2023-06-09 05:14:26.000000 pancollection-0.2a0/pancollection/models/base_model.py
--rw-rw-rw-   0        0        0      550 2023-06-09 05:08:57.000000 pancollection-0.2a0/pancollection/run_pansharpening.py
--rw-rw-rw-   0        0        0      528 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/run_test_pansharpening.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/
--rw-rw-rw-   0        0        0     5824 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3195 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 06:06:42.000000 pancollection-0.2a0/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-06-09 06:06:19.000000 pancollection-0.2a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/
+-rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 pancollection-0.2b0/LICENSE
+-rw-rw-rw-   0        0        0     5824 2023-06-09 06:53:33.000000 pancollection-0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     5293 2023-06-07 04:18:18.000000 pancollection-0.2b0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/
+-rw-rw-rw-   0        0        0      229 2023-06-06 18:32:01.000000 pancollection-0.2b0/pancollection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/common/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/common/FS_index/
+-rw-rw-rw-   0        0        0     2364 2022-11-23 12:43:13.000000 pancollection-0.2b0/pancollection/common/FS_index/D_lambda_K.py
+-rw-rw-rw-   0        0        0     2392 2022-11-22 05:24:39.000000 pancollection-0.2b0/pancollection/common/FS_index/HQNR.py
+-rw-rw-rw-   0        0        0     2213 2023-03-27 15:42:39.000000 pancollection-0.2b0/pancollection/common/FS_index/MTF.py
+-rw-rw-rw-   0        0        0     2224 2023-03-27 15:50:01.000000 pancollection-0.2b0/pancollection/common/FS_index/MTF_pan.py
+-rw-rw-rw-   0        0        0      146 2023-06-09 06:53:23.000000 pancollection-0.2b0/pancollection/common/FS_index/__init__.py
+-rw-rw-rw-   0        0        0     2593 2022-11-21 08:49:04.000000 pancollection-0.2b0/pancollection/common/FS_index/genMTF.py
+-rw-rw-rw-   0        0        0      730 2023-03-27 15:48:45.000000 pancollection-0.2b0/pancollection/common/FS_index/genMTF_pan.py
+-rw-rw-rw-   0        0        0     5365 2020-06-04 11:13:21.000000 pancollection-0.2b0/pancollection/common/FS_index/imresize.py
+-rw-rw-rw-   0        0        0     9088 2022-11-21 16:19:17.000000 pancollection-0.2b0/pancollection/common/FS_index/indexes_evaluation_FS.py
+-rw-rw-rw-   0        0        0     3106 2021-11-30 08:46:49.000000 pancollection-0.2b0/pancollection/common/FS_index/interp23.py
+-rw-rw-rw-   0        0        0     6395 2022-11-23 12:43:13.000000 pancollection-0.2b0/pancollection/common/FS_index/my_D_s.py
+-rw-rw-rw-   0        0        0     8378 2022-11-21 12:22:10.000000 pancollection-0.2b0/pancollection/common/FS_index/my_q2n.py
+-rw-rw-rw-   0        0        0     1237 2020-06-04 13:59:20.000000 pancollection-0.2b0/pancollection/common/FS_index/tools.py
+-rw-rw-rw-   0        0        0       22 2023-06-09 06:43:23.000000 pancollection-0.2b0/pancollection/common/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-06-09 05:15:41.000000 pancollection-0.2b0/pancollection/common/builder.py
+-rw-rw-rw-   0        0        0    14450 2023-06-09 05:14:41.000000 pancollection-0.2b0/pancollection/common/dataset.py
+-rw-rw-rw-   0        0        0     2238 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/common/dataset_hp.py
+-rw-rw-rw-   0        0        0    16414 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/common/evaluate.py
+-rw-rw-rw-   0        0        0     7163 2023-06-06 18:38:21.000000 pancollection-0.2b0/pancollection/common/psdata.py
+-rw-rw-rw-   0        0        0     4847 2023-03-30 10:19:53.000000 pancollection-0.2b0/pancollection/common/test_panloader.py
+-rw-rw-rw-   0        0        0     3965 2023-06-06 18:38:37.000000 pancollection-0.2b0/pancollection/common/train_panloader.py
+-rw-rw-rw-   0        0        0     3958 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/common/valid_panloader.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/configs/
+-rw-rw-rw-   0        0        0      336 2023-06-06 18:33:33.000000 pancollection-0.2b0/pancollection/configs/__init__.py
+-rw-rw-rw-   0        0        0     1151 2023-06-09 05:08:57.000000 pancollection-0.2b0/pancollection/configs/configs.py
+-rw-rw-rw-   0        0        0      824 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/configs/hook_configs.py
+-rw-rw-rw-   0        0        0     3078 2023-06-06 18:51:23.000000 pancollection-0.2b0/pancollection/configs/option_DCFNet.py
+-rw-rw-rw-   0        0        0     2927 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_LAGNet.py
+-rw-rw-rw-   0        0        0     2896 2023-06-06 18:51:14.000000 pancollection-0.2b0/pancollection/configs/option_bdpn.py
+-rw-rw-rw-   0        0        0     2811 2023-06-06 18:51:32.000000 pancollection-0.2b0/pancollection/configs/option_dicnn.py
+-rw-rw-rw-   0        0        0     2878 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_drpnn.py
+-rw-rw-rw-   0        0        0     3220 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_fusionnet.py
+-rw-rw-rw-   0        0        0     2921 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_msdcnn.py
+-rw-rw-rw-   0        0        0     3087 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_pannet.py
+-rw-rw-rw-   0        0        0     2865 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_pnn.py
+-rw-rw-rw-   0        0        0      703 2023-06-09 05:02:24.000000 pancollection-0.2b0/pancollection/hug_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/ADKNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:55:31.000000 pancollection-0.2b0/pancollection/models/ADKNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/
+-rw-rw-rw-   0        0        0       18 2023-03-22 11:48:22.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/__init__.py
+-rw-rw-rw-   0        0        0    11638 2023-03-22 11:48:22.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/ddf.py
+-rw-rw-rw-   0        0        0     2289 2023-03-22 11:48:22.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/BDPN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/BDPN/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-06-06 18:36:55.000000 pancollection-0.2b0/pancollection/models/BDPN/bdpn_main.py
+-rw-rw-rw-   0        0        0     7813 2023-06-09 05:15:23.000000 pancollection-0.2b0/pancollection/models/BDPN/model_bdpn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DCFNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DCFNet/__init__.py
+-rw-rw-rw-   0        0        0    32420 2023-06-09 05:14:16.000000 pancollection-0.2b0/pancollection/models/DCFNet/model_fcc_dense_head.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DHIFNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DHIFNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DRPNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DRPNN/__init__.py
+-rw-rw-rw-   0        0        0     3849 2023-06-06 18:36:22.000000 pancollection-0.2b0/pancollection/models/DRPNN/drpnn_main.py
+-rw-rw-rw-   0        0        0     5302 2023-06-09 05:15:15.000000 pancollection-0.2b0/pancollection/models/DRPNN/model_drpnn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DiCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DiCNN/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-06-06 18:35:36.000000 pancollection-0.2b0/pancollection/models/DiCNN/dicnn_main.py
+-rw-rw-rw-   0        0        0     3768 2023-06-09 05:14:16.000000 pancollection-0.2b0/pancollection/models/DiCNN/model_dicnn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/FusionNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/FusionNet/__init__.py
+-rw-rw-rw-   0        0        0     3501 2023-06-06 18:35:47.000000 pancollection-0.2b0/pancollection/models/FusionNet/fusionnet_main.py
+-rw-rw-rw-   0        0        0     5615 2023-06-09 05:14:50.000000 pancollection-0.2b0/pancollection/models/FusionNet/model_fusionnet.py
+-rw-rw-rw-   0        0        0      518 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/FusionNet/run_fusionnet.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/GPPNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/GPPNN/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/GPPNN/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/GPPNN/models/
+-rw-rw-rw-   0        0        0     4902 2023-06-09 06:05:48.000000 pancollection-0.2b0/pancollection/models/GPPNN/models/GPPNN.py
+-rw-rw-rw-   0        0        0      686 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/GPPNN/models/__init__.py
+-rw-rw-rw-   0        0        0    38742 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/GPPNN/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/LAGConv/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/LAGConv/__init__.py
+-rw-rw-rw-   0        0        0     2254 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/LAGConv/data.py
+-rw-rw-rw-   0        0        0     6962 2023-06-09 06:05:48.000000 pancollection-0.2b0/pancollection/models/LAGConv/model.py
+-rw-rw-rw-   0        0        0     1990 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/LAGConv/test.py
+-rw-rw-rw-   0        0        0     7423 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/LAGConv/train.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/MSDCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/MSDCNN/__init__.py
+-rw-rw-rw-   0        0        0     5864 2023-06-09 06:05:48.000000 pancollection-0.2b0/pancollection/models/MSDCNN/model_msdcnn.py
+-rw-rw-rw-   0        0        0     3845 2023-06-06 18:37:05.000000 pancollection-0.2b0/pancollection/models/MSDCNN/msdcnn_main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/MUCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/MUCNN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/
+-rw-rw-rw-   0        0        0       81 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/__init__.py
+-rw-rw-rw-   0        0        0      940 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/data.py
+-rw-rw-rw-   0        0        0     3897 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/datasets.py
+-rw-rw-rw-   0        0        0     5410 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/evaluate.py
+-rw-rw-rw-   0        0        0     3027 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/model.py
+-rw-rw-rw-   0        0        0     1328 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/utils.py
+-rw-rw-rw-   0        0        0     3395 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/MUCNN/main_test_multi.py
+-rw-rw-rw-   0        0        0     2670 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/MUCNN/main_test_single.py
+-rw-rw-rw-   0        0        0     8936 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/MUCNN/train.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/PNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/PNN/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-09 05:14:58.000000 pancollection-0.2b0/pancollection/models/PNN/model_pnn.py
+-rw-rw-rw-   0        0        0     4390 2023-06-06 18:35:57.000000 pancollection-0.2b0/pancollection/models/PNN/pnn_main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/PanNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/PanNet/__init__.py
+-rw-rw-rw-   0        0        0     4917 2023-06-09 05:15:07.000000 pancollection-0.2b0/pancollection/models/PanNet/model_pannet.py
+-rw-rw-rw-   0        0        0     3813 2023-06-06 18:36:06.000000 pancollection-0.2b0/pancollection/models/PanNet/pannet_main.py
+-rw-rw-rw-   0        0        0      508 2023-06-09 05:14:16.000000 pancollection-0.2b0/pancollection/models/__init__.py
+-rw-rw-rw-   0        0        0     3123 2023-06-09 05:14:26.000000 pancollection-0.2b0/pancollection/models/base_model.py
+-rw-rw-rw-   0        0        0      550 2023-06-09 05:08:57.000000 pancollection-0.2b0/pancollection/run_pansharpening.py
+-rw-rw-rw-   0        0        0      528 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/run_test_pansharpening.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/
+-rw-rw-rw-   0        0        0     5824 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3739 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:53:33.000000 pancollection-0.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2023-06-09 06:43:29.000000 pancollection-0.2b0/setup.py
```

### Comparing `pancollection-0.2a0/LICENSE` & `pancollection-0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/PKG-INFO` & `pancollection-0.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.2a0
+Version: 0.2b0
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pancollection-0.2a0/README.md` & `pancollection-0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/builder.py` & `pancollection-0.2b0/pancollection/common/builder.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/dataset.py` & `pancollection-0.2b0/pancollection/common/dataset.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/dataset_hp.py` & `pancollection-0.2b0/pancollection/common/dataset_hp.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/evaluate.py` & `pancollection-0.2b0/pancollection/common/evaluate.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/psdata.py` & `pancollection-0.2b0/pancollection/common/psdata.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/test_panloader.py` & `pancollection-0.2b0/pancollection/common/test_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/train_panloader.py` & `pancollection-0.2b0/pancollection/common/train_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/common/valid_panloader.py` & `pancollection-0.2b0/pancollection/common/valid_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/configs.py` & `pancollection-0.2b0/pancollection/configs/configs.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/hook_configs.py` & `pancollection-0.2b0/pancollection/configs/hook_configs.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_DCFNet.py` & `pancollection-0.2b0/pancollection/configs/option_DCFNet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_LAGNet.py` & `pancollection-0.2b0/pancollection/configs/option_LAGNet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_bdpn.py` & `pancollection-0.2b0/pancollection/configs/option_bdpn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_dicnn.py` & `pancollection-0.2b0/pancollection/configs/option_dicnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_drpnn.py` & `pancollection-0.2b0/pancollection/configs/option_drpnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_fusionnet.py` & `pancollection-0.2b0/pancollection/configs/option_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_msdcnn.py` & `pancollection-0.2b0/pancollection/configs/option_msdcnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_pannet.py` & `pancollection-0.2b0/pancollection/configs/option_pannet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/configs/option_pnn.py` & `pancollection-0.2b0/pancollection/configs/option_pnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/hug_demo.py` & `pancollection-0.2b0/pancollection/hug_demo.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/ADKNet/ddf/ddf.py` & `pancollection-0.2b0/pancollection/models/ADKNet/ddf/ddf.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/ADKNet/ddf/setup.py` & `pancollection-0.2b0/pancollection/models/ADKNet/ddf/setup.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/BDPN/bdpn_main.py` & `pancollection-0.2b0/pancollection/models/BDPN/bdpn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/BDPN/model_bdpn.py` & `pancollection-0.2b0/pancollection/models/BDPN/model_bdpn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/DCFNet/model_fcc_dense_head.py` & `pancollection-0.2b0/pancollection/models/DCFNet/model_fcc_dense_head.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/DRPNN/drpnn_main.py` & `pancollection-0.2b0/pancollection/models/DRPNN/drpnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/DRPNN/model_drpnn.py` & `pancollection-0.2b0/pancollection/models/DRPNN/model_drpnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/DiCNN/dicnn_main.py` & `pancollection-0.2b0/pancollection/models/DiCNN/dicnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/DiCNN/model_dicnn.py` & `pancollection-0.2b0/pancollection/models/DiCNN/model_dicnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/FusionNet/fusionnet_main.py` & `pancollection-0.2b0/pancollection/models/FusionNet/fusionnet_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/FusionNet/model_fusionnet.py` & `pancollection-0.2b0/pancollection/models/FusionNet/model_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/FusionNet/run_fusionnet.py` & `pancollection-0.2b0/pancollection/models/FusionNet/run_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/GPPNN/metrics.py` & `pancollection-0.2b0/pancollection/models/GPPNN/metrics.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/GPPNN/models/GPPNN.py` & `pancollection-0.2b0/pancollection/models/GPPNN/models/GPPNN.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/GPPNN/models/__init__.py` & `pancollection-0.2b0/pancollection/models/GPPNN/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/GPPNN/utils.py` & `pancollection-0.2b0/pancollection/models/GPPNN/utils.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/LAGConv/data.py` & `pancollection-0.2b0/pancollection/models/LAGConv/data.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/LAGConv/model.py` & `pancollection-0.2b0/pancollection/models/LAGConv/model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/LAGConv/test.py` & `pancollection-0.2b0/pancollection/models/LAGConv/test.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/LAGConv/train.py` & `pancollection-0.2b0/pancollection/models/LAGConv/train.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MSDCNN/model_msdcnn.py` & `pancollection-0.2b0/pancollection/models/MSDCNN/model_msdcnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MSDCNN/msdcnn_main.py` & `pancollection-0.2b0/pancollection/models/MSDCNN/msdcnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/lib/data.py` & `pancollection-0.2b0/pancollection/models/MUCNN/lib/data.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/lib/datasets.py` & `pancollection-0.2b0/pancollection/models/MUCNN/lib/datasets.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/lib/evaluate.py` & `pancollection-0.2b0/pancollection/models/MUCNN/lib/evaluate.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/lib/model.py` & `pancollection-0.2b0/pancollection/models/MUCNN/lib/model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/lib/utils.py` & `pancollection-0.2b0/pancollection/models/MUCNN/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/main_test_multi.py` & `pancollection-0.2b0/pancollection/models/MUCNN/main_test_multi.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/main_test_single.py` & `pancollection-0.2b0/pancollection/models/MUCNN/main_test_single.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/MUCNN/train.py` & `pancollection-0.2b0/pancollection/models/MUCNN/train.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/PNN/model_pnn.py` & `pancollection-0.2b0/pancollection/models/PNN/model_pnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/PNN/pnn_main.py` & `pancollection-0.2b0/pancollection/models/PNN/pnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/PanNet/model_pannet.py` & `pancollection-0.2b0/pancollection/models/PanNet/model_pannet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/PanNet/pannet_main.py` & `pancollection-0.2b0/pancollection/models/PanNet/pannet_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/models/base_model.py` & `pancollection-0.2b0/pancollection/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/run_pansharpening.py` & `pancollection-0.2b0/pancollection/run_pansharpening.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection/run_test_pansharpening.py` & `pancollection-0.2b0/pancollection/run_test_pansharpening.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2a0/pancollection.egg-info/PKG-INFO` & `pancollection-0.2b0/pancollection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.2a0
+Version: 0.2b0
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pancollection-0.2a0/pancollection.egg-info/SOURCES.txt` & `pancollection-0.2b0/pancollection.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,27 @@
 pancollection/common/dataset.py
 pancollection/common/dataset_hp.py
 pancollection/common/evaluate.py
 pancollection/common/psdata.py
 pancollection/common/test_panloader.py
 pancollection/common/train_panloader.py
 pancollection/common/valid_panloader.py
+pancollection/common/FS_index/D_lambda_K.py
+pancollection/common/FS_index/HQNR.py
+pancollection/common/FS_index/MTF.py
+pancollection/common/FS_index/MTF_pan.py
+pancollection/common/FS_index/__init__.py
+pancollection/common/FS_index/genMTF.py
+pancollection/common/FS_index/genMTF_pan.py
+pancollection/common/FS_index/imresize.py
+pancollection/common/FS_index/indexes_evaluation_FS.py
+pancollection/common/FS_index/interp23.py
+pancollection/common/FS_index/my_D_s.py
+pancollection/common/FS_index/my_q2n.py
+pancollection/common/FS_index/tools.py
 pancollection/configs/__init__.py
 pancollection/configs/configs.py
 pancollection/configs/hook_configs.py
 pancollection/configs/option_DCFNet.py
 pancollection/configs/option_LAGNet.py
 pancollection/configs/option_bdpn.py
 pancollection/configs/option_dicnn.py
```

### Comparing `pancollection-0.2a0/setup.py` & `pancollection-0.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name='pancollection',
     description="PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)",
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="XiaoXiao-Woo",
     author_email="wxwsx1997@gmail.com",
     url='https://github.com/XiaoXiao-Woo/PanCollection',
-    version='0.2a',
+    version='0.2b',
     include_package_data=True,
     packages=find_packages(),
     package_data={'pancollection': ['models/*']},
     license='GPLv3',
     python_requires='>=3.7',
     install_requires=[
         "psutil",
```

