# Comparing `tmp/pancollection-0.2b0.tar.gz` & `tmp/pancollection-0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pancollection-0.2b0.tar", last modified: Fri Jun  9 06:53:33 2023, max compression
+gzip compressed data, was "dist\pancollection-0.2rc0.tar", last modified: Fri Jun  9 11:06:21 2023, max compression
```

## Comparing `pancollection-0.2b0.tar` & `pancollection-0.2rc0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/
--rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 pancollection-0.2b0/LICENSE
--rw-rw-rw-   0        0        0     5824 2023-06-09 06:53:33.000000 pancollection-0.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     5293 2023-06-07 04:18:18.000000 pancollection-0.2b0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/
--rw-rw-rw-   0        0        0      229 2023-06-06 18:32:01.000000 pancollection-0.2b0/pancollection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/common/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/common/FS_index/
--rw-rw-rw-   0        0        0     2364 2022-11-23 12:43:13.000000 pancollection-0.2b0/pancollection/common/FS_index/D_lambda_K.py
--rw-rw-rw-   0        0        0     2392 2022-11-22 05:24:39.000000 pancollection-0.2b0/pancollection/common/FS_index/HQNR.py
--rw-rw-rw-   0        0        0     2213 2023-03-27 15:42:39.000000 pancollection-0.2b0/pancollection/common/FS_index/MTF.py
--rw-rw-rw-   0        0        0     2224 2023-03-27 15:50:01.000000 pancollection-0.2b0/pancollection/common/FS_index/MTF_pan.py
--rw-rw-rw-   0        0        0      146 2023-06-09 06:53:23.000000 pancollection-0.2b0/pancollection/common/FS_index/__init__.py
--rw-rw-rw-   0        0        0     2593 2022-11-21 08:49:04.000000 pancollection-0.2b0/pancollection/common/FS_index/genMTF.py
--rw-rw-rw-   0        0        0      730 2023-03-27 15:48:45.000000 pancollection-0.2b0/pancollection/common/FS_index/genMTF_pan.py
--rw-rw-rw-   0        0        0     5365 2020-06-04 11:13:21.000000 pancollection-0.2b0/pancollection/common/FS_index/imresize.py
--rw-rw-rw-   0        0        0     9088 2022-11-21 16:19:17.000000 pancollection-0.2b0/pancollection/common/FS_index/indexes_evaluation_FS.py
--rw-rw-rw-   0        0        0     3106 2021-11-30 08:46:49.000000 pancollection-0.2b0/pancollection/common/FS_index/interp23.py
--rw-rw-rw-   0        0        0     6395 2022-11-23 12:43:13.000000 pancollection-0.2b0/pancollection/common/FS_index/my_D_s.py
--rw-rw-rw-   0        0        0     8378 2022-11-21 12:22:10.000000 pancollection-0.2b0/pancollection/common/FS_index/my_q2n.py
--rw-rw-rw-   0        0        0     1237 2020-06-04 13:59:20.000000 pancollection-0.2b0/pancollection/common/FS_index/tools.py
--rw-rw-rw-   0        0        0       22 2023-06-09 06:43:23.000000 pancollection-0.2b0/pancollection/common/__init__.py
--rw-rw-rw-   0        0        0      697 2023-06-09 05:15:41.000000 pancollection-0.2b0/pancollection/common/builder.py
--rw-rw-rw-   0        0        0    14450 2023-06-09 05:14:41.000000 pancollection-0.2b0/pancollection/common/dataset.py
--rw-rw-rw-   0        0        0     2238 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/common/dataset_hp.py
--rw-rw-rw-   0        0        0    16414 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/common/evaluate.py
--rw-rw-rw-   0        0        0     7163 2023-06-06 18:38:21.000000 pancollection-0.2b0/pancollection/common/psdata.py
--rw-rw-rw-   0        0        0     4847 2023-03-30 10:19:53.000000 pancollection-0.2b0/pancollection/common/test_panloader.py
--rw-rw-rw-   0        0        0     3965 2023-06-06 18:38:37.000000 pancollection-0.2b0/pancollection/common/train_panloader.py
--rw-rw-rw-   0        0        0     3958 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/common/valid_panloader.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/configs/
--rw-rw-rw-   0        0        0      336 2023-06-06 18:33:33.000000 pancollection-0.2b0/pancollection/configs/__init__.py
--rw-rw-rw-   0        0        0     1151 2023-06-09 05:08:57.000000 pancollection-0.2b0/pancollection/configs/configs.py
--rw-rw-rw-   0        0        0      824 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/configs/hook_configs.py
--rw-rw-rw-   0        0        0     3078 2023-06-06 18:51:23.000000 pancollection-0.2b0/pancollection/configs/option_DCFNet.py
--rw-rw-rw-   0        0        0     2927 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_LAGNet.py
--rw-rw-rw-   0        0        0     2896 2023-06-06 18:51:14.000000 pancollection-0.2b0/pancollection/configs/option_bdpn.py
--rw-rw-rw-   0        0        0     2811 2023-06-06 18:51:32.000000 pancollection-0.2b0/pancollection/configs/option_dicnn.py
--rw-rw-rw-   0        0        0     2878 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_drpnn.py
--rw-rw-rw-   0        0        0     3220 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_fusionnet.py
--rw-rw-rw-   0        0        0     2921 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_msdcnn.py
--rw-rw-rw-   0        0        0     3087 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_pannet.py
--rw-rw-rw-   0        0        0     2865 2023-06-06 18:52:03.000000 pancollection-0.2b0/pancollection/configs/option_pnn.py
--rw-rw-rw-   0        0        0      703 2023-06-09 05:02:24.000000 pancollection-0.2b0/pancollection/hug_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/ADKNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:55:31.000000 pancollection-0.2b0/pancollection/models/ADKNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/
--rw-rw-rw-   0        0        0       18 2023-03-22 11:48:22.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/__init__.py
--rw-rw-rw-   0        0        0    11638 2023-03-22 11:48:22.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/ddf.py
--rw-rw-rw-   0        0        0     2289 2023-03-22 11:48:22.000000 pancollection-0.2b0/pancollection/models/ADKNet/ddf/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/BDPN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/BDPN/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-06-06 18:36:55.000000 pancollection-0.2b0/pancollection/models/BDPN/bdpn_main.py
--rw-rw-rw-   0        0        0     7813 2023-06-09 05:15:23.000000 pancollection-0.2b0/pancollection/models/BDPN/model_bdpn.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DCFNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DCFNet/__init__.py
--rw-rw-rw-   0        0        0    32420 2023-06-09 05:14:16.000000 pancollection-0.2b0/pancollection/models/DCFNet/model_fcc_dense_head.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DHIFNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DHIFNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DRPNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DRPNN/__init__.py
--rw-rw-rw-   0        0        0     3849 2023-06-06 18:36:22.000000 pancollection-0.2b0/pancollection/models/DRPNN/drpnn_main.py
--rw-rw-rw-   0        0        0     5302 2023-06-09 05:15:15.000000 pancollection-0.2b0/pancollection/models/DRPNN/model_drpnn.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/DiCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/DiCNN/__init__.py
--rw-rw-rw-   0        0        0     3840 2023-06-06 18:35:36.000000 pancollection-0.2b0/pancollection/models/DiCNN/dicnn_main.py
--rw-rw-rw-   0        0        0     3768 2023-06-09 05:14:16.000000 pancollection-0.2b0/pancollection/models/DiCNN/model_dicnn.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/FusionNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/FusionNet/__init__.py
--rw-rw-rw-   0        0        0     3501 2023-06-06 18:35:47.000000 pancollection-0.2b0/pancollection/models/FusionNet/fusionnet_main.py
--rw-rw-rw-   0        0        0     5615 2023-06-09 05:14:50.000000 pancollection-0.2b0/pancollection/models/FusionNet/model_fusionnet.py
--rw-rw-rw-   0        0        0      518 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/FusionNet/run_fusionnet.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/GPPNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/GPPNN/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/GPPNN/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/GPPNN/models/
--rw-rw-rw-   0        0        0     4902 2023-06-09 06:05:48.000000 pancollection-0.2b0/pancollection/models/GPPNN/models/GPPNN.py
--rw-rw-rw-   0        0        0      686 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/GPPNN/models/__init__.py
--rw-rw-rw-   0        0        0    38742 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/GPPNN/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/LAGConv/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/LAGConv/__init__.py
--rw-rw-rw-   0        0        0     2254 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/LAGConv/data.py
--rw-rw-rw-   0        0        0     6962 2023-06-09 06:05:48.000000 pancollection-0.2b0/pancollection/models/LAGConv/model.py
--rw-rw-rw-   0        0        0     1990 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/LAGConv/test.py
--rw-rw-rw-   0        0        0     7423 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/models/LAGConv/train.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/MSDCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/MSDCNN/__init__.py
--rw-rw-rw-   0        0        0     5864 2023-06-09 06:05:48.000000 pancollection-0.2b0/pancollection/models/MSDCNN/model_msdcnn.py
--rw-rw-rw-   0        0        0     3845 2023-06-06 18:37:05.000000 pancollection-0.2b0/pancollection/models/MSDCNN/msdcnn_main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/MUCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/MUCNN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/
--rw-rw-rw-   0        0        0       81 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/__init__.py
--rw-rw-rw-   0        0        0      940 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/data.py
--rw-rw-rw-   0        0        0     3897 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/datasets.py
--rw-rw-rw-   0        0        0     5410 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/evaluate.py
--rw-rw-rw-   0        0        0     3027 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/model.py
--rw-rw-rw-   0        0        0     1328 2022-03-08 03:11:12.000000 pancollection-0.2b0/pancollection/models/MUCNN/lib/utils.py
--rw-rw-rw-   0        0        0     3395 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/MUCNN/main_test_multi.py
--rw-rw-rw-   0        0        0     2670 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/MUCNN/main_test_single.py
--rw-rw-rw-   0        0        0     8936 2023-03-22 11:48:24.000000 pancollection-0.2b0/pancollection/models/MUCNN/train.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/PNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/PNN/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-06-09 05:14:58.000000 pancollection-0.2b0/pancollection/models/PNN/model_pnn.py
--rw-rw-rw-   0        0        0     4390 2023-06-06 18:35:57.000000 pancollection-0.2b0/pancollection/models/PNN/pnn_main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection/models/PanNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2b0/pancollection/models/PanNet/__init__.py
--rw-rw-rw-   0        0        0     4917 2023-06-09 05:15:07.000000 pancollection-0.2b0/pancollection/models/PanNet/model_pannet.py
--rw-rw-rw-   0        0        0     3813 2023-06-06 18:36:06.000000 pancollection-0.2b0/pancollection/models/PanNet/pannet_main.py
--rw-rw-rw-   0        0        0      508 2023-06-09 05:14:16.000000 pancollection-0.2b0/pancollection/models/__init__.py
--rw-rw-rw-   0        0        0     3123 2023-06-09 05:14:26.000000 pancollection-0.2b0/pancollection/models/base_model.py
--rw-rw-rw-   0        0        0      550 2023-06-09 05:08:57.000000 pancollection-0.2b0/pancollection/run_pansharpening.py
--rw-rw-rw-   0        0        0      528 2023-03-27 06:21:37.000000 pancollection-0.2b0/pancollection/run_test_pansharpening.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/
--rw-rw-rw-   0        0        0     5824 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3739 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 06:53:33.000000 pancollection-0.2b0/pancollection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 06:53:33.000000 pancollection-0.2b0/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-06-09 06:43:29.000000 pancollection-0.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/
+-rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 pancollection-0.2rc0/LICENSE
+-rw-rw-rw-   0        0        0     5825 2023-06-09 11:06:21.000000 pancollection-0.2rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     5293 2023-06-07 04:18:18.000000 pancollection-0.2rc0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/
+-rw-rw-rw-   0        0        0      332 2023-06-09 10:56:50.000000 pancollection-0.2rc0/pancollection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/common/
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/common/FS_index/
+-rw-rw-rw-   0        0        0     2364 2022-11-23 12:43:13.000000 pancollection-0.2rc0/pancollection/common/FS_index/D_lambda_K.py
+-rw-rw-rw-   0        0        0     2392 2022-11-22 05:24:39.000000 pancollection-0.2rc0/pancollection/common/FS_index/HQNR.py
+-rw-rw-rw-   0        0        0     2213 2023-03-27 15:42:39.000000 pancollection-0.2rc0/pancollection/common/FS_index/MTF.py
+-rw-rw-rw-   0        0        0     2224 2023-03-27 15:50:01.000000 pancollection-0.2rc0/pancollection/common/FS_index/MTF_pan.py
+-rw-rw-rw-   0        0        0      146 2023-06-09 06:53:23.000000 pancollection-0.2rc0/pancollection/common/FS_index/__init__.py
+-rw-rw-rw-   0        0        0     2593 2022-11-21 08:49:04.000000 pancollection-0.2rc0/pancollection/common/FS_index/genMTF.py
+-rw-rw-rw-   0        0        0      730 2023-03-27 15:48:45.000000 pancollection-0.2rc0/pancollection/common/FS_index/genMTF_pan.py
+-rw-rw-rw-   0        0        0     5365 2020-06-04 11:13:21.000000 pancollection-0.2rc0/pancollection/common/FS_index/imresize.py
+-rw-rw-rw-   0        0        0     9088 2022-11-21 16:19:17.000000 pancollection-0.2rc0/pancollection/common/FS_index/indexes_evaluation_FS.py
+-rw-rw-rw-   0        0        0     3106 2021-11-30 08:46:49.000000 pancollection-0.2rc0/pancollection/common/FS_index/interp23.py
+-rw-rw-rw-   0        0        0     6395 2022-11-23 12:43:13.000000 pancollection-0.2rc0/pancollection/common/FS_index/my_D_s.py
+-rw-rw-rw-   0        0        0     8378 2022-11-21 12:22:10.000000 pancollection-0.2rc0/pancollection/common/FS_index/my_q2n.py
+-rw-rw-rw-   0        0        0     1237 2020-06-04 13:59:20.000000 pancollection-0.2rc0/pancollection/common/FS_index/tools.py
+-rw-rw-rw-   0        0        0       72 2023-06-09 10:36:34.000000 pancollection-0.2rc0/pancollection/common/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-06-09 05:15:41.000000 pancollection-0.2rc0/pancollection/common/builder.py
+-rw-rw-rw-   0        0        0    14450 2023-06-09 05:14:41.000000 pancollection-0.2rc0/pancollection/common/dataset.py
+-rw-rw-rw-   0        0        0     2238 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/common/dataset_hp.py
+-rw-rw-rw-   0        0        0    16414 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/common/evaluate.py
+-rw-rw-rw-   0        0        0     7163 2023-06-06 18:38:21.000000 pancollection-0.2rc0/pancollection/common/psdata.py
+-rw-rw-rw-   0        0        0     4847 2023-03-30 10:19:53.000000 pancollection-0.2rc0/pancollection/common/test_panloader.py
+-rw-rw-rw-   0        0        0     3965 2023-06-06 18:38:37.000000 pancollection-0.2rc0/pancollection/common/train_panloader.py
+-rw-rw-rw-   0        0        0     3958 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/common/valid_panloader.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/configs/
+-rw-rw-rw-   0        0        0      336 2023-06-06 18:33:33.000000 pancollection-0.2rc0/pancollection/configs/__init__.py
+-rw-rw-rw-   0        0        0     1151 2023-06-09 05:08:57.000000 pancollection-0.2rc0/pancollection/configs/configs.py
+-rw-rw-rw-   0        0        0      824 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/configs/hook_configs.py
+-rw-rw-rw-   0        0        0     3075 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_DCFNet.py
+-rw-rw-rw-   0        0        0     2924 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_LAGNet.py
+-rw-rw-rw-   0        0        0     2893 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_bdpn.py
+-rw-rw-rw-   0        0        0     2808 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_dicnn.py
+-rw-rw-rw-   0        0        0     2875 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_drpnn.py
+-rw-rw-rw-   0        0        0     3217 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_fusionnet.py
+-rw-rw-rw-   0        0        0     2918 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_msdcnn.py
+-rw-rw-rw-   0        0        0     3084 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_pannet.py
+-rw-rw-rw-   0        0        0     2862 2023-06-09 10:44:29.000000 pancollection-0.2rc0/pancollection/configs/option_pnn.py
+-rw-rw-rw-   0        0        0      703 2023-06-09 05:02:24.000000 pancollection-0.2rc0/pancollection/hug_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/ADKNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:55:31.000000 pancollection-0.2rc0/pancollection/models/ADKNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/ADKNet/ddf/
+-rw-rw-rw-   0        0        0       18 2023-03-22 11:48:22.000000 pancollection-0.2rc0/pancollection/models/ADKNet/ddf/__init__.py
+-rw-rw-rw-   0        0        0    11638 2023-03-22 11:48:22.000000 pancollection-0.2rc0/pancollection/models/ADKNet/ddf/ddf.py
+-rw-rw-rw-   0        0        0     2289 2023-03-22 11:48:22.000000 pancollection-0.2rc0/pancollection/models/ADKNet/ddf/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/BDPN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/BDPN/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-06-06 18:36:55.000000 pancollection-0.2rc0/pancollection/models/BDPN/bdpn_main.py
+-rw-rw-rw-   0        0        0     7813 2023-06-09 05:15:23.000000 pancollection-0.2rc0/pancollection/models/BDPN/model_bdpn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/DCFNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/DCFNet/__init__.py
+-rw-rw-rw-   0        0        0    32420 2023-06-09 05:14:16.000000 pancollection-0.2rc0/pancollection/models/DCFNet/model_fcc_dense_head.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/DHIFNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/DHIFNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/DRPNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/DRPNN/__init__.py
+-rw-rw-rw-   0        0        0     3849 2023-06-06 18:36:22.000000 pancollection-0.2rc0/pancollection/models/DRPNN/drpnn_main.py
+-rw-rw-rw-   0        0        0     5302 2023-06-09 05:15:15.000000 pancollection-0.2rc0/pancollection/models/DRPNN/model_drpnn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/DiCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/DiCNN/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-06-06 18:35:36.000000 pancollection-0.2rc0/pancollection/models/DiCNN/dicnn_main.py
+-rw-rw-rw-   0        0        0     3768 2023-06-09 05:14:16.000000 pancollection-0.2rc0/pancollection/models/DiCNN/model_dicnn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/FusionNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/FusionNet/__init__.py
+-rw-rw-rw-   0        0        0     3501 2023-06-06 18:35:47.000000 pancollection-0.2rc0/pancollection/models/FusionNet/fusionnet_main.py
+-rw-rw-rw-   0        0        0     5615 2023-06-09 05:14:50.000000 pancollection-0.2rc0/pancollection/models/FusionNet/model_fusionnet.py
+-rw-rw-rw-   0        0        0      518 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/models/FusionNet/run_fusionnet.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/GPPNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/GPPNN/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-03-22 11:48:24.000000 pancollection-0.2rc0/pancollection/models/GPPNN/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/GPPNN/models/
+-rw-rw-rw-   0        0        0     4902 2023-06-09 06:05:48.000000 pancollection-0.2rc0/pancollection/models/GPPNN/models/GPPNN.py
+-rw-rw-rw-   0        0        0      686 2023-03-22 11:48:24.000000 pancollection-0.2rc0/pancollection/models/GPPNN/models/__init__.py
+-rw-rw-rw-   0        0        0    38742 2023-03-22 11:48:24.000000 pancollection-0.2rc0/pancollection/models/GPPNN/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/LAGConv/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/LAGConv/__init__.py
+-rw-rw-rw-   0        0        0     2254 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/models/LAGConv/data.py
+-rw-rw-rw-   0        0        0     6962 2023-06-09 06:05:48.000000 pancollection-0.2rc0/pancollection/models/LAGConv/model.py
+-rw-rw-rw-   0        0        0     1990 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/models/LAGConv/test.py
+-rw-rw-rw-   0        0        0     7423 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/models/LAGConv/train.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/MSDCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/MSDCNN/__init__.py
+-rw-rw-rw-   0        0        0     5864 2023-06-09 06:05:48.000000 pancollection-0.2rc0/pancollection/models/MSDCNN/model_msdcnn.py
+-rw-rw-rw-   0        0        0     3845 2023-06-06 18:37:05.000000 pancollection-0.2rc0/pancollection/models/MSDCNN/msdcnn_main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/MUCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/MUCNN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/
+-rw-rw-rw-   0        0        0       81 2022-03-08 03:11:12.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/__init__.py
+-rw-rw-rw-   0        0        0      940 2022-03-08 03:11:12.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/data.py
+-rw-rw-rw-   0        0        0     3897 2022-03-08 03:11:12.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/datasets.py
+-rw-rw-rw-   0        0        0     5410 2022-03-08 03:11:12.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/evaluate.py
+-rw-rw-rw-   0        0        0     3027 2022-03-08 03:11:12.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/model.py
+-rw-rw-rw-   0        0        0     1328 2022-03-08 03:11:12.000000 pancollection-0.2rc0/pancollection/models/MUCNN/lib/utils.py
+-rw-rw-rw-   0        0        0     3395 2023-03-22 11:48:24.000000 pancollection-0.2rc0/pancollection/models/MUCNN/main_test_multi.py
+-rw-rw-rw-   0        0        0     2670 2023-03-22 11:48:24.000000 pancollection-0.2rc0/pancollection/models/MUCNN/main_test_single.py
+-rw-rw-rw-   0        0        0     8936 2023-03-22 11:48:24.000000 pancollection-0.2rc0/pancollection/models/MUCNN/train.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/PNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/PNN/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-09 05:14:58.000000 pancollection-0.2rc0/pancollection/models/PNN/model_pnn.py
+-rw-rw-rw-   0        0        0     4390 2023-06-06 18:35:57.000000 pancollection-0.2rc0/pancollection/models/PNN/pnn_main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection/models/PanNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2rc0/pancollection/models/PanNet/__init__.py
+-rw-rw-rw-   0        0        0     4917 2023-06-09 05:15:07.000000 pancollection-0.2rc0/pancollection/models/PanNet/model_pannet.py
+-rw-rw-rw-   0        0        0     3813 2023-06-06 18:36:06.000000 pancollection-0.2rc0/pancollection/models/PanNet/pannet_main.py
+-rw-rw-rw-   0        0        0      508 2023-06-09 05:14:16.000000 pancollection-0.2rc0/pancollection/models/__init__.py
+-rw-rw-rw-   0        0        0     3123 2023-06-09 05:14:26.000000 pancollection-0.2rc0/pancollection/models/base_model.py
+-rw-rw-rw-   0        0        0      706 2023-06-09 11:02:40.000000 pancollection-0.2rc0/pancollection/run_pansharpening.py
+-rw-rw-rw-   0        0        0      528 2023-03-27 06:21:37.000000 pancollection-0.2rc0/pancollection/run_test_pansharpening.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection.egg-info/
+-rw-rw-rw-   0        0        0     5825 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3739 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 11:06:21.000000 pancollection-0.2rc0/pancollection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:06:21.000000 pancollection-0.2rc0/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-06-09 11:06:19.000000 pancollection-0.2rc0/setup.py
```

### Comparing `pancollection-0.2b0/LICENSE` & `pancollection-0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/PKG-INFO` & `pancollection-0.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.2b0
+Version: 0.2rc0
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pancollection-0.2b0/README.md` & `pancollection-0.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/D_lambda_K.py` & `pancollection-0.2rc0/pancollection/common/FS_index/D_lambda_K.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/HQNR.py` & `pancollection-0.2rc0/pancollection/common/FS_index/HQNR.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/MTF.py` & `pancollection-0.2rc0/pancollection/common/FS_index/MTF.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/MTF_pan.py` & `pancollection-0.2rc0/pancollection/common/FS_index/MTF_pan.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/genMTF.py` & `pancollection-0.2rc0/pancollection/common/FS_index/genMTF.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/genMTF_pan.py` & `pancollection-0.2rc0/pancollection/common/FS_index/genMTF_pan.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/imresize.py` & `pancollection-0.2rc0/pancollection/common/FS_index/imresize.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/indexes_evaluation_FS.py` & `pancollection-0.2rc0/pancollection/common/FS_index/indexes_evaluation_FS.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/interp23.py` & `pancollection-0.2rc0/pancollection/common/FS_index/interp23.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/my_D_s.py` & `pancollection-0.2rc0/pancollection/common/FS_index/my_D_s.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/my_q2n.py` & `pancollection-0.2rc0/pancollection/common/FS_index/my_q2n.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/FS_index/tools.py` & `pancollection-0.2rc0/pancollection/common/FS_index/tools.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/builder.py` & `pancollection-0.2rc0/pancollection/common/builder.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/dataset.py` & `pancollection-0.2rc0/pancollection/common/dataset.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/dataset_hp.py` & `pancollection-0.2rc0/pancollection/common/dataset_hp.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/evaluate.py` & `pancollection-0.2rc0/pancollection/common/evaluate.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/psdata.py` & `pancollection-0.2rc0/pancollection/common/psdata.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/test_panloader.py` & `pancollection-0.2rc0/pancollection/common/test_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/train_panloader.py` & `pancollection-0.2rc0/pancollection/common/train_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/common/valid_panloader.py` & `pancollection-0.2rc0/pancollection/common/valid_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/configs/configs.py` & `pancollection-0.2rc0/pancollection/configs/configs.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/configs/hook_configs.py` & `pancollection-0.2rc0/pancollection/configs/hook_configs.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/configs/option_DCFNet.py` & `pancollection-0.2rc0/pancollection/configs/option_DCFNet.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import warnings
 
 class parser_args(TaskDispatcher, name='DCFNet'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
 
         root_dir = script_path.split(cfg.task)[0]
         model_path = f'{root_dir}/{cfg.task}/models/DCFNet/PanCollectionWeights/dcfnet_wv3.pth'
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
                             help='path to save model')
         # * Training
