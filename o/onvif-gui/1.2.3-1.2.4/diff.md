# Comparing `tmp/onvif-gui-1.2.3.tar.gz` & `tmp/onvif-gui-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.2.3.tar", last modified: Tue Jun  6 16:18:04 2023, max compression
+gzip compressed data, was "onvif-gui-1.2.4.tar", last modified: Fri Jun  9 16:06:35 2023, max compression
```

## Comparing `onvif-gui-1.2.3.tar` & `onvif-gui-1.2.4.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.531755 onvif-gui-1.2.3/
--rw-rw-rw-   0        0        0    11558 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      221 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9056 2023-06-06 16:18:04.530759 onvif-gui-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     8359 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.817764 onvif-gui-1.2.3/detectron2/
--rw-rw-rw-   0        0        0       68 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.832715 onvif-gui-1.2.3/detectron2/checkpoint/
--rw-rw-rw-   0        0        0      357 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/__init__.py
--rw-rw-rw-   0        0        0    18177 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/c2_model_loading.py
--rw-rw-rw-   0        0        0     5800 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/catalog.py
--rw-rw-rw-   0        0        0     5379 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.855638 onvif-gui-1.2.3/detectron2/config/
--rw-rw-rw-   0        0        0      623 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/__init__.py
--rw-rw-rw-   0        0        0     8119 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/compat.py
--rw-rw-rw-   0        0        0     9476 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/config.py
--rw-rw-rw-   0        0        0    30158 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/defaults.py
--rw-rw-rw-   0        0        0     3103 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/instantiate.py
--rw-rw-rw-   0        0        0    15786 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/lazy.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.858628 onvif-gui-1.2.3/detectron2/configs/
--rw-rw-rw-   0        0        0     1360 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/Base-RCNN-FPN.yaml
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.861618 onvif-gui-1.2.3/detectron2/configs/COCO-InstanceSegmentation/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-rw-rw-   0        0        0      201 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.866956 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/
--rw-rw-rw-   0        0        0      542 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/__init__.py
--rw-rw-rw-   0        0        0      190 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.891875 onvif-gui-1.2.3/detectron2/data/
--rw-rw-rw-   0        0        0      663 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/__init__.py
--rw-rw-rw-   0        0        0     7603 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/benchmark.py
--rw-rw-rw-   0        0        0    21787 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/build.py
--rw-rw-rw-   0        0        0     7460 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/catalog.py
--rw-rw-rw-   0        0        0     9406 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/common.py
--rw-rw-rw-   0        0        0     8360 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.938718 onvif-gui-1.2.3/detectron2/data/datasets/
--rw-rw-rw-   0        0        0      532 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    10433 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/builtin.py
--rw-rw-rw-   0        0        0    22191 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/builtin_meta.py
--rw-rw-rw-   0        0        0    13496 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/cityscapes.py
--rw-rw-rw-   0        0        0     8008 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/cityscapes_panoptic.py
--rw-rw-rw-   0        0        0    24004 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/coco.py
--rw-rw-rw-   0        0        0     9205 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/coco_panoptic.py
--rw-rw-rw-   0        0        0     9864 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis.py
--rw-rw-rw-   0        0        0   223770 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-rw-rw-   0        0        0   219193 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_categories.py
--rw-rw-rw-   0        0        0    39434 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-rw-rw-   0        0        0     3210 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/pascal_voc.py
--rw-rw-rw-   0        0        0      172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/register_coco.py
--rw-rw-rw-   0        0        0    23487 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/detection_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.947688 onvif-gui-1.2.3/detectron2/data/samplers/
--rw-rw-rw-   0        0        0      429 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/samplers/__init__.py
--rw-rw-rw-   0        0        0    12067 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/samplers/distributed_sampler.py
--rw-rw-rw-   0        0        0     1991 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.960645 onvif-gui-1.2.3/detectron2/data/transforms/
--rw-rw-rw-   0        0        0      480 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/__init__.py
--rw-rw-rw-   0        0        0    14492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/augmentation.py
--rw-rw-rw-   0        0        0    23683 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/augmentation_impl.py
--rw-rw-rw-   0        0        0    12980 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/transform.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.004168 onvif-gui-1.2.3/detectron2/layers/
--rw-rw-rw-   0        0        0      900 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/__init__.py
--rw-rw-rw-   0        0        0     5908 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/aspp.py
--rw-rw-rw-   0        0        0    12431 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/batch_norm.py
--rw-rw-rw-   0        0        0     3135 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/blocks.py
--rw-rw-rw-   0        0        0    17492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/deform_conv.py
--rw-rw-rw-   0        0        0     4335 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/losses.py
--rw-rw-rw-   0        0        0    11154 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/mask_ops.py
--rw-rw-rw-   0        0        0     6629 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/nms.py
--rw-rw-rw-   0        0        0     3172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/roi_align.py
--rw-rw-rw-   0        0        0     3393 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/roi_align_rotated.py
--rw-rw-rw-   0        0        0      673 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/rotated_boxes.py
--rw-rw-rw-   0        0        0      555 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/shape_spec.py
--rw-rw-rw-   0        0        0     5271 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.033071 onvif-gui-1.2.3/detectron2/modeling/
--rw-rw-rw-   0        0        0     1632 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/__init__.py
--rw-rw-rw-   0        0        0    15825 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.068838 onvif-gui-1.2.3/detectron2/modeling/backbone/
--rw-rw-rw-   0        0        0      618 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/backbone.py
--rw-rw-rw-   0        0        0     1048 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/build.py
--rw-rw-rw-   0        0        0    10628 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/fpn.py
--rw-rw-rw-   0        0        0    16434 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/mvit.py
--rw-rw-rw-   0        0        0    17108 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/regnet.py
--rw-rw-rw-   0        0        0    24352 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/resnet.py
--rw-rw-rw-   0        0        0    25785 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/swin.py
--rw-rw-rw-   0        0        0     6546 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/utils.py
--rw-rw-rw-   0        0        0    19860 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/vit.py
--rw-rw-rw-   0        0        0    15492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/box_regression.py
--rw-rw-rw-   0        0        0     6391 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/matcher.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.100696 onvif-gui-1.2.3/detectron2/modeling/meta_arch/
--rw-rw-rw-   0        0        0      524 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/__init__.py
--rw-rw-rw-   0        0        0      839 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/build.py
--rw-rw-rw-   0        0        0    11940 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/dense_detector.py
--rw-rw-rw-   0        0        0    13541 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/fcos.py
--rw-rw-rw-   0        0        0    10676 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-rw-rw-   0        0        0    14237 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/rcnn.py
--rw-rw-rw-   0        0        0    18704 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/retinanet.py
--rw-rw-rw-   0        0        0    10173 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/semantic_seg.py
--rw-rw-rw-   0        0        0    11104 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/mmdet_wrapper.py
--rw-rw-rw-   0        0        0    11575 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/poolers.py
--rw-rw-rw-   0        0        0     4145 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.117131 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/
--rw-rw-rw-   0        0        0      236 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/__init__.py
--rw-rw-rw-   0        0        0      860 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/build.py
--rw-rw-rw-   0        0        0     8333 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-rw-rw-   0        0        0    24347 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rpn.py
--rw-rw-rw-   0        0        0     9016 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.143585 onvif-gui-1.2.3/detectron2/modeling/roi_heads/
--rw-rw-rw-   0        0        0      797 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/__init__.py
--rw-rw-rw-   0        0        0     4195 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/box_head.py
--rw-rw-rw-   0        0        0    13289 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-rw-rw-   0        0        0    25959 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-rw-rw-   0        0        0    11428 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/keypoint_head.py
--rw-rw-rw-   0        0        0    12467 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/mask_head.py
--rw-rw-rw-   0        0        0    38578 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/roi_heads.py
--rw-rw-rw-   0        0        0    11446 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-rw-rw-   0        0        0     2388 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/sampling.py
--rw-rw-rw-   0        0        0    12723 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/test_time_augmentation.py
--rw-rw-rw-   0        0        0     1829 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/predictor.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.167351 onvif-gui-1.2.3/detectron2/structures/
--rw-rw-rw-   0        0        0      662 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/__init__.py
--rw-rw-rw-   0        0        0    14854 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/boxes.py
--rw-rw-rw-   0        0        0     5649 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/image_list.py
--rw-rw-rw-   0        0        0     6807 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/instances.py
--rw-rw-rw-   0        0        0     9269 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/keypoints.py
--rw-rw-rw-   0        0        0    20336 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/masks.py
--rw-rw-rw-   0        0        0    19356 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/rotated_boxes.py
--rw-rw-rw-   0        0        0     2775 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.224177 onvif-gui-1.2.3/detectron2/utils/
--rw-rw-rw-   0        0        0       52 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/__init__.py
--rw-rw-rw-   0        0        0     6205 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/analysis.py
--rw-rw-rw-   0        0        0     8633 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/collect_env.py
--rw-rw-rw-   0        0        0     4254 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/colormap.py
--rw-rw-rw-   0        0        0     5807 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/comm.py
--rw-rw-rw-   0        0        0     1911 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/develop.py
--rw-rw-rw-   0        0        0     5814 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/env.py
--rw-rw-rw-   0        0        0    17508 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/events.py
--rw-rw-rw-   0        0        0     1226 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/file_io.py
--rw-rw-rw-   0        0        0     8044 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/logger.py
--rw-rw-rw-   0        0        0     2667 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/memory.py
--rw-rw-rw-   0        0        0     1934 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/registry.py
--rw-rw-rw-   0        0        0     1096 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/serialize.py
--rw-rw-rw-   0        0        0    18576 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/testing.py
--rw-rw-rw-   0        0        0    11606 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/video_visualizer.py
--rw-rw-rw-   0        0        0    52426 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.236097 onvif-gui-1.2.3/gui/
--rw-rw-rw-   0        0        0       28 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.259860 onvif-gui-1.2.3/gui/components/
--rw-rw-rw-   0        0        0      286 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/components/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/comboselector.py
--rw-rw-rw-   0        0        0     2459 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/directoryselector.py
--rw-rw-rw-   0        0        0     2172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/fileselector.py
--rw-rw-rw-   0        0        0     6416 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/components/labelselector.py
--rw-rw-rw-   0        0        0     4194 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/progress.py
--rw-rw-rw-   0        0        0     1962 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/thresholdslider.py
--rw-rw-rw-   0        0        0      855 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/components/waitdialog.py
--rw-rw-rw-   0        0        0     2054 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/glwidget.py
--rw-rw-rw-   0        0        0    17483 2023-06-06 16:00:40.000000 onvif-gui-1.2.3/gui/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.282627 onvif-gui-1.2.3/gui/onvif/
--rw-rw-rw-   0        0        0      196 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/__init__.py
--rw-rw-rw-   0        0        0     5870 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/admintab.py
--rw-rw-rw-   0        0        0     4051 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/imagetab.py
--rw-rw-rw-   0        0        0     2484 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/logindialog.py
--rw-rw-rw-   0        0        0     5364 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/networktab.py
--rw-rw-rw-   0        0        0     5241 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/ptztab.py
--rw-rw-rw-   0        0        0     4640 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/videotab.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.300061 onvif-gui-1.2.3/gui/panels/
--rw-rw-rw-   0        0        0      184 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/panels/__init__.py
--rw-rw-rw-   0        0        0     3802 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/audiopanel.py
--rw-rw-rw-   0        0        0    13667 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/camerapanel.py
--rw-rw-rw-   0        0        0    14756 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/filepanel.py
--rw-rw-rw-   0        0        0    14134 2023-06-06 15:29:24.000000 onvif-gui-1.2.3/gui/panels/settingspanel.py
--rw-rw-rw-   0        0        0     3806 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/videopanel.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.341396 onvif-gui-1.2.3/gui/resources/
--rw-rw-rw-   0        0        0     2021 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/LICENSE
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/__init__.py
--rw-rw-rw-   0        0        0      252 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/apply.png
--rw-rw-rw-   0        0        0      245 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/apply_hi.png
--rw-rw-rw-   0        0        0      244 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/apply_lo.png
--rw-rw-rw-   0        0        0      911 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/audio.png
--rw-rw-rw-   0        0        0      536 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/audio_hi.png
--rw-rw-rw-   0        0        0      920 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/audio_lo.png
--rw-rw-rw-   0        0        0      203 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_closed.png
--rw-rw-rw-   0        0        0      219 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_closed_hi.png
--rw-rw-rw-   0        0        0      211 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_closed_lo.png
--rw-rw-rw-   0        0        0      199 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_open.png
--rw-rw-rw-   0        0        0      168 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_open_hi.png
--rw-rw-rw-   0        0        0      172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_open_lo.png
--rw-rw-rw-   0        0        0      267 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/checked.png
--rw-rw-rw-   0        0        0      235 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/checked_hi.png
--rw-rw-rw-   0        0        0      246 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/checked_lo.png
--rw-rw-rw-   0        0        0    13358 2023-05-26 17:50:15.000000 onvif-gui-1.2.3/gui/resources/darkstyle.qss
--rw-rw-rw-   0        0        0      910 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/discover.png
--rw-rw-rw-   0        0        0      849 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/discover_hi.png
--rw-rw-rw-   0        0        0      937 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/discover_lo.png
--rw-rw-rw-   0        0        0      425 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/fast-forward.png
--rw-rw-rw-   0        0        0      253 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/fast-forward_hi.png
--rw-rw-rw-   0        0        0      433 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/fast-forward_lo.png
--rw-rw-rw-   0        0        0      641 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/mute.png
--rw-rw-rw-   0        0        0      346 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/mute_hi.png
--rw-rw-rw-   0        0        0      618 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/mute_lo.png
--rw-rw-rw-   0        0        0      347 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/next.png
--rw-rw-rw-   0        0        0      225 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/next_hi.png
--rw-rw-rw-   0        0        0      348 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/next_lo.png
--rw-rw-rw-   0        0        0   207707 2023-06-04 21:18:37.000000 onvif-gui-1.2.3/gui/resources/onvif-gui.ico
--rw-rw-rw-   0        0        0    46084 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/onvif-gui.png
--rw-rw-rw-   0        0        0      172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/pause.png
--rw-rw-rw-   0        0        0      144 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/pause_hi.png
--rw-rw-rw-   0        0        0      149 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/pause_lo.png
--rw-rw-rw-   0        0        0      321 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/play.png
--rw-rw-rw-   0        0        0      209 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/play_hi.png
--rw-rw-rw-   0        0        0      316 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/play_lo.png
--rw-rw-rw-   0        0        0      349 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/previous.png
--rw-rw-rw-   0        0        0      232 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/previous_hi.png
--rw-rw-rw-   0        0        0      348 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/previous_lo.png
--rw-rw-rw-   0        0        0      324 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-off.png
--rw-rw-rw-   0        0        0      250 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-off_hi.png
--rw-rw-rw-   0        0        0      324 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-off_lo.png
--rw-rw-rw-   0        0        0      350 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-on.png
--rw-rw-rw-   0        0        0      263 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-on_hi.png
--rw-rw-rw-   0        0        0      343 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-on_lo.png
--rw-rw-rw-   0        0        0      395 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/record.png
--rw-rw-rw-   0        0        0      394 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/record_hi.png
--rw-rw-rw-   0        0        0      425 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/record_lo.png
--rw-rw-rw-   0        0        0      408 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/recording.png
--rw-rw-rw-   0        0        0      435 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/recording_hi.png
--rw-rw-rw-   0        0        0      532 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/recording_lo.png
--rw-rw-rw-   0        0        0      454 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/rewind.png
--rw-rw-rw-   0        0        0      250 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/rewind_hi.png
--rw-rw-rw-   0        0        0      457 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/rewind_lo.png
--rw-rw-rw-   0        0        0      187 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_left.png
--rw-rw-rw-   0        0        0      183 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_left_hi.png
--rw-rw-rw-   0        0        0      189 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_left_lo.png
--rw-rw-rw-   0        0        0      162 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_up.png
--rw-rw-rw-   0        0        0      160 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_up_hi.png
--rw-rw-rw-   0        0        0      161 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_up_lo.png
--rw-rw-rw-   0        0        0    19236 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/resources/spinner.gif
--rw-rw-rw-   0        0        0      158 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/stop.png
--rw-rw-rw-   0        0        0      140 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/stop_hi.png
--rw-rw-rw-   0        0        0      151 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/stop_lo.png
--rw-rw-rw-   0        0        0      143 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/unchecked.png
--rw-rw-rw-   0        0        0      142 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/unchecked_hi.png
--rw-rw-rw-   0        0        0      143 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/unchecked_lo.png
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.341396 onvif-gui-1.2.3/modules/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.345379 onvif-gui-1.2.3/modules/audio/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/audio/__init__.py
--rw-rw-rw-   0        0        0     3492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/audio/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.370296 onvif-gui-1.2.3/modules/video/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/video/__init__.py
--rw-rw-rw-   0        0        0     8911 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/keypoint.py
--rw-rw-rw-   0        0        0     6297 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/retinanet.py
--rw-rw-rw-   0        0        0     3244 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/sample.py
--rw-rw-rw-   0        0        0     9442 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/segment.py
--rw-rw-rw-   0        0        0    16288 2023-06-05 18:24:56.000000 onvif-gui-1.2.3/modules/video/yolov7.py
--rw-rw-rw-   0        0        0    15675 2023-06-05 18:24:50.000000 onvif-gui-1.2.3/modules/video/yolov8.py
--rw-rw-rw-   0        0        0    17631 2023-06-05 14:49:36.000000 onvif-gui-1.2.3/modules/video/yolox.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.387239 onvif-gui-1.2.3/onvif_gui.egg-info/
--rw-rw-rw-   0        0        0     9056 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8475 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1688 2023-06-06 16:00:30.000000 onvif-gui-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 16:18:04.531755 onvif-gui-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1549 2023-06-06 16:00:23.000000 onvif-gui-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.408169 onvif-gui-1.2.3/tracker/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/basetrack.py
--rw-rw-rw-   0        0        0    12632 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/byte_tracker.py
--rw-rw-rw-   0        0        0     9816 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/kalman_filter.py
--rw-rw-rw-   0        0        0     6304 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/matching.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.408169 onvif-gui-1.2.3/yolov7/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.430096 onvif-gui-1.2.3/yolov7/models/
--rw-rw-rw-   0        0        0        6 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/__init__.py
--rw-rw-rw-   0        0        0    86435 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/common.py
--rw-rw-rw-   0        0        0    11177 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/experimental.py
--rw-rw-rw-   0        0        0    40895 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.484912 onvif-gui-1.2.3/yolov7/utils/
--rw-rw-rw-   0        0        0        6 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/__init__.py
--rw-rw-rw-   0        0        0     2320 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/activations.py
--rw-rw-rw-   0        0        0     5771 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/add_nms.py
--rw-rw-rw-   0        0        0     7321 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/autoanchor.py
--rw-rw-rw-   0        0        0    57559 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/datasets.py
--rw-rw-rw-   0        0        0    37789 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/general.py
--rw-rw-rw-   0        0        0     4996 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/google_utils.py
--rw-rw-rw-   0        0        0    76741 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/loss.py
--rw-rw-rw-   0        0        0     9537 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/metrics.py
--rw-rw-rw-   0        0        0    21424 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/plots.py
--rw-rw-rw-   0        0        0    15840 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.485909 onvif-gui-1.2.3/yolox/
--rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.523782 onvif-gui-1.2.3/yolox/models/
--rw-rw-rw-   0        0        0      961 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/__init__.py
--rw-rw-rw-   0        0        0     5019 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/build.py
--rw-rw-rw-   0        0        0     6840 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/darknet.py
--rw-rw-rw-   0        0        0     2372 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/losses.py
--rw-rw-rw-   0        0        0     6944 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/network_blocks.py
--rw-rw-rw-   0        0        0     3202 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolo_fpn.py
--rw-rw-rw-   0        0        0    26204 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolo_head.py
--rw-rw-rw-   0        0        0     4288 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolo_pafpn.py
--rw-rw-rw-   0        0        0     2054 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolox.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.530759 onvif-gui-1.2.3/yolox/utils/
--rw-rw-rw-   0        0        0      130 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/utils/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.680408 onvif-gui-1.2.4/
+-rw-rw-rw-   0        0        0    11558 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0      221 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9056 2023-06-09 16:06:35.680408 onvif-gui-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8359 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.446088 onvif-gui-1.2.4/detectron2/
+-rw-rw-rw-   0        0        0       68 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.446088 onvif-gui-1.2.4/detectron2/checkpoint/
+-rw-rw-rw-   0        0        0      357 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/checkpoint/__init__.py
+-rw-rw-rw-   0        0        0    18177 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-rw-   0        0        0     5800 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/checkpoint/catalog.py
+-rw-rw-rw-   0        0        0     5379 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.446088 onvif-gui-1.2.4/detectron2/config/
+-rw-rw-rw-   0        0        0      623 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/config/__init__.py
+-rw-rw-rw-   0        0        0     8119 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/config/compat.py
+-rw-rw-rw-   0        0        0     9476 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/config/config.py
+-rw-rw-rw-   0        0        0    30158 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/config/defaults.py
+-rw-rw-rw-   0        0        0     3103 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/config/instantiate.py
+-rw-rw-rw-   0        0        0    15786 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/config/lazy.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.446088 onvif-gui-1.2.4/detectron2/configs/
+-rw-rw-rw-   0        0        0     1360 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/Base-RCNN-FPN.yaml
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.446088 onvif-gui-1.2.4/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.461710 onvif-gui-1.2.4/detectron2/configs/COCO-Keypoints/
+-rw-rw-rw-   0        0        0      542 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.461710 onvif-gui-1.2.4/detectron2/data/
+-rw-rw-rw-   0        0        0      663 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/__init__.py
+-rw-rw-rw-   0        0        0     7603 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/benchmark.py
+-rw-rw-rw-   0        0        0    21787 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/build.py
+-rw-rw-rw-   0        0        0     7460 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/catalog.py
+-rw-rw-rw-   0        0        0     9406 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/common.py
+-rw-rw-rw-   0        0        0     8360 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.477331 onvif-gui-1.2.4/detectron2/data/datasets/
+-rw-rw-rw-   0        0        0      532 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    10433 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/builtin.py
+-rw-rw-rw-   0        0        0    22191 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/builtin_meta.py
+-rw-rw-rw-   0        0        0    13496 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/cityscapes.py
+-rw-rw-rw-   0        0        0     8008 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-rw-   0        0        0    24004 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/coco.py
+-rw-rw-rw-   0        0        0     9205 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-rw-   0        0        0     9864 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/lvis.py
+-rw-rw-rw-   0        0        0   223770 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-rw-   0        0        0   219193 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-rw-   0        0        0    39434 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-rw-   0        0        0     3210 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/pascal_voc.py
+-rw-rw-rw-   0        0        0      172 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/datasets/register_coco.py
+-rw-rw-rw-   0        0        0    23487 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/detection_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.477331 onvif-gui-1.2.4/detectron2/data/samplers/
+-rw-rw-rw-   0        0        0      429 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/samplers/__init__.py
+-rw-rw-rw-   0        0        0    12067 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-rw-   0        0        0     1991 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.477331 onvif-gui-1.2.4/detectron2/data/transforms/
+-rw-rw-rw-   0        0        0      480 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/transforms/__init__.py
+-rw-rw-rw-   0        0        0    14492 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/transforms/augmentation.py
+-rw-rw-rw-   0        0        0    23683 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-rw-   0        0        0    12980 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/data/transforms/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.477331 onvif-gui-1.2.4/detectron2/layers/
+-rw-rw-rw-   0        0        0      900 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/__init__.py
+-rw-rw-rw-   0        0        0     5908 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/aspp.py
+-rw-rw-rw-   0        0        0    12431 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/batch_norm.py
+-rw-rw-rw-   0        0        0     3135 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/blocks.py
+-rw-rw-rw-   0        0        0    17492 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/deform_conv.py
+-rw-rw-rw-   0        0        0     4335 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/losses.py
+-rw-rw-rw-   0        0        0    11154 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/mask_ops.py
+-rw-rw-rw-   0        0        0     6629 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/nms.py
+-rw-rw-rw-   0        0        0     3172 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/roi_align.py
+-rw-rw-rw-   0        0        0     3393 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/roi_align_rotated.py
+-rw-rw-rw-   0        0        0      673 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/rotated_boxes.py
+-rw-rw-rw-   0        0        0      555 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/shape_spec.py
+-rw-rw-rw-   0        0        0     5271 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/layers/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.492952 onvif-gui-1.2.4/detectron2/modeling/
+-rw-rw-rw-   0        0        0     1632 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/__init__.py
+-rw-rw-rw-   0        0        0    15825 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.492952 onvif-gui-1.2.4/detectron2/modeling/backbone/
+-rw-rw-rw-   0        0        0      618 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/backbone.py
+-rw-rw-rw-   0        0        0     1048 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/build.py
+-rw-rw-rw-   0        0        0    10628 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/fpn.py
+-rw-rw-rw-   0        0        0    16434 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/mvit.py
+-rw-rw-rw-   0        0        0    17108 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/regnet.py
+-rw-rw-rw-   0        0        0    24352 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/resnet.py
+-rw-rw-rw-   0        0        0    25785 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/swin.py
+-rw-rw-rw-   0        0        0     6546 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/utils.py
+-rw-rw-rw-   0        0        0    19860 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/backbone/vit.py
+-rw-rw-rw-   0        0        0    15492 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/box_regression.py
+-rw-rw-rw-   0        0        0     6391 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/matcher.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.508573 onvif-gui-1.2.4/detectron2/modeling/meta_arch/
+-rw-rw-rw-   0        0        0      524 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-rw-   0        0        0      839 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/build.py
+-rw-rw-rw-   0        0        0    11940 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-rw-   0        0        0    13541 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-rw-   0        0        0    10676 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-rw-   0        0        0    14237 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-rw-   0        0        0    18704 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-rw-   0        0        0    10173 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-rw-   0        0        0    11104 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-rw-   0        0        0    11575 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/poolers.py
+-rw-rw-rw-   0        0        0     4145 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.508573 onvif-gui-1.2.4/detectron2/modeling/proposal_generator/
+-rw-rw-rw-   0        0        0      236 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/proposal_generator/build.py
+-rw-rw-rw-   0        0        0     8333 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-rw-   0        0        0    24347 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-rw-   0        0        0     9016 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.508573 onvif-gui-1.2.4/detectron2/modeling/roi_heads/
+-rw-rw-rw-   0        0        0      797 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-rw-   0        0        0     4195 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-rw-   0        0        0    13289 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-rw-   0        0        0    25959 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-rw-   0        0        0    11428 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-rw-   0        0        0    12467 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-rw-   0        0        0    38578 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-rw-   0        0        0    11446 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-rw-   0        0        0     2388 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/sampling.py
+-rw-rw-rw-   0        0        0    12723 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/modeling/test_time_augmentation.py
+-rw-rw-rw-   0        0        0     1829 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/predictor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.524195 onvif-gui-1.2.4/detectron2/structures/
+-rw-rw-rw-   0        0        0      662 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/__init__.py
+-rw-rw-rw-   0        0        0    14854 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/boxes.py
+-rw-rw-rw-   0        0        0     5649 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/image_list.py
+-rw-rw-rw-   0        0        0     6807 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/instances.py
+-rw-rw-rw-   0        0        0     9269 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/keypoints.py
+-rw-rw-rw-   0        0        0    20336 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/masks.py
+-rw-rw-rw-   0        0        0    19356 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/structures/rotated_boxes.py
+-rw-rw-rw-   0        0        0     2775 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/tracker.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.524195 onvif-gui-1.2.4/detectron2/utils/
+-rw-rw-rw-   0        0        0       52 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/__init__.py
+-rw-rw-rw-   0        0        0     6205 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/analysis.py
+-rw-rw-rw-   0        0        0     8633 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/collect_env.py
+-rw-rw-rw-   0        0        0     4254 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/colormap.py
+-rw-rw-rw-   0        0        0     5807 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/comm.py
+-rw-rw-rw-   0        0        0     1911 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/develop.py
+-rw-rw-rw-   0        0        0     5814 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/env.py
+-rw-rw-rw-   0        0        0    17508 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/events.py
+-rw-rw-rw-   0        0        0     1226 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/file_io.py
+-rw-rw-rw-   0        0        0     8044 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/logger.py
+-rw-rw-rw-   0        0        0     2667 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/memory.py
+-rw-rw-rw-   0        0        0     1934 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/registry.py
+-rw-rw-rw-   0        0        0     1096 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/serialize.py
+-rw-rw-rw-   0        0        0    18576 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/testing.py
+-rw-rw-rw-   0        0        0    11606 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/video_visualizer.py
+-rw-rw-rw-   0        0        0    52426 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/detectron2/utils/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.539816 onvif-gui-1.2.4/gui/
+-rw-rw-rw-   0        0        0       28 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.539816 onvif-gui-1.2.4/gui/components/
+-rw-rw-rw-   0        0        0      286 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/__init__.py
+-rw-rw-rw-   0        0        0     1824 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/comboselector.py
+-rw-rw-rw-   0        0        0     2459 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/directoryselector.py
+-rw-rw-rw-   0        0        0     2172 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/fileselector.py
+-rw-rw-rw-   0        0        0     6416 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/labelselector.py
+-rw-rw-rw-   0        0        0     4194 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/progress.py
+-rw-rw-rw-   0        0        0     1962 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/thresholdslider.py
+-rw-rw-rw-   0        0        0      855 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/components/waitdialog.py
+-rw-rw-rw-   0        0        0     2054 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/glwidget.py
+-rw-rw-rw-   0        0        0    17484 2023-06-09 16:05:33.000000 onvif-gui-1.2.4/gui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.555438 onvif-gui-1.2.4/gui/onvif/
+-rw-rw-rw-   0        0        0      196 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/__init__.py
+-rw-rw-rw-   0        0        0     5870 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/admintab.py
+-rw-rw-rw-   0        0        0     4051 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/imagetab.py
+-rw-rw-rw-   0        0        0     2484 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/logindialog.py
+-rw-rw-rw-   0        0        0     5364 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/networktab.py
+-rw-rw-rw-   0        0        0     5241 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/ptztab.py
+-rw-rw-rw-   0        0        0     4640 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/onvif/videotab.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.555438 onvif-gui-1.2.4/gui/panels/
+-rw-rw-rw-   0        0        0      184 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/panels/__init__.py
+-rw-rw-rw-   0        0        0     3802 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/panels/audiopanel.py
+-rw-rw-rw-   0        0        0    13667 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/panels/camerapanel.py
+-rw-rw-rw-   0        0        0    14756 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/panels/filepanel.py
+-rw-rw-rw-   0        0        0    14134 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/panels/settingspanel.py
+-rw-rw-rw-   0        0        0     3806 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/panels/videopanel.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.602302 onvif-gui-1.2.4/gui/resources/
+-rw-rw-rw-   0        0        0     2021 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/apply.png
+-rw-rw-rw-   0        0        0      245 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/apply_hi.png
+-rw-rw-rw-   0        0        0      244 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/apply_lo.png
+-rw-rw-rw-   0        0        0      911 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/audio.png
+-rw-rw-rw-   0        0        0      536 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/audio_hi.png
+-rw-rw-rw-   0        0        0      920 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/audio_lo.png
+-rw-rw-rw-   0        0        0      203 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/branch_closed.png
+-rw-rw-rw-   0        0        0      219 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/branch_closed_hi.png
+-rw-rw-rw-   0        0        0      211 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/branch_closed_lo.png
+-rw-rw-rw-   0        0        0      199 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/branch_open.png
+-rw-rw-rw-   0        0        0      168 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/branch_open_hi.png
+-rw-rw-rw-   0        0        0      172 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/branch_open_lo.png
+-rw-rw-rw-   0        0        0      267 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/checked.png
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/checked_hi.png
+-rw-rw-rw-   0        0        0      246 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/checked_lo.png
+-rw-rw-rw-   0        0        0    13358 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/darkstyle.qss
+-rw-rw-rw-   0        0        0      910 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/discover.png
+-rw-rw-rw-   0        0        0      849 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/discover_hi.png
+-rw-rw-rw-   0        0        0      937 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/discover_lo.png
+-rw-rw-rw-   0        0        0      425 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/fast-forward.png
+-rw-rw-rw-   0        0        0      253 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/fast-forward_hi.png
+-rw-rw-rw-   0        0        0      433 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/fast-forward_lo.png
+-rw-rw-rw-   0        0        0      641 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/mute.png
+-rw-rw-rw-   0        0        0      346 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/mute_hi.png
+-rw-rw-rw-   0        0        0      618 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/mute_lo.png
+-rw-rw-rw-   0        0        0      347 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/next.png
+-rw-rw-rw-   0        0        0      225 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/next_hi.png
+-rw-rw-rw-   0        0        0      348 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/next_lo.png
+-rw-rw-rw-   0        0        0   207707 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/onvif-gui.ico
+-rw-rw-rw-   0        0        0    46084 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/onvif-gui.png
+-rw-rw-rw-   0        0        0      172 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/pause.png
+-rw-rw-rw-   0        0        0      144 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/pause_hi.png
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/pause_lo.png
+-rw-rw-rw-   0        0        0      321 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/play.png
+-rw-rw-rw-   0        0        0      209 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/play_hi.png
+-rw-rw-rw-   0        0        0      316 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/play_lo.png
+-rw-rw-rw-   0        0        0      349 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/previous.png
+-rw-rw-rw-   0        0        0      232 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/previous_hi.png
+-rw-rw-rw-   0        0        0      348 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/previous_lo.png
+-rw-rw-rw-   0        0        0      324 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/radio-off.png
+-rw-rw-rw-   0        0        0      250 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/radio-off_hi.png
+-rw-rw-rw-   0        0        0      324 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/radio-off_lo.png
+-rw-rw-rw-   0        0        0      350 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/radio-on.png
+-rw-rw-rw-   0        0        0      263 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/radio-on_hi.png
+-rw-rw-rw-   0        0        0      343 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/radio-on_lo.png
+-rw-rw-rw-   0        0        0      395 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/record.png
+-rw-rw-rw-   0        0        0      394 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/record_hi.png
+-rw-rw-rw-   0        0        0      425 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/record_lo.png
+-rw-rw-rw-   0        0        0      408 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/recording.png
+-rw-rw-rw-   0        0        0      435 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/recording_hi.png
+-rw-rw-rw-   0        0        0      532 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/recording_lo.png
+-rw-rw-rw-   0        0        0      454 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/rewind.png
+-rw-rw-rw-   0        0        0      250 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/rewind_hi.png
+-rw-rw-rw-   0        0        0      457 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/rewind_lo.png
+-rw-rw-rw-   0        0        0      187 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/small_arrow_left.png
+-rw-rw-rw-   0        0        0      183 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/small_arrow_left_hi.png
+-rw-rw-rw-   0        0        0      189 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/small_arrow_left_lo.png
+-rw-rw-rw-   0        0        0      162 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/small_arrow_up.png
+-rw-rw-rw-   0        0        0      160 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/small_arrow_up_hi.png
+-rw-rw-rw-   0        0        0      161 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/small_arrow_up_lo.png
+-rw-rw-rw-   0        0        0    19236 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/spinner.gif
+-rw-rw-rw-   0        0        0      158 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/stop.png
+-rw-rw-rw-   0        0        0      140 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/stop_hi.png
+-rw-rw-rw-   0        0        0      151 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/stop_lo.png
+-rw-rw-rw-   0        0        0      143 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/unchecked.png
+-rw-rw-rw-   0        0        0      142 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/unchecked_hi.png
+-rw-rw-rw-   0        0        0      143 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/gui/resources/unchecked_lo.png
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.602302 onvif-gui-1.2.4/modules/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.617923 onvif-gui-1.2.4/modules/audio/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/modules/audio/__init__.py
+-rw-rw-rw-   0        0        0     3492 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/modules/audio/sample.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.633545 onvif-gui-1.2.4/modules/video/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/modules/video/__init__.py
+-rw-rw-rw-   0        0        0     8912 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/keypoint.py
+-rw-rw-rw-   0        0        0     5977 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/retinanet.py
+-rw-rw-rw-   0        0        0     3418 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/sample.py
+-rw-rw-rw-   0        0        0     9443 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/segment.py
+-rw-rw-rw-   0        0        0    16289 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/yolov7.py
+-rw-rw-rw-   0        0        0    15676 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/yolov8.py
+-rw-rw-rw-   0        0        0    17632 2023-06-09 16:02:19.000000 onvif-gui-1.2.4/modules/video/yolox.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.649166 onvif-gui-1.2.4/onvif_gui.egg-info/
+-rw-rw-rw-   0        0        0     9056 2023-06-09 16:06:35.000000 onvif-gui-1.2.4/onvif_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8475 2023-06-09 16:06:35.000000 onvif-gui-1.2.4/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:06:35.000000 onvif-gui-1.2.4/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-09 16:06:35.000000 onvif-gui-1.2.4/onvif_gui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-06-09 16:06:35.000000 onvif-gui-1.2.4/onvif_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-06-09 16:06:35.000000 onvif-gui-1.2.4/onvif_gui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1688 2023-06-09 16:05:16.000000 onvif-gui-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 16:06:35.680408 onvif-gui-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-06-09 16:05:10.000000 onvif-gui-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.649166 onvif-gui-1.2.4/tracker/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/tracker/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/tracker/basetrack.py
+-rw-rw-rw-   0        0        0    12632 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/tracker/byte_tracker.py
+-rw-rw-rw-   0        0        0     9816 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/tracker/kalman_filter.py
+-rw-rw-rw-   0        0        0     6304 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/tracker/matching.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.649166 onvif-gui-1.2.4/yolov7/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.664787 onvif-gui-1.2.4/yolov7/models/
+-rw-rw-rw-   0        0        0        6 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/models/__init__.py
+-rw-rw-rw-   0        0        0    86435 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/models/common.py
+-rw-rw-rw-   0        0        0    11177 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/models/experimental.py
+-rw-rw-rw-   0        0        0    40895 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.664787 onvif-gui-1.2.4/yolov7/utils/
+-rw-rw-rw-   0        0        0        6 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/activations.py
+-rw-rw-rw-   0        0        0     5771 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/add_nms.py
+-rw-rw-rw-   0        0        0     7321 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/autoanchor.py
+-rw-rw-rw-   0        0        0    57559 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/datasets.py
+-rw-rw-rw-   0        0        0    37789 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/general.py
+-rw-rw-rw-   0        0        0     4996 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/google_utils.py
+-rw-rw-rw-   0        0        0    76741 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/loss.py
+-rw-rw-rw-   0        0        0     9537 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/metrics.py
+-rw-rw-rw-   0        0        0    21424 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/plots.py
+-rw-rw-rw-   0        0        0    15840 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolov7/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.664787 onvif-gui-1.2.4/yolox/
+-rw-rw-rw-   0        0        0        0 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.680408 onvif-gui-1.2.4/yolox/models/
+-rw-rw-rw-   0        0        0      961 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/__init__.py
+-rw-rw-rw-   0        0        0     5019 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/build.py
+-rw-rw-rw-   0        0        0     6840 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/darknet.py
+-rw-rw-rw-   0        0        0     2372 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/losses.py
+-rw-rw-rw-   0        0        0     6944 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/network_blocks.py
+-rw-rw-rw-   0        0        0     3202 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/yolo_fpn.py
+-rw-rw-rw-   0        0        0    26204 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/yolo_head.py
+-rw-rw-rw-   0        0        0     4288 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/yolo_pafpn.py
+-rw-rw-rw-   0        0        0     2054 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/models/yolox.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:06:35.680408 onvif-gui-1.2.4/yolox/utils/
+-rw-rw-rw-   0        0        0      130 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/utils/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-06-09 15:31:39.000000 onvif-gui-1.2.4/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.2.3/LICENSE` & `onvif-gui-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/PKG-INFO` & `onvif-gui-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.2.3
+Version: 1.2.4
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.2.3/README.md` & `onvif-gui-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.2.4/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/checkpoint/catalog.py` & `onvif-gui-1.2.4/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.2.4/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/config/__init__.py` & `onvif-gui-1.2.4/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/config/compat.py` & `onvif-gui-1.2.4/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/config/config.py` & `onvif-gui-1.2.4/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/config/defaults.py` & `onvif-gui-1.2.4/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/config/instantiate.py` & `onvif-gui-1.2.4/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/config/lazy.py` & `onvif-gui-1.2.4/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.2.4/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.2.4/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/__init__.py` & `onvif-gui-1.2.4/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/benchmark.py` & `onvif-gui-1.2.4/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/build.py` & `onvif-gui-1.2.4/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/catalog.py` & `onvif-gui-1.2.4/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/common.py` & `onvif-gui-1.2.4/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/dataset_mapper.py` & `onvif-gui-1.2.4/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/__init__.py` & `onvif-gui-1.2.4/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/builtin.py` & `onvif-gui-1.2.4/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.2.4/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.2.4/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.2.4/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/coco.py` & `onvif-gui-1.2.4/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.2.4/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/lvis.py` & `onvif-gui-1.2.4/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.2.4/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.2.4/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.2.4/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.2.4/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/detection_utils.py` & `onvif-gui-1.2.4/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.2.4/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.2.4/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.2.4/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.2.4/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/data/transforms/transform.py` & `onvif-gui-1.2.4/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/__init__.py` & `onvif-gui-1.2.4/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/aspp.py` & `onvif-gui-1.2.4/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/batch_norm.py` & `onvif-gui-1.2.4/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/blocks.py` & `onvif-gui-1.2.4/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/deform_conv.py` & `onvif-gui-1.2.4/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/losses.py` & `onvif-gui-1.2.4/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/mask_ops.py` & `onvif-gui-1.2.4/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/nms.py` & `onvif-gui-1.2.4/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/roi_align.py` & `onvif-gui-1.2.4/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.2.4/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.2.4/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/shape_spec.py` & `onvif-gui-1.2.4/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/layers/wrappers.py` & `onvif-gui-1.2.4/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/__init__.py` & `onvif-gui-1.2.4/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.2.4/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/build.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.2.4/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/box_regression.py` & `onvif-gui-1.2.4/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/matcher.py` & `onvif-gui-1.2.4/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/__init__.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.2.4/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.2.4/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/poolers.py` & `onvif-gui-1.2.4/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/postprocessing.py` & `onvif-gui-1.2.4/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.2.4/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.2.4/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.2.4/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.2.4/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.2.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/sampling.py` & `onvif-gui-1.2.4/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.2.4/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/predictor.py` & `onvif-gui-1.2.4/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/__init__.py` & `onvif-gui-1.2.4/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/boxes.py` & `onvif-gui-1.2.4/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/image_list.py` & `onvif-gui-1.2.4/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/instances.py` & `onvif-gui-1.2.4/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/keypoints.py` & `onvif-gui-1.2.4/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/masks.py` & `onvif-gui-1.2.4/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.2.4/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/tracker.py` & `onvif-gui-1.2.4/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/analysis.py` & `onvif-gui-1.2.4/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/collect_env.py` & `onvif-gui-1.2.4/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/colormap.py` & `onvif-gui-1.2.4/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/comm.py` & `onvif-gui-1.2.4/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/develop.py` & `onvif-gui-1.2.4/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/env.py` & `onvif-gui-1.2.4/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/events.py` & `onvif-gui-1.2.4/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/file_io.py` & `onvif-gui-1.2.4/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/logger.py` & `onvif-gui-1.2.4/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/memory.py` & `onvif-gui-1.2.4/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/registry.py` & `onvif-gui-1.2.4/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/serialize.py` & `onvif-gui-1.2.4/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/testing.py` & `onvif-gui-1.2.4/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/video_visualizer.py` & `onvif-gui-1.2.4/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/detectron2/utils/visualizer.py` & `onvif-gui-1.2.4/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/comboselector.py` & `onvif-gui-1.2.4/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/directoryselector.py` & `onvif-gui-1.2.4/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/fileselector.py` & `onvif-gui-1.2.4/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/labelselector.py` & `onvif-gui-1.2.4/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/progress.py` & `onvif-gui-1.2.4/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/thresholdslider.py` & `onvif-gui-1.2.4/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/components/waitdialog.py` & `onvif-gui-1.2.4/gui/components/waitdialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/glwidget.py` & `onvif-gui-1.2.4/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/main.py` & `onvif-gui-1.2.4/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 from loguru import logger
 if sys.platform == "win32":
     filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
 else:
     filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-logger.add(filename, retention="1 days")
