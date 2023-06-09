# Comparing `tmp/pancollection-0.2.tar.gz` & `tmp/pancollection-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pancollection-0.2.tar", last modified: Wed Jun  7 10:10:00 2023, max compression
+gzip compressed data, was "dist\pancollection-0.2a0.tar", last modified: Fri Jun  9 06:06:42 2023, max compression
```

## Comparing `pancollection-0.2.tar` & `pancollection-0.2a0.tar`

### file list

```diff
@@ -1,115 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/
--rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 pancollection-0.2/LICENSE
--rw-rw-rw-   0        0        0     5822 2023-06-07 10:10:00.000000 pancollection-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5293 2023-06-07 04:18:18.000000 pancollection-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/
--rw-rw-rw-   0        0        0      229 2023-06-06 18:32:01.000000 pancollection-0.2/pancollection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/common/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/common/__init__.py
--rw-rw-rw-   0        0        0      693 2023-06-06 19:04:11.000000 pancollection-0.2/pancollection/common/builder.py
--rw-rw-rw-   0        0        0    14446 2023-06-06 17:48:27.000000 pancollection-0.2/pancollection/common/dataset.py
--rw-rw-rw-   0        0        0     2238 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/common/dataset_hp.py
--rw-rw-rw-   0        0        0    16414 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/common/evaluate.py
--rw-rw-rw-   0        0        0     7163 2023-06-06 18:38:21.000000 pancollection-0.2/pancollection/common/psdata.py
--rw-rw-rw-   0        0        0     4847 2023-03-30 10:19:53.000000 pancollection-0.2/pancollection/common/test_panloader.py
--rw-rw-rw-   0        0        0     3965 2023-06-06 18:38:37.000000 pancollection-0.2/pancollection/common/train_panloader.py
--rw-rw-rw-   0        0        0     3958 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/common/valid_panloader.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/configs/
--rw-rw-rw-   0        0        0      336 2023-06-06 18:33:33.000000 pancollection-0.2/pancollection/configs/__init__.py
--rw-rw-rw-   0        0        0     1143 2023-06-06 18:53:16.000000 pancollection-0.2/pancollection/configs/configs.py
--rw-rw-rw-   0        0        0      824 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/configs/hook_configs.py
--rw-rw-rw-   0        0        0     3078 2023-06-06 18:51:23.000000 pancollection-0.2/pancollection/configs/option_DCFNet.py
--rw-rw-rw-   0        0        0     2927 2023-06-06 18:52:03.000000 pancollection-0.2/pancollection/configs/option_LAGNet.py
--rw-rw-rw-   0        0        0     2896 2023-06-06 18:51:14.000000 pancollection-0.2/pancollection/configs/option_bdpn.py
--rw-rw-rw-   0        0        0     2811 2023-06-06 18:51:32.000000 pancollection-0.2/pancollection/configs/option_dicnn.py
--rw-rw-rw-   0        0        0     2878 2023-06-06 18:52:03.000000 pancollection-0.2/pancollection/configs/option_drpnn.py
--rw-rw-rw-   0        0        0     3220 2023-06-06 18:52:03.000000 pancollection-0.2/pancollection/configs/option_fusionnet.py
--rw-rw-rw-   0        0        0     2921 2023-06-06 18:52:03.000000 pancollection-0.2/pancollection/configs/option_msdcnn.py
--rw-rw-rw-   0        0        0     3087 2023-06-06 18:52:03.000000 pancollection-0.2/pancollection/configs/option_pannet.py
--rw-rw-rw-   0        0        0     2865 2023-06-06 18:52:03.000000 pancollection-0.2/pancollection/configs/option_pnn.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/ADKNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:55:31.000000 pancollection-0.2/pancollection/models/ADKNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/ADKNet/ddf/
--rw-rw-rw-   0        0        0       18 2023-03-22 11:48:22.000000 pancollection-0.2/pancollection/models/ADKNet/ddf/__init__.py
--rw-rw-rw-   0        0        0    11638 2023-03-22 11:48:22.000000 pancollection-0.2/pancollection/models/ADKNet/ddf/ddf.py
--rw-rw-rw-   0        0        0     2289 2023-03-22 11:48:22.000000 pancollection-0.2/pancollection/models/ADKNet/ddf/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/BDPN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/BDPN/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-06-06 18:36:55.000000 pancollection-0.2/pancollection/models/BDPN/bdpn_main.py
--rw-rw-rw-   0        0        0     7809 2023-06-06 17:50:46.000000 pancollection-0.2/pancollection/models/BDPN/model_bdpn.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/DCFNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/DCFNet/__init__.py
--rw-rw-rw-   0        0        0    32416 2023-06-06 18:36:31.000000 pancollection-0.2/pancollection/models/DCFNet/model_fcc_dense_head.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/DHIFNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/DHIFNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/DRPNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/DRPNN/__init__.py
--rw-rw-rw-   0        0        0     3849 2023-06-06 18:36:22.000000 pancollection-0.2/pancollection/models/DRPNN/drpnn_main.py
--rw-rw-rw-   0        0        0     5298 2023-06-06 17:49:56.000000 pancollection-0.2/pancollection/models/DRPNN/model_drpnn.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/DiCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/DiCNN/__init__.py
--rw-rw-rw-   0        0        0     3840 2023-06-06 18:35:36.000000 pancollection-0.2/pancollection/models/DiCNN/dicnn_main.py
--rw-rw-rw-   0        0        0     3764 2023-06-06 18:35:04.000000 pancollection-0.2/pancollection/models/DiCNN/model_dicnn.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/FusionNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/FusionNet/__init__.py
--rw-rw-rw-   0        0        0     3501 2023-06-06 18:35:47.000000 pancollection-0.2/pancollection/models/FusionNet/fusionnet_main.py
--rw-rw-rw-   0        0        0     5611 2023-06-06 17:49:04.000000 pancollection-0.2/pancollection/models/FusionNet/model_fusionnet.py
--rw-rw-rw-   0        0        0      518 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/models/FusionNet/run_fusionnet.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/GPPNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/GPPNN/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GPPNN/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/GPPNN/models/
--rw-rw-rw-   0        0        0     4904 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GPPNN/models/GPPNN.py
--rw-rw-rw-   0        0        0      686 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GPPNN/models/__init__.py
--rw-rw-rw-   0        0        0    38742 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GPPNN/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/GTP-PNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/GTP-PNet/__init__.py
--rw-rw-rw-   0        0        0    28370 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GTP-PNet/model_P.py
--rw-rw-rw-   0        0        0    14671 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GTP-PNet/model_T.py
--rw-rw-rw-   0        0        0    18011 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GTP-PNet/test.py
--rw-rw-rw-   0        0        0     1922 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GTP-PNet/train_P.py
--rw-rw-rw-   0        0        0     1922 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GTP-PNet/train_T.py
--rw-rw-rw-   0        0        0     9261 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/GTP-PNet/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/LAGConv/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/LAGConv/__init__.py
--rw-rw-rw-   0        0        0     2254 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/models/LAGConv/data.py
--rw-rw-rw-   0        0        0     6976 2023-06-06 18:36:55.000000 pancollection-0.2/pancollection/models/LAGConv/model.py
--rw-rw-rw-   0        0        0     1990 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/models/LAGConv/test.py
--rw-rw-rw-   0        0        0     7423 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/models/LAGConv/train.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/MSDCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/MSDCNN/__init__.py
--rw-rw-rw-   0        0        0     5858 2023-06-06 17:50:57.000000 pancollection-0.2/pancollection/models/MSDCNN/model_msdcnn.py
--rw-rw-rw-   0        0        0     3845 2023-06-06 18:37:05.000000 pancollection-0.2/pancollection/models/MSDCNN/msdcnn_main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/MUCNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/MUCNN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/MUCNN/lib/
--rw-rw-rw-   0        0        0       81 2022-03-08 03:11:12.000000 pancollection-0.2/pancollection/models/MUCNN/lib/__init__.py
--rw-rw-rw-   0        0        0      940 2022-03-08 03:11:12.000000 pancollection-0.2/pancollection/models/MUCNN/lib/data.py
--rw-rw-rw-   0        0        0     3897 2022-03-08 03:11:12.000000 pancollection-0.2/pancollection/models/MUCNN/lib/datasets.py
--rw-rw-rw-   0        0        0     5410 2022-03-08 03:11:12.000000 pancollection-0.2/pancollection/models/MUCNN/lib/evaluate.py
--rw-rw-rw-   0        0        0     3027 2022-03-08 03:11:12.000000 pancollection-0.2/pancollection/models/MUCNN/lib/model.py
--rw-rw-rw-   0        0        0     1328 2022-03-08 03:11:12.000000 pancollection-0.2/pancollection/models/MUCNN/lib/utils.py
--rw-rw-rw-   0        0        0     3395 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/MUCNN/main_test_multi.py
--rw-rw-rw-   0        0        0     2670 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/MUCNN/main_test_single.py
--rw-rw-rw-   0        0        0     8936 2023-03-22 11:48:24.000000 pancollection-0.2/pancollection/models/MUCNN/train.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/PNN/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/PNN/__init__.py
--rw-rw-rw-   0        0        0     2552 2023-06-06 17:49:16.000000 pancollection-0.2/pancollection/models/PNN/model_pnn.py
--rw-rw-rw-   0        0        0     4390 2023-06-06 18:35:57.000000 pancollection-0.2/pancollection/models/PNN/pnn_main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection/models/PanNet/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2/pancollection/models/PanNet/__init__.py
--rw-rw-rw-   0        0        0     4913 2023-06-06 17:49:30.000000 pancollection-0.2/pancollection/models/PanNet/model_pannet.py
--rw-rw-rw-   0        0        0     3813 2023-06-06 18:36:06.000000 pancollection-0.2/pancollection/models/PanNet/pannet_main.py
--rw-rw-rw-   0        0        0      509 2023-06-07 09:25:05.000000 pancollection-0.2/pancollection/models/__init__.py
--rw-rw-rw-   0        0        0     3119 2023-06-06 18:35:26.000000 pancollection-0.2/pancollection/models/base_model.py
--rw-rw-rw-   0        0        0      546 2023-06-06 19:05:19.000000 pancollection-0.2/pancollection/run_pansharpening.py
--rw-rw-rw-   0        0        0      528 2023-03-27 06:21:37.000000 pancollection-0.2/pancollection/run_test_pansharpening.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection.egg-info/
--rw-rw-rw-   0        0        0     5822 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 10:10:00.000000 pancollection-0.2/pancollection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 10:10:00.000000 pancollection-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-06-07 10:09:57.000000 pancollection-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/
+-rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 pancollection-0.2a0/LICENSE
+-rw-rw-rw-   0        0        0     5824 2023-06-09 06:06:42.000000 pancollection-0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5293 2023-06-07 04:18:18.000000 pancollection-0.2a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/
+-rw-rw-rw-   0        0        0      229 2023-06-06 18:32:01.000000 pancollection-0.2a0/pancollection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/common/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/common/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-06-09 05:15:41.000000 pancollection-0.2a0/pancollection/common/builder.py
+-rw-rw-rw-   0        0        0    14450 2023-06-09 05:14:41.000000 pancollection-0.2a0/pancollection/common/dataset.py
+-rw-rw-rw-   0        0        0     2238 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/common/dataset_hp.py
+-rw-rw-rw-   0        0        0    16414 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/common/evaluate.py
+-rw-rw-rw-   0        0        0     7163 2023-06-06 18:38:21.000000 pancollection-0.2a0/pancollection/common/psdata.py
+-rw-rw-rw-   0        0        0     4847 2023-03-30 10:19:53.000000 pancollection-0.2a0/pancollection/common/test_panloader.py
+-rw-rw-rw-   0        0        0     3965 2023-06-06 18:38:37.000000 pancollection-0.2a0/pancollection/common/train_panloader.py
+-rw-rw-rw-   0        0        0     3958 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/common/valid_panloader.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/configs/
+-rw-rw-rw-   0        0        0      336 2023-06-06 18:33:33.000000 pancollection-0.2a0/pancollection/configs/__init__.py
+-rw-rw-rw-   0        0        0     1151 2023-06-09 05:08:57.000000 pancollection-0.2a0/pancollection/configs/configs.py
+-rw-rw-rw-   0        0        0      824 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/configs/hook_configs.py
+-rw-rw-rw-   0        0        0     3078 2023-06-06 18:51:23.000000 pancollection-0.2a0/pancollection/configs/option_DCFNet.py
+-rw-rw-rw-   0        0        0     2927 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_LAGNet.py
+-rw-rw-rw-   0        0        0     2896 2023-06-06 18:51:14.000000 pancollection-0.2a0/pancollection/configs/option_bdpn.py
+-rw-rw-rw-   0        0        0     2811 2023-06-06 18:51:32.000000 pancollection-0.2a0/pancollection/configs/option_dicnn.py
+-rw-rw-rw-   0        0        0     2878 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_drpnn.py
+-rw-rw-rw-   0        0        0     3220 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_fusionnet.py
+-rw-rw-rw-   0        0        0     2921 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_msdcnn.py
+-rw-rw-rw-   0        0        0     3087 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_pannet.py
+-rw-rw-rw-   0        0        0     2865 2023-06-06 18:52:03.000000 pancollection-0.2a0/pancollection/configs/option_pnn.py
+-rw-rw-rw-   0        0        0      703 2023-06-09 05:02:24.000000 pancollection-0.2a0/pancollection/hug_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/ADKNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:55:31.000000 pancollection-0.2a0/pancollection/models/ADKNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/
+-rw-rw-rw-   0        0        0       18 2023-03-22 11:48:22.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/__init__.py
+-rw-rw-rw-   0        0        0    11638 2023-03-22 11:48:22.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/ddf.py
+-rw-rw-rw-   0        0        0     2289 2023-03-22 11:48:22.000000 pancollection-0.2a0/pancollection/models/ADKNet/ddf/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/BDPN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/BDPN/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-06-06 18:36:55.000000 pancollection-0.2a0/pancollection/models/BDPN/bdpn_main.py
+-rw-rw-rw-   0        0        0     7813 2023-06-09 05:15:23.000000 pancollection-0.2a0/pancollection/models/BDPN/model_bdpn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DCFNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DCFNet/__init__.py
+-rw-rw-rw-   0        0        0    32420 2023-06-09 05:14:16.000000 pancollection-0.2a0/pancollection/models/DCFNet/model_fcc_dense_head.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DHIFNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DHIFNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DRPNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DRPNN/__init__.py
+-rw-rw-rw-   0        0        0     3849 2023-06-06 18:36:22.000000 pancollection-0.2a0/pancollection/models/DRPNN/drpnn_main.py
+-rw-rw-rw-   0        0        0     5302 2023-06-09 05:15:15.000000 pancollection-0.2a0/pancollection/models/DRPNN/model_drpnn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/DiCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/DiCNN/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-06-06 18:35:36.000000 pancollection-0.2a0/pancollection/models/DiCNN/dicnn_main.py
+-rw-rw-rw-   0        0        0     3768 2023-06-09 05:14:16.000000 pancollection-0.2a0/pancollection/models/DiCNN/model_dicnn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/FusionNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/FusionNet/__init__.py
+-rw-rw-rw-   0        0        0     3501 2023-06-06 18:35:47.000000 pancollection-0.2a0/pancollection/models/FusionNet/fusionnet_main.py
+-rw-rw-rw-   0        0        0     5615 2023-06-09 05:14:50.000000 pancollection-0.2a0/pancollection/models/FusionNet/model_fusionnet.py
+-rw-rw-rw-   0        0        0      518 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/FusionNet/run_fusionnet.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/GPPNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/GPPNN/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/GPPNN/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/GPPNN/models/
+-rw-rw-rw-   0        0        0     4902 2023-06-09 06:05:48.000000 pancollection-0.2a0/pancollection/models/GPPNN/models/GPPNN.py
+-rw-rw-rw-   0        0        0      686 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/GPPNN/models/__init__.py
+-rw-rw-rw-   0        0        0    38742 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/GPPNN/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/LAGConv/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/LAGConv/__init__.py
+-rw-rw-rw-   0        0        0     2254 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/LAGConv/data.py
+-rw-rw-rw-   0        0        0     6962 2023-06-09 06:05:48.000000 pancollection-0.2a0/pancollection/models/LAGConv/model.py
+-rw-rw-rw-   0        0        0     1990 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/LAGConv/test.py
+-rw-rw-rw-   0        0        0     7423 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/models/LAGConv/train.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection/models/MSDCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/MSDCNN/__init__.py
+-rw-rw-rw-   0        0        0     5864 2023-06-09 06:05:48.000000 pancollection-0.2a0/pancollection/models/MSDCNN/model_msdcnn.py
+-rw-rw-rw-   0        0        0     3845 2023-06-06 18:37:05.000000 pancollection-0.2a0/pancollection/models/MSDCNN/msdcnn_main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/MUCNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/MUCNN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/
+-rw-rw-rw-   0        0        0       81 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/__init__.py
+-rw-rw-rw-   0        0        0      940 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/data.py
+-rw-rw-rw-   0        0        0     3897 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/datasets.py
+-rw-rw-rw-   0        0        0     5410 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/evaluate.py
+-rw-rw-rw-   0        0        0     3027 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/model.py
+-rw-rw-rw-   0        0        0     1328 2022-03-08 03:11:12.000000 pancollection-0.2a0/pancollection/models/MUCNN/lib/utils.py
+-rw-rw-rw-   0        0        0     3395 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/MUCNN/main_test_multi.py
+-rw-rw-rw-   0        0        0     2670 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/MUCNN/main_test_single.py
+-rw-rw-rw-   0        0        0     8936 2023-03-22 11:48:24.000000 pancollection-0.2a0/pancollection/models/MUCNN/train.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/PNN/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/PNN/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-09 05:14:58.000000 pancollection-0.2a0/pancollection/models/PNN/model_pnn.py
+-rw-rw-rw-   0        0        0     4390 2023-06-06 18:35:57.000000 pancollection-0.2a0/pancollection/models/PNN/pnn_main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:42.000000 pancollection-0.2a0/pancollection/models/PanNet/
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:54:54.000000 pancollection-0.2a0/pancollection/models/PanNet/__init__.py
+-rw-rw-rw-   0        0        0     4917 2023-06-09 05:15:07.000000 pancollection-0.2a0/pancollection/models/PanNet/model_pannet.py
+-rw-rw-rw-   0        0        0     3813 2023-06-06 18:36:06.000000 pancollection-0.2a0/pancollection/models/PanNet/pannet_main.py
+-rw-rw-rw-   0        0        0      508 2023-06-09 05:14:16.000000 pancollection-0.2a0/pancollection/models/__init__.py
+-rw-rw-rw-   0        0        0     3123 2023-06-09 05:14:26.000000 pancollection-0.2a0/pancollection/models/base_model.py
+-rw-rw-rw-   0        0        0      550 2023-06-09 05:08:57.000000 pancollection-0.2a0/pancollection/run_pansharpening.py
+-rw-rw-rw-   0        0        0      528 2023-03-27 06:21:37.000000 pancollection-0.2a0/pancollection/run_test_pansharpening.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/
+-rw-rw-rw-   0        0        0     5824 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3195 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 06:06:41.000000 pancollection-0.2a0/pancollection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:06:42.000000 pancollection-0.2a0/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2023-06-09 06:06:19.000000 pancollection-0.2a0/setup.py
```

### Comparing `pancollection-0.2/LICENSE` & `pancollection-0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/PKG-INFO` & `pancollection-0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.2
+Version: 0.2a0
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pancollection-0.2/README.md` & `pancollection-0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/common/builder.py` & `pancollection-0.2a0/pancollection/common/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) UESTC
 # All Rights Reserved 
 #
 # @Time    : 2022/9/16 22:10
 # @Author  : Xiao Wu
 # @reference: 
 #