@@ -42,15 +42,15 @@
         parser.add_argument('--dataset', default={'train': 'wv3', 'test': 'test_wv3_multiExm1.h5'}, type=str,
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
                                      'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5'],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=True, type=bool,
                             help="performing evalution for patch2entire")
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = "Test"
 
         cfg.merge_args2cfg(args)
         cfg.img_range = 2047.0
         cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_LAGNet.py` & `pancollection-0.2rc0/pancollection/configs/option_LAGNet.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 
 class parser_args(TaskDispatcher, name='LAGNet'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
         root_dir = script_path.split(cfg.task)[0]
 
         model_path = f'.pth.tar'
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
                             help='path to save model')
@@ -40,15 +40,15 @@
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
                                      'wv2_hp', ..., 'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5'],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=False, type=bool,
                             help="performing evalution for patch2entire")
 
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = 'Test'
         cfg.merge_args2cfg(args)
         cfg.save_fmt = "png"
         cfg.workflow = [('train', 1)]
         cfg.img_range = 2047.0
         # cfg.config = f"{script_path}/configs/hook_configs.py"
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_bdpn.py` & `pancollection-0.2rc0/pancollection/configs/option_bdpn.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pancollection.configs.configs import TaskDispatcher
 import os
 
 class parser_args(TaskDispatcher, name='BDPN'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
         root_dir = script_path.split(cfg.task)[0]
 
         model_path = f'{root_dir}/results/{cfg.task}/wv3/BDPN/Test/.pth.tar'
 
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
@@ -37,15 +37,15 @@
         parser.add_argument('--dataset', default={'train': 'wv3', 'test': 'wv3_multiExm1.h5'}, type=str,
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
                                      'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5', ...],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=False, type=bool,
                             help="performing evalution for patch2entire")
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = "Test"
         # cfg.save_fmt = 'png'
         cfg.img_range = 2047.0
         cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
 
         cfg.merge_args2cfg(args)
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_dicnn.py` & `pancollection-0.2rc0/pancollection/configs/option_pnn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import argparse
 from pancollection.configs.configs import TaskDispatcher
 import os
 
