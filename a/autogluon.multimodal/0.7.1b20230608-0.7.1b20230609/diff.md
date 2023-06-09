# Comparing `tmp/autogluon.multimodal-0.7.1b20230608.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230608.tar", last modified: Thu Jun  8 09:04:22 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230609.tar", last modified: Fri Jun  9 09:04:06 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230608.tar` & `autogluon.multimodal-0.7.1b20230609.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.766211 autogluon.multimodal-0.7.1b20230608/
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-08 09:04:22.766211 autogluon.multimodal-0.7.1b20230608/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:04:22.766211 autogluon.multimodal-0.7.1b20230608/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.738210 autogluon.multimodal-0.7.1b20230608/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.738210 autogluon.multimodal-0.7.1b20230608/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.742210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.750210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.754211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.754211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.754211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.758211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.758211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.758211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   119344 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26148 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.762210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.742210 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.565841 autogluon.multimodal-0.7.1b20230609/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-09 09:04:06.561840 autogluon.multimodal-0.7.1b20230609/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:04:06.565841 autogluon.multimodal-0.7.1b20230609/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.545839 autogluon.multimodal-0.7.1b20230609/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.545839 autogluon.multimodal-0.7.1b20230609/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.553840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.553840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.553840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.553840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.553840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.553840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87088 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.557840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.557840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.557840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121028 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.561840 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-09 09:03:31.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:06.549840 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:06.000000 autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230608/PKG-INFO` & `autogluon.multimodal-0.7.1b20230609/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230608
+Version: 0.7.1b20230609
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230608/setup.py` & `autogluon.multimodal-0.7.1b20230609/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/matcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,21 +86,21 @@
     get_minmax_mode,
     get_stopping_threshold,
     hyperparameter_tune,
     infer_dtypes_by_model_names,
     infer_metrics,
     infer_precision,
     init_df_preprocessor,
-    init_pretrained_matcher,
     load_text_tokenizers,
     predict,
     save_pretrained_model_configs,
     save_text_tokenizers,
     select_model,
     setup_save_path,
+    split_hyperparameters,
     split_train_tuning_data,
     update_hyperparameters,
     upgrade_config,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -122,14 +122,16 @@
         presets: Optional[str] = None,
         eval_metric: Optional[str] = None,
         hyperparameters: Optional[dict] = None,
         path: Optional[str] = None,
         verbosity: Optional[int] = 3,
         warn_if_exist: Optional[bool] = True,
         enable_progress_bar: Optional[bool] = None,
+        pretrained: Optional[bool] = True,
+        validation_metric: Optional[str] = None,
     ):
         """
         Parameters
         ----------
         query
             Column names of query data.
         response
@@ -149,15 +151,15 @@
             if the label column contains binary, multiclass, or numeric labels.
             If `problem_type = None`, the prediction problem type is inferred
             based on the label-values in provided dataset.
         presets
             Presets regarding model quality, e.g., best_quality, high_quality, and medium_quality.
         eval_metric
             Evaluation metric name. If `eval_metric = None`, it is automatically chosen based on `problem_type`.
-            Defaults to 'accuracy' for binary and multiclass classification, 'root_mean_squared_error' for regression.
+            Defaults to 'roc_auc' for binary classification and 'spearmanr' for multiclass classification and regression.
         path
             Path to directory where models and intermediate outputs should be saved.
             If unspecified, a time-stamped folder called "AutogluonAutoMM/ag-[TIMESTAMP]"
             will be created in the working directory to store all models.
             Note: To call `fit()` twice and save all results of each fit,
             you must specify different `path` locations or don't specify `path` at all.
             Otherwise files from first `fit()` will be overwritten by second `fit()`.
@@ -168,14 +170,19 @@
             where `L` ranges from 0 to 50
             (Note: higher values of `L` correspond to fewer print statements, opposite of verbosity levels)
         warn_if_exist
             Whether to raise warning if the specified path already exists.
         enable_progress_bar
             Whether to show progress bar. It will be True by default and will also be
             disabled if the environment variable os.environ["AUTOMM_DISABLE_PROGRESS_BAR"] is set.
+        pretrained
+            Whether to init model with pretrained weights. If False, it creates a model with random initialization.
+        validation_metric
+            Validation metric name. If `validation_metric = None`, it is automatically chosen based on `problem_type`.
+            Defaults to 'roc_auc' for binary classification and 'spearmanr' for multiclass classification and regression.
         """
         if eval_metric is not None and not isinstance(eval_metric, str):
             eval_metric = eval_metric.name
 
         if os.environ.get(AUTOMM_TUTORIAL_MODE):
             verbosity = 1  # don't use 3, which doesn't suppress logger.info() in .load().
             enable_progress_bar = False
@@ -197,20 +204,22 @@
         self._response = response
         self._data_format = PAIR  # TODO: Support Triplet
         self._match_label = match_label
         self._label_column = label
         self._problem_type = None  # always infer problem type for matching.
         self._pipeline = problem_type.lower() if problem_type is not None else None
         self._presets = presets.lower() if presets else None