+logger.add(filename, retention="10 days")
 
 import time
 from datetime import datetime
 import importlib.util
 from pathlib import Path
 from PyQt6.QtWidgets import QApplication, QMainWindow, QLabel, QSplitter, \
     QTabWidget, QMessageBox
@@ -59,15 +59,15 @@
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
 
-        self.program_name = "onvif gui version 1.2.3"
+        self.program_name = "onvif gui version 1.2.4"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
```

### Comparing `onvif-gui-1.2.3/gui/onvif/admintab.py` & `onvif-gui-1.2.4/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/onvif/imagetab.py` & `onvif-gui-1.2.4/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/onvif/logindialog.py` & `onvif-gui-1.2.4/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/onvif/networktab.py` & `onvif-gui-1.2.4/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/onvif/ptztab.py` & `onvif-gui-1.2.4/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/onvif/videotab.py` & `onvif-gui-1.2.4/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/panels/audiopanel.py` & `onvif-gui-1.2.4/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/panels/camerapanel.py` & `onvif-gui-1.2.4/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/panels/filepanel.py` & `onvif-gui-1.2.4/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/panels/settingspanel.py` & `onvif-gui-1.2.4/gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/panels/videopanel.py` & `onvif-gui-1.2.4/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/LICENSE` & `onvif-gui-1.2.4/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/audio.png` & `onvif-gui-1.2.4/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/audio_hi.png` & `onvif-gui-1.2.4/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/audio_lo.png` & `onvif-gui-1.2.4/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/darkstyle.qss` & `onvif-gui-1.2.4/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/discover.png` & `onvif-gui-1.2.4/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/discover_hi.png` & `onvif-gui-1.2.4/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/discover_lo.png` & `onvif-gui-1.2.4/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/mute.png` & `onvif-gui-1.2.4/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/mute_lo.png` & `onvif-gui-1.2.4/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/onvif-gui.ico` & `onvif-gui-1.2.4/gui/resources/onvif-gui.ico`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/onvif-gui.png` & `onvif-gui-1.2.4/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/recording_lo.png` & `onvif-gui-1.2.4/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/gui/resources/spinner.gif` & `onvif-gui-1.2.4/gui/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/modules/audio/sample.py` & `onvif-gui-1.2.4/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/modules/video/keypoint.py` & `onvif-gui-1.2.4/modules/video/keypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import os
     import sys
     from loguru import logger
     if sys.platform == "win32":
         filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
     else:
         filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-    logger.add(filename, retention="1 days")
+    logger.add(filename, retention="10 days")
 
     import numpy as np
     import cv2
     import math
     from pathlib import Path
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from gui.components import ThresholdSlider
```