-class parser_args(TaskDispatcher, name='DiCNN1'):
+class parser_args(TaskDispatcher, name='PNN'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
-        root_dir = script_path.split(cfg.task)[0]
+        script_path = os.path.dirname(os.getcwd())
+        root_dir = script_path.split(cfg.task)[0].replace('\\', '/')
 
-        model_path = f'{root_dir}/results/{cfg.task}/wv3/DiCNN1/Test/.pth.tar'
+        model_path = f'.pth.tar'
 
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
                             help='path to save model')
         # * Training
-        parser.add_argument('--lr', default=2e-4, type=float)  # 1e-4 2e-4 8
+        parser.add_argument('--lr', default=1e-3, type=float)  # 1e-4 2e-4 8
         parser.add_argument('--lr_scheduler', default=True, type=bool)
         parser.add_argument('--samples_per_gpu', default=64, type=int,  # 8
                             metavar='N', help='mini-batch size (default: 256)')
-        parser.add_argument('--print-freq', '-p', default=1, type=int,
+        parser.add_argument('--print-freq', '-p', default=500, type=int,
                             metavar='N', help='print frequency (default: 10)')
-        parser.add_argument('--epochs', default=5000, type=int)
+        parser.add_argument('--seed', default=1, type=int,
+                            help='seed for initializing training. ')
+        parser.add_argument('--epochs', default=12000, type=int)
         parser.add_argument('--workers_per_gpu', default=0, type=int)
         parser.add_argument('--resume_from',
                             default=model_path,
                             type=str, metavar='PATH',
                             help='path to latest checkpoint (default: none)')
         # * Model and Dataset
-        parser.add_argument('--arch', '-a', metavar='ARCH', default='DiCNN1', type=str,
+        parser.add_argument('--arch', '-a', metavar='ARCH', default='PNN', type=str,
                             choices=['PanNet', 'DiCNN', 'PNN', 'FusionNet'])
         parser.add_argument('--dataset', default={'train': 'wv3', 'test': 'wv3_multiExm1.h5'}, type=str,
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
-                                     'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5', ...],
+                                     'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5'],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=False, type=bool,
                             help="performing evalution for patch2entire")