-import udl.Basis.option
+import udl_vis.Basis.option
 
 def build_model(arch, task, cfg=None):
 
     if task == "pansharpening":
         from pancollection.models.base_model import PanSharpeningModel as MODELS
 
         return MODELS.build_model(cfg)
```

### Comparing `pancollection-0.2/pancollection/common/dataset.py` & `pancollection-0.2a0/pancollection/common/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import os
 # import datetime
 # import imageio
 import torch.nn.functional as F
 from scipy import io as sio
 from torch.utils.data import Dataset
-from udl.Basis.postprocess import showimage8
+from udl_vis.Basis.postprocess import showimage8
 import matplotlib.pyplot as plt
 # from UDL.Basis.zoom_image_region import show_region_images
 # from logging import info as log_string
 
 class Dataset_Pro(data.Dataset):
     def __init__(self, file_path, img_scale):
         super(Dataset_Pro, self).__init__()
```

### Comparing `pancollection-0.2/pancollection/common/dataset_hp.py` & `pancollection-0.2a0/pancollection/common/dataset_hp.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/common/evaluate.py` & `pancollection-0.2a0/pancollection/common/evaluate.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/common/psdata.py` & `pancollection-0.2a0/pancollection/common/psdata.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/common/test_panloader.py` & `pancollection-0.2a0/pancollection/common/test_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/common/train_panloader.py` & `pancollection-0.2a0/pancollection/common/train_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/common/valid_panloader.py` & `pancollection-0.2a0/pancollection/common/valid_panloader.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/configs.py` & `pancollection-0.2a0/pancollection/configs/configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import platform
 import warnings