-        self._eval_metric_name = eval_metric
-        self._validation_metric_name = None
+        self._eval_metric_name = eval_metric.lower() if eval_metric else None
+        self._validation_metric_name = validation_metric.lower() if validation_metric else None
+        self._hyperparameters = hyperparameters
         self._output_shape = None
         self._save_path = path
         self._ckpt_path = None
         self._pretrained_path = None
+        self._pretrained = pretrained
         self._config = None
         self._query_config = None
         self._response_config = None
         self._query_df_preprocessor = None
         self._response_df_preprocessor = None
         self._label_df_preprocessor = None
         self._column_types = None
@@ -221,27 +230,14 @@
         self._response_model = None
         self._resume = False
         self._fit_called = False
         self._verbosity = verbosity
         self._warn_if_exist = warn_if_exist
         self._enable_progress_bar = enable_progress_bar if enable_progress_bar is not None else True
 
-        if self._pipeline is not None:  # TODO: do not create pretrained model for HPO presets.
-            (
-                self._config,
-                self._query_config,
-                self._response_config,
-                self._query_model,
-                self._response_model,
-                self._query_processors,
-                self._response_processors,
-            ) = init_pretrained_matcher(
-                pipeline=self._pipeline, presets=self._presets, hyperparameters=hyperparameters
-            )
-
     @property
     def query(self):
         return self._query
 
     @property
     def response(self):
         return self._response