-
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
-        args.experimental_desc = "Test"
-        # cfg.save_fmt = 'png'
-        cfg.img_range = 2047.0#1023.0
+        args.experimental_desc = 'Test'
+        cfg.merge_args2cfg(args)
+        cfg.workflow = [('train', 1)]
+        cfg.img_range = 2047.0
         cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
 
-        cfg.merge_args2cfg(args)
         print(cfg.pretty_text)
-        cfg.workflow = [('train', 1)]
-        self.merge_from_dict(cfg)
+
+        self.merge_from_dict(cfg)
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_drpnn.py` & `pancollection-0.2rc0/pancollection/configs/option_drpnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 
 class parser_args(TaskDispatcher, name='DRPNN'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
         root_dir = script_path.split(cfg.task)[0]
 
         model_path = f'{root_dir}/results/{cfg.task}/wv3/DRPNN/Test/.pth.tar'
 
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
@@ -39,15 +39,15 @@
         parser.add_argument('--dataset', default={'train': 'wv3', 'test': 'wv3_multiExm1.h5'}, type=str,
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
                                      'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5'],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=False, type=bool,
                             help="performing evalution for patch2entire")
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = "Test"
         # cfg.save_fmt = 'png'
         cfg.img_range = 2047.0
         cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
 
         cfg.merge_args2cfg(args)
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_fusionnet.py` & `pancollection-0.2rc0/pancollection/configs/option_fusionnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 
 class parser_args(TaskDispatcher, name='FusionNet'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
         root_dir = script_path.split(cfg.task)[0]
 
         model_path = f'.pth.tar'
 
 
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
@@ -43,15 +43,15 @@
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf2',
                                      'wv3_OrigScale_multiExm1.h5', 'test_wv3_multiExm1.h5'],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=False, type=bool,
                             help="performing evaluation out of training process, which can avoid dead loop !!")
 
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = 'Test'
         cfg.merge_args2cfg(args)
         cfg.save_fmt = "mat"
         # cfg.workflow = [('train', 10), ('val', 1)]
         cfg.workflow = [('train', 1)]
         # cfg.config = f"{script_path}/configs/hook_configs.py"
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_msdcnn.py` & `pancollection-0.2rc0/pancollection/configs/option_dicnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 import argparse
 from pancollection.configs.configs import TaskDispatcher
 import os
 