-from udl.Basis.option import common_cfg
-from udl.Basis.python_sub_class import TaskDispatcher
+from udl_vis.Basis.option import common_cfg
+from udl_vis.Basis.python_sub_class import TaskDispatcher
 
 
 class panshaprening_cfg(TaskDispatcher, name='pansharpening'):
 
 
     def __init__(self, cfg=None, arch=None):
         super(panshaprening_cfg, self).__init__()
```

### Comparing `pancollection-0.2/pancollection/configs/hook_configs.py` & `pancollection-0.2a0/pancollection/configs/hook_configs.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_DCFNet.py` & `pancollection-0.2a0/pancollection/configs/option_DCFNet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_LAGNet.py` & `pancollection-0.2a0/pancollection/configs/option_LAGNet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_bdpn.py` & `pancollection-0.2a0/pancollection/configs/option_bdpn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_dicnn.py` & `pancollection-0.2a0/pancollection/configs/option_dicnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_drpnn.py` & `pancollection-0.2a0/pancollection/configs/option_drpnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_fusionnet.py` & `pancollection-0.2a0/pancollection/configs/option_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_msdcnn.py` & `pancollection-0.2a0/pancollection/configs/option_msdcnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_pannet.py` & `pancollection-0.2a0/pancollection/configs/option_pannet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/configs/option_pnn.py` & `pancollection-0.2a0/pancollection/configs/option_pnn.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/ADKNet/ddf/ddf.py` & `pancollection-0.2a0/pancollection/models/ADKNet/ddf/ddf.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/ADKNet/ddf/setup.py` & `pancollection-0.2a0/pancollection/models/ADKNet/ddf/setup.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/BDPN/bdpn_main.py` & `pancollection-0.2a0/pancollection/models/BDPN/bdpn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/BDPN/model_bdpn.py` & `pancollection-0.2a0/pancollection/models/BDPN/model_bdpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GPL License
 # Copyright (C) UESTC
 # All Rights Reserved
 # @Author  : Xiao Wu
 # @reference:
 import torch
 import torch.nn as nn
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 # from UDL.pansharpening.models import PanSharpeningModel
 
 # -------------Initialization----------------------------------------
 def init_weights(*modules):
     for module in modules:
         for m in module.modules():
             if isinstance(m, nn.Conv2d):   ## initialization for Conv2d
