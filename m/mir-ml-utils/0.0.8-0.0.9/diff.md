# Comparing `tmp/mir_ml_utils-0.0.8.tar.gz` & `tmp/mir_ml_utils-0.0.9.tar.gz`

## Comparing `mir_ml_utils-0.0.8.tar` & `mir_ml_utils-0.0.9.tar`

### file list

```diff
@@ -1,196 +1,196 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/requirements.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/.gitignore
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/src.iml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/vcs.xml
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/workspace.xml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/config.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/data_handlers/__init__.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/data_handlers/dataset_with_masks.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/data_handlers/images_dataset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/__init__.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/utils.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/cub.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/default_configs.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/easy_set.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/bd_cspn.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/finetune.py
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/matching_networks.py
--rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/relation_networks.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/tim.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/modules/__init__.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/modules/resnet.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/samplers/__init__.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/samplers/task_sampler.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/factories/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/factories/loss_function_factory.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/factories/model_adaptor_factory.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/factories/model_builder_factory.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/factories/optimzer_factory.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/loss_functions/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/loss_functions/loss_function_result.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/loss_functions/loss_function_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/examples/python/README.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/__init__.py
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py
--rw-r--r--   0        0        0   316358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png
--rw-r--r--   0        0        0    40344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg
--rw-r--r--   0        0        0   771052 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4
--rw-r--r--   0        0        0    97422 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg
--rw-r--r--   0        0        0    90796 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg
--rw-r--r--   0        0        0    35364 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json
--rw-r--r--   0        0        0    70126 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg
--rw-r--r--   0        0        0   858575 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png
--rw-r--r--   0        0        0   632918 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png
--rw-r--r--   0        0        0   300404 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/__init__.py
--rw-r--r--   0        0        0    16652 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/__init__.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/presets.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/sampler.py
--rw-r--r--   0        0        0    22550 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/train.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py
--rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/transforms.py
--rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/__init__.py
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/__init__.py
--rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py
--rw-r--r--   0        0        0    33426 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py
--rw-r--r--   0        0        0    25981 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py
--rw-r--r--   0        0        0   273008 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg
--rw-r--r--   0        0        0  1343300 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg
--rw-r--r--   0        0        0  1781352 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg
--rw-r--r--   0        0        0   321833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/__init__.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py
--rw-r--r--   0        0        0    17472 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/norm.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/__init__.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/engine.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/presets.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/train.py
--rw-r--r--   0        0        0    23337 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/transforms.py
--rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/utils.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/__init__.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py
--rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/train.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/presets.py
--rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/train.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/utils.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/__init__.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/loss.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/model.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/sampler.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/test.py
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/train.py
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/datasets.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/presets.py
--rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/train.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/transforms.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/utils.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/__init__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/collect_model_urls.py
--rwxr-xr-x   0        0        0     1147 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/release_notes/__init__.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/__init__.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/linear_regressor_model_tester.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/model_adaptor.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/model_adaptor_type_enum.py
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/model_loaders.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/models_enum.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/pytorch_util_modules/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/pytorch_util_modules/flatten_module.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/pytorch_util_modules/utils.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/testers/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/testers/inference_enum_types.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/testers/test_wrapper.py
--rw-r--r--   0        0        0    23901 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/model_trainer_type_enum.py
--rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/pytorch_trainer.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/trainer_info.py
--rw-r--r--   0        0        0    13573 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/trainer_wrapper.py
--rw-r--r--   0        0        0    38550 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/__init__.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/apps_utils.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/array_utils.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/exceptions.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/file_utils.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/function_wrappers.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/math_ops.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/src/mir_ml_utils/utils/mode_enum.py
--rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/corrosion_4.png
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/highres_raw_train_two_classes.csv
--rw-r--r--   0        0        0   195177 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/hull001_label.jpg
--rw-r--r--   0        0        0   462993 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/best_model.pth
--rw-r--r--   0        0        0   166635 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/train_prototypes.pth
--rw-r--r--   0        0        0   151371 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_1.png
--rw-r--r--   0        0        0   162210 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_2.png
--rw-r--r--   0        0        0   140763 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_3.png
--rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_4.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_images_dataset.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_img_pipeline.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_img_utils.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_math_ops.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_prototypical_loss.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_pytorch_trainer.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/tests/test_suite.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/trainer_wrapper_config_template/config.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/README.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/.gitignore
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/modules.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/src.iml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/vcs.xml
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/workspace.xml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/config.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/data_handlers/__init__.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/data_handlers/dataset_with_masks.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/data_handlers/images_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/__init__.py
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/utils.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/cub.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/default_configs.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/easy_set.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/__init__.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/bd_cspn.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/finetune.py
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/matching_networks.py
+-rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/relation_networks.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/tim.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/modules/__init__.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/modules/resnet.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/samplers/__init__.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/samplers/task_sampler.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/factories/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/factories/loss_function_factory.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/factories/model_adaptor_factory.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/factories/model_builder_factory.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/factories/optimzer_factory.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/loss_functions/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/loss_functions/loss_function_result.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/loss_functions/loss_function_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/examples/python/README.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/__init__.py
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py
+-rw-r--r--   0        0        0   316358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png
+-rw-r--r--   0        0        0    40344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg
+-rw-r--r--   0        0        0   771052 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4
+-rw-r--r--   0        0        0    97422 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg
+-rw-r--r--   0        0        0    90796 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg
+-rw-r--r--   0        0        0    35364 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json
+-rw-r--r--   0        0        0    70126 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg
+-rw-r--r--   0        0        0   858575 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png
+-rw-r--r--   0        0        0   632918 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png
+-rw-r--r--   0        0        0   300404 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/__init__.py
+-rw-r--r--   0        0        0    16652 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/__init__.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/presets.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/sampler.py
+-rw-r--r--   0        0        0    22550 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/train.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py
+-rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/transforms.py
+-rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/__init__.py
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/__init__.py
+-rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py
+-rw-r--r--   0        0        0    33426 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py
+-rw-r--r--   0        0        0    25981 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py
+-rw-r--r--   0        0        0   273008 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg
+-rw-r--r--   0        0        0  1343300 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg
+-rw-r--r--   0        0        0  1781352 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg
+-rw-r--r--   0        0        0   321833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/__init__.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py
+-rw-r--r--   0        0        0    17472 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/norm.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/__init__.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/engine.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/presets.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/train.py
+-rw-r--r--   0        0        0    23337 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/transforms.py
+-rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/utils.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/__init__.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py
+-rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/train.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/presets.py
+-rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/train.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/utils.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/__init__.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/loss.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/model.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/sampler.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/test.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/train.py
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/datasets.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/presets.py
+-rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/train.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/transforms.py
+-rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/utils.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/collect_model_urls.py
+-rwxr-xr-x   0        0        0     1147 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/release_notes/__init__.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/__init__.py
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/linear_regressor_model_tester.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/model_adaptor.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/model_adaptor_type_enum.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/model_loaders.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/models_enum.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/pytorch_util_modules/__init__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/pytorch_util_modules/flatten_module.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/pytorch_util_modules/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/testers/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/testers/inference_enum_types.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/testers/test_wrapper.py
+-rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/__init__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/model_trainer_type_enum.py
+-rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/pytorch_trainer.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/trainer_info.py
+-rw-r--r--   0        0        0    13573 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/trainer_wrapper.py
+-rw-r--r--   0        0        0    38550 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/__init__.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/apps_utils.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/array_utils.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/exceptions.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/file_utils.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/function_wrappers.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/math_ops.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/src/mir_ml_utils/utils/mode_enum.py
+-rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/corrosion_4.png
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/highres_raw_train_two_classes.csv
+-rw-r--r--   0        0        0   195177 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/hull001_label.jpg
+-rw-r--r--   0        0        0   462993 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/best_model.pth
+-rw-r--r--   0        0        0   166635 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/train_prototypes.pth
+-rw-r--r--   0        0        0   151371 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_1.png
+-rw-r--r--   0        0        0   162210 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_2.png
+-rw-r--r--   0        0        0   140763 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_3.png
+-rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_4.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_images_dataset.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_img_pipeline.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_img_utils.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_math_ops.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_prototypical_loss.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_pytorch_trainer.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/tests/test_suite.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/trainer_wrapper_config_template/config.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.9/PKG-INFO
```