### Comparing `onvif-gui-1.2.3/modules/video/retinanet.py` & `onvif-gui-1.2.4/modules/video/retinanet.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import os
     import sys
     from loguru import logger
     if sys.platform == "win32":
         filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
     else:
         filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-    logger.add(filename, retention="1 days")
+    logger.add(filename, retention="10 days")
 
     import cv2
     import numpy as np
     from contextlib import redirect_stderr
     from PyQt6.QtWidgets import QGridLayout, QWidget, QLabel, QMessageBox
     from PyQt6.QtCore import Qt
     from gui.components.thresholdslider import ThresholdSlider
@@ -97,20 +97,15 @@
             if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
                 return
             
             self.mw.signals.showWait.emit()
 
             self.model = None
             weights=torchvision.models.detection.RetinaNet_ResNet50_FPN_Weights.DEFAULT
-            if os.path.split(sys.executable)[1] == "pythonw.exe":
-                with open('onvif-gui-errors.txt', 'w') as f:
-                    with redirect_stderr(f):
-                        self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=weights, progress=False)
-            else:
-                self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=weights, progress=True)
+            self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=weights, progress=True)
 
             self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
             self.model.eval().to(self.device)
             with torch.no_grad():
                 self.model(torch.zeros(1, 3, 1280, 720).to(self.device))
 
             self.mw.signals.hideWait.emit()