```

### Comparing `pancollection-0.2/pancollection/models/DCFNet/model_fcc_dense_head.py` & `pancollection-0.2a0/pancollection/models/DCFNet/model_fcc_dense_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from __future__ import print_function
 import os
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import optim
-from udl.Basis.criterion_metrics import SetCriterion
+from udl_vis.Basis.criterion_metrics import SetCriterion
 # from UDL.pansharpening.models import PanSharpeningModel
 from pancollection.models.base_model import PanSharpeningModel
 
 BN_MOMENTUM = 0.01
 
 def conv3x3(in_planes, out_planes, stride=1):
     """3x3 convolution with padding"""
```

### Comparing `pancollection-0.2/pancollection/models/DRPNN/drpnn_main.py` & `pancollection-0.2a0/pancollection/models/DRPNN/drpnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/DRPNN/model_drpnn.py` & `pancollection-0.2a0/pancollection/models/DRPNN/model_drpnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import math
 import torch.nn.init as int
 
 import torch
 import torch.nn as nn
 import math
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 # from UDL.pansharpening.models import PanSharpeningModel
 
 # -------------Initialization----------------------------------------
 def init_weights(*modules):
     for module in modules:
         for m in module.modules():
             if isinstance(m, nn.Conv2d):
```

### Comparing `pancollection-0.2/pancollection/models/DiCNN/dicnn_main.py` & `pancollection-0.2a0/pancollection/models/DiCNN/dicnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/DiCNN/model_dicnn.py` & `pancollection-0.2a0/pancollection/models/DiCNN/model_dicnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) UESTC
 # All Rights Reserved
 # @Author  : Xiao Wu
 # @reference:
 import torch
 import torch.nn as nn
 import math
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 # from UDL.pansharpening.models import PanSharpeningModel
 from pancollection.models.base_model import PanSharpeningModel
 
 # -------------Initialization----------------------------------------
 def init_weights(*modules):
     for module in modules:
         for m in module.modules():