@@ -281,14 +277,74 @@
         verbosity
             The verbosity level
 
         """
         self._verbosity = verbosity
         set_logger_verbosity(verbosity, logger=logger)
 
+    def _init_pretrained(self):
+
+        if self._config is None:
+            # split out the hyperparameters whose values are complex objects
+            hyperparameters, advanced_hyperparameters = split_hyperparameters(self._hyperparameters)
+            self._config = get_config(
+                problem_type=self._pipeline,
+                presets=self._presets,
+                overrides=hyperparameters,
+                extra=["matcher"],
+            )
+        else:
+            advanced_hyperparameters = None
+
+        assert (
+            len(self._config.model.names) == 1
+        ), f"Zero shot mode only supports using one model, but detects multiple models {self._config.model.names}"
+
+        if self._query_config is None:
+            self._query_config = copy.deepcopy(self._config)
+            # customize config model names to make them consistent with model prefixes.
+            self._query_config.model, query_advanced_hyperparameters = customize_model_names(
+                config=self._query_config.model,
+                customized_names=[f"{n}_{QUERY}" for n in self._query_config.model.names],
+                advanced_hyperparameters=advanced_hyperparameters,
+            )
+        else:
+            query_advanced_hyperparameters = (None,)
+
+        if self._response_config is None:
+            self._response_config = copy.deepcopy(self._config)
+            # customize config model names to make them consistent with model prefixes.
+            self._response_config.model, response_advanced_hyperparameters = customize_model_names(
+                config=self._response_config.model,
+                customized_names=[f"{n}_{RESPONSE}" for n in self._response_config.model.names],
+                advanced_hyperparameters=advanced_hyperparameters,
+            )
+        else:
+            response_advanced_hyperparameters = None
+
+        if self._query_model is None or self._response_model is None:
+            self._query_model, self._response_model = create_siamese_model(
+                query_config=self._query_config,
+                response_config=self._response_config,
+                pretrained=self._pretrained,
+            )
+
+        self._query_processors, self._response_processors, self._label_processors = self._get_matcher_data_processors(
+            query_model=self._query_model,
+            query_config=self._query_config,
+            response_model=self._response_model,
+            response_config=self._response_config,
+            query_advanced_hyperparameters=query_advanced_hyperparameters,
+            response_advanced_hyperparameters=response_advanced_hyperparameters,
+        )
+
+    def _ensure_inference_ready(self):
+        if not self._fit_called:
+            self._init_pretrained()
+
     def fit(
         self,
         train_data: pd.DataFrame,
         id_mappings: Optional[Union[Dict[str, Dict], Dict[str, pd.Series]]] = None,
         presets: Optional[str] = None,
         tuning_data: Optional[pd.DataFrame] = None,
         time_limit: Optional[int] = None,
@@ -450,20 +506,28 @@
 
         # set attributes for saving and prediction
         self._eval_metric_name = eval_metric_name  # In case eval_metric isn't provided in __init__().
         self._validation_metric_name = validation_metric_name
         self._output_shape = output_shape
         self._column_types = column_types
 
+        if self._hyperparameters and hyperparameters:
+            self._hyperparameters.update(hyperparameters)
+        elif hyperparameters:
+            self._hyperparameters = hyperparameters
+
         hyperparameters, hyperparameter_tune_kwargs = update_hyperparameters(
             problem_type=self._pipeline,
             presets=presets,
-            provided_hyperparameters=hyperparameters,
+            provided_hyperparameters=self._hyperparameters,
             provided_hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
         )
+        # split out the hyperparameters whose values are complex objects
+        hyperparameters, advanced_hyperparameters = split_hyperparameters(hyperparameters)
+
         hpo_mode = True if hyperparameter_tune_kwargs else False
         if hpo_mode:
             hyperparameters = filter_hyperparameters(
                 hyperparameters=hyperparameters,
                 column_types=column_types,
                 config=self._config,
                 fit_called=fit_called,
@@ -478,14 +542,15 @@
             max_time=time_limit,
             save_path=self._save_path,
             ckpt_path=None if hpo_mode else self._ckpt_path,
             resume=False if hpo_mode else self._resume,
             enable_progress_bar=False if hpo_mode else self._enable_progress_bar,
             presets=presets,
             hyperparameters=hyperparameters,
+            advanced_hyperparameters=advanced_hyperparameters,
             hpo_mode=hpo_mode,  # skip average checkpoint if in hpo mode
         )
 
         if hpo_mode:
             # TODO: allow custom gpu
             assert self._resume is False, "You can not resume training with HPO"
             resources = dict(num_gpus=torch.cuda.device_count())
@@ -557,35 +622,39 @@
 
     def _get_matcher_data_processors(
         self,
         query_model: Optional[nn.Module] = None,
         query_config: Optional[DictConfig] = None,
         response_model: Optional[nn.Module] = None,
         response_config: Optional[DictConfig] = None,
+        query_advanced_hyperparameters: Optional[Dict] = None,
+        response_advanced_hyperparameters: Optional[Dict] = None,
     ):
         if query_model is None:
             query_processors = None
         elif self._query_processors is None and all(v is not None for v in [query_model, query_config]):
             query_processors = create_fusion_data_processors(
                 model=query_model,
                 config=query_config,
                 requires_label=False,
                 requires_data=True,
+                advanced_hyperparameters=query_advanced_hyperparameters,
             )
         else:  # continuing training
             query_processors = self._query_processors
 
         if response_model is None:
             response_processors = None
         elif self._response_processors is None and all(v is not None for v in [response_model, response_config]):
             response_processors = create_fusion_data_processors(
                 model=response_model,
                 config=response_config,
                 requires_label=False,
                 requires_data=True,
+                advanced_hyperparameters=response_advanced_hyperparameters,
             )
         else:  # continuing training
             response_processors = self._response_processors
 
         # only need labels for the response model
         if response_model is None:
             label_processors = None
@@ -613,14 +682,15 @@
         max_time: timedelta,
         save_path: str,
         ckpt_path: str,
         resume: bool,
         enable_progress_bar: bool,
         presets: Optional[str] = None,
         hyperparameters: Optional[Union[str, Dict, List[str]]] = None,
+        advanced_hyperparameters: Optional[Dict] = None,
         hpo_mode: bool = False,
         **hpo_kwargs,
     ):
         # TODO(?) We should have a separate "_pre_training_event()" for logging messages.
         logger.info(get_fit_start_message(save_path, validation_metric_name))
         config = self._config
         config = get_config(
@@ -630,29 +700,34 @@
             overrides=hyperparameters,
             extra=["matcher"],
         )
 
         if self._query_config is None:
             query_config = copy.deepcopy(config)
             # customize config model names to make them consistent with model prefixes.
-            query_config.model, _ = customize_model_names(
-                config=query_config.model, customized_names=[f"{n}_{QUERY}" for n in query_config.model.names]
+            query_config.model, query_advanced_hyperparameters = customize_model_names(
+                config=query_config.model,
+                customized_names=[f"{n}_{QUERY}" for n in query_config.model.names],
+                advanced_hyperparameters=advanced_hyperparameters,
             )
         else:
             query_config = self._query_config
+            query_advanced_hyperparameters = None
 
         if self._response_config is None:
             response_config = copy.deepcopy(config)
             # customize config model names to make them consistent with model prefixes.
-            response_config.model, _ = customize_model_names(
+            response_config.model, response_advanced_hyperparameters = customize_model_names(
                 config=response_config.model,
                 customized_names=[f"{n}_{RESPONSE}" for n in response_config.model.names],
+                advanced_hyperparameters=advanced_hyperparameters,
             )
         else:
             response_config = self._response_config
+            response_advanced_hyperparameters = None
 
         query_df_preprocessor, response_df_preprocessor, label_df_preprocessor = self._get_matcher_df_preprocessor(
             data=train_df,
             column_types=self._column_types,
             query_config=query_config,
             response_config=response_config,
             query_columns=self._query,
@@ -662,24 +737,27 @@
         query_config = select_model(config=query_config, df_preprocessor=query_df_preprocessor, strict=False)
         response_config = select_model(config=response_config, df_preprocessor=response_df_preprocessor, strict=False)
 
         if self._query_model is None or self._response_model is None:
             query_model, response_model = create_siamese_model(
                 query_config=query_config,
                 response_config=response_config,
+                pretrained=self._pretrained,
             )
         else:  # continuing training
             query_model = self._query_model
             response_model = self._response_model
 
         query_processors, response_processors, label_processors = self._get_matcher_data_processors(
             query_model=query_model,
             query_config=query_config,
             response_model=response_model,
             response_config=response_config,
+            query_advanced_hyperparameters=query_advanced_hyperparameters,
+            response_advanced_hyperparameters=response_advanced_hyperparameters,
         )
 
         query_processors_count = {k: len(v) for k, v in query_processors.items()}
         logger.debug(f"query_processors_count: {query_processors_count}")
         response_processors_count = {k: len(v) for k, v in response_processors.items()}
         logger.debug(f"response_processors_count: {response_processors_count}")
         if label_processors:
@@ -1443,14 +1521,15 @@
             and sample number.
 
         Returns
         -------
         A dictionary with the metric names and their corresponding scores.
         Optionally return a dataframe of prediction results.
         """