-class parser_args(TaskDispatcher, name='MSDCNN'):
+class parser_args(TaskDispatcher, name='DiCNN1'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
         root_dir = script_path.split(cfg.task)[0]
 
-        model_path = f'{root_dir}/results/{cfg.task}/wv3/MSDCNN/Test/.pth.tar'
+        model_path = f'{root_dir}/results/{cfg.task}/wv3/DiCNN1/Test/.pth.tar'
 
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
                             help='path to save model')
         # * Training
-        parser.add_argument('--lr', default=0.0001, type=float)  # 1e-4 2e-4 8
+        parser.add_argument('--lr', default=2e-4, type=float)  # 1e-4 2e-4 8
         parser.add_argument('--lr_scheduler', default=True, type=bool)
         parser.add_argument('--samples_per_gpu', default=64, type=int,  # 8
                             metavar='N', help='mini-batch size (default: 256)')
-        parser.add_argument('--print-freq', '-p', default=100, type=int,
+        parser.add_argument('--print-freq', '-p', default=1, type=int,
                             metavar='N', help='print frequency (default: 10)')
-        parser.add_argument('--epochs', default=200, type=int)
+        parser.add_argument('--epochs', default=5000, type=int)
         parser.add_argument('--workers_per_gpu', default=0, type=int)
         parser.add_argument('--resume_from',
                             default=model_path,
                             type=str, metavar='PATH',
                             help='path to latest checkpoint (default: none)')
         # * Model and Dataset
-        parser.add_argument('--arch', '-a', metavar='ARCH', default='MSDCNN', type=str,
+        parser.add_argument('--arch', '-a', metavar='ARCH', default='DiCNN1', type=str,
                             choices=['PanNet', 'DiCNN', 'PNN', 'FusionNet'])
-        # wv3 qb wv2
         parser.add_argument('--dataset', default={'train': 'wv3', 'test': 'wv3_multiExm1.h5'}, type=str,
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
-                                     'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5'],
+                                     'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5', ...],
                             help="performing evalution for patch2entire")