```

### Comparing `pancollection-0.2/pancollection/models/FusionNet/fusionnet_main.py` & `pancollection-0.2a0/pancollection/models/FusionNet/fusionnet_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/FusionNet/model_fusionnet.py` & `pancollection-0.2a0/pancollection/models/FusionNet/model_fusionnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @reference:
 
 import torch
 import torch.nn as nn
 import numpy as np
 import math
 import torch.nn.init as int
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 
 
 class loss_with_l2_regularization(nn.Module):
     def __init__(self):
         super(loss_with_l2_regularization, self).__init__()
 
     def forward(self, criterion, model, weight_decay=1e-5, flag=False):
```

### Comparing `pancollection-0.2/pancollection/models/FusionNet/run_fusionnet.py` & `pancollection-0.2a0/pancollection/models/FusionNet/run_fusionnet.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/GPPNN/metrics.py` & `pancollection-0.2a0/pancollection/models/GPPNN/metrics.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/GPPNN/models/GPPNN.py` & `pancollection-0.2a0/pancollection/models/GPPNN/models/GPPNN.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
         
         for i in range(len(self.lr_blocks)):
             HR = self.lr_blocks[i](HR, ms)
             HR = self.pan_blocks[i](HR, pan)
             
         return HR  
 
-from UDL.Basis.python_sub_class import PanSharpeningModel
-from UDL.Basis.criterion_metrics import SetCriterion
+from pancollection.models import PanSharpeningModel
+from udl_vis.Basis.criterion_metrics import SetCriterion
 from torch import optim
 class build_model(PanSharpeningModel, name="GPPNN"):
     def __call__(self, args):
         if any(["wv" in v for v in args.dataset.values()]):
             spectral_num = 8
         else:
             spectral_num = 4