+        self._ensure_inference_ready()
         if all(v is not None for v in [data, query_data, response_data]):
             if isinstance(query_data, list):
                 assert (
                     self._query is not None
                 ), "query_data is a list. Need a dict or dataframe, whose keys or headers should be in data's headers."
 
             if isinstance(response_data, list):
@@ -1515,14 +1594,15 @@
             If not specified, we would infer it on based on the data modalities
             and sample number.
 
         Returns
         -------
         Array of predictions, one corresponding to each row in given dataset.
         """
+        self._ensure_inference_ready()
         outputs = predict(
             predictor=self,
             data=data,
             id_mappings=id_mappings,
             requires_label=False,
             is_matching=True,
             realtime=realtime,
@@ -1576,14 +1656,15 @@
 
         Returns
         -------
         Array of predicted class-probabilities, corresponding to each row in the given data.
         When as_multiclass is True, the output will always have shape (#samples, #classes).
         Otherwise, the output will have shape (#samples,)
         """
+        self._ensure_inference_ready()
         outputs = predict(
             predictor=self,
             data=data,
             id_mappings=id_mappings,
             requires_label=False,
             is_matching=True,
             realtime=realtime,
@@ -1632,14 +1713,15 @@
 
         Returns
         -------
         Array of embeddings, corresponding to each row in the given data.
         It will have shape (#samples, D) where the embedding dimension D is determined
         by the neural network's architecture.
         """
+        self._ensure_inference_ready()
         if signature is None:
             if self._query or self._response:
                 if isinstance(data, list):
                     raise ValueError("data can't be a list. Provide a dict or a dataframe instead.")
                 else:
                     data = data_to_df(data=data)
                     if self._query and all(c in data.columns for c in self._query):
@@ -1788,14 +1870,15 @@
                     "problem_type": self._problem_type,
                     "pipeline": self._pipeline,
                     "presets": self._presets,
                     "eval_metric_name": self._eval_metric_name,
                     "validation_metric_name": self._validation_metric_name,
                     "output_shape": self._output_shape,
                     "save_path": self._save_path,
+                    "pretrained": self._pretrained,
                     "pretrained_path": self._pretrained_path,
                     "fit_called": self._fit_called,
                     "version": ag_version.__version__,
                 },
                 fp,
                 ensure_ascii=True,
             )
@@ -1891,15 +1974,17 @@
         matcher._pipeline = assets["pipeline"]
         if "presets" in assets:
             matcher._presets = assets["presets"]
         matcher._eval_metric_name = assets["eval_metric_name"]
         matcher._verbosity = verbosity
         matcher._resume = resume
         matcher._save_path = path  # in case the original exp dir is copied to somewhere else
-        matcher._pretrain_path = path
+        matcher._pretrained_path = path
+        if "pretrained" in assets:
+            matcher._pretrained = assets["pretrained"]
         if "fit_called" in assets:
             matcher._fit_called = assets["fit_called"]
         else:
             matcher._fit_called = True  # backward compatible
         matcher._config = config
         matcher._query_config = query_config
         matcher._response_config = response_config
```

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,26 +131,26 @@
     filter_hyperparameters,
     get_available_devices,
     get_config,
     get_detection_classes,
     get_dir_ckpt_paths,
     get_fit_complete_message,
     get_fit_start_message,
+    get_gpu_message,
     get_load_ckpt_paths,
     get_local_pretrained_config_paths,
     get_minmax_mode,
     get_mixup,
     get_stopping_threshold,
     hyperparameter_tune,
     infer_dtypes_by_model_names,
     infer_metrics,
     infer_precision,
     infer_scarcity_mode_by_data_size,
     init_df_preprocessor,
-    init_pretrained,
     is_lazy_weight_tensor,
     list_timm_models,
     load_text_tokenizers,
     logits_to_prob,
     merge_bio_format,
     modify_duplicate_model_names,
     object_detection_data_to_df,
@@ -199,14 +199,16 @@
         path: Optional[str] = None,
         verbosity: Optional[int] = 2,
         num_classes: Optional[int] = None,  # TODO: can we infer this from data?
         classes: Optional[list] = None,
         warn_if_exist: Optional[bool] = True,
         enable_progress_bar: Optional[bool] = None,
         init_scratch: Optional[bool] = False,
+        pretrained: Optional[bool] = True,
+        validation_metric: Optional[str] = None,
         sample_data_path: Optional[str] = None,
     ):
         """
         Parameters
         ----------
         label
             Name of the column that contains the target variable to predict.
@@ -260,15 +262,15 @@
             If match_label is not provided, every sample is assumed to have a unique label.
         pipeline
             Pipeline has been deprecated and merged in problem_type.
         presets
             Presets regarding model quality, e.g., best_quality, high_quality, and medium_quality.
         eval_metric
             Evaluation metric name. If `eval_metric = None`, it is automatically chosen based on `problem_type`.
-            Defaults to 'accuracy' for binary and multiclass classification, 'root_mean_squared_error' for regression.
+            Defaults to 'accuracy' for multiclass classification, `roc_auc` for binary classification, and 'root_mean_squared_error' for regression.
         hyperparameters
             This is to override some default configurations.
             For example, changing the text and image backbones can be done by formatting:
 
             a string
             hyperparameters = "model.hf_text.checkpoint_name=google/electra-small-discriminator model.timm_image.checkpoint_name=swin_small_patch4_window7_224"
 
@@ -300,17 +302,19 @@
         classes
             All classes in this dataset.
         warn_if_exist
             Whether to raise warning if the specified path already exists.
         enable_progress_bar
             Whether to show progress bar. It will be True by default and will also be
             disabled if the environment variable os.environ["AUTOMM_DISABLE_PROGRESS_BAR"] is set.
-        init_scratch
-            Whether to init model from scratch. It's useful when we want to load a checkpoints
-            without its weights.
+        pretrained
+            Whether to init model with pretrained weights. If False, it creates a model with random initialization.
+        validation_metric
+            Validation metric name. If `validation_metric = None`, it is automatically chosen based on `problem_type`.
+            Defaults to 'accuracy' for multiclass classification, `roc_auc` for binary classification, and 'root_mean_squared_error' for regression.
         sample_data_path
             This is used for automatically inference num_classes, classes, or label.
 
         """
 
         # Handle the deprecated pipeline flag
         if pipeline is not None:
@@ -381,38 +385,43 @@
             enable_progress_bar = False
             # Also disable progress bar of transformers package
             transformers.logging.disable_progress_bar()
 
         if verbosity is not None:
             set_logger_verbosity(verbosity)
 
+        if init_scratch:
+            warnings.warn("init_scratch is deprecated. Try pretrained=False instead.", UserWarning)
+            pretrained = False
+
         self._label_column = label
         self._problem_type = problem_type
         self._presets = presets.lower() if presets else None
-        self._eval_metric_name = eval_metric
-        self._validation_metric_name = None
+        self._eval_metric_name = eval_metric.lower() if eval_metric else None
+        self._validation_metric_name = validation_metric.lower() if validation_metric else None
         self._output_shape = num_classes
         self._classes = classes
         self._ckpt_path = None
         self._pretrained_path = None
+        self._pretrained = pretrained
         self._config = None
         self._df_preprocessor = None
         self._column_types = None
         self._data_processors = None
         self._model_postprocess_fn = None
         self._model = None
         self._resume = False
         self._verbosity = verbosity
         self._warn_if_exist = warn_if_exist
         self._enable_progress_bar = enable_progress_bar if enable_progress_bar is not None else True
-        self._init_scratch = init_scratch
         self._sample_data_path = sample_data_path
         self._fit_called = False  # While using ddp, after fit called, we can only use single gpu.
         self._matcher = None
         self._save_path = path
+        self._hyperparameters = hyperparameters
 
         # Summary statistics used in fit summary. TODO: wrap it in a class.
         self._total_train_time = None
         self._best_score = None
 
         if self.problem_property and self.problem_property.is_matching:
             self._matcher = MultiModalMatcher(
@@ -424,39 +433,25 @@
                 presets=presets,
                 hyperparameters=hyperparameters,
                 eval_metric=eval_metric,
                 path=path,
                 verbosity=verbosity,
                 warn_if_exist=warn_if_exist,
                 enable_progress_bar=enable_progress_bar,
+                pretrained=pretrained,
+                validation_metric=validation_metric,
             )
             return
 
         if self._problem_type == OBJECT_DETECTION:
             self._label_column = "label"
             if self._sample_data_path is not None:
                 self._classes = get_detection_classes(self._sample_data_path)
                 self._output_shape = len(self._classes)
 
-        if self._problem_type is not None:
-            if self.problem_property.support_zero_shot:
-                # Load pretrained model via the provided hyperparameters and presets
-                # TODO: do not create pretrained model for HPO presets.
-                self._config, self._model, self._data_processors = init_pretrained(
-                    problem_type=self._problem_type,
-                    presets=self._presets,
-                    hyperparameters=hyperparameters,
-                    num_classes=self._output_shape,
-                    classes=self._classes,
-                    init_scratch=self._init_scratch,
-                )
-                self._validation_metric_name = self._config["optimization"][
-                    "val_metric"
-                ]  # TODO: only object detection is using this
-
     @property
     def path(self):
         if self._matcher:
             return self._matcher.path
         else:
             return self._save_path
 
@@ -489,22 +484,25 @@
             return self._matcher.match_label
         else:
             warnings.warn("Matcher is not used. No match_label is available.", UserWarning)
             return None
 
     @property
     def problem_type(self):
-        return self._problem_type
+        if self._matcher:
+            return self._matcher._pipeline
+        else:
+            return self._problem_type
 
     @property
     def problem_property(self):
-        if self._problem_type is None:
+        if self.problem_type is None:
             return None
         else:
-            return PROBLEM_TYPES_REG.get(self._problem_type)
+            return PROBLEM_TYPES_REG.get(self.problem_type)
 
     @property
     def column_types(self):
         if self._matcher:
             return self._matcher.column_types
         else:
             return self._column_types
@@ -800,18 +798,23 @@
             time_limit = timedelta(seconds=time_limit)
 
         # set attributes for saving and prediction
         self._eval_metric_name = eval_metric_name  # In case eval_metric isn't provided in __init__().
         self._validation_metric_name = validation_metric_name
         self._column_types = column_types
 
+        if self._hyperparameters and hyperparameters:
+            self._hyperparameters.update(hyperparameters)
+        elif hyperparameters:
+            self._hyperparameters = hyperparameters
+
         hyperparameters, hyperparameter_tune_kwargs = update_hyperparameters(
             problem_type=self._problem_type,
             presets=presets,
-            provided_hyperparameters=hyperparameters,
+            provided_hyperparameters=self._hyperparameters,
             provided_hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
             teacher_predictor=teacher_predictor,
         )
         # split out the hyperparameters whose values are complex objects
         hyperparameters, advanced_hyperparameters = split_hyperparameters(hyperparameters)
 
         hpo_mode = True if hyperparameter_tune_kwargs else False
@@ -909,22 +912,46 @@
             label=self.label,
             test_size=holdout_frac,
             problem_type=problem_type_for_split,
             random_state=random_state,
         )
         return train_data, tuning_data
 
-    def _verify_inference_ready(self):
+    def _init_pretrained(self):
+        # split out the hyperparameters whose values are complex objects
+        hyperparameters, advanced_hyperparameters = split_hyperparameters(self._hyperparameters)
+
+        if self._config is None:
+            self._config = get_config(
+                problem_type=self._problem_type, presets=self._presets, overrides=hyperparameters
+            )
+        if self._model is None:
+            assert (
+                len(self._config.model.names) == 1
+            ), f"Zero shot mode only supports using one model, but detects multiple models {self._config.model.names}"
+            self._model = create_fusion_model(
+                config=self._config, pretrained=self._pretrained, num_classes=self._output_shape, classes=self._classes
+            )
+        if self._data_processors is None:
+            self._data_processors = create_fusion_data_processors(
+                config=self._config,
+                model=self._model,
+                advanced_hyperparameters=advanced_hyperparameters,
+            )
+
+    def _ensure_inference_ready(self):
         if not self._fit_called:
-            if self._problem_type and not self.problem_property.support_zero_shot:
+            if not self._problem_type or not self.problem_property.support_zero_shot:
                 raise RuntimeError(
                     f"problem_type='{self._problem_type}' does not support running inference directly. "
                     f"You need to call `predictor.fit()`, or load a predictor first before "
                     f"running `predictor.predict()`, `predictor.evaluate()` or `predictor.extract_embedding()`."
                 )
+            else:
+                self._init_pretrained()
 
     def _setup_distillation(
         self,
         teacher_predictor: Union[str, MultiModalPredictor],
     ):
         """
         Prepare for distillation. It verifies whether the student and teacher predictors have consistent
@@ -1391,14 +1418,15 @@
         tb_logger = pl.loggers.TensorBoardLogger(
             save_dir=save_path,
             name="",
             version="",
         )
 
         num_gpus = compute_num_gpus(config_num_gpus=config.env.num_gpus, strategy=config.env.strategy)
+        logger.info(get_gpu_message(detected_num_gpus=ResourceManager.get_gpu_count_torch(), used_num_gpus=num_gpus))
 
         precision = infer_precision(num_gpus=num_gpus, precision=config.env.precision)
 
         if num_gpus == 0:  # CPU only training
             grad_steps = max(
                 config.env.batch_size // (config.env.per_gpu_batch_size * config.env.num_nodes),
                 1,
@@ -1491,15 +1519,15 @@
                 task,
                 datamodule=train_dm,
                 ckpt_path=ckpt_path if resume else None,  # this is to resume training that was broken accidentally
             )
 
         if trainer.global_rank == 0:
             # We do not perform averaging checkpoint in the case of hpo for each trial
-            # We only averaging the checkpoint of the best trial in the end in the master process
+            # We only average the checkpoint of the best trial at the end in the master process.
             if not hpo_mode:
                 self._top_k_average(
                     model=model,
                     save_path=save_path,
                     minmax_mode=minmax_mode,
                     is_distill=is_distill,
                     top_k_average_method=config.optimization.top_k_average_method,
@@ -1922,29 +1950,30 @@
             The eval_tool for object detection. Could be "pycocotools" or "torchmetrics".
 
         Returns
         -------
         A dictionary with the metric names and their corresponding scores.
         Optionally return a dataframe of prediction results.
         """
-        self._verify_inference_ready()
         if self._matcher:
             return self._matcher.evaluate(
                 data=data,
                 query_data=query_data,
                 response_data=response_data,
                 id_mappings=id_mappings,
                 chunk_size=chunk_size,
                 similarity_type=similarity_type,
                 cutoffs=cutoffs,
                 label=label,
                 metrics=metrics,
                 return_pred=return_pred,
                 realtime=realtime,
             )
+
+        self._ensure_inference_ready()
         if self._problem_type == OBJECT_DETECTION:
             if realtime:
                 return NotImplementedError(
                     f"Current problem type {self._problem_type} does not support realtime predict."
                 )
             if isinstance(data, str):
                 return evaluate_coco(
@@ -2112,23 +2141,23 @@
         save_results
             Whether to save the prediction results (only works for detection now)
 
         Returns
         -------
         Array of predictions, one corresponding to each row in given dataset.
         """
-        self._verify_inference_ready()
-
         if self._matcher:
             return self._matcher.predict(
                 data=data,
                 id_mappings=id_mappings,
                 as_pandas=as_pandas,
                 realtime=realtime,
             )
+
+        self._ensure_inference_ready()
         if self._problem_type == OBJECT_DETECTION:
             data = object_detection_data_to_df(data)
 
             if self._label_column not in data:
                 self._label_column = None
 
         if self._problem_type in [OBJECT_DETECTION, OCR_TEXT_DETECTION]:
@@ -2263,24 +2292,25 @@
 
         Returns
         -------
         Array of predicted class-probabilities, corresponding to each row in the given data.
         When as_multiclass is True, the output will always have shape (#samples, #classes).
         Otherwise, the output will have shape (#samples,)
         """
-        self._verify_inference_ready()
+
         if self._matcher:
             return self._matcher.predict_proba(
                 data=data,
                 id_mappings=id_mappings,
                 as_pandas=as_pandas,
                 as_multiclass=as_multiclass,
                 realtime=realtime,
             )
 
+        self._ensure_inference_ready()
         assert self._problem_type not in [
             REGRESSION,
         ], f"Problem {self._problem_type} has no probability output."
 
         if candidate_data:
             prob = self._match_queries_and_candidates(
                 query_data=data,
@@ -2351,25 +2381,25 @@
 
         Returns
         -------
         Array of embeddings, corresponding to each row in the given data.
         It will have shape (#samples, D) where the embedding dimension D is determined
         by the neural network's architecture.
         """
-        self._verify_inference_ready()
         if self._matcher:
             return self._matcher.extract_embedding(
                 data=data,
                 signature=signature,
                 id_mappings=id_mappings,
                 as_tensor=as_tensor,
                 as_pandas=as_pandas,
                 realtime=realtime,
             )
 
+        self._ensure_inference_ready()
         turn_on_off_feature_column_info(
             data_processors=self._data_processors,
             flag=True,
         )
         outputs = predict(
             predictor=self,
             data=data,
@@ -2504,14 +2534,15 @@
                     "problem_type": self._problem_type,
                     "presets": self._presets,
                     "eval_metric_name": self._eval_metric_name,
                     "validation_metric_name": self._validation_metric_name,
                     "output_shape": self._output_shape,
                     "classes": self._classes,
                     "save_path": self._save_path,
+                    "pretrained": self._pretrained,
                     "pretrained_path": self._pretrained_path,
                     "fit_called": self._fit_called,
                     "best_score": self._best_score,
                     "total_train_time": self._total_train_time,
                     "version": ag_version.__version__,
                 },
                 fp,
@@ -2604,15 +2635,17 @@
             predictor._best_score = assets["best_score"]
         if "total_train_time" in assets:  # backward compatibility
             predictor._total_train_time = assets["total_train_time"]
         predictor._eval_metric_name = assets["eval_metric_name"]
         predictor._verbosity = verbosity
         predictor._resume = resume
         predictor._save_path = path  # in case the original exp dir is copied to somewhere else
-        predictor._pretrain_path = path
+        predictor._pretrained_path = path
+        if "pretrained" in assets:
+            predictor._pretrained = assets["pretrained"]
         if "fit_called" in assets:
             predictor._fit_called = assets["fit_called"]
         else:
             predictor._fit_called = True  # backward compatible
         predictor._config = config
         predictor._output_shape = assets["output_shape"]
         if "classes" in assets:
@@ -2662,14 +2695,15 @@
             assets = json.load(fp)
         if "class_name" in assets and assets["class_name"] == "MultiModalMatcher":
             predictor._matcher = MultiModalMatcher.load(
                 path=path,
                 resume=resume,
                 verbosity=verbosity,
             )
+            predictor._problem_type = predictor._matcher._pipeline
             return predictor
 
         predictor = cls._load_metadata(predictor=predictor, path=dir_path, resume=resume, verbosity=verbosity)
 
         efficient_finetune = OmegaConf.select(predictor._config, "optimization.efficient_finetune")
 
         model = create_fusion_model(
```

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,14 @@
         "optimization.lr_decay": 0.9,
         "optimization.lr_mult": 100,
         "optimization.lr_choice": "two_stages",
         "optimization.top_k": 1,
         "optimization.top_k_average_method": "best",
         "optimization.warmup_steps": 0.0,
         "optimization.patience": 10,
-        "optimization.val_metric": "map",
         "optimization.val_check_interval": 0.5,
         "optimization.check_val_every_n_epoch": 1,
     }
     hyperparameter_tune_kwargs = {}
 
     presets, use_hpo = parse_presets_str(presets)
     if use_hpo:
```

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,22 @@
     is_interactive,
     move_to_device,
 )
 from .export import ExportMixin
 from .hpo import hyperparameter_tune
 from .inference import extract_from_output, infer_batch, predict, process_batch, use_realtime
 from .load import CustomUnpickler, get_dir_ckpt_paths, get_load_ckpt_paths, load_text_tokenizers
-from .log import LogFilter, apply_log_filter, get_fit_complete_message, get_fit_start_message, make_exp_dir
+from .log import (
+    LogFilter,
+    apply_log_filter,
+    get_fit_complete_message,
+    get_fit_start_message,
+    get_gpu_message,
+    make_exp_dir,
+)
 from .map import MeanAveragePrecision
 from .matcher import compute_semantic_similarity, convert_data_for_ranking, create_siamese_model, semantic_search
 from .metric import compute_ranking_score, compute_score, get_minmax_mode, get_stopping_threshold, infer_metrics
 from .misc import logits_to_prob, merge_bio_format, shopee_dataset, tensor_to_ndarray, visualize_ner
 from .mmcv import CollateMMDet, CollateMMOcr
 from .model import (
     create_fusion_model,
```

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime
 import logging
 import os
 from contextlib import contextmanager
 from typing import Dict, List, Optional, Tuple, Union
 
 import pytz
+import torch
 
-from ..constants import AUTOMM
+from .. import version as ag_version
 
 logger = logging.getLogger(__name__)
 
 
 def make_exp_dir(
     root_path: str,
     job_name: str,
@@ -138,14 +139,18 @@
         remove_log_filter(logging.getLogger("pytorch_lightning"), log_filter)
 
 
 def get_fit_start_message(save_path, validation_metric_name):
     return f"""\
 AutoMM starts to create your model. ✨
 
+- AutoGluon version is {ag_version.__version__}.
+
+- Pytorch version is {torch.__version__}.
+
 - Model will be saved to "{save_path}".
 
 - Validation metric is "{validation_metric_name}".
 
 - To track the learning progress, you can open a terminal and launch Tensorboard:
     ```shell
     # Assume you have installed tensorboard
@@ -173,7 +178,33 @@
     ```
 
 - If you are not satisfied with the model, try to increase the training time, 
 adjust the hyperparameters (https://auto.gluon.ai/stable/tutorials/multimodal/advanced_topics/customization.html),
 or post issues on GitHub: https://github.com/autogluon/autogluon
 
 """
+
+
+def get_gpu_message(detected_num_gpus: int, used_num_gpus: int):
+    """
+    Get the GPU related info (GPU name, total memory, free memory, and CUDA version) for logging.
+
+    Parameters
+    ----------
+    detected_num_gpus
+        Number of detected GPUs.
+    used_num_gpus
+        Number of GPUs to be used.
+
+    Returns
+    -------
+    A string with the GPU info.
+    """
+    gpu_message = f"{detected_num_gpus} GPUs are detected, and {used_num_gpus} GPUs will be used.\n"
+    for i in range(detected_num_gpus):
+        free_memory, total_memory = torch.cuda.mem_get_info(i)
+        gpu_message += f"   - GPU {i} name: {torch.cuda.get_device_name(i)}\n"
+        gpu_message += f"   - GPU {i} memory: {free_memory * 1e-9:.2f}GB/{total_memory * 1e-9:.2f}GB (Free/Total)\n"
+    if torch.cuda.is_available():
+        gpu_message += f"CUDA version is {torch.version.cuda}.\n"
+
+    return gpu_message
```

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230609/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230608
+Version: 0.7.1b20230609
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230609/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230608
-autogluon.features==0.7.1b20230608
-autogluon.common==0.7.1b20230608
+autogluon.core[raytune]==0.7.1b20230609
+autogluon.features==0.7.1b20230609
+autogluon.common==0.7.1b20230609
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