### Comparing `mir_ml_utils-0.0.8/src/.idea/workspace.xml` & `mir_ml_utils-0.0.9/src/.idea/workspace.xml`

 * *Files 7% similar despite different names*

#### Comparing `mir_ml_utils-0.0.8/src/.idea/workspace.xml` & `mir_ml_utils-0.0.9/src/.idea/workspace.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="855a915d-2248-4c7a-ae77-d8a1e1cb69cb" name="Changes" comment="">
       <change beforePath="$PROJECT_DIR$/../pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/../pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/../requirements.txt" beforeDir="false" afterPath="$PROJECT_DIR$/../requirements.txt" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/mir_ml_utils/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/mir_ml_utils/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/mir_ml_utils/trainers/trainer_wrapper_pimpl.py" beforeDir="false" afterPath="$PROJECT_DIR$/mir_ml_utils/trainers/trainer_wrapper_pimpl.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -19,21 +19,21 @@
   </component>
   <component name="ProjectId" id="2PvNMtHwYS70xhaoYFmNmSi11iu"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;last_opened_file_path&quot;: &quot;/home/alex/qi3/mir_ml_utils/pyproject.toml&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.OpenProjectViewOnStart": "true",
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "last_opened_file_path": "/home/alex/qi3/mir_ml_utils/pyproject.toml"
   }