```

### Comparing `pancollection-0.2/pancollection/models/GPPNN/models/__init__.py` & `pancollection-0.2a0/pancollection/models/GPPNN/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/GPPNN/utils.py` & `pancollection-0.2a0/pancollection/models/GPPNN/utils.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/LAGConv/data.py` & `pancollection-0.2a0/pancollection/models/LAGConv/data.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/LAGConv/model.py` & `pancollection-0.2a0/pancollection/models/LAGConv/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         sr = self(lms, pan)
 
         return sr, gt
 
 
 
 from pancollection.models.base_model import PanSharpeningModel
-from pancollection.models.FusionNet.fusionnet_main import SetCriterion
+from udl_vis.Basis.criterion_metrics import SetCriterion
 from torch import optim
 
 class build_LAGNet(PanSharpeningModel, name='LAGNet'):
     def __call__(self, cfg):
         if any(["wv" in v for v in cfg.dataset.values()]):
             spectral_num = 8
         else:
```

### Comparing `pancollection-0.2/pancollection/models/LAGConv/test.py` & `pancollection-0.2a0/pancollection/models/LAGConv/test.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/LAGConv/train.py` & `pancollection-0.2a0/pancollection/models/LAGConv/train.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MSDCNN/model_msdcnn.py` & `pancollection-0.2a0/pancollection/models/MSDCNN/model_msdcnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GPL License
 # Copyright (C) UESTC
 # All Rights Reserved
 # @Author  : Xiao Wu
 # @reference:
 import torch
 from torch import nn
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 
 # -------------Initialization----------------------------------------
 def init_weights(*modules):
     for module in modules:
         for m in module.modules():
             if isinstance(m, nn.Conv2d):   ## initialization for Conv2d
                 # try:
