# Comparing `tmp/deepdoctection-0.23.tar.gz` & `tmp/deepdoctection-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdoctection-0.23.tar", last modified: Sun May  7 17:40:46 2023, max compression
+gzip compressed data, was "deepdoctection-0.24.tar", last modified: Fri Jun  9 06:39:44 2023, max compression
```

## Comparing `deepdoctection-0.23.tar` & `deepdoctection-0.24.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.479299 deepdoctection-0.23/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.23/LICENSE
--rw-rw-r--   0 janis     (1000) janis     (1000)    10493 2023-05-07 17:40:46.479299 deepdoctection-0.23/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     9769 2023-05-07 15:01:33.000000 deepdoctection-0.23/README.md
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11864 2023-05-07 17:39:00.000000 deepdoctection-0.23/deepdoctection/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11612 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/analyzer/dd.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/configs/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/configs/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1032 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/configs/conf_dd_one.yaml
--rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/configs/conf_tesseract.yaml
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10039 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.23/deepdoctection/dataflow/custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15599 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/dataflow/serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/dataflow/stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19092 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datapoint/annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23301 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/datapoint/box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datapoint/convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    27037 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/datapoint/image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    28742 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/datapoint/view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7391 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datasets/adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datasets/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/dataflow_builder.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19410 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/info.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datasets/instances/doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/datasets/instances/fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.23/deepdoctection/datasets/instances/publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/datasets/instances/pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/datasets/instances/pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/xfund.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/datasets/instances/xsl/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/datasets/instances/xsl/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
--rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/save.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.23/deepdoctection/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    16253 2023-02-23 18:53:18.000000 deepdoctection-0.23/deepdoctection/eval/eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/eval/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/eval/tedsmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/tp_eval_callback.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11828 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11010 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/extern/d2detect.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12381 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/extern/doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/extern/hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    39080 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    46200 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/extern/model.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/pdftext.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/pt/
--rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/pt/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.23/deepdoctection/extern/pt/ptutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12369 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/extern/texocr.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.23/deepdoctection/extern/tp/tfutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpcompat.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/common.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/config.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/predict.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/preproc.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/extern/tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.23/deepdoctection/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14674 2023-02-20 09:20:02.000000 deepdoctection-0.23/deepdoctection/mapper/cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6866 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/mapper/hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    33982 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/maputils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/match.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.23/deepdoctection/mapper/pascalstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.23/deepdoctection/mapper/prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23607 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1100 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13801 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/pipe/anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13221 2023-04-11 09:55:32.000000 deepdoctection-0.23/deepdoctection/pipe/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10805 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/pipe/cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14447 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9425 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8816 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/doctectionpipe.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6075 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4589 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/pipe/layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/pipe/lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    22256 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.23/deepdoctection/pipe/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    47806 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/pipe/segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    29038 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/pipe/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/py.typed
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/train/d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/train/hf_detr_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19404 2023-02-03 14:03:14.000000 deepdoctection-0.23/deepdoctection/train/hf_layoutlm_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/train/tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.23/deepdoctection/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.23/deepdoctection/utils/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/context.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.23/deepdoctection/utils/detection_types.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/develop.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/utils/file_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.23/deepdoctection/utils/fs.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/utils/identifier.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/logger.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/metacfg.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/pdf_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/utils/settings.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/systools.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.23/deepdoctection/utils/tqdm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/utils/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.23/deepdoctection/utils/utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9216 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/utils/viz.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection.egg-info/
--rw-rw-r--   0 janis     (1000) janis     (1000)    10493 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     7904 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/SOURCES.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/dependency_links.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/requires.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/top_level.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2346 2023-05-07 17:40:46.479299 deepdoctection-0.23/setup.cfg
--rw-rw-r--   0 janis     (1000) janis     (1000)     6406 2023-05-07 17:40:38.000000 deepdoctection-0.23/setup.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/tests/
--rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.23/tests/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/tests/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5142 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/analyzer/test_dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-05-03 16:43:31.000000 deepdoctection-0.23/tests/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.23/tests/data.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/tests/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/dataflow/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/dataflow/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.23/tests/datapoint/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/datapoint/test_annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/datapoint/test_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/datapoint/test_convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/datapoint/test_image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/datapoint/test_view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datasets/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datasets/instances/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.23/tests/datasets/instances/test_doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/datasets/instances/test_funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/datasets/instances/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/datasets/instances/test_layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/datasets/instances/test_pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.23/tests/datasets/test_adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/datasets/test_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/datasets/test_registry.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/eval/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/eval/test_accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/eval/test_cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/eval/test_eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/eval/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/eval/test_tedsmetric.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/extern/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/extern/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.23/tests/extern/test_deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4973 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/extern/test_doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/extern/test_fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/extern/test_hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/extern/test_hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/extern/test_pdftext.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/extern/test_tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/extern/test_texocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/extern/test_tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/mapper/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10530 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/mapper/test_cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/mapper/test_cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/mapper/test_d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/mapper/test_hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/mapper/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5504 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/mapper/test_prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/mapper/test_pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/mapper/test_tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.23/tests/pipe/test_anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/pipe/test_cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.23/tests/pipe/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3049 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/pipe/test_language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.23/tests/pipe/test_layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/pipe/test_lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/pipe/test_refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/pipe/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/pipe/test_segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9811 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/pipe/test_text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.23/tests/pipe/test_transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/test_utils.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/train/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/train/test_d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/train/test_tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.479299 deepdoctection-0.23/tests_d2/
--rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests_d2/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.23/tests_d2/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests_d2/test_d2detect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.24/LICENSE
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10917 2023-06-09 06:39:44.115722 deepdoctection-0.24/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10193 2023-06-09 06:36:46.000000 deepdoctection-0.24/README.md
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11864 2023-06-09 06:36:56.000000 deepdoctection-0.24/deepdoctection/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11612 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/analyzer/dd.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/configs/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/configs/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1032 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/configs/conf_dd_one.yaml
+-rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/configs/conf_tesseract.yaml
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10039 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.24/deepdoctection/dataflow/custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15599 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/dataflow/serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/dataflow/stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2023-06-01 11:26:25.000000 deepdoctection-0.24/deepdoctection/datapoint/annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23301 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/datapoint/box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/datapoint/convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    27294 2023-05-23 14:43:35.000000 deepdoctection-0.24/deepdoctection/datapoint/image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    29405 2023-06-08 09:26:52.000000 deepdoctection-0.24/deepdoctection/datapoint/view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7421 2023-06-06 08:01:17.000000 deepdoctection-0.24/deepdoctection/datasets/adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/datasets/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/dataflow_builder.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20603 2023-05-31 17:59:53.000000 deepdoctection-0.24/deepdoctection/datasets/info.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/datasets/instances/doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/datasets/instances/fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.24/deepdoctection/datasets/instances/publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/datasets/instances/pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/datasets/instances/pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/xfund.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/datasets/instances/xsl/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/datasets/instances/xsl/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/save.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.24/deepdoctection/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19345 2023-06-04 08:35:17.000000 deepdoctection-0.24/deepdoctection/eval/eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/eval/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/eval/tedsmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/tp_eval_callback.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11828 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11010 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/extern/d2detect.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12381 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/extern/doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/extern/hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    39423 2023-06-06 08:40:23.000000 deepdoctection-0.24/deepdoctection/extern/hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    46200 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/extern/model.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/pdftext.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/pt/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/pt/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.24/deepdoctection/extern/pt/ptutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12369 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/extern/texocr.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.24/deepdoctection/extern/tp/tfutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpcompat.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/common.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/config.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/predict.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/preproc.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/extern/tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.24/deepdoctection/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15505 2023-06-05 15:22:36.000000 deepdoctection-0.24/deepdoctection/mapper/cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8536 2023-06-06 09:46:17.000000 deepdoctection-0.24/deepdoctection/mapper/d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/mapper/hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    35638 2023-05-31 17:59:53.000000 deepdoctection-0.24/deepdoctection/mapper/laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/maputils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/match.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/mapper/misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.24/deepdoctection/mapper/pascalstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.24/deepdoctection/mapper/prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23583 2023-05-30 11:17:24.000000 deepdoctection-0.24/deepdoctection/mapper/pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/mapper/tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1100 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13801 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/pipe/anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13245 2023-05-31 12:44:11.000000 deepdoctection-0.24/deepdoctection/pipe/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11062 2023-05-23 14:43:35.000000 deepdoctection-0.24/deepdoctection/pipe/cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14447 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9425 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8816 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/doctectionpipe.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6075 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4589 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/pipe/layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/pipe/lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22256 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.24/deepdoctection/pipe/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    47806 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/pipe/segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    29451 2023-06-04 09:02:46.000000 deepdoctection-0.24/deepdoctection/pipe/text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/pipe/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/py.typed
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/train/d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/train/hf_detr_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    21125 2023-06-04 08:51:52.000000 deepdoctection-0.24/deepdoctection/train/hf_layoutlm_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/train/tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.24/deepdoctection/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.24/deepdoctection/utils/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/context.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.24/deepdoctection/utils/detection_types.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/develop.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/utils/file_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.24/deepdoctection/utils/fs.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/utils/identifier.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/logger.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/metacfg.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/pdf_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/utils/settings.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/systools.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.24/deepdoctection/utils/tqdm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/utils/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.24/deepdoctection/utils/utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10115 2023-06-04 09:03:45.000000 deepdoctection-0.24/deepdoctection/utils/viz.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection.egg-info/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10917 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7904 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/SOURCES.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/dependency_links.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/requires.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/top_level.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2368 2023-06-09 06:39:44.115722 deepdoctection-0.24/setup.cfg
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6406 2023-06-09 06:38:44.000000 deepdoctection-0.24/setup.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.091722 deepdoctection-0.24/tests/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.24/tests/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.091722 deepdoctection-0.24/tests/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5142 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/analyzer/test_dd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-05-03 16:43:31.000000 deepdoctection-0.24/tests/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.24/tests/data.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.091722 deepdoctection-0.24/tests/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/dataflow/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/dataflow/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.095722 deepdoctection-0.24/tests/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.24/tests/datapoint/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/datapoint/test_annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/datapoint/test_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/datapoint/test_convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/datapoint/test_image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/datapoint/test_view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.095722 deepdoctection-0.24/tests/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datasets/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.099722 deepdoctection-0.24/tests/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datasets/instances/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.24/tests/datasets/instances/test_doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/datasets/instances/test_funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/datasets/instances/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/datasets/instances/test_layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/datasets/instances/test_pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.24/tests/datasets/test_adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/datasets/test_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/datasets/test_registry.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.103722 deepdoctection-0.24/tests/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/eval/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/eval/test_accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/eval/test_cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/eval/test_eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/eval/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/eval/test_tedsmetric.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.107722 deepdoctection-0.24/tests/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/extern/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/extern/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.24/tests/extern/test_deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4973 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/extern/test_doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/extern/test_fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/extern/test_hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/extern/test_hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/extern/test_pdftext.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/extern/test_tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/extern/test_texocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/extern/test_tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.111722 deepdoctection-0.24/tests/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/mapper/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-06-05 12:09:33.000000 deepdoctection-0.24/tests/mapper/test_cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/mapper/test_cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/mapper/test_d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/mapper/test_hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/mapper/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5556 2023-05-31 18:16:38.000000 deepdoctection-0.24/tests/mapper/test_laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/test_misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/mapper/test_prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/mapper/test_pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/mapper/test_tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/test_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/test_xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/tests/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.24/tests/pipe/test_anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/pipe/test_cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.24/tests/pipe/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3049 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/pipe/test_language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.24/tests/pipe/test_layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/pipe/test_lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/pipe/test_refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/pipe/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/pipe/test_segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9811 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/pipe/test_text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.24/tests/pipe/test_transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/test_utils.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/tests/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/train/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/train/test_d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/train/test_tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/tests_d2/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests_d2/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.24/tests_d2/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests_d2/test_d2detect.py
```

### Comparing `deepdoctection-0.23/LICENSE` & `deepdoctection-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/PKG-INFO` & `deepdoctection-0.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.23
+Version: 0.24
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -52,16 +52,20 @@
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
    provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). Check the notebook repo or 