```

### Comparing `onvif-gui-1.2.3/modules/video/sample.py` & `onvif-gui-1.2.4/modules/video/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
+import os
+import sys
 import numpy as np
 import cv2
-from loguru import logger
 from PyQt6.QtWidgets import QGridLayout, QWidget, QCheckBox
+from loguru import logger
+if sys.platform == "win32":
+    filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+else:
+    filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+logger.add(filename, retention="10 days")
 
 MODULE_NAME = "sample"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
-            logger.add("onvif-gui-errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.showBorderKey = "Module/" + MODULE_NAME + "/showBorder"
             self.chkShowBorder = QCheckBox("Show Border")
             self.chkShowBorder.setChecked(int(self.mw.settings.value(self.showBorderKey, 0)))
             self.chkShowBorder.stateChanged.connect(self.chkShowBorderClicked)
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkShowBorder, 0, 0, 1, 1)
```

### Comparing `onvif-gui-1.2.3/modules/video/segment.py` & `onvif-gui-1.2.4/modules/video/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import os
     import sys
     from loguru import logger
     if sys.platform == "win32":
         filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
     else:
         filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-    logger.add(filename, retention="1 days")
+    logger.add(filename, retention="10 days")
 
     import cv2
     import numpy as np
     from pathlib import Path
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from PyQt6.QtCore import Qt
     from gui.components import ThresholdSlider, LabelSelector