-}</component>
+}]]></component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="855a915d-2248-4c7a-ae77-d8a1e1cb69cb" name="Changes" comment=""/>
       <created>1684333550243</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
@@ -56,11 +56,16 @@
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/mir_ml_utils/easyfsl/methods/relation_networks.py</url>
           <line>5</line>
           <option name="timeStamp" value="1"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/mir_ml_utils/trainers/trainer_wrapper.py</url>
+          <line>4</line>
+          <option name="timeStamp" value="2"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
 </project>
```

### Comparing `mir_ml_utils-0.0.8/src/.idea/inspectionProfiles/Project_Default.xml` & `mir_ml_utils-0.0.9/src/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/data_handlers/dataset_with_masks.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/data_handlers/dataset_with_masks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/data_handlers/images_dataset.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/data_handlers/images_dataset.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/cub.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/cub.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/default_configs.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/default_configs.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/easy_set.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/easy_set.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/bd_cspn.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/bd_cspn.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/finetune.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/finetune.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/matching_networks.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/matching_networks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/relation_networks.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/relation_networks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/tim.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/tim.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/methods/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/methods/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/modules/resnet.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/easyfsl/samplers/task_sampler.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/easyfsl/samplers/task_sampler.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/factories/model_adaptor_factory.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/factories/model_adaptor_factory.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/factories/model_builder_factory.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/factories/model_builder_factory.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/factories/optimzer_factory.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/factories/optimzer_factory.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/presets.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/sampler.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/sampler.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/classification/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/engine.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/engine.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/presets.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/detection/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/detection/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/presets.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/segmentation/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/loss.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/loss.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/sampler.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/sampler.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/test.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/test.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/similarity/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/similarity/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/README.md` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/presets.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/train.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/references/video_classification/utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/references/video_classification/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/README.rst` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/linear_regressor_model_tester.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/linear_regressor_model_tester.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/model_adaptor.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/model_adaptor.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/model_adaptor_type_enum.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/model_adaptor_type_enum.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/model_loaders.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/model_loaders.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/models_enum.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/models_enum.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/testers/test_wrapper.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/testers/test_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 
 from mir_ml_utils.factories.model_adaptor_factory import model_adaptor_builder
 from mir_ml_utils.factories.model_builder_factory import model_loader
 from mir_ml_utils.trainers.model_trainer_type_enum import ModelTrainerTypeEnum
 from mir_ml_utils.models.model_adaptor_type_enum import ModelAdaptorTypeEnum
 from mir_ml_utils.models.easyfsl_proto_net_classifier import EasyFSLProtoNetClassifier
-from .inference_enum_types import InferenceTypeEnum
+from mir_ml_utils.testers.inference_enum_types import InferenceTypeEnum
 
 
 def _init_class_dict(classes: List[str]):
     class_dict = {}
     for class_name in classes:
         class_dict[class_name] = 0
     return class_dict