-        parser.add_argument('--eval', default=True, type=bool,
+        parser.add_argument('--eval', default=False, type=bool,
                             help="performing evalution for patch2entire")
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = "Test"
         # cfg.save_fmt = 'png'
-        cfg.img_range = 2047.0
+        cfg.img_range = 2047.0#1023.0
+        cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
 
         cfg.merge_args2cfg(args)
         print(cfg.pretty_text)
-        # cfg.workflow = [('train', 50), ('val', 1)]
-        # cfg.workflow = [('val', 1)]
-        cfg.workflow = [('train', 50)]
-        cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
-
+        cfg.workflow = [('train', 1)]
         self.merge_from_dict(cfg)
-
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_pannet.py` & `pancollection-0.2rc0/pancollection/configs/option_pannet.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 
 class parser_args(TaskDispatcher, name='PanNet'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
+        script_path = os.path.dirname(os.getcwd())
         root_dir = script_path.split(cfg.task)[0]
 
 
         # model_path = f'{root_dir}/results/{cfg.task}/qb_hp/PanNet/Test/.pth.tar'
         model_path = f'{root_dir}/results/{cfg.task}/wv3_hp/PanNet/Test/.pth.tar'
         
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
@@ -44,15 +44,15 @@
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
                                      'wv2_hp', ...,
                                      'wv3_OrigScale_multiExm_hp.h5', 'wv3_multiExm1_hp.h5'],
                             help="performing evalution for patch2entire")
         parser.add_argument('--eval', default=False, type=bool,
                             help="performing evalution for patch2entire")
 