```

### Comparing `onvif-gui-1.2.3/modules/video/yolov7.py` & `onvif-gui-1.2.4/modules/video/yolov7.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import os
     import sys
     from loguru import logger
     if sys.platform == "win32":
         filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
     else:
         filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-    logger.add(filename, retention="1 days")
+    logger.add(filename, retention="10 days")
 
     import gc
     import cv2
     import numpy as np
     from datetime import datetime
     from pathlib import Path
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
```

### Comparing `onvif-gui-1.2.3/modules/video/yolov8.py` & `onvif-gui-1.2.4/modules/video/yolov8.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import os
     import sys
     from loguru import logger
     if sys.platform == "win32":
         filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
     else:
         filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-    logger.add(filename, retention="1 days")
+    logger.add(filename, retention="10 days")
 
     import cv2
     import numpy as np
     from datetime import datetime
     from pathlib import Path
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox, QLineEdit
```

### Comparing `onvif-gui-1.2.3/modules/video/yolox.py` & `onvif-gui-1.2.4/modules/video/yolox.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import os
     import sys
     from loguru import logger
     if sys.platform == "win32":
         filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
     else:
         filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
-    logger.add(filename, retention="1 days")
+    logger.add(filename, retention="10 days")
 
     import cv2
     import numpy as np
     from pathlib import Path
     from datetime import datetime
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox, QLineEdit
```

### Comparing `onvif-gui-1.2.3/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.2.4/onvif_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.2.3
+Version: 1.2.4
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.2.3/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.2.4/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/pyproject.toml` & `onvif-gui-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.2.3"  
+version = "1.2.4"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.2.3/setup.py` & `onvif-gui-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.2.3",
+    version="1.2.4",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.2.3/tracker/basetrack.py` & `onvif-gui-1.2.4/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/tracker/byte_tracker.py` & `onvif-gui-1.2.4/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/tracker/kalman_filter.py` & `onvif-gui-1.2.4/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/tracker/matching.py` & `onvif-gui-1.2.4/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/models/common.py` & `onvif-gui-1.2.4/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/models/experimental.py` & `onvif-gui-1.2.4/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/models/yolo.py` & `onvif-gui-1.2.4/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/activations.py` & `onvif-gui-1.2.4/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/add_nms.py` & `onvif-gui-1.2.4/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/autoanchor.py` & `onvif-gui-1.2.4/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/datasets.py` & `onvif-gui-1.2.4/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/general.py` & `onvif-gui-1.2.4/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/google_utils.py` & `onvif-gui-1.2.4/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/loss.py` & `onvif-gui-1.2.4/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/metrics.py` & `onvif-gui-1.2.4/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/plots.py` & `onvif-gui-1.2.4/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolov7/utils/torch_utils.py` & `onvif-gui-1.2.4/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/__init__.py` & `onvif-gui-1.2.4/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/build.py` & `onvif-gui-1.2.4/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/darknet.py` & `onvif-gui-1.2.4/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/losses.py` & `onvif-gui-1.2.4/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/network_blocks.py` & `onvif-gui-1.2.4/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/yolo_fpn.py` & `onvif-gui-1.2.4/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/yolo_head.py` & `onvif-gui-1.2.4/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/yolo_pafpn.py` & `onvif-gui-1.2.4/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/models/yolox.py` & `onvif-gui-1.2.4/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.3/yolox/utils/utils.py` & `onvif-gui-1.2.4/yolox/utils/utils.py`

 * *Files identical despite different names*