-   the documentation on how to train a model on your custom task or how to setup a pipeline.
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). 
+
+   [**!new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE) 
+   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v1_on_custom_token_classification.ipynb)
+   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3. Training 
+   scripts can now be tracked with W&B. Check the experimentation result of the notebooks [here](https://wandb.ai/jm76/FRFPE_layoutlmv1?workspace=user-jm76).
  - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself.
```

### Comparing `deepdoctection-0.23/README.md` & `deepdoctection-0.24/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,20 @@
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
    provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). Check the notebook repo or 
-   the documentation on how to train a model on your custom task or how to setup a pipeline.
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). 
+
+   [**!new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE) 
+   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v1_on_custom_token_classification.ipynb)
+   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3. Training 
+   scripts can now be tracked with W&B. Check the experimentation result of the notebooks [here](https://wandb.ai/jm76/FRFPE_layoutlmv1?workspace=user-jm76).
  - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself.
```

### Comparing `deepdoctection-0.23/deepdoctection/__init__.py` & `deepdoctection-0.24/deepdoctection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import TYPE_CHECKING
 
 from packaging import version
 
 from .utils.file_utils import _LazyModule, get_tf_version, pytorch_available, tf_available
 from .utils.logger import logger
 
-__version__ = 0.23
+__version__ = 0.24
 
 _IMPORT_STRUCTURE = {
     "analyzer": ["get_dd_analyzer", "build_analyzer"],
     "configs": [],
     "dataflow": [
         "DataFlowTerminated",
         "DataFlowResetStateNotCalled",
```

### Comparing `deepdoctection-0.23/deepdoctection/analyzer/__init__.py` & `deepdoctection-0.24/deepdoctection/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/analyzer/dd.py` & `deepdoctection-0.24/deepdoctection/analyzer/dd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/configs/__init__.py` & `deepdoctection-0.24/deepdoctection/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/configs/conf_dd_one.yaml` & `deepdoctection-0.24/deepdoctection/configs/conf_dd_one.yaml`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/__init__.py` & `deepdoctection-0.24/deepdoctection/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/base.py` & `deepdoctection-0.24/deepdoctection/dataflow/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/common.py` & `deepdoctection-0.24/deepdoctection/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/custom.py` & `deepdoctection-0.24/deepdoctection/dataflow/custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/custom_serialize.py` & `deepdoctection-0.24/deepdoctection/dataflow/custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/parallel_map.py` & `deepdoctection-0.24/deepdoctection/dataflow/parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/serialize.py` & `deepdoctection-0.24/deepdoctection/dataflow/serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/dataflow/stats.py` & `deepdoctection-0.24/deepdoctection/dataflow/stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datapoint/__init__.py` & `deepdoctection-0.24/deepdoctection/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datapoint/annotation.py` & `deepdoctection-0.24/deepdoctection/datapoint/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         self._assert_attributes_have_str(state_id=True)
         super().__post_init__()
 
     def dump_sub_category(
         self, sub_category_name: TypeOrStr, annotation: "CategoryAnnotation", *container_id_context: Optional[str]
     ) -> None:
         """
-        Storage of sub-categories. Since sub-categories usually only depend on very few attributes and the parent
+        Storage of sub-categories. As sub-categories usually only depend on very few attributes and the parent
         category cannot yet be stored in a comprehensive container, it is possible to include a context of the
         annotation id in order to ensure that the sub-category annotation id is unambiguously created.
 
         :param sub_category_name: key for defining the sub category.
         :param annotation: Annotation instance to dump
         :param container_id_context: Tuple/list of context ids.
         """
```

### Comparing `deepdoctection-0.23/deepdoctection/datapoint/box.py` & `deepdoctection-0.24/deepdoctection/datapoint/box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datapoint/convert.py` & `deepdoctection-0.24/deepdoctection/datapoint/convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datapoint/image.py` & `deepdoctection-0.24/deepdoctection/datapoint/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 Dataclass Image
 """
 import json
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Union, no_type_check
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Union, no_type_check
 
 import numpy as np
 from numpy import uint8
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
 from ..utils.identifier import get_uuid, is_uuid_like
 from ..utils.settings import ObjectTypes, get_type
@@ -514,14 +514,15 @@
         :param kwargs: dict with  `Image` attributes and nested dicts for initializing annotations,
         :return: Initialized image
         """
         image = cls(kwargs.get("file_name"), kwargs.get("location"), kwargs.get("external_id"))
         image._image_id = kwargs.get("_image_id")
         _image = kwargs.get("_image")
         image.page_number = int(kwargs.get("page_number", 0))
+        image.document_id = kwargs.get("document_id", image._image_id)
         if _image is not None:
             image.image = _image
         if box_kwargs := kwargs.get("_bbox"):
             image._bbox = BoundingBox.from_dict(**box_kwargs)
         for image_id, box_dict in kwargs.get("embeddings").items():
             image.set_embedding(image_id, BoundingBox.from_dict(**box_dict))
         for ann_dict in kwargs.get("annotations"):
@@ -628,7 +629,11 @@
         if image_to_json and self.image is not None:
             export_dict["_image"] = convert_np_array_to_b64(self.image)
         if dry:
             return export_dict
         with open(path_json, "w", encoding="UTF-8") as file:
             json.dump(export_dict, file, indent=2)
         return None
+
+    def get_categories_from_current_state(self) -> Set[str]:
+        """Returns all active dumped categories"""
+        return {ann.category_name for ann in self.get_annotation()}
```

### Comparing `deepdoctection-0.23/deepdoctection/datapoint/view.py` & `deepdoctection-0.24/deepdoctection/datapoint/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,32 +243,42 @@
                 html_list.insert(html_index, cell.text)  # type: ignore
             except ValueError:
                 logger.warning("html construction not possible due to ValueError in: %s", cell.annotation_id)
 
         return "".join(html_list)
 
     def get_attribute_names(self) -> Set[str]:
-        return set(TableType).union(super().get_attribute_names()).union({"cells", "rows", "columns", "html"})
+        return (
+            set(TableType)
+            .union(super().get_attribute_names())
+            .union({"cells", "rows", "columns", "html", "csv", "text"})
+        )
 
     @property
     def csv(self) -> List[List[str]]:
         """Returns a csv-style representation of a table as list of lists of string. Cell content of cell with higher
         row or column spans will be shown at the upper left cell tile. All other tiles covered by the cell will be left
         as blank
         """
         cells = self.cells
         table_list = [["" for _ in range(self.number_of_columns)] for _ in range(self.number_of_rows)]  # type: ignore
         for cell in cells:
-            table_list[cell.row_number - 1][cell.column_number - 1] = cell.text  # type: ignore
+            table_list[cell.row_number - 1][cell.column_number - 1] = (  # type: ignore
+                table_list[cell.row_number - 1][cell.column_number - 1] + cell.text  # type: ignore
+            )
         return table_list
 
     def __str__(self) -> str:
         out = " ".join([" ".join(row + ["\n"]) for row in self.csv])
         return out
 
+    @property
+    def text(self) -> str:
+        return str(self)
+
 
 IMAGE_ANNOTATION_TO_LAYOUTS: Dict[ObjectTypes, Type[Union[Layout, Table, Word]]] = {
     **{i: Layout for i in LayoutType if (i not in {LayoutType.table, LayoutType.word, LayoutType.cell})},
     LayoutType.table: Table,
     LayoutType.word: Word,
     LayoutType.cell: Cell,
     CellType.projected_row_header: Cell,
@@ -503,20 +513,22 @@
         linebreak = "\n" if block_name == "layouts" else " "
         for block in block_with_order:
             block_attr = "text" if not isinstance(block, Word) else "characters"
             text += f"{linebreak}{getattr(block, block_attr)}"
         return text
 
     @property
-    def chunks(self) -> List[Tuple[str, str, str, str, str, str]]:
+    def chunks(self) -> List[Tuple[str, str, int, str, str, str, str]]:
         """
         :return: Returns a "chunk" of a layout element or a table as 6-tuple containing
 
                     - document id
                     - image id
+                    - page number
+                    - annotation_id
                     - reading order
                     - category name
                     - text string
 
         """
         block_with_order = self._order("layouts")
         for table in self.tables:
@@ -524,14 +536,15 @@
                 block_with_order.append(table)
         all_chunks = []
         for chunk in block_with_order:
             all_chunks.append(
                 (
                     self.document_id,
                     self.image_id,
+                    self.page_number,
                     chunk.annotation_id,
                     chunk.reading_order,
                     chunk.category_name,
                     chunk.text,
                 )
             )
         return all_chunks  # type: ignore
@@ -584,20 +597,20 @@
         category_names_list: List[Union[str, None]] = []
         box_stack = []
         cells_found = False
 
         if show_layouts:
             for item in self.layouts:
                 box_stack.append(item.bbox)
-                category_names_list.append(item.category_name)
+                category_names_list.append(item.category_name.value)
 
         if show_tables:
             for table in self.tables:
                 box_stack.append(table.bbox)
-                category_names_list.append(LayoutType.table)
+                category_names_list.append(LayoutType.table.value)
                 if show_cells:
                     for cell in table.cells:
                         if cell.category_name in {
                             LayoutType.cell,
                             CellType.projected_row_header,
                             CellType.spanning,
                             CellType.row_header,
@@ -622,32 +635,34 @@
                     box_stack.append(ann.bbox)
                     category_names_list.append(None)
 
         if show_words:
             all_words = []
             for layout in self.layouts:
                 all_words.extend(layout.words)
+            if not all_words:
+                all_words = self.get_annotation(category_names=LayoutType.word)
             for word in all_words:
                 box_stack.append(word.bbox)
                 if show_token_class:
-                    category_names_list.append(str(word.token_class).replace("TokenClasses", ""))
+                    category_names_list.append(word.token_class.value)
                 else:
-                    category_names_list.append(str(word.token_tag))
+                    category_names_list.append(word.token_tag.value)
+
 
         if self.image is not None:
             if box_stack:
                 boxes = np.vstack(box_stack)
                 if show_words:
                     img = draw_boxes(
                         self.image,
                         boxes,
                         category_names_list,
-                        color=(255, 222, 173),
                         font_scale=0.25,
-                        rectangle_thickness=1,
+                        rectangle_thickness=4,
                     )
                 else:
                     img = draw_boxes(self.image, boxes, category_names_list)
                 img = cv2.resize(img, None, fx=1.3, fy=1.3, interpolation=cv2.INTER_CUBIC)
             else:
                 img = self.image
 
@@ -658,15 +673,28 @@
         return None
 
     @staticmethod
     def get_attribute_names() -> Set[str]:
         """
         :return: A set of registered attributes.
         """
-        return set(PageType).union({"text", "tables", "layouts", "words", "residual_words"})
+        return set(PageType).union(
+            {
+                "text",
+                "chunks",
+                "tables",
+                "layouts",
+                "words",
+                "residual_words",
+                "file_name",
+                "location",
+                "document_id",
+                "page_number",
+            }
+        )
 
     def save(
         self,
         image_to_json: bool = True,
         highest_hierarchy_only: bool = False,
         path: Optional[Pathlike] = None,
         dry: bool = False,
```

### Comparing `deepdoctection-0.23/deepdoctection/datasets/__init__.py` & `deepdoctection-0.24/deepdoctection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/adapter.py` & `deepdoctection-0.24/deepdoctection/datasets/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                         anns = dp.get_annotation()
                         cat_ids = [int(ann.category_id) for ann in anns]
 
                     elif self.dataset.dataset_info.type == DatasetType.sequence_classification:
                         cat_ids = dp.summary.get_sub_category(PageType.document_type).category_id
 
                     elif self.dataset.dataset_info.type == DatasetType.token_classification:
-                        anns = dp.get_annotation()
+                        anns = dp.get_annotation(category_names=LayoutType.word)
                         if use_token_tag:
                             cat_ids = [ann.get_sub_category(WordType.token_tag).category_id for ann in anns]
                         else:
                             cat_ids = [ann.get_sub_category(WordType.token_class).category_id for ann in anns]
 
                     if _data_statistics:
                         summarizer.dump(cat_ids)
```

### Comparing `deepdoctection-0.23/deepdoctection/datasets/base.py` & `deepdoctection-0.24/deepdoctection/datasets/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/dataflow_builder.py` & `deepdoctection-0.24/deepdoctection/datasets/dataflow_builder.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/info.py` & `deepdoctection-0.24/deepdoctection/datasets/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 Module for storing dataset info (e.g. general meta data or categories)
 """
 
 from copy import copy
 from dataclasses import dataclass, field
 from itertools import chain
-from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence, Set, Union, overload
+from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence, Set, Union, no_type_check, overload
 
 from ..utils.settings import DefaultType, ObjectTypes, TypeOrStr, get_type
 from ..utils.utils import call_only_once
 
 __all__ = ["DatasetInfo", "DatasetCategories", "get_merged_categories"]
 
 
@@ -226,15 +226,15 @@
             _categories = self.get_categories(as_dict=False, filtered=True)
             if _categories is None:
                 _categories = []
         if sub_categories is None:
             sub_categories = {}
 
         sub_cat: Dict[ObjectTypes, Union[ObjectTypes, List[ObjectTypes]]] = {}
-        for cat in _categories:  # pylint: disable=R1702
+        for cat in _categories:
             assert cat in self.get_categories(  # pylint: disable=E1135
                 as_dict=False, filtered=True
             ), f"{cat} not in categories. Maybe it has been replaced with sub category"
             sub_cat_dict = self.init_sub_categories.get(cat)
             if sub_cat_dict is None:
                 if self._cat_to_sub_cat:
                     for key, val in self._cat_to_sub_cat.items():
@@ -366,14 +366,15 @@
         return False
 
     def _init_sanity_check(self) -> None:
         # all values of possible sub categories must be listed
         assert all(isinstance(val, dict) for val in self.init_sub_categories.values())
 
 
+@no_type_check
 def get_merged_categories(*categories: DatasetCategories) -> DatasetCategories:
     """
     Given a set of `DatasetCategories`, a `DatasetCategories` instance will be returned that summarize the category
     properties of merged dataset. This means it will save the union of all possible categories as its init categories.
     Regarding sub categories, only those will be accessible if and only if they are a sub category of a category for all
     merged datasets. E.g. if dataset A has category `foo` with sub category `foo`:`bak` and dataset B has category `foo`
     as well but no sub category than the merged dataset will have no sub categories at all. Whereas in a similar setting
@@ -416,13 +417,31 @@
         for sub_cat_key in intersect_sub_cat_per_key:
             val: Set[ObjectTypes] = set()
             for cat in categories:
                 val.update(cat.init_sub_categories[key][sub_cat_key])
             intersect_init_sub_cat_values[sub_cat_key] = list(val)
         intersect_init_sub_cat[key] = intersect_init_sub_cat_values
 
+    # Building sub cats such that the result is deterministic. Because we use sets in several occasions above the
+    # construction is not deterministic but guarantees for unique values in all sub categories. Now we build the
+    # ensemble dict of sub categories where we guarantee unique values on one hand side and always maintain the
+    # same arrangements for all category/ sub category lists
+    init_sub_cat: Dict[ObjectTypes, Any] = {}
+    for category in categories:
+        for cat in intersect_sub_cat_keys:
+            for sub_cat_key in category.init_sub_categories[cat]:
+                if sub_cat_key in intersect_init_sub_cat[cat]:
+                    for sub_cat_val in category.init_sub_categories[cat][sub_cat_key]:
+                        if sub_cat_val in intersect_init_sub_cat[cat][sub_cat_key]:
+                            if cat not in init_sub_cat:
+                                init_sub_cat[cat] = {}
+                            if sub_cat_key not in init_sub_cat[cat]:
+                                init_sub_cat[cat][sub_cat_key] = [sub_cat_val]
+                            else:
+                                init_sub_cat[cat][sub_cat_key].append(sub_cat_val)
+
     # Next, build the DatasetCategories instance.
-    merged_categories = DatasetCategories(init_categories=init_categories, init_sub_categories=intersect_init_sub_cat)
+    merged_categories = DatasetCategories(init_categories=init_categories, init_sub_categories=init_sub_cat)
     merged_categories._categories_update = categories_update  # pylint: disable = W0212
     merged_categories._allow_update = False  # pylint: disable = W0212
     setattr(merged_categories, "_categories_filter_update", categories_filtered)
     return merged_categories
```

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/__init__.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/doclaynet.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/fintabnet.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/funsd.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/iiitar13k.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/layouttest.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/publaynet.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/pubtables1m.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/pubtabnet.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/rvlcdip.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/xfund.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/xfund.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/xsl/__init__.py` & `deepdoctection-0.24/deepdoctection/datasets/instances/xsl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/instances/xsl/pascal_voc.xsl` & `deepdoctection-0.24/deepdoctection/datasets/instances/xsl/pascal_voc.xsl`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/registry.py` & `deepdoctection-0.24/deepdoctection/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/datasets/save.py` & `deepdoctection-0.24/deepdoctection/datasets/save.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/__init__.py` & `deepdoctection-0.24/deepdoctection/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/accmetric.py` & `deepdoctection-0.24/deepdoctection/eval/accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/base.py` & `deepdoctection-0.24/deepdoctection/eval/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/cocometric.py` & `deepdoctection-0.24/deepdoctection/eval/cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/eval.py` & `deepdoctection-0.24/deepdoctection/eval/eval.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from ..pipe.base import LanguageModelPipelineComponent, PredictorPipelineComponent
 from ..pipe.common import PageParsingService
 from ..pipe.concurrency import MultiThreadPipelineComponent
 from ..pipe.doctectionpipe import DoctectionPipe
 from ..utils.detection_types import ImageType
 from ..utils.file_utils import detectron2_available, wandb_available
 from ..utils.logger import logger
-from ..utils.settings import DatasetType, LayoutType, TypeOrStr
+from ..utils.settings import DatasetType, LayoutType, TypeOrStr, get_type
 from ..utils.viz import interactive_imshow
 from .base import MetricBase
 
 if wandb_available():
     import wandb  # pylint:disable=W0611
     from wandb import Artifact, Table
 
@@ -134,17 +134,47 @@
         if not isinstance(metric, MetricBase):
             self.metric = self.metric()  # type: ignore
 
         self._sanity_checks()
 
         self.wandb_table_agent: Optional[WandbTableAgent]
         if run is not None:
-            self.wandb_table_agent = WandbTableAgent(
-                run, self.dataset.dataset_info.name, 50, self.dataset.dataflow.categories.get_categories(filtered=True)
-            )
+            if self.dataset.dataset_info.type == DatasetType.object_detection:
+                self.wandb_table_agent = WandbTableAgent(
+                    run,
+                    self.dataset.dataset_info.name,
+                    50,
+                    self.dataset.dataflow.categories.get_categories(filtered=True),
+                )
+            elif self.dataset.dataset_info.type == DatasetType.token_classification:
+                if hasattr(self.metric, "sub_cats"):
+                    sub_cat_key, sub_cat_val_list = list(self.metric.sub_cats.items())[0]  # type: ignore
+                    sub_cat_val = sub_cat_val_list[0]
+                    sub_cats = {sub_cat_key: sub_cat_val}
+                    self.wandb_table_agent = WandbTableAgent(
+                        run,
+                        self.dataset.dataset_info.name,
+                        50,
+                        self.dataset.dataflow.categories.get_categories(filtered=True),
+                        self.dataset.dataflow.categories.get_sub_categories(
+                            categories=sub_cat_key,
+                            sub_categories=sub_cats,
+                            keys=False,
+                            values_as_dict=True,
+                            name_as_key=False,
+                        )[sub_cat_key][sub_cat_val],
+                        sub_cats,
+                    )
+                else:
+                    raise AttributeError(
+                        "metric has no attribute sub_cats and cannot be used for token classification " "datasets"
+                    )
+            else:
+                raise NotImplementedError
+
         else:
             self.wandb_table_agent = None
 
     @overload
     def run(
         self, output_as_dict: Literal[False] = False, **dataflow_build_kwargs: Union[str, int]
     ) -> List[Dict[str, float]]:
@@ -239,27 +269,34 @@
             sub_cats_to_remove = meta_anns["sub_categories"]
             df_pr = MapData(df_pr, remove_cats(sub_categories=sub_cats_to_remove))
         else:
             raise NotImplementedError
 
         return df_pr
 
-    def compare(self, interactive: bool = False, **dataflow_build_kwargs: Union[str, int]) -> Optional[ImageType]:
+    def compare(self, interactive: bool = False, **kwargs: Union[str, int]) -> Optional[ImageType]:
         """
         Visualize ground truth and prediction datapoint. Given a dataflow config it will run predictions per sample
         and concat the prediction image (with predicted bounding boxes) with ground truth image.
 
         :param interactive: If set to True will open an interactive image, otherwise it will return a numpy array that
                             can be displayed differently (e.g. matplotlib). Note that, if the interactive mode is being
                             used, more than one sample can be iteratively be displayed.
-        :param dataflow_build_kwargs: Dataflow configs for displaying specific image splits
+        :param kwargs: Dataflow configs for displaying specific image splits and visualisation configs:
+                       `show_tables`, `show_layouts`, `show_table_structure`, `show_words`
         :return: Image as numpy array
         """
-        df_gt = self.dataset.dataflow.build(**dataflow_build_kwargs)
-        df_pr = self.dataset.dataflow.build(**dataflow_build_kwargs)
+
+        show_tables = kwargs.pop("show_tables", True)
+        show_layouts = kwargs.pop("show_layouts", True)
+        show_table_structure = kwargs.pop("show_table_structure", True)
+        show_words = kwargs.pop("show_words", False)
+
+        df_gt = self.dataset.dataflow.build(**kwargs)
+        df_pr = self.dataset.dataflow.build(**kwargs)
         df_gt = MapData(df_gt, maybe_load_image)
         df_pr = MapData(df_pr, maybe_load_image)
         df_pr = MapData(df_pr, deepcopy)
         df_pr = self._clean_up_predict_dataflow_annotations(df_pr)
 
         page_parsing_component = PageParsingService(
             text_container=LayoutType.word,
@@ -282,15 +319,25 @@
             df_pr = self.pipe.analyze(dataset_dataflow=df_pr)
         else:
             raise ValueError("Neither pipe_component nor pipe has been defined")
 
         df_pr.reset_state()
         df_gt.reset_state()
         for dp_gt, dp_pred in zip(df_gt, df_pr):
-            img_gt, img_pred = dp_gt.viz(), dp_pred.viz()
+            img_gt, img_pred = dp_gt.viz(
+                show_tables=show_tables,
+                show_layouts=show_layouts,
+                show_table_structure=show_table_structure,
+                show_words=show_words,
+            ), dp_pred.viz(
+                show_tables=show_tables,
+                show_layouts=show_layouts,
+                show_table_structure=show_table_structure,
+                show_words=show_words,
+            )
             img_concat = np.concatenate((img_gt, img_pred), axis=1)
             if interactive:
                 interactive_imshow(img_concat)
             else:
                 return img_concat
         return None
 
@@ -310,26 +357,37 @@
 
     def __init__(
         self,
         wandb_run: "wandb.sdk.wandb_run.Run",
         dataset_name: str,
         num_samples: int,
         categories: Mapping[str, TypeOrStr],
+        sub_categories: Optional[Mapping[str, TypeOrStr]] = None,
+        cat_to_sub_cat: Optional[Mapping[TypeOrStr, TypeOrStr]] = None,
     ):
         """
         :param wandb_run: An `wandb.run` instance for tracking. Use `run=wandb.init(project=project, config=config,
                           **kwargs)` to generate a `run`.
         :param dataset_name: name for tracking
         :param num_samples: When dumping images to a table it will stop adding samples after `num_samples` instances
         :param categories: dict of all possible categories
+        :param sub_categories:  dict of sub categories. If provided, these categories will define the classes for the
+                                table
+        :param cat_to_sub_cat: dict of category to sub category keys. Suppose your category `foo` has a sub category
+                               defined by the key `sub_foo`. The range sub category values must then be given by
+                               `sub_categories` and to extract the sub category values one must pass `{"foo": "sub_foo"}
         """
 
         self.dataset_name = dataset_name
         self.num_samples = num_samples
         self.categories = categories
+        self.sub_categories = sub_categories
+        if cat_to_sub_cat is None:
+            cat_to_sub_cat = {}
+        self.cat_to_sub_cat = {get_type(cat): get_type(sub_cat) for cat, sub_cat in cat_to_sub_cat.items()}
         self._run = wandb_run
         self._counter = 0
 
         # Table logging utils
         self._table_cols: List[str] = ["file_name", "image"]
         self._table_rows: List[Any] = []
         self._table_ref = None
@@ -340,15 +398,17 @@
         to the table
 
         :param dp: datapoint image
         :return: same as input
         """
         if self.num_samples > self._counter:
             dp = maybe_load_image(dp)
-            self._table_rows.append(to_wandb_image(self.categories)(dp))  # pylint: disable=E1102
+            self._table_rows.append(
+                to_wandb_image(self.categories, self.sub_categories, self.cat_to_sub_cat)(dp)  # pylint: disable=E1102
+            )
             dp = maybe_remove_image(dp)
             self._counter += 1
         return dp
 
     def reset(self) -> None:
         """
         Reset table rows
```

### Comparing `deepdoctection-0.23/deepdoctection/eval/registry.py` & `deepdoctection-0.24/deepdoctection/eval/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/tedsmetric.py` & `deepdoctection-0.24/deepdoctection/eval/tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/eval/tp_eval_callback.py` & `deepdoctection-0.24/deepdoctection/eval/tp_eval_callback.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/__init__.py` & `deepdoctection-0.24/deepdoctection/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/base.py` & `deepdoctection-0.24/deepdoctection/extern/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/d2detect.py` & `deepdoctection-0.24/deepdoctection/extern/d2detect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/deskew.py` & `deepdoctection-0.24/deepdoctection/extern/deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/doctrocr.py` & `deepdoctection-0.24/deepdoctection/extern/doctrocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/fastlang.py` & `deepdoctection-0.24/deepdoctection/extern/fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/hfdetr.py` & `deepdoctection-0.24/deepdoctection/extern/hfdetr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/hflayoutlm.py` & `deepdoctection-0.24/deepdoctection/extern/hflayoutlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,34 +69,48 @@
 def predict_token_classes(
     uuids: List[List[str]],
     input_ids: "Tensor",
     attention_mask: "Tensor",
     token_type_ids: "Tensor",
     boxes: "Tensor",
     tokens: List[List[str]],
-    model: "LayoutLMForTokenClassification",
+    model: Union["LayoutLMForTokenClassification",
+                 "LayoutLMv2ForTokenClassification",
+                 "LayoutLMv3ForTokenClassification"],
     images: Optional["Tensor"] = None,
 ) -> List[TokenClassResult]:
     """
     :param uuids: A list of uuids that correspond to a word that induces the resulting token
     :param input_ids: Token converted to ids to be taken from LayoutLMTokenizer
     :param attention_mask: The associated attention masks from padded sequences taken from LayoutLMTokenizer
     :param token_type_ids: Torch tensor of token type ids taken from LayoutLMTokenizer
     :param boxes: Torch tensor of bounding boxes of type 'xyxy'
     :param tokens: List of original tokens taken from LayoutLMTokenizer
     :param model: layoutlm model for token classification
     :param images: A list of torch image tensors or None
     :return: A list of TokenClassResults
     """
+
     if images is None:
         outputs = model(input_ids=input_ids, bbox=boxes, attention_mask=attention_mask, token_type_ids=token_type_ids)
-    else:
+    elif isinstance(model, LayoutLMv2ForTokenClassification):
         outputs = model(
             input_ids=input_ids, bbox=boxes, attention_mask=attention_mask, token_type_ids=token_type_ids, image=images
         )
+    elif isinstance(model, LayoutLMv3ForTokenClassification):
+        outputs = model(
+            input_ids=input_ids,
+            bbox=boxes,
+            attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+            pixel_values=images,
+        )
+    else:
+        raise ValueError(f"Cannot call model {type(model)}")
+
     soft_max = F.softmax(outputs.logits, dim=2)
     score = torch.max(soft_max, dim=2)[0].tolist()
     token_class_predictions_ = outputs.logits.argmax(-1).tolist()
     input_ids_list = input_ids.tolist()
 
     all_results = defaultdict(list)
     for idx, uuid_list in enumerate(uuids):
@@ -308,15 +322,15 @@
             layoutlm = HFLayoutLmTokenClassifier("path/to/config.json","path/to/model.bin",
                                                   categories= ['B-answer', 'B-header', 'B-question', 'E-answer',
                                                                'E-header', 'E-question', 'I-answer', 'I-header',
                                                                'I-question', 'O', 'S-answer', 'S-header',
                                                                'S-question'])
 
             # token classification service
-            layoutlm_service = LMTokenClassifierService(tokenizer,layoutlm, image_to_layoutlm_features)
+            layoutlm_service = LMTokenClassifierService(tokenizer,layoutlm)
 
             pipe = DoctectionPipe(pipeline_component_list=[ocr_service,layoutlm_service])
 
             path = "path/to/some/form"
             df = pipe.analyze(path=path)
 
             for dp in df:
@@ -396,15 +410,15 @@
             layoutlm = HFLayoutLmv2TokenClassifier("path/to/config.json","path/to/model.bin",
                                                   categories= ['B-answer', 'B-header', 'B-question', 'E-answer',
                                                                'E-header', 'E-question', 'I-answer', 'I-header',
                                                                'I-question', 'O', 'S-answer', 'S-header',
                                                                'S-question'])
 
             # token classification service
-            layoutlm_service = LMTokenClassifierService(tokenizer,layoutlm, image_to_layoutlm_features)
+            layoutlm_service = LMTokenClassifierService(tokenizer,layoutlm)
 
             pipe = DoctectionPipe(pipeline_component_list=[ocr_service,layoutlm_service])
 
             path = "path/to/some/form"
             df = pipe.analyze(path=path)
 
             for dp in df:
@@ -497,15 +511,15 @@
             layoutlm = HFLayoutLmv3TokenClassifier("path/to/config.json","path/to/model.bin",
                                                   categories= ['B-answer', 'B-header', 'B-question', 'E-answer',
                                                                'E-header', 'E-question', 'I-answer', 'I-header',
                                                                'I-question', 'O', 'S-answer', 'S-header',
                                                                'S-question'])
 
             # token classification service
-            layoutlm_service = LMTokenClassifierService(tokenizer, layoutlm, image_to_layoutlm_features)
+            layoutlm_service = LMTokenClassifierService(tokenizer, layoutlm)
 
             pipe = DoctectionPipe(pipeline_component_list=[ocr_service,layoutlm_service])
 
             path = "path/to/some/form"
             df = pipe.analyze(path=path)
 
             for dp in df:
@@ -696,15 +710,15 @@
 
             # hf tokenizer and token classifier
             tokenizer = LayoutLMTokenizerFast.from_pretrained("microsoft/layoutlm-base-uncased")
             layoutlm = HFLayoutLmSequenceClassifier("path/to/config.json","path/to/model.bin",
                                                   categories=["handwritten", "presentation", "resume"])
 
             # token classification service
-            layoutlm_service = LMSequenceClassifierService(tokenizer,layoutlm, image_to_layoutlm_features)
+            layoutlm_service = LMSequenceClassifierService(tokenizer,layoutlm)
 
             pipe = DoctectionPipe(pipeline_component_list=[ocr_service,layoutlm_service])
 
             path = "path/to/some/form"
             df = pipe.analyze(path=path)
 
             for dp in df:
@@ -757,15 +771,15 @@
 
             # hf tokenizer and token classifier
             tokenizer = LayoutLMTokenizerFast.from_pretrained("microsoft/layoutlm-base-uncased")
             layoutlm = HFLayoutLmv2SequenceClassifier("path/to/config.json","path/to/model.bin",
                                                   categories=["handwritten", "presentation", "resume"])
 
             # token classification service
-            layoutlm_service = LMSequenceClassifierService(tokenizer,layoutlm, image_to_layoutlm_features)
+            layoutlm_service = LMSequenceClassifierService(tokenizer,layoutlm)
 
             pipe = DoctectionPipe(pipeline_component_list=[ocr_service,layoutlm_service])
 
             path = "path/to/some/form"
             df = pipe.analyze(path=path)
 
             for dp in df:
@@ -825,15 +839,15 @@
 
             # hf tokenizer and token classifier
             tokenizer = RobertaTokenizerFast.from_pretrained("roberta-base")
             layoutlm = HFLayoutLmv3SequenceClassifier("path/to/config.json","path/to/model.bin",
                                                   categories=["handwritten", "presentation", "resume"])
 
             # token classification service
-            layoutlm_service = LMSequenceClassifierService(tokenizer,layoutlm, image_to_layoutlm_features)
+            layoutlm_service = LMSequenceClassifierService(tokenizer,layoutlm)
 
             pipe = DoctectionPipe(pipeline_component_list=[ocr_service,layoutlm_service])
 
             path = "path/to/some/form"
             df = pipe.analyze(path=path)
 
             for dp in df:
```

### Comparing `deepdoctection-0.23/deepdoctection/extern/model.py` & `deepdoctection-0.24/deepdoctection/extern/model.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/pdftext.py` & `deepdoctection-0.24/deepdoctection/extern/pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/pt/__init__.py` & `deepdoctection-0.24/deepdoctection/extern/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/pt/ptutils.py` & `deepdoctection-0.24/deepdoctection/extern/pt/ptutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tessocr.py` & `deepdoctection-0.24/deepdoctection/extern/tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/texocr.py` & `deepdoctection-0.24/deepdoctection/extern/texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/__init__.py` & `deepdoctection-0.24/deepdoctection/extern/tp/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tfutils.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tfutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpcompat.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpcompat.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/common.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/config.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/config.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/predict.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/predict.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/preproc.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/preproc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py` & `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/extern/tpdetect.py` & `deepdoctection-0.24/deepdoctection/extern/tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/__init__.py` & `deepdoctection-0.24/deepdoctection/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/cats.py` & `deepdoctection-0.24/deepdoctection/mapper/cats.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 Categories related mapping functions. They can be set within a pipeline directly after a dataflow
 builder method of a dataset.
 """
 
 from collections import defaultdict
-from typing import Dict, List, Literal, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 from ..datapoint.annotation import CategoryAnnotation, ContainerAnnotation, ImageAnnotation, SummaryAnnotation
 from ..datapoint.image import Image
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from .maputils import LabelSummarizer, curry
 
 
@@ -57,33 +57,47 @@
             ann.category_name = sub_cat.category_name
             ann.category_id = categories_dict[ann.category_name]
 
     return dp
 
 
 @curry
-def re_assign_cat_ids(dp: Image, categories_dict_name_as_key: Dict[TypeOrStr, str]) -> Image:
+def re_assign_cat_ids(
+    dp: Image,
+    categories_dict_name_as_key: Optional[Dict[TypeOrStr, str]] = None,
+    cat_to_sub_cat_mapping: Optional[Mapping[ObjectTypes, Any]] = None,
+) -> Image:
     """
     Re-assigning category ids is sometimes necessary to align with categories of the `DatasetCategories` . E.g.
     consider the situation where some categories are filtered. In order to guarantee alignment of category ids of the
     `DatasetCategories` the ids in the annotation have to be re-assigned.
 
-    Annotations that as not in the dictionary provided will removed from the image.
+    Annotations that are not in the dictionary provided will be removed.
 
     :param dp: Image
-    :param categories_dict_name_as_key:
+    :param categories_dict_name_as_key: e.g. {"foo": "1", "bak": "2"}
+    :param cat_to_sub_cat_mapping:
     :return: Image
     """
 
     anns_to_remove: List[ImageAnnotation] = []
     for ann in dp.get_annotation_iter():
-        if ann.category_name in categories_dict_name_as_key:
-            ann.category_id = categories_dict_name_as_key[ann.category_name]
-        else:
-            anns_to_remove.append(ann)
+        if categories_dict_name_as_key is not None:
+            if ann.category_name in categories_dict_name_as_key:
+                ann.category_id = categories_dict_name_as_key[ann.category_name]
+            else:
+                anns_to_remove.append(ann)
+
+        if cat_to_sub_cat_mapping:
+            if ann.category_name in cat_to_sub_cat_mapping:
+                sub_cat_keys_to_sub_cat_values = cat_to_sub_cat_mapping[get_type(ann.category_name)]
+                for key in sub_cat_keys_to_sub_cat_values:
+                    sub_cat_values_dict = sub_cat_keys_to_sub_cat_values[key]
+                    sub_category = ann.get_sub_category(key)
+                    sub_category.category_id = sub_cat_values_dict.get(sub_category.category_name, "")
 
     for ann in anns_to_remove:
         dp.remove(ann)
 
     return dp
 
 
@@ -115,32 +129,37 @@
     dp = re_assign_cat_ids_mapper(dp)
 
     return dp
 
 
 @curry
 def filter_summary(
-    dp: Image, sub_cat_to_sub_cat_names_or_ids: Mapping[TypeOrStr, Sequence[TypeOrStr]], use_category_name: bool = True
+    dp: Image,
+    sub_cat_to_sub_cat_names_or_ids: Mapping[TypeOrStr, Sequence[TypeOrStr]],
+    mode: Literal["name", "id", "value"] = "name",
 ) -> Optional[Image]:
     """
     Filters datapoints with given summary conditions. If several conditions are given, it will filter out datapoints
     that do not satisfy all conditions.
 
     :param dp: Image datapoint
     :param sub_cat_to_sub_cat_names_or_ids: A dict of list. The key correspond to the sub category key to look for in
                                             the summary. The value correspond to a sequence of either category names
                                             or category ids
-    :param use_category_name: With respect to the previous argument, if set to True, it will look if the category name
-                              corresponds to any of the given values. If False it will look for category ids.
+    :param mode: With respect to the previous argument, it will look if the category name, the value or the category_id
+                 corresponds to any of the given values.
     :return: Image or None
     """
     for key, values in sub_cat_to_sub_cat_names_or_ids.items():
-        if use_category_name and dp.summary:
+        if mode == "name" and dp.summary:
             if dp.summary.get_sub_category(get_type(key)).category_name in values:
                 return dp
+        elif mode == "value" and dp.summary:
+            if dp.summary.get_sub_category(get_type(key)).value in values:  # type: ignore
+                return dp
         elif dp.summary:
             if dp.summary.get_sub_category(get_type(key)).category_id in values:
                 return dp
     return None
 
 
 @curry
@@ -216,15 +235,15 @@
             if isinstance(val, str):
                 val = [val]
             tmp_sub_category_names[key] = val
 
     if id_name_or_value not in ("id", "name", "value"):
         raise ValueError(f"id_name_or_value must be in ('id', 'name', 'value') but is {id_name_or_value}")
 
-    if category_names or sub_categories:  # pylint: disable=R1702
+    if category_names or sub_categories:
         for ann in dp.get_annotation_iter():
             if ann.category_name in category_names:
                 cat_container[ann.category_name].append(int(ann.category_id))
             if ann.category_name in tmp_sub_category_names:
                 for sub_cat_name in tmp_sub_category_names[ann.category_name]:
                     sub_cat = ann.get_sub_category(get_type(sub_cat_name))
                     if sub_cat is not None:
```

### Comparing `deepdoctection-0.23/deepdoctection/mapper/cocostruct.py` & `deepdoctection-0.24/deepdoctection/mapper/cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/hfstruct.py` & `deepdoctection-0.24/deepdoctection/mapper/hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/laylmstruct.py` & `deepdoctection-0.24/deepdoctection/mapper/laylmstruct.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # limitations under the License.
 
 """
 Module for mapping annotations from image to layout lm input structure. Heavily inspired by the notebooks
 <https://github.com/NielsRogge/Transformers-Tutorials>
 """
 
+import random
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, List, Literal, NewType, Optional, Sequence, Union
 
 import numpy as np
 import numpy.typing as npt
 from cv2 import INTER_LINEAR
 
@@ -158,18 +159,16 @@
             box = ann.bounding_box
         assert box is not None, box
         if not box.absolute_coords:
             box = box.transform(dp.width, dp.height, absolute_coords=True)
         all_boxes.append(word_id_to_segment_box.get(ann.annotation_id, box).to_list(mode="xyxy"))
 
         if (
-            WordType.token_tag in ann.sub_categories
-            and WordType.token_class in ann.sub_categories
-            and dataset_type == DatasetType.token_classification
-        ):
+            WordType.token_tag in ann.sub_categories or WordType.token_class in ann.sub_categories
+        ) and dataset_type == DatasetType.token_classification:
             if use_token_tag:
                 all_labels.append(int(ann.get_sub_category(WordType.token_tag).category_id) - 1)
             else:
                 all_labels.append(int(ann.get_sub_category(WordType.token_class).category_id) - 1)
 
     if dp.summary is not None and dataset_type == DatasetType.sequence_classification:
         all_labels.append(int(dp.summary.get_sub_category(PageType.document_type).category_id) - 1)
@@ -238,21 +237,25 @@
     return features
 
 
 def _tokenize_with_sliding_window(
     raw_features: List[RawLayoutLMFeatures],
     tokenizer: "PreTrainedTokenizerFast",
     sliding_window_stride: int,
+    max_batch_size: int,
     return_tensors: Optional[Literal["pt"]] = None,
 ) -> Union[JsonDict, "BatchEncoding"]:
     """
     Runs a tokenizer: If there are no overflowing tokens, the tokenizer output will be returned as it is.
     If there are overflowing tokens, sliding windows have to be built. As it is easier to prepare the sliding windows
     from raw tokenized outputs we run the tokenizer a second time without truncating and build the sliding windows from
     this second output.
+    The current implementation has a bug in that sense, that for higher batch sizes it will only return overflowing
+    samples. It is therefore recommended that if the dataset consist of many samples with lots of tokens one should
+    use a low per device batch size.
     """
     # first try: we require return_overflowing_tokens=True. If the number of raw features is equal to
     # overflow_to_sample_mapping then there is nothing more to do because the sample has less than max_length
     # tokens
     tokenized_inputs = tokenizer(
         [dp["words"] for dp in raw_features],
         padding="max_length",
@@ -357,14 +360,39 @@
                 all_attention_mask.append(attention_mask)
                 word_ids = word_ids_orig[start:end]
                 word_ids.insert(0, None)
                 pad_none = [None for _ in range(pad_last + 1)]
                 word_ids.extend(pad_none)
                 all_word_ids.append(word_ids)
 
+    if max_batch_size:
+        if max_batch_size < len(overflow_to_sample_mapping):
+            (
+                overflow_to_sample_mapping,
+                all_input_ids,
+                all_token_type_ids,
+                all_attention_mask,
+                all_word_ids,
+                all_tokens,
+            ) = zip(
+                *random.sample(
+                    list(
+                        zip(
+                            overflow_to_sample_mapping,
+                            all_input_ids,
+                            all_token_type_ids,
+                            all_attention_mask,
+                            all_word_ids,
+                            all_tokens,
+                        )
+                    ),
+                    max_batch_size,
+                )
+            )
+
     slided_tokenized_inputs: Dict[str, Union[List[Union[str, int]], torch.Tensor]] = {}
     if return_tensors == "pt":
         slided_tokenized_inputs["overflow_to_sample_mapping"] = torch.tensor(overflow_to_sample_mapping)
         slided_tokenized_inputs["input_ids"] = torch.tensor(all_input_ids)
         slided_tokenized_inputs["token_type_ids"] = torch.tensor(all_token_type_ids)
         slided_tokenized_inputs["attention_mask"] = torch.tensor(all_attention_mask)
     else:
@@ -382,14 +410,15 @@
     tokenizer: "PreTrainedTokenizerFast",
     padding: Literal["max_length", "do_not_pad", "longest"] = "max_length",
     truncation: bool = True,
     return_overflowing_tokens: bool = False,
     return_tensors: Optional[Literal["pt"]] = None,
     remove_columns_for_training: bool = False,
     sliding_window_stride: int = 0,
+    max_batch_size: int = 0,
 ) -> LayoutLMFeatures:
     """
     Mapping raw features to tokenized input sequences for LayoutLM models.
 
     :param raw_features: A dictionary with the following arguments: `image_id, width, height, ann_ids, words,
                          boxes, dataset_type`.
     :param tokenizer: A fast tokenizer for the model. Note, that the conventional python based tokenizer provided by the
@@ -429,15 +458,17 @@
         and raw_features[0].get("labels") is not None
     )
     _has_labels = bool(_has_token_labels or _has_sequence_labels)
     _image_key = "pixel_values" if "pixel_values" in raw_features[0] else "image"
 
     if sliding_window_stride:
         return_overflowing_tokens = True
-        tokenized_inputs = _tokenize_with_sliding_window(raw_features, tokenizer, sliding_window_stride, return_tensors)
+        tokenized_inputs = _tokenize_with_sliding_window(
+            raw_features, tokenizer, sliding_window_stride, max_batch_size, return_tensors
+        )
 
     else:
         tokenized_inputs = tokenizer(
             [dp["words"] for dp in raw_features],
             padding=padding,
             truncation=truncation,
             return_overflowing_tokens=return_overflowing_tokens,
@@ -562,22 +593,27 @@
                        If `False` then no truncation (i.e., can output batch with sequence lengths greater than the
                        model maximum admissible input size).
     :param return_overflowing_tokens: If a sequence (due to a truncation strategy) overflows the overflowing tokens can
                                   be returned as an additional batch element. Not that in this case, the number of input
                                   batch samples will be smaller than the output batch samples.
     :param return_tensors: If `pt` will return torch Tensors. If no argument is provided that the batches will be lists
                            of lists.
+    :param sliding_window_stride: If the output of the tokenizer exceeds the max_length sequence length sliding windows
+                           will be created with each window having max_length sequence input. When using
+                           `sliding_window_stride=0` no strides will be created, otherwise it will create slides
+                           with windows shifted `sliding_window_stride` to the right.
     """
 
     tokenizer: "PreTrainedTokenizerFast"
     padding: Literal["max_length", "do_not_pad", "longest"] = field(default="max_length")
     truncation: bool = field(default=True)
     return_overflowing_tokens: bool = field(default=False)
     return_tensors: Optional[Literal["pt"]] = field(default=None)
     sliding_window_stride: int = field(default=0)
+    max_batch_size: int = field(default=0)
 
     def __post_init__(self) -> None:
         assert isinstance(self.tokenizer, PreTrainedTokenizerFast), "Tokenizer must be a fast tokenizer"
         if self.return_tensors:
             assert self.padding not in ("do_not_pad",), self.padding
             assert self.truncation, self.truncation
         if self.return_overflowing_tokens:
@@ -596,14 +632,15 @@
             self.tokenizer,
             self.padding,
             self.truncation,
             self.return_overflowing_tokens,
             self.return_tensors,
             True,
             self.sliding_window_stride,
+            self.max_batch_size,
         )
 
 
 @curry
 def image_to_layoutlm_features(
     dp: Image,
     tokenizer: "PreTrainedTokenizerFast",
```

### Comparing `deepdoctection-0.23/deepdoctection/mapper/maputils.py` & `deepdoctection-0.24/deepdoctection/mapper/maputils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/match.py` & `deepdoctection-0.24/deepdoctection/mapper/match.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/misc.py` & `deepdoctection-0.24/deepdoctection/mapper/misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/pascalstruct.py` & `deepdoctection-0.24/deepdoctection/mapper/pascalstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/prodigystruct.py` & `deepdoctection-0.24/deepdoctection/mapper/prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/pubstruct.py` & `deepdoctection-0.24/deepdoctection/mapper/pubstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             else:
                 break
         cell_ids.append(cell_id_per_row)
 
     tiling = [[-1] * number_of_cols for _ in range(number_of_rows)]  # initialize placeholders
     table = zip(cell_ids, row_spans, col_spans)
 
-    for row_id, row in enumerate(table):  # type: ignore # pylint: disable=R1702
+    for row_id, row in enumerate(table):  # type: ignore
         for cell in zip(row[0], row[1], row[2]):  # type: ignore
             cell_id = cell[0]
             row_span = cell[1]
             col_span = cell[2]
             if 0 in tiling[row_id]:  # calculate actual position of the cell
                 col = tiling[row_id].index(0)
             else:
```

### Comparing `deepdoctection-0.23/deepdoctection/mapper/tpstruct.py` & `deepdoctection-0.24/deepdoctection/mapper/tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/mapper/xfundstruct.py` & `deepdoctection-0.24/deepdoctection/mapper/xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/__init__.py` & `deepdoctection-0.24/deepdoctection/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/anngen.py` & `deepdoctection-0.24/deepdoctection/pipe/anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/base.py` & `deepdoctection-0.24/deepdoctection/pipe/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,12 +312,12 @@
         :param position: position of the pipeline component in the pipeline
         :param name: name of the pipeline component to search for
         :return: Either a full dictionary with position and name of all pipeline components or the name, if the position
                  has been passed or the position if the name has been passed.
         """
         comp_info = {key: comp.name for key, comp in enumerate(self.pipe_component_list)}
         comp_info_name_as_key = {value: key for key, value in comp_info.items()}
-        if position:
+        if position is not None:
             return comp_info[position]
-        if name:
+        if name is not None:
             return comp_info_name_as_key[name]
         return comp_info
```

### Comparing `deepdoctection-0.23/deepdoctection/pipe/cell.py` & `deepdoctection-0.24/deepdoctection/pipe/cell.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,16 @@
                                 box=[0.0, 0.0, float(self.width), float(self.height)],  # type: ignore
                                 class_id=int(category_id),
                                 class_name=self.categories[category_id],
                                 score=0.0,
                                 absolute_coords=self.absolute_coords,
                             )
                         )
+        # resetting before finishing this sample
+        self.dummy_for_group_generated = self._initialize_dummy_for_group_generated()
         return detect_result_list
 
     def _create_condition(self, detect_result_list: List[DetectionResult]) -> Dict[str, int]:
         count = Counter([str(ann.class_id) for ann in detect_result_list])
         cat_to_group_sum = {}
         for group in self.group_categories:
             group_sum = 0
@@ -111,14 +113,17 @@
         for idx, group in enumerate(self.group_categories):
             if category_id in group:
                 is_generated = self.dummy_for_group_generated[idx]
                 self.dummy_for_group_generated[idx] = True
                 return is_generated
         return False
 
+    def _initialize_dummy_for_group_generated(self) -> List[bool]:
+        return [False for _ in self.group_categories]
+
 
 @pipeline_component_registry.register("SubImageLayoutService")
 class SubImageLayoutService(PredictorPipelineComponent):
     """
     Component in which the selected ImageAnnotation can be selected with cropped images and presented to a detector.
 
     The detected DetectResults are transformed into ImageAnnotations and stored both in the cache of the parent image
```

### Comparing `deepdoctection-0.23/deepdoctection/pipe/common.py` & `deepdoctection-0.24/deepdoctection/pipe/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/concurrency.py` & `deepdoctection-0.24/deepdoctection/pipe/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/doctectionpipe.py` & `deepdoctection-0.24/deepdoctection/pipe/doctectionpipe.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/language.py` & `deepdoctection-0.24/deepdoctection/pipe/language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/layout.py` & `deepdoctection-0.24/deepdoctection/pipe/layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/lm.py` & `deepdoctection-0.24/deepdoctection/pipe/lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/refine.py` & `deepdoctection-0.24/deepdoctection/pipe/refine.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/registry.py` & `deepdoctection-0.24/deepdoctection/pipe/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/segment.py` & `deepdoctection-0.24/deepdoctection/pipe/segment.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/pipe/text.py` & `deepdoctection-0.24/deepdoctection/pipe/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,16 +413,16 @@
         text_block_names: Optional[Union[str, Sequence[str]]] = None,
         text_containers_to_text_block: bool = False,
     ) -> None:
         """
         :param text_container: name of an image annotation that has a CHARS sub category. These annotations will be
                                ordered within all text blocks.
         :param floating_text_block_names: name of image annotation that belong to floating text. These annotations form
-                                          the highest hierarchy of text blocks that will ordered to generate a sensible
-                                          output of text
+                                          the highest hierarchy of text blocks that will be ordered to generate a
+                                          sensible output of text
         :param text_block_names: name of image annotation that have a relation with text containers (or which might be
                                  text containers themselves).
         :param text_containers_to_text_block: Text containers are in general no text blocks and belong to a lower
                                               hierarchy. However, if a text container is not assigned to a text block
                                               you can add it to the text block ordering to ensure that the full text is
                                               part of the subsequent sub process. Note however, that if the text
                                               container is on word level rather than line level, the results will not be
@@ -443,14 +443,29 @@
         self._text_containers_to_text_block = text_containers_to_text_block
         self.starting_point_tolerance = 0.05
         self.height_tolerance = 2.0
         self.ignore_category_when_building_column_blocks = [LayoutType.table]
         self._init_sanity_checks()
         super().__init__("text_order")
 
+    @property
+    def text_container(self) -> str:
+        """text container"""
+        return self._text_container
+
+    @property
+    def floating_text_block_names(self) -> Sequence[str]:
+        """floating text block names"""
+        return self._floating_text_block_names
+
+    @property
+    def text_block_names(self) -> Sequence[str]:
+        """text block names"""
+        return self._text_block_names
+
     def serve(self, dp: Image) -> None:
         # select all text blocks that are considered to be relevant for page text. This does not include some layout
         # items that have to be considered independently (e.g. tables). Order the blocks by column wise reading order
         floating_text_block_anns = dp.get_annotation(category_names=self._floating_text_block_names)
         number_floating_text_block_anns_orig = len(floating_text_block_anns)
         # maybe add all text containers that are not mapped to any text block
         if self._text_containers_to_text_block:
```

### Comparing `deepdoctection-0.23/deepdoctection/pipe/transform.py` & `deepdoctection-0.24/deepdoctection/pipe/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/train/__init__.py` & `deepdoctection-0.24/deepdoctection/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/train/d2_frcnn_train.py` & `deepdoctection-0.24/deepdoctection/train/d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/train/hf_detr_train.py` & `deepdoctection-0.24/deepdoctection/train/hf_detr_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/train/hf_layoutlm_train.py` & `deepdoctection-0.24/deepdoctection/train/hf_layoutlm_train.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 """
 Module for training Huggingface implementation of LayoutLm
 """
 
 import copy
 import json
+import os
 import pprint
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
 
 from torch.nn import Module
 from torch.utils.data import Dataset
 from transformers import (
     IntervalStrategy,
@@ -57,18 +58,22 @@
     HFLayoutLmv3SequenceClassifier,
     HFLayoutLmv3TokenClassifier,
 )
 from ..mapper.laylmstruct import LayoutLMDataCollator, image_to_raw_layoutlm_features
 from ..pipe.base import LanguageModelPipelineComponent
 from ..pipe.lm import get_tokenizer_from_architecture
 from ..pipe.registry import pipeline_component_registry
+from ..utils.file_utils import wandb_available
 from ..utils.logger import logger
 from ..utils.settings import DatasetType, LayoutType, ObjectTypes, WordType
 from ..utils.utils import string_to_dict
 
+if wandb_available():
+    import wandb
+
 _ARCHITECTURES_TO_MODEL_CLASS = {
     "LayoutLMForTokenClassification": (LayoutLMForTokenClassification, HFLayoutLmTokenClassifier, PretrainedConfig),
     "LayoutLMForSequenceClassification": (
         LayoutLMForSequenceClassification,
         HFLayoutLmSequenceClassifier,
         PretrainedConfig,
     ),
@@ -148,27 +153,29 @@
         super().__init__(model, args, data_collator, train_dataset)
 
     def setup_evaluator(
         self,
         dataset_val: DatasetBase,
         pipeline_component: LanguageModelPipelineComponent,
         metric: Union[Type[ClassificationMetric], ClassificationMetric],
+        run: Optional["wandb.sdk.wandb_run.Run"] = None,
         **build_eval_kwargs: Union[str, int],
     ) -> None:
         """
         Setup of evaluator before starting training. During training, predictors will be replaced by current
         checkpoints.
 
         :param dataset_val: dataset on which to run evaluation
         :param pipeline_component: pipeline component to plug into the evaluator
         :param metric: A metric class
+        :param run: WandB run
         :param build_eval_kwargs:
         """
 
-        self.evaluator = Evaluator(dataset_val, pipeline_component, metric, num_threads=1)
+        self.evaluator = Evaluator(dataset_val, pipeline_component, metric, num_threads=1, run=run)
         assert self.evaluator.pipe_component
         for comp in self.evaluator.pipe_component.pipe_components:
             comp.language_model.model = None  # type: ignore
         self.build_eval_kwargs = build_eval_kwargs
 
     def evaluate(
         self,
@@ -366,44 +373,78 @@
         "remove_unused_columns": False,
         "per_device_train_batch_size": 8,
         "max_steps": number_samples,
         "evaluation_strategy": "steps"
         if (dataset_val is not None and metric is not None and pipeline_component_name is not None)
         else "no",
         "eval_steps": 100,
+        "use_wandb": False,
+        "wandb_project": None,
+        "wandb_repo": "deepdoctection",
+        "sliding_window_stride": 0,
+        "max_batch_size": 0,
     }
 
     # We allow to overwrite the default setting by the user.
     for conf in config_overwrite:
         key, val = conf.split("=", maxsplit=1)
         try:
             val = int(val)  # type: ignore
         except ValueError:
             try:
                 val = float(val)  # type: ignore
             except ValueError:
                 pass
         conf_dict[key] = val
 
-    # Will inform about dataloader warnings if max_steps exceeds length of dataset
+    max_batch_size = conf_dict.pop("max_batch_size")
+    sliding_window_stride = conf_dict.pop("sliding_window_stride")
+    if sliding_window_stride and not max_batch_size:
+        logger.warning(
+            "sliding_window_stride is not 0 and max_batch_size is 0. This can result in CUDA out of memory because the "
+            "batch size can be higher than per_device_train_batch_size. Set max_batch_size to a positive number if you"
+            "encounter this type of problem.",
+            number_samples,
+        )
+
+    use_wandb = conf_dict.pop("use_wandb")
+    wandb_project = conf_dict.pop("wandb_project")
+    wandb_repo = conf_dict.pop("wandb_repo")
+
+    # Initialize Wandb, if necessary
+    run = None
+    if use_wandb:
+        if not wandb_available():
+            raise ModuleNotFoundError("WandB must be installed separately")
+        run = wandb.init(project=wandb_project, config=conf_dict)  # type: ignore
+        run._label(repo=wandb_repo)  # type: ignore # pylint: disable=W0212
+    else:
+        os.environ["WANDB_DISABLED"] = "True"
+
+        # Will inform about dataloader warnings if max_steps exceeds length of dataset
     if conf_dict["max_steps"] > number_samples:  # type: ignore
         logger.warning(
             "After %s dataloader will log warning at every iteration about unexpected samples", number_samples
         )
 
-    arguments = TrainingArguments(**conf_dict)
+    arguments = TrainingArguments(**conf_dict)  # pylint: disable=E1123
     logger.info("Config: \n %s", str(arguments.to_dict()), arguments.to_dict())
 
     id2label = {int(k) - 1: v for v, k in categories_dict_name_as_key.items()}
 
     logger.info("Will setup a head with the following classes\n %s", pprint.pformat(id2label, width=100, compact=True))
 
     config = config_cls.from_pretrained(pretrained_model_name_or_path=path_config_json, id2label=id2label)
     model = model_cls.from_pretrained(pretrained_model_name_or_path=path_weights, config=config)
-    data_collator = LayoutLMDataCollator(tokenizer_fast, return_tensors="pt")
+    data_collator = LayoutLMDataCollator(
+        tokenizer_fast,
+        return_tensors="pt",
+        sliding_window_stride=sliding_window_stride,  # type: ignore
+        max_batch_size=max_batch_size,  # type: ignore
+    )
     trainer = LayoutLMTrainer(model, arguments, data_collator, dataset)
 
     if arguments.evaluation_strategy in (IntervalStrategy.STEPS,):
         assert metric is not None  # silence mypy
         if dataset_type == DatasetType.sequence_classification:
             categories = dataset_val.dataflow.categories.get_categories(filtered=True)  # type: ignore
         else:
@@ -423,13 +464,18 @@
             categories=categories,
             device="cuda",
         )
         pipeline_component_cls = pipeline_component_registry.get(pipeline_component_name)
         if dataset_type == DatasetType.sequence_classification:
             pipeline_component = pipeline_component_cls(tokenizer_fast, dd_model)
         else:
-            pipeline_component = pipeline_component_cls(tokenizer_fast, dd_model, use_other_as_default_category=True)
+            pipeline_component = pipeline_component_cls(
+                tokenizer_fast,
+                dd_model,
+                use_other_as_default_category=True,
+                sliding_window_stride=sliding_window_stride,
+            )
         assert isinstance(pipeline_component, LanguageModelPipelineComponent)
 
-        trainer.setup_evaluator(dataset_val, pipeline_component, metric, **build_val_dict)  # type: ignore
+        trainer.setup_evaluator(dataset_val, pipeline_component, metric, run, **build_val_dict)  # type: ignore
 
     trainer.train()
```

### Comparing `deepdoctection-0.23/deepdoctection/train/tp_frcnn_train.py` & `deepdoctection-0.24/deepdoctection/train/tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/__init__.py` & `deepdoctection-0.24/deepdoctection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/concurrency.py` & `deepdoctection-0.24/deepdoctection/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/context.py` & `deepdoctection-0.24/deepdoctection/utils/context.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/detection_types.py` & `deepdoctection-0.24/deepdoctection/utils/detection_types.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/develop.py` & `deepdoctection-0.24/deepdoctection/utils/develop.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/file_utils.py` & `deepdoctection-0.24/deepdoctection/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/fs.py` & `deepdoctection-0.24/deepdoctection/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/identifier.py` & `deepdoctection-0.24/deepdoctection/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/logger.py` & `deepdoctection-0.24/deepdoctection/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/metacfg.py` & `deepdoctection-0.24/deepdoctection/utils/metacfg.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/pdf_utils.py` & `deepdoctection-0.24/deepdoctection/utils/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/settings.py` & `deepdoctection-0.24/deepdoctection/utils/settings.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/systools.py` & `deepdoctection-0.24/deepdoctection/utils/systools.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/tqdm.py` & `deepdoctection-0.24/deepdoctection/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/transform.py` & `deepdoctection-0.24/deepdoctection/utils/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/utils.py` & `deepdoctection-0.24/deepdoctection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection/utils/viz.py` & `deepdoctection-0.24/deepdoctection/utils/viz.py`

 * *Files 6% similar despite different names*

```diff
@@ -219,26 +219,35 @@
 def draw_boxes(
     np_image: ImageType,
     boxes: npt.NDArray[float32],
     category_names_list: Optional[List[Optional[str]]] = None,
     color: Optional[Tuple[int, int, int]] = None,
     font_scale: float = 1.0,
     rectangle_thickness: int = 4,
+    box_color_by_category: bool = True,
 ) -> ImageType:
     """
     Dray bounding boxes with category names into image.
 
     :param np_image: Image as np.ndarray
     :param boxes: A numpy array of shape Nx4 where each row is [x1, y1, x2, y2].
     :param category_names_list: List of N category names.
     :param color: A 3-tuple BGR color (in range [0, 255])
     :param font_scale: Font scale of text box
     :param rectangle_thickness: Thickness of bounding box
+    :param box_color_by_category:
     :return: A new image np.ndarray
     """
+    if color is not None:
+        box_color_by_category = False
+
+    category_to_color = {}
+    if box_color_by_category:
+        category_names = set(category_names_list)  # type: ignore
+        category_to_color = {category: random_color() for category in category_names}
 
     boxes = np.asarray(boxes, dtype="int32")
     if category_names_list is not None:
         assert len(category_names_list) == len(boxes), f"{len(category_names_list)} != {len(boxes)}"
     areas = (boxes[:, 2] - boxes[:, 0] + 1) * (boxes[:, 3] - boxes[:, 1] + 1)
     sorted_inds = np.argsort(-areas)  # draw large ones first
     assert areas.min() > 0, areas.min()
@@ -253,22 +262,34 @@
     np_image = np_image.copy()
 
     if np_image.ndim == 2 or (np_image.ndim == 3 and np_image.shape[2] == 1):
         np_image = cv2.cvtColor(np_image, cv2.COLOR_GRAY2BGR)
     for i in sorted_inds:
         box = boxes[i, :]
         if category_names_list is not None:
-            choose_color = random_color() if color is None else color
+            choose_color = category_to_color.get(category_names_list[i]) if category_to_color is not None else color
+            if choose_color is None:
+                choose_color = random_color()
             if category_names_list[i] is not None:
                 np_image = draw_text(
                     np_image, (box[0], box[1]), category_names_list[i], color=choose_color, font_scale=font_scale
                 )
             cv2.rectangle(
                 np_image, (box[0], box[1]), (box[2], box[3]), color=choose_color, thickness=rectangle_thickness
             )
+
+    # draw a (very ugly) color palette
+    y_0 = np_image.shape[0]
+    for category, col in category_to_color.items():
+        if category is not None:
+            np_image = draw_text(np_image, (np_image.shape[1], y_0), category, color=col, font_scale=2)
+            font = cv2.FONT_HERSHEY_SIMPLEX
+            ((_, text_h), _) = cv2.getTextSize(category, font, font_scale, 2)
+            y_0 = y_0 - int(10 * text_h)
+
     return np_image
 
 
 def interactive_imshow(
     img: ImageType,
     lclick_cb: Optional[Callable[[npt.NDArray[float32], int, int], None]] = None,
     rclick_cb: Optional[Callable[[npt.NDArray[float32], int, int], None]] = None,
```

### Comparing `deepdoctection-0.23/deepdoctection.egg-info/PKG-INFO` & `deepdoctection-0.24/deepdoctection.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.23
+Version: 0.24
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -52,16 +52,20 @@
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
    provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). Check the notebook repo or 
-   the documentation on how to train a model on your custom task or how to setup a pipeline.
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). 
+
+   [**!new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE) 
+   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v1_on_custom_token_classification.ipynb)
+   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3. Training 
+   scripts can now be tracked with W&B. Check the experimentation result of the notebooks [here](https://wandb.ai/jm76/FRFPE_layoutlmv1?workspace=user-jm76).
  - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself.
```

### Comparing `deepdoctection-0.23/deepdoctection.egg-info/SOURCES.txt` & `deepdoctection-0.24/deepdoctection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/deepdoctection.egg-info/requires.txt` & `deepdoctection-0.24/deepdoctection.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/setup.cfg` & `deepdoctection-0.24/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 [pylint.FORMAT]
 max-module-lines = 2500
 max-line-length = 120
 good-names = x,y,k,n,dp,df,el,ex,cx,cy,w,h,l,i,rs,cs,p6,H1,H2,H3,B1,B2,B3,B1_proposal,B2_proposal,GroupNorm,c2,c3,c4,c5,G,q
 
 [pylint.DESIGN]
 max-args = 16
-max-branches = 25
+max-branches = 27
 max-attributes = 18
 max-locals = 44
 max-returns = 8
 max-statements = 100
 max-public-methods = 30
 min-public-methods = 1
+max-nested-blocks = 8
 
 [pylint.MISCELLANEOUS]
 unsafe-load-any-extension = y # https://pylint.pycqa.org/en/2.6/technical_reference/c_extensions.html that is esp. needed
 
 [MESSAGES CONTROL]
 enable = useless-suppression
```

### Comparing `deepdoctection-0.23/setup.py` & `deepdoctection-0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 # TODO: add function that lists correct not pre-installed third party libs in package, such that requirement errors
 #  can be printed with correct version dependencies.
 # when uploading to pypi first comment all source extra dependencies so that there are no dependencies to dataflow
 
 EXTRA_DEPS = {
     "tf": tf_deps,
     "pt": pt_deps,
-    #"source-pt": source_pt_deps,
+#    "source-pt": source_pt_deps,
     "docs": docs_deps,
     "dev": dev_deps,
     "test": test_deps,
     "hf": pt_deps,
 }
 
 setup(
```

### Comparing `deepdoctection-0.23/tests/__init__.py` & `deepdoctection-0.24/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/analyzer/__init__.py` & `deepdoctection-0.24/tests/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/analyzer/test_dd.py` & `deepdoctection-0.24/tests/analyzer/test_dd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/conftest.py` & `deepdoctection-0.24/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/data.py` & `deepdoctection-0.24/tests/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/__init__.py` & `deepdoctection-0.24/tests/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/conftest.py` & `deepdoctection-0.24/tests/dataflow/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/test_common.py` & `deepdoctection-0.24/tests/dataflow/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/test_custom.py` & `deepdoctection-0.24/tests/dataflow/test_custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/test_custom_serialize.py` & `deepdoctection-0.24/tests/dataflow/test_custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/test_parallel_map.py` & `deepdoctection-0.24/tests/dataflow/test_parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/dataflow/test_stats.py` & `deepdoctection-0.24/tests/dataflow/test_stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/__init__.py` & `deepdoctection-0.24/tests/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/conftest.py` & `deepdoctection-0.24/tests/datapoint/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/test_annotation.py` & `deepdoctection-0.24/tests/datapoint/test_annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/test_box.py` & `deepdoctection-0.24/tests/datapoint/test_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/test_convert.py` & `deepdoctection-0.24/tests/datapoint/test_convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/test_image.py` & `deepdoctection-0.24/tests/datapoint/test_image.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datapoint/test_view.py` & `deepdoctection-0.24/tests/datapoint/test_view.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/__init__.py` & `deepdoctection-0.24/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/__init__.py` & `deepdoctection-0.24/tests/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/conftest.py` & `deepdoctection-0.24/tests/datasets/instances/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_doclaynet.py` & `deepdoctection-0.24/tests/datasets/instances/test_doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_fintabnet.py` & `deepdoctection-0.24/tests/datasets/instances/test_fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_funsd.py` & `deepdoctection-0.24/tests/datasets/instances/test_funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_iiitar13k.py` & `deepdoctection-0.24/tests/datasets/instances/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_layouttest.py` & `deepdoctection-0.24/tests/datasets/instances/test_layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_publaynet.py` & `deepdoctection-0.24/tests/datasets/instances/test_publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_pubtables1m.py` & `deepdoctection-0.24/tests/datasets/instances/test_pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_pubtabnet.py` & `deepdoctection-0.24/tests/datasets/instances/test_pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/instances/test_rvlcdip.py` & `deepdoctection-0.24/tests/datasets/instances/test_rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/test_adapter.py` & `deepdoctection-0.24/tests/datasets/test_adapter.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/test_info.py` & `deepdoctection-0.24/tests/datasets/test_info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/datasets/test_registry.py` & `deepdoctection-0.24/tests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/__init__.py` & `deepdoctection-0.24/tests/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/conftest.py` & `deepdoctection-0.24/tests/eval/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/test_accmetric.py` & `deepdoctection-0.24/tests/eval/test_accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/test_cocometric.py` & `deepdoctection-0.24/tests/eval/test_cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/test_eval.py` & `deepdoctection-0.24/tests/eval/test_eval.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/test_registry.py` & `deepdoctection-0.24/tests/eval/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/eval/test_tedsmetric.py` & `deepdoctection-0.24/tests/eval/test_tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/conftest.py` & `deepdoctection-0.24/tests/extern/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/data.py` & `deepdoctection-0.24/tests/extern/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_deskew.py` & `deepdoctection-0.24/tests/extern/test_deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_doctrocr.py` & `deepdoctection-0.24/tests/extern/test_doctrocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_fastlang.py` & `deepdoctection-0.24/tests/extern/test_fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_hfdetr.py` & `deepdoctection-0.24/tests/extern/test_hfdetr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_hflayoutlm.py` & `deepdoctection-0.24/tests/extern/test_hflayoutlm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_pdftext.py` & `deepdoctection-0.24/tests/extern/test_pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_tessocr.py` & `deepdoctection-0.24/tests/extern/test_tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_texocr.py` & `deepdoctection-0.24/tests/extern/test_texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/extern/test_tpdetect.py` & `deepdoctection-0.24/tests/extern/test_tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/__init__.py` & `deepdoctection-0.24/tests/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/conftest.py` & `deepdoctection-0.24/tests/mapper/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/data.py` & `deepdoctection-0.24/tests/mapper/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_cats.py` & `deepdoctection-0.24/tests/mapper/test_cats.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,28 +115,28 @@
 @pytest.mark.basic
 def test_filter_summary_1(datapoint_image_with_summary: Image) -> None:
     """
     test func:`filter_summary` does not filter dataset, if condition is satisfied.
     """
 
     # Arrange
-    output = filter_summary({"BAK": "FOO"}, True)(datapoint_image_with_summary)
+    output = filter_summary({"BAK": "FOO"})(datapoint_image_with_summary)
 
     # Assert
     assert output is not None
 
 
 @pytest.mark.basic
 def test_filter_summary_2(datapoint_image_with_summary: Image) -> None:
     """
     test func:`filter_summary`  does filter dataset, if condition is not satisfied.
     """
 
     # Arrange
-    output = filter_summary({"BAK": ["BAZ"]}, True)(datapoint_image_with_summary)
+    output = filter_summary({"BAK": ["BAZ"]})(datapoint_image_with_summary)
 
     # Assert
     assert output is None
 
 
 @pytest.mark.basic
 def test_image_to_cat_id_1(dp_image_fully_segmented: Image) -> None:
```

### Comparing `deepdoctection-0.23/tests/mapper/test_cocostruct.py` & `deepdoctection-0.24/tests/mapper/test_cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_d2struct.py` & `deepdoctection-0.24/tests/mapper/test_d2struct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_hfstruct.py` & `deepdoctection-0.24/tests/mapper/test_hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_iiitar13k.py` & `deepdoctection-0.24/tests/mapper/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_laylmstruct.py` & `deepdoctection-0.24/tests/mapper/test_laylmstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     )
 
     assert image is not None
 
     for ann in image.get_annotation():
         ann.remove_sub_category(WordType.token_class)
         ann.remove_sub_category(WordType.tag)
+        ann.remove_sub_category(WordType.token_tag)
 
     # Act
     raw_features = image_to_raw_layoutlm_features(DatasetType.token_classification)(image)
 
     # Assert
     assert raw_features is not None
     assert raw_features["image_id"] == raw_layoutlm_features["image_id"]
```

### Comparing `deepdoctection-0.23/tests/mapper/test_misc.py` & `deepdoctection-0.24/tests/mapper/test_misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_prodigystruct.py` & `deepdoctection-0.24/tests/mapper/test_prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_pubstruct.py` & `deepdoctection-0.24/tests/mapper/test_pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_tpstruct.py` & `deepdoctection-0.24/tests/mapper/test_tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_utils.py` & `deepdoctection-0.24/tests/mapper/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/mapper/test_xfundstruct.py` & `deepdoctection-0.24/tests/mapper/test_xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/__init__.py` & `deepdoctection-0.24/tests/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_anngen.py` & `deepdoctection-0.24/tests/pipe/test_anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_cell.py` & `deepdoctection-0.24/tests/pipe/test_cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_common.py` & `deepdoctection-0.24/tests/pipe/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_language.py` & `deepdoctection-0.24/tests/pipe/test_language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_layout.py` & `deepdoctection-0.24/tests/pipe/test_layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_lm.py` & `deepdoctection-0.24/tests/pipe/test_lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_refine.py` & `deepdoctection-0.24/tests/pipe/test_refine.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_registry.py` & `deepdoctection-0.24/tests/pipe/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_segment.py` & `deepdoctection-0.24/tests/pipe/test_segment.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_text.py` & `deepdoctection-0.24/tests/pipe/test_text.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/pipe/test_transform.py` & `deepdoctection-0.24/tests/pipe/test_transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/test_utils.py` & `deepdoctection-0.24/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/train/__init__.py` & `deepdoctection-0.24/tests/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/train/conftest.py` & `deepdoctection-0.24/tests/train/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/train/test_d2_frcnn_train.py` & `deepdoctection-0.24/tests/train/test_d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests/train/test_tp_frcnn_train.py` & `deepdoctection-0.24/tests/train/test_tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests_d2/__init__.py` & `deepdoctection-0.24/tests_d2/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests_d2/conftest.py` & `deepdoctection-0.24/tests_d2/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.23/tests_d2/test_d2detect.py` & `deepdoctection-0.24/tests_d2/test_d2detect.py`

 * *Files identical despite different names*