-        args = parser.parse_args()
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
         args.experimental_desc = "Test"
 
 
         cfg.merge_args2cfg(args)
         cfg.img_range = 2047.0
         cfg.reg = True
```

### Comparing `pancollection-0.2b0/pancollection/configs/option_pnn.py` & `pancollection-0.2rc0/pancollection/configs/option_msdcnn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 import argparse
 from pancollection.configs.configs import TaskDispatcher
 import os
 
-class parser_args(TaskDispatcher, name='PNN'):
+class parser_args(TaskDispatcher, name='MSDCNN'):
     def __init__(self, cfg=None):
         super(parser_args, self).__init__()
 
         if cfg is None:
-            from UDL.Basis.option import panshaprening_cfg
+            from udl_vis.Basis.option import panshaprening_cfg
             cfg = panshaprening_cfg()
 
-        script_path = os.path.dirname(os.path.dirname(__file__))
-        root_dir = script_path.split(cfg.task)[0].replace('\\', '/')
+        script_path = os.path.dirname(os.getcwd())
+        root_dir = script_path.split(cfg.task)[0]
 
-        model_path = f'.pth.tar'
+        model_path = f'{root_dir}/results/{cfg.task}/wv3/MSDCNN/Test/.pth.tar'
 
         parser = argparse.ArgumentParser(description='PyTorch Pansharpening Training')
         # * Logger
         parser.add_argument('--out_dir', metavar='DIR', default=f'{root_dir}/results/{cfg.task}',
                             help='path to save model')
         # * Training
-        parser.add_argument('--lr', default=1e-3, type=float)  # 1e-4 2e-4 8
+        parser.add_argument('--lr', default=0.0001, type=float)  # 1e-4 2e-4 8
         parser.add_argument('--lr_scheduler', default=True, type=bool)
         parser.add_argument('--samples_per_gpu', default=64, type=int,  # 8
                             metavar='N', help='mini-batch size (default: 256)')