@@ -122,10 +122,10 @@
 
 
 
 if __name__ == '__main__':
     lms = torch.randn([1, 8, 64, 64])
     pan = torch.randn([1, 1, 64, 64])
     ms = torch.randn([1, 8, 16, 16])
-    model = BDPN(8, None)
+    model = MSDCNN(8, None)
     x,_ = model(ms, pan)
     print(x.shape)
```

### Comparing `pancollection-0.2/pancollection/models/MSDCNN/msdcnn_main.py` & `pancollection-0.2a0/pancollection/models/MSDCNN/msdcnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/lib/data.py` & `pancollection-0.2a0/pancollection/models/MUCNN/lib/data.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/lib/datasets.py` & `pancollection-0.2a0/pancollection/models/MUCNN/lib/datasets.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/lib/evaluate.py` & `pancollection-0.2a0/pancollection/models/MUCNN/lib/evaluate.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/lib/model.py` & `pancollection-0.2a0/pancollection/models/MUCNN/lib/model.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/lib/utils.py` & `pancollection-0.2a0/pancollection/models/MUCNN/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/main_test_multi.py` & `pancollection-0.2a0/pancollection/models/MUCNN/main_test_multi.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/main_test_single.py` & `pancollection-0.2a0/pancollection/models/MUCNN/main_test_single.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/MUCNN/train.py` & `pancollection-0.2a0/pancollection/models/MUCNN/train.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/PNN/model_pnn.py` & `pancollection-0.2a0/pancollection/models/PNN/model_pnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All Rights Reserved
 # @Author  : Xiao Wu, LiangJian Deng
 # @reference:
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
 import math
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 # from UDL.pansharpening.models import PanSharpeningModel
 # from models.base_model import PanSharpeningModel
 
 class PNN(nn.Module):
     def __init__(self, spectral_num, criterion, channel=64):
         super(PNN, self).__init__()
```

### Comparing `pancollection-0.2/pancollection/models/PNN/pnn_main.py` & `pancollection-0.2a0/pancollection/models/PNN/pnn_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/PanNet/model_pannet.py` & `pancollection-0.2a0/pancollection/models/PanNet/model_pannet.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @reference:
 
 import torch
 import torch.nn as nn
 import numpy as np
 import math
 import torch.nn.init as int
-from udl.Basis.variance_sacling_initializer import variance_scaling_initializer
+from udl_vis.Basis.variance_sacling_initializer import variance_scaling_initializer
 # from UDL.pansharpening.models import PanSharpeningModel
 # from models.base_model import PanSharpeningModel
 
 # -------------Initialization----------------------------------------
 def init_weights(*modules):
     for module in modules:
         for m in module.modules():