```

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from loguru import logger
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader, Dataset
 from torchvision import transforms
 import cv2
 
-import src.data_handlers.img_utils as img_utils
-from src.models.easyfsl_proto_net_classifier import EasyFSLProtoNetClassifier
+import navalmartin_mir_vision_utils.image_utils as img_utils
+from mir_ml_utils.models.easyfsl_proto_net_classifier import EasyFSLProtoNetClassifier
 
 
 class TwoClassPyTorchModelTester(object):
 
     def __init__(self, options: dict):
         self.options: dict = options
 
@@ -50,18 +50,18 @@
             raise ValueError("Invalid dataloader type. Dataloader has to be in "
                              "[torch.utils.data.DataLoader, torch.utils.data.Dataset]")
 
     @staticmethod
     def build_simple_segmentation(model: nn.Module, options: dict):
 
         # get the images
-        test_class_0_images = img_utils.get_img_files(img_dir=options['test_class_0_images_path'],
+        test_class_0_images = img_utils.get_img_files(base_path=options['test_class_0_images_path'],
                                                       img_formats=['jpg', 'png', 'jpeg'])
 
-        test_class_1_images = img_utils.get_img_files(img_dir=options['test_class_1_images_path'],
+        test_class_1_images = img_utils.get_img_files(base_path=options['test_class_1_images_path'],
                                                       img_formats=['jpg', 'png', 'jpeg'])
 
         images = test_class_1_images + test_class_0_images
 
         data_out_dir = options['simple_segmentation_out']
 
         counter = 0
```

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/pytorch_trainer.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/pytorch_trainer.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/trainer_info.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/trainer_info.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/trainer_wrapper.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/trainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/utils/apps_utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/utils/apps_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/utils/array_utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/utils/exceptions.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/utils/file_utils.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/utils/function_wrappers.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/utils/function_wrappers.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/src/mir_ml_utils/utils/math_ops.py` & `mir_ml_utils-0.0.9/src/mir_ml_utils/utils/math_ops.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/corrosion_4.png` & `mir_ml_utils-0.0.9/testing_data/corrosion_4.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/hull001_label.jpg` & `mir_ml_utils-0.0.9/testing_data/hull001_label.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/best_model.pth` & `mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/best_model.pth`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/train_prototypes.pth` & `mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/train_prototypes.pth`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_1.png` & `mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_1.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_2.png` & `mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_2.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_3.png` & `mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_3.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/testing_data/prototypical_net_test_data/inference/corrosion_4.png` & `mir_ml_utils-0.0.9/testing_data/prototypical_net_test_data/inference/corrosion_4.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/tests/test_images_dataset.py` & `mir_ml_utils-0.0.9/tests/test_images_dataset.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/tests/test_img_pipeline.py` & `mir_ml_utils-0.0.9/tests/test_img_pipeline.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/tests/test_img_utils.py` & `mir_ml_utils-0.0.9/tests/test_img_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/tests/test_prototypical_loss.py` & `mir_ml_utils-0.0.9/tests/test_prototypical_loss.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/tests/test_pytorch_trainer.py` & `mir_ml_utils-0.0.9/tests/test_pytorch_trainer.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/tests/test_suite.py` & `mir_ml_utils-0.0.9/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/trainer_wrapper_config_template/config.json` & `mir_ml_utils-0.0.9/trainer_wrapper_config_template/config.json`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/.gitignore` & `mir_ml_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/LICENSE` & `mir_ml_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/README.md` & `mir_ml_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.8/pyproject.toml` & `mir_ml_utils-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling", "torch", "torchvision", "numpy",
 	    "dataclasses", "Pillow", "matplotlib", "loguru", "opencv-python",
             "torchcam", "torch-summary",  "tqdm", "pycocotools", "navalmartin-mir-vision-utils"]
 build-backend = "hatchling.build"
 [project]
 name = "mir_ml_utils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Alexandros Giavaras", email="a.giavaras@gmail.com" },
 ]
 description = "Various utilities for machine learning training in Python 3. for the mir project"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mir_ml_utils-0.0.8/PKG-INFO` & `mir_ml_utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mir_ml_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Various utilities for machine learning training in Python 3. for the mir project
 Project-URL: Homepage, https://github.com/Navalmartin/mir_ml_utils
 Project-URL: Bug Tracker, https://github.com/Navalmartin/mir_ml_utils/issues
 Author-email: Alexandros Giavaras <a.giavaras@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mir_ml_utils Version: 0.0.8 Summary: Various
+Metadata-Version: 2.1 Name: mir_ml_utils Version: 0.0.9 Summary: Various
 utilities for machine learning training in Python 3. for the mir project
 Project-URL: Homepage, https://github.com/Navalmartin/mir_ml_utils Project-URL:
 Bug Tracker, https://github.com/Navalmartin/mir_ml_utils/issues Author-email:
 Alexandros Giavaras
 giavaras@gmail.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
```