-        parser.add_argument('--print-freq', '-p', default=500, type=int,
+        parser.add_argument('--print-freq', '-p', default=100, type=int,
                             metavar='N', help='print frequency (default: 10)')
-        parser.add_argument('--seed', default=1, type=int,
-                            help='seed for initializing training. ')
-        parser.add_argument('--epochs', default=12000, type=int)
+        parser.add_argument('--epochs', default=200, type=int)
         parser.add_argument('--workers_per_gpu', default=0, type=int)
         parser.add_argument('--resume_from',
                             default=model_path,
                             type=str, metavar='PATH',
                             help='path to latest checkpoint (default: none)')
         # * Model and Dataset
-        parser.add_argument('--arch', '-a', metavar='ARCH', default='PNN', type=str,
+        parser.add_argument('--arch', '-a', metavar='ARCH', default='MSDCNN', type=str,
                             choices=['PanNet', 'DiCNN', 'PNN', 'FusionNet'])
+        # wv3 qb wv2
         parser.add_argument('--dataset', default={'train': 'wv3', 'test': 'wv3_multiExm1.h5'}, type=str,
                             choices=[None, 'wv2', 'wv3', 'wv4', 'qb', 'gf',
                                      'wv3_OrigScale_multiExm1.h5', 'wv3_multiExm1.h5'],
                             help="performing evalution for patch2entire")
-        parser.add_argument('--eval', default=False, type=bool,
+        parser.add_argument('--eval', default=True, type=bool,
                             help="performing evalution for patch2entire")
-        args = parser.parse_args()
+
+        args = parser.parse_args(args=[])
         args.start_epoch = args.best_epoch = 1
-        args.experimental_desc = 'Test'
-        cfg.merge_args2cfg(args)
-        cfg.workflow = [('train', 1)]
+        args.experimental_desc = "Test"
+        # cfg.save_fmt = 'png'
         cfg.img_range = 2047.0
-        cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
 
+        cfg.merge_args2cfg(args)
         print(cfg.pretty_text)
+        # cfg.workflow = [('train', 50), ('val', 1)]
+        # cfg.workflow = [('val', 1)]
+        cfg.workflow = [('train', 50)]
+        cfg.dataloader_name = "PanCollection_dataloader"  # PanCollection_dataloader, oldPan_dataloader, DLPan_dataloader
+
+        self.merge_from_dict(cfg)
 
-        self.merge_from_dict(cfg)
```

### Comparing `pancollection-0.2b0/pancollection/hug_demo.py` & `pancollection-0.2rc0/pancollection/hug_demo.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/ADKNet/ddf/ddf.py` & `pancollection-0.2rc0/pancollection/models/ADKNet/ddf/ddf.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/ADKNet/ddf/setup.py` & `pancollection-0.2rc0/pancollection/models/ADKNet/ddf/setup.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/BDPN/bdpn_main.py` & `pancollection-0.2rc0/pancollection/models/BDPN/bdpn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/BDPN/model_bdpn.py` & `pancollection-0.2rc0/pancollection/models/BDPN/model_bdpn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/DCFNet/model_fcc_dense_head.py` & `pancollection-0.2rc0/pancollection/models/DCFNet/model_fcc_dense_head.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/DRPNN/drpnn_main.py` & `pancollection-0.2rc0/pancollection/models/DRPNN/drpnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/DRPNN/model_drpnn.py` & `pancollection-0.2rc0/pancollection/models/DRPNN/model_drpnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/DiCNN/dicnn_main.py` & `pancollection-0.2rc0/pancollection/models/DiCNN/dicnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/DiCNN/model_dicnn.py` & `pancollection-0.2rc0/pancollection/models/DiCNN/model_dicnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/FusionNet/fusionnet_main.py` & `pancollection-0.2rc0/pancollection/models/FusionNet/fusionnet_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/FusionNet/model_fusionnet.py` & `pancollection-0.2rc0/pancollection/models/FusionNet/model_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/FusionNet/run_fusionnet.py` & `pancollection-0.2rc0/pancollection/models/FusionNet/run_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/GPPNN/metrics.py` & `pancollection-0.2rc0/pancollection/models/GPPNN/metrics.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/GPPNN/models/GPPNN.py` & `pancollection-0.2rc0/pancollection/models/GPPNN/models/GPPNN.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/GPPNN/models/__init__.py` & `pancollection-0.2rc0/pancollection/models/GPPNN/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/GPPNN/utils.py` & `pancollection-0.2rc0/pancollection/models/GPPNN/utils.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/LAGConv/data.py` & `pancollection-0.2rc0/pancollection/models/LAGConv/data.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/LAGConv/model.py` & `pancollection-0.2rc0/pancollection/models/LAGConv/model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/LAGConv/test.py` & `pancollection-0.2rc0/pancollection/models/LAGConv/test.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/LAGConv/train.py` & `pancollection-0.2rc0/pancollection/models/LAGConv/train.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MSDCNN/model_msdcnn.py` & `pancollection-0.2rc0/pancollection/models/MSDCNN/model_msdcnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MSDCNN/msdcnn_main.py` & `pancollection-0.2rc0/pancollection/models/MSDCNN/msdcnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/lib/data.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/lib/data.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/lib/datasets.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/lib/datasets.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/lib/evaluate.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/lib/evaluate.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/lib/model.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/lib/model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/lib/utils.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/main_test_multi.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/main_test_multi.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/main_test_single.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/main_test_single.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/MUCNN/train.py` & `pancollection-0.2rc0/pancollection/models/MUCNN/train.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/PNN/model_pnn.py` & `pancollection-0.2rc0/pancollection/models/PNN/model_pnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/PNN/pnn_main.py` & `pancollection-0.2rc0/pancollection/models/PNN/pnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/PanNet/model_pannet.py` & `pancollection-0.2rc0/pancollection/models/PanNet/model_pannet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/PanNet/pannet_main.py` & `pancollection-0.2rc0/pancollection/models/PanNet/pannet_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/models/base_model.py` & `pancollection-0.2rc0/pancollection/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection/run_pansharpening.py` & `pancollection-0.2rc0/pancollection/run_pansharpening.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 # All Rights Reserved 
 #
 # @Time    : 2022/4/25 0:17
 # @Author  : Xiao Wu
 # @reference:
 
 def run_demo():
-    from pancollection.configs.configs import TaskDispatcher
-    from udl_vis.AutoDL.trainer import main
-    from pancollection.common.builder import build_model, getDataSession
 
+    from pancollection import TaskDispatcher, trainer, build_model, getDataSession
     cfg = TaskDispatcher.new(task='pansharpening', mode='entrypoint', arch='FusionNet')
     print(TaskDispatcher._task.keys())
-    main(cfg, build_model, getDataSession)
+    trainer.main(cfg, build_model, getDataSession)
+    # or
+    # import pancollection as pan
+    # cfg = pan.TaskDispatcher.new(task='pansharpening', mode='entrypoint', arch='FusionNet')
+    # print(pan.TaskDispatcher._task)
+    # pan.trainer.main(cfg, pan.build_model, pan.getDataSession)
 
 if __name__ == '__main__':
     run_demo()
```

### Comparing `pancollection-0.2b0/pancollection/run_test_pansharpening.py` & `pancollection-0.2rc0/pancollection/run_test_pansharpening.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/pancollection.egg-info/PKG-INFO` & `pancollection-0.2rc0/pancollection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.2b0
+Version: 0.2rc0
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pancollection-0.2b0/pancollection.egg-info/SOURCES.txt` & `pancollection-0.2rc0/pancollection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pancollection-0.2b0/setup.py` & `pancollection-0.2rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name='pancollection',
     description="PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)",
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="XiaoXiao-Woo",
     author_email="wxwsx1997@gmail.com",
     url='https://github.com/XiaoXiao-Woo/PanCollection',
-    version='0.2b',
+    version='0.2c',
     include_package_data=True,
     packages=find_packages(),
     package_data={'pancollection': ['models/*']},
     license='GPLv3',
     python_requires='>=3.7',
     install_requires=[
         "psutil",
@@ -29,10 +29,11 @@
         "imageio",
         "colorlog",
         "scipy",
         "h5py",
         "regex",
         "packaging",
         "colorlog",
-        "pyyaml"
+        "pyyaml",
+        "udl-vis"
     ],
 )
```