```

### Comparing `pancollection-0.2/pancollection/models/PanNet/pannet_main.py` & `pancollection-0.2a0/pancollection/models/PanNet/pannet_main.py`

 * *Files identical despite different names*

### Comparing `pancollection-0.2/pancollection/models/base_model.py` & `pancollection-0.2a0/pancollection/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GPL License
 # Copyright (C) UESTC
 # All Rights Reserved
 # @Time    : 2023/3/27 13:40
 # @Author  : Xiao Wu
 # @reference:
-from udl.Basis.python_sub_class import ModelDispatcher
+from udl_vis.Basis.python_sub_class import ModelDispatcher
 import numpy as np
 import torch
 from torch.nn import functional as F
 from pancollection.common.evaluate import analysis_accu
 from pancollection.common.dataset import save_results
 
 class PanSharpeningModel(ModelDispatcher, name='pansharpening'):
```

### Comparing `pancollection-0.2/pancollection/run_pansharpening.py` & `pancollection-0.2a0/pancollection/run_test_pansharpening.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-# GPL License
-# Copyright (C) UESTC
-# All Rights Reserved 
-#
-# @Time    : 2022/4/25 0:17
-# @Author  : Xiao Wu
-# @reference:
-
-def run_demo():
-    from pancollection.configs.configs import TaskDispatcher
-    from udl.AutoDL.trainer import main
-    from pancollection.common.builder import build_model, getDataSession
-
-    cfg = TaskDispatcher.new(task='pansharpening', mode='entrypoint', arch='FusionNet')
-    print(TaskDispatcher._task.keys())
-    main(cfg, build_model, getDataSession)
+from configs.configs import TaskDispatcher
+from UDL.AutoDL.trainer import main
+from common.builder import build_model, getDataSession
 
 if __name__ == '__main__':
-    run_demo()
+    # cfg = parser_args()
+    cfg = TaskDispatcher.new(task='pansharpening', mode='entrypoint', arch='BDPN')
+    cfg.eval = True  # perform test on the dataset of wv3_multiExm.h5.
+    # cfg.dataset = {'train': 'wv3', 'valid': 'wv3_multiExm.h5'} #'wv3_OrigScale_multiExm1.h5'
+    print(TaskDispatcher._task.keys())
+    main(cfg, build_model, getDataSession)
```

### Comparing `pancollection-0.2/pancollection.egg-info/PKG-INFO` & `pancollection-0.2a0/pancollection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancollection
-Version: 0.2
+Version: 0.2a0
 Summary: PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pancollection-0.2/pancollection.egg-info/SOURCES.txt` & `pancollection-0.2a0/pancollection.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 pancollection/__init__.py
+pancollection/hug_demo.py
 pancollection/run_pansharpening.py
 pancollection/run_test_pansharpening.py
 pancollection.egg-info/PKG-INFO
 pancollection.egg-info/SOURCES.txt
 pancollection.egg-info/dependency_links.txt
 pancollection.egg-info/requires.txt
 pancollection.egg-info/top_level.txt
@@ -53,21 +54,14 @@
 pancollection/models/FusionNet/model_fusionnet.py
 pancollection/models/FusionNet/run_fusionnet.py
 pancollection/models/GPPNN/__init__.py
 pancollection/models/GPPNN/metrics.py
 pancollection/models/GPPNN/utils.py
 pancollection/models/GPPNN/models/GPPNN.py
 pancollection/models/GPPNN/models/__init__.py
-pancollection/models/GTP-PNet/__init__.py
-pancollection/models/GTP-PNet/model_P.py
-pancollection/models/GTP-PNet/model_T.py
-pancollection/models/GTP-PNet/test.py
-pancollection/models/GTP-PNet/train_P.py
-pancollection/models/GTP-PNet/train_T.py
-pancollection/models/GTP-PNet/utils.py
 pancollection/models/LAGConv/__init__.py
 pancollection/models/LAGConv/data.py
 pancollection/models/LAGConv/model.py
 pancollection/models/LAGConv/test.py
 pancollection/models/LAGConv/train.py
 pancollection/models/MSDCNN/__init__.py
 pancollection/models/MSDCNN/model_msdcnn.py
```

### Comparing `pancollection-0.2/setup.py` & `pancollection-0.2a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name='pancollection',
     description="PanCollection based on UDL (https://github.com/XiaoXiao-Woo/UDL)",
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="XiaoXiao-Woo",
     author_email="wxwsx1997@gmail.com",
     url='https://github.com/XiaoXiao-Woo/PanCollection',
-    version='0.2',
+    version='0.2a',
     include_package_data=True,
     packages=find_packages(),
     package_data={'pancollection': ['models/*']},
     license='GPLv3',
     python_requires='>=3.7',
     install_requires=[
         "psutil",
```

