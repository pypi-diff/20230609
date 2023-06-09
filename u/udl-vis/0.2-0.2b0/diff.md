# Comparing `tmp/udl_vis-0.2.tar.gz` & `tmp/udl_vis-0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\udl_vis-0.2.tar", last modified: Wed Jun  7 10:07:30 2023, max compression
+gzip compressed data, was "dist\udl_vis-0.2b0.tar", last modified: Fri Jun  9 11:12:34 2023, max compression
```

## Comparing `udl_vis-0.2.tar` & `udl_vis-0.2b0.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/
--rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 udl_vis-0.2/LICENSE
--rw-rw-rw-   0        0        0     5771 2023-06-07 10:07:30.000000 udl_vis-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5271 2023-06-07 04:18:04.000000 udl_vis-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 10:07:30.000000 udl_vis-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1168 2023-06-07 10:05:08.000000 udl_vis-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/AutoDL/
--rw-rw-rw-   0        0        0      121 2023-03-27 06:21:37.000000 udl_vis-0.2/udl_vis/AutoDL/__init__.py
--rw-rw-rw-   0        0        0    13693 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/AutoDL/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/Basis/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:56:36.000000 udl_vis-0.2/udl_vis/Basis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/
--rw-rw-rw-   0        0        0      134 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/__init__.py
--rw-rw-rw-   0        0        0     1084 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/base.py
--rw-rw-rw-   0        0        0     7303 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/fp16_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/
--rw-rw-rw-   0        0        0      787 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/__init__.py
--rw-rw-rw-   0        0        0     1142 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/__main__.py
--rw-rw-rw-   0        0        0     9296 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/compute_flops.py
--rw-rw-rw-   0        0        0     6085 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/compute_madd.py
--rw-rw-rw-   0        0        0     4016 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/compute_memory.py
--rw-rw-rw-   0        0        0    10202 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/model_hook.py
--rw-rw-rw-   0        0        0     3758 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/reporter.py
--rw-rw-rw-   0        0        0     5899 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/stat_tree.py
--rw-rw-rw-   0        0        0     3364 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/statistics.py
--rw-rw-rw-   0        0        0    11956 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/Basis/auxiliary/utils.py
--rw-rw-rw-   0        0        0     2851 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/cal_ssim.py
--rw-rw-rw-   0        0        0    29004 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/Basis/config.py
--rw-rw-rw-   0        0        0     4087 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/Basis/criterion_metrics.py
--rw-rw-rw-   0        0        0     6622 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/dist_utils.py
--rw-rw-rw-   0        0        0    14882 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/launch.py
--rw-rw-rw-   0        0        0     8754 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/Basis/logger.py
--rw-rw-rw-   0        0        0     3145 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/Basis/metrics.py
--rw-rw-rw-   0        0        0    16848 2022-09-16 14:28:57.000000 udl_vis-0.2/udl_vis/Basis/module.py
--rw-rw-rw-   0        0        0     9926 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/Basis/optim.py
--rw-rw-rw-   0        0        0     6197 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/Basis/option.py
--rw-rw-rw-   0        0        0    17306 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/Basis/postprocess.py
--rw-rw-rw-   0        0        0     5203 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/Basis/python_sub_class.py
--rw-rw-rw-   0        0        0     3145 2023-06-07 03:16:59.000000 udl_vis-0.2/udl_vis/Basis/variance_sacling_initializer.py
--rw-rw-rw-   0        0        0      169 2023-06-06 17:42:12.000000 udl_vis-0.2/udl_vis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/
--rw-rw-rw-   0        0        0      367 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/arraymisc/
--rw-rw-rw-   0        0        0      137 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/arraymisc/__init__.py
--rw-rw-rw-   0        0        0     1879 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/arraymisc/quantization.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/cnn/
--rw-rw-rw-   0        0        0     2479 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/__init__.py
--rw-rw-rw-   0        0        0     2051 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/alexnet.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/
--rw-rw-rw-   0        0        0     1767 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/__init__.py
--rw-rw-rw-   0        0        0     2582 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/activation.py
--rw-rw-rw-   0        0        0     4806 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/context_block.py
--rw-rw-rw-   0        0        0     1490 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv.py
--rw-rw-rw-   0        0        0     2576 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-rw-rw-   0        0        0     8946 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv_module.py
--rw-rw-rw-   0        0        0     5565 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv_ws.py
--rw-rw-rw-   0        0        0     4238 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-rw-rw-   0        0        0     2217 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/drop.py
--rw-rw-rw-   0        0        0    16408 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/generalized_attention.py
--rw-rw-rw-   0        0        0     1592 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/hsigmoid.py
--rw-rw-rw-   0        0        0      680 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/hswish.py
--rw-rw-rw-   0        0        0    11318 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/non_local.py
--rw-rw-rw-   0        0        0     5255 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/norm.py
--rw-rw-rw-   0        0        0     1163 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/padding.py
--rw-rw-rw-   0        0        0     2593 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/plugin.py
--rw-rw-rw-   0        0        0      654 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/registry.py
--rw-rw-rw-   0        0        0      598 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/scale.py
--rw-rw-rw-   0        0        0      510 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/swish.py
--rw-rw-rw-   0        0        0    38090 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/transformer.py
--rw-rw-rw-   0        0        0     2962 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/upsample.py
--rw-rw-rw-   0        0        0     7141 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/bricks/wrappers.py
--rw-rw-rw-   0        0        0     1119 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/builder.py
--rw-rw-rw-   0        0        0    10271 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/resnet.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/cnn/utils/
--rw-rw-rw-   0        0        0     1042 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/utils/__init__.py
--rw-rw-rw-   0        0        0    22678 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/utils/flops_counter.py
--rw-rw-rw-   0        0        0     1940 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/utils/fuse_conv_bn.py
--rw-rw-rw-   0        0        0     2358 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/utils/sync_bn.py
--rw-rw-rw-   0        0        0    26645 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/utils/weight_init.py
--rw-rw-rw-   0        0        0     6228 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/cnn/vgg.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/engine/
--rw-rw-rw-   0        0        0      274 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/engine/__init__.py
--rw-rw-rw-   0        0        0     7350 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/engine/test.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/fileio/
--rw-rw-rw-   0        0        0      489 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/__init__.py
--rw-rw-rw-   0        0        0    43043 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/fileio/file_client.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/fileio/handlers/
--rw-rw-rw-   0        0        0      285 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/handlers/__init__.py
--rw-rw-rw-   0        0        0     1023 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/handlers/base.py
--rw-rw-rw-   0        0        0     1104 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/handlers/json_handler.py
--rw-rw-rw-   0        0        0      845 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/handlers/pickle_handler.py
--rw-rw-rw-   0        0        0      689 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/handlers/yaml_handler.py
--rw-rw-rw-   0        0        0     5671 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/io.py
--rw-rw-rw-   0        0        0     3555 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/fileio/parse.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/image/
--rw-rw-rw-   0        0        0     1753 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/image/__init__.py
--rw-rw-rw-   0        0        0    10197 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/image/colorspace.py
--rw-rw-rw-   0        0        0    25898 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/image/geometric.py
--rw-rw-rw-   0        0        0    11973 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/image/io.py
--rw-rw-rw-   0        0        0     2000 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/image/misc.py
--rw-rw-rw-   0        0        0    15427 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/image/photometric.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/onnx/
--rw-rw-rw-   0        0        0      201 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/onnx/__init__.py
--rw-rw-rw-   0        0        0      611 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/onnx/info.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/onnx/onnx_utils/
--rw-rw-rw-   0        0        0       49 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/onnx/onnx_utils/__init__.py
--rw-rw-rw-   0        0        0    11503 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/onnx/onnx_utils/symbolic_helper.py
--rw-rw-rw-   0        0        0    19620 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/onnx/symbolic.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/ops/
--rw-rw-rw-   0        0        0     5108 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/__init__.py
--rw-rw-rw-   0        0        0     2162 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/active_rotated_filter.py
--rw-rw-rw-   0        0        0     4678 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/assign_score_withk.py
--rw-rw-rw-   0        0        0     1775 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/ball_query.py
--rw-rw-rw-   0        0        0     2665 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/bbox.py
--rw-rw-rw-   0        0        0     3812 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/border_align.py
--rw-rw-rw-   0        0        0     5319 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/box_iou_rotated.py
--rw-rw-rw-   0        0        0    10187 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/carafe.py
--rw-rw-rw-   0        0        0     3130 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/cc_attention.py
--rw-rw-rw-   0        0        0     1843 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/contour_expand.py
--rw-rw-rw-   0        0        0     1719 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/convex_iou.py
--rw-rw-rw-   0        0        0     4920 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/corner_pool.py
--rw-rw-rw-   0        0        0     6893 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/correlation.py
--rw-rw-rw-   0        0        0    15999 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/deform_conv.py
--rw-rw-rw-   0        0        0     7614 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/deform_roi_pool.py
--rw-rw-rw-   0        0        0     1629 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/deprecated_wrappers.py
--rw-rw-rw-   0        0        0     6794 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/focal_loss.py
--rw-rw-rw-   0        0        0     2672 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/furthest_point_sample.py
--rw-rw-rw-   0        0        0    10385 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/fused_bias_leakyrelu.py
--rw-rw-rw-   0        0        0     1682 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/gather_points.py
--rw-rw-rw-   0        0        0     8617 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/group_points.py
--rw-rw-rw-   0        0        0      923 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/info.py
--rw-rw-rw-   0        0        0     3227 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/iou3d.py
--rw-rw-rw-   0        0        0     2692 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/knn.py
--rw-rw-rw-   0        0        0     3870 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/masked_conv.py
--rw-rw-rw-   0        0        0     5552 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/merge_cells.py
--rw-rw-rw-   0        0        0      573 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/min_area_polygons.py
--rw-rw-rw-   0        0        0    10872 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/modulated_deform_conv.py
--rw-rw-rw-   0        0        0    15562 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/multi_scale_deform_attn.py
--rw-rw-rw-   0        0        0    17688 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/nms.py
--rw-rw-rw-   0        0        0     3214 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/pixel_group.py
--rw-rw-rw-   0        0        0    12787 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/point_sample.py
--rw-rw-rw-   0        0        0     5503 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/points_in_boxes.py
--rw-rw-rw-   0        0        0     1506 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/points_in_polygons.py
--rw-rw-rw-   0        0        0     6272 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/points_sampler.py
--rw-rw-rw-   0        0        0     2865 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/psa_mask.py
--rw-rw-rw-   0        0        0     4852 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/riroi_align_rotated.py
--rw-rw-rw-   0        0        0     8742 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/roi_align.py
--rw-rw-rw-   0        0        0     6611 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/roi_align_rotated.py
--rw-rw-rw-   0        0        0     2603 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/roi_pool.py
--rw-rw-rw-   0        0        0     4358 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/roiaware_pool3d.py
--rw-rw-rw-   0        0        0     3085 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/roipoint_pool3d.py
--rw-rw-rw-   0        0        0     2994 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/rotated_feature_align.py
--rw-rw-rw-   0        0        0     5970 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/saconv.py
--rw-rw-rw-   0        0        0     5563 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/scatter_points.py
--rw-rw-rw-   0        0        0    11526 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/sync_bn.py
--rw-rw-rw-   0        0        0     2315 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/three_interpolate.py
--rw-rw-rw-   0        0        0     1590 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/three_nn.py
--rw-rw-rw-   0        0        0     2279 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/tin_shift.py
--rw-rw-rw-   0        0        0    12132 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/upfirdn2d.py
--rw-rw-rw-   0        0        0     5875 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/ops/voxelize.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/parallel/
--rw-rw-rw-   0        0        0      518 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/__init__.py
--rw-rw-rw-   0        0        0     2775 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/_functions.py
--rw-rw-rw-   0        0        0     3749 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/collate.py
--rw-rw-rw-   0        0        0     2454 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/data_container.py
--rw-rw-rw-   0        0        0     4588 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/data_parallel.py
--rw-rw-rw-   0        0        0     4945 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/parallel/distributed.py
--rw-rw-rw-   0        0        0     2887 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/distributed_deprecated.py
--rw-rw-rw-   0        0        0      328 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/parallel/registry.py
--rw-rw-rw-   0        0        0     2366 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/scatter_gather.py
--rw-rw-rw-   0        0        0      728 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/parallel/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/runner/
--rw-rw-rw-   0        0        0     4385 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/__init__.py
--rw-rw-rw-   0        0        0    14570 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/base_module.py
--rw-rw-rw-   0        0        0    22884 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/base_runner.py
--rw-rw-rw-   0        0        0      690 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/builder.py
--rw-rw-rw-   0        0        0    33627 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/checkpoint.py
--rw-rw-rw-   0        0        0     1952 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/default_constructor.py
--rw-rw-rw-   0        0        0     5559 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/dist_utils.py
--rw-rw-rw-   0        0        0    13655 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/epoch_based_runner.py
--rw-rw-rw-   0        0        0    16873 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/fp16_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/
--rw-rw-rw-   0        0        0     2402 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/__init__.py
--rw-rw-rw-   0        0        0    18943 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/checkpoint.py
--rw-rw-rw-   0        0        0      280 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/closure.py
--rw-rw-rw-   0        0        0     3674 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/ema.py
--rw-rw-rw-   0        0        0    22909 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/evaluation.py
--rw-rw-rw-   0        0        0     2841 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/hook.py
--rw-rw-rw-   0        0        0      521 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/iter_timer.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/
--rw-rw-rw-   0        0        0      537 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/__init__.py
--rw-rw-rw-   0        0        0     6151 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/base.py
--rw-rw-rw-   0        0        0     2294 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/dvclive.py
--rw-rw-rw-   0        0        0     2995 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/mlflow.py
--rw-rw-rw-   0        0        0     3338 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/neptune.py
--rw-rw-rw-   0        0        0     5269 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/pavi.py
--rw-rw-rw-   0        0        0     2739 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/tensorboard.py
--rw-rw-rw-   0        0        0    11234 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/text.py
--rw-rw-rw-   0        0        0     4009 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/wandb.py
--rw-rw-rw-   0        0        0    27815 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/lr_updater.py
--rw-rw-rw-   0        0        0      682 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/memory.py
--rw-rw-rw-   0        0        0    23465 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/momentum_updater.py
--rw-rw-rw-   0        0        0     1602 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/nni_hook.py
--rw-rw-rw-   0        0        0    25296 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/optimizer.py
--rw-rw-rw-   0        0        0     8221 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/profiler.py
--rw-rw-rw-   0        0        0      867 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/sampler_seed.py
--rw-rw-rw-   0        0        0      729 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/hooks/sync_buffer.py
--rw-rw-rw-   0        0        0    11438 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/iter_based_runner.py
--rw-rw-rw-   0        0        0     1880 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/log_buffer.py
--rw-rw-rw-   0        0        0     1241 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/misc.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/runner/optimizer/
--rw-rw-rw-   0        0        0      379 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/optimizer/__init__.py
--rw-rw-rw-   0        0        0     1390 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/optimizer/builder.py
--rw-rw-rw-   0        0        0    11971 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/optimizer/default_constructor.py
--rw-rw-rw-   0        0        0     1658 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/runner/priority.py
--rw-rw-rw-   0        0        0    11163 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/record.py
--rw-rw-rw-   0        0        0     3014 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/runner/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/tensorrt/
--rw-rw-rw-   0        0        0      788 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/tensorrt/__init__.py
--rw-rw-rw-   0        0        0      916 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/tensorrt/init_plugins.py
--rw-rw-rw-   0        0        0     4459 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/tensorrt/preprocess.py
--rw-rw-rw-   0        0        0     8417 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/tensorrt/tensorrt_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/utils/
--rw-rw-rw-   0        0        0     4027 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/__init__.py
--rw-rw-rw-   0        0        0    27039 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/config.py
--rw-rw-rw-   0        0        0     3407 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/utils/env.py
--rw-rw-rw-   0        0        0     2092 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/ext_loader.py
--rw-rw-rw-   0        0        0     6167 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/hub.py
--rw-rw-rw-   0        0        0    13305 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/logging.py
--rw-rw-rw-   0        0        0    11864 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/misc.py
--rw-rw-rw-   0        0        0      940 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/parrots_jit.py
--rw-rw-rw-   0        0        0     3643 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/parrots_wrapper.py
--rw-rw-rw-   0        0        0     3516 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/path.py
--rw-rw-rw-   0        0        0     7313 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/progressbar.py
--rw-rw-rw-   0        0        0    11722 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/registry.py
--rw-rw-rw-   0        0        0     4429 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/testing.py
--rw-rw-rw-   0        0        0     3180 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/timer.py
--rw-rw-rw-   0        0        0      806 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/utils/trace.py
--rw-rw-rw-   0        0        0     2763 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/utils/version_utils.py
--rw-rw-rw-   0        0        0     1211 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/version.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/video/
--rw-rw-rw-   0        0        0      581 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/video/__init__.py
--rw-rw-rw-   0        0        0    10517 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/video/io.py
--rw-rw-rw-   0        0        0     9942 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/video/optflow.py
--rw-rw-rw-   0        0        0     5439 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/video/processing.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis/mmcv/visualization/
--rw-rw-rw-   0        0        0      347 2022-10-04 08:46:06.000000 udl_vis-0.2/udl_vis/mmcv/visualization/__init__.py
--rw-rw-rw-   0        0        0     1420 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/visualization/color.py
--rw-rw-rw-   0        0        0     5285 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/visualization/image.py
--rw-rw-rw-   0        0        0     3477 2023-06-07 03:14:13.000000 udl_vis-0.2/udl_vis/mmcv/visualization/optflow.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis.egg-info/
--rw-rw-rw-   0        0        0     5771 2023-06-07 10:07:29.000000 udl_vis-0.2/udl_vis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7849 2023-06-07 10:07:30.000000 udl_vis-0.2/udl_vis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:07:29.000000 udl_vis-0.2/udl_vis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-06-07 10:07:29.000000 udl_vis-0.2/udl_vis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 10:07:29.000000 udl_vis-0.2/udl_vis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/
+-rw-rw-rw-   0        0        0    35823 2022-10-04 08:46:06.000000 udl_vis-0.2b0/LICENSE
+-rw-rw-rw-   0        0        0     5773 2023-06-09 11:12:34.000000 udl_vis-0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     5271 2023-06-07 04:18:04.000000 udl_vis-0.2b0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:12:34.000000 udl_vis-0.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1169 2023-06-09 11:09:34.000000 udl_vis-0.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/AutoDL/
+-rw-rw-rw-   0        0        0       15 2023-06-09 09:55:01.000000 udl_vis-0.2b0/udl_vis/AutoDL/__init__.py
+-rw-rw-rw-   0        0        0    13693 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/AutoDL/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/Basis/
+-rw-rw-rw-   0        0        0       15 2023-06-09 09:55:01.000000 udl_vis-0.2b0/udl_vis/Basis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/
+-rw-rw-rw-   0        0        0      134 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/__init__.py
+-rw-rw-rw-   0        0        0     1084 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/base.py
+-rw-rw-rw-   0        0        0     7303 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/fp16_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/
+-rw-rw-rw-   0        0        0      787 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/__init__.py
+-rw-rw-rw-   0        0        0     1142 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/__main__.py
+-rw-rw-rw-   0        0        0     9296 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/compute_flops.py
+-rw-rw-rw-   0        0        0     6085 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/compute_madd.py
+-rw-rw-rw-   0        0        0     4016 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/compute_memory.py
+-rw-rw-rw-   0        0        0    10202 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/model_hook.py
+-rw-rw-rw-   0        0        0     3758 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/reporter.py
+-rw-rw-rw-   0        0        0     5899 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/stat_tree.py
+-rw-rw-rw-   0        0        0     3364 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/statistics.py
+-rw-rw-rw-   0        0        0    11956 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/Basis/auxiliary/utils.py
+-rw-rw-rw-   0        0        0     2851 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/cal_ssim.py
+-rw-rw-rw-   0        0        0    29004 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/Basis/config.py
+-rw-rw-rw-   0        0        0     4087 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/Basis/criterion_metrics.py
+-rw-rw-rw-   0        0        0     6622 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/dist_utils.py
+-rw-rw-rw-   0        0        0    14882 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/launch.py
+-rw-rw-rw-   0        0        0     8754 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/Basis/logger.py
+-rw-rw-rw-   0        0        0     3145 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/Basis/metrics.py
+-rw-rw-rw-   0        0        0    16848 2022-09-16 14:28:57.000000 udl_vis-0.2b0/udl_vis/Basis/module.py
+-rw-rw-rw-   0        0        0     9926 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/Basis/optim.py
+-rw-rw-rw-   0        0        0     6206 2023-06-09 09:58:03.000000 udl_vis-0.2b0/udl_vis/Basis/option.py
+-rw-rw-rw-   0        0        0    17306 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/Basis/postprocess.py
+-rw-rw-rw-   0        0        0     5203 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/Basis/python_sub_class.py
+-rw-rw-rw-   0        0        0     3145 2023-06-07 03:16:59.000000 udl_vis-0.2b0/udl_vis/Basis/variance_sacling_initializer.py
+-rw-rw-rw-   0        0        0      250 2023-06-09 10:56:31.000000 udl_vis-0.2b0/udl_vis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/
+-rw-rw-rw-   0        0        0      367 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/arraymisc/
+-rw-rw-rw-   0        0        0      137 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/arraymisc/__init__.py
+-rw-rw-rw-   0        0        0     1879 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/arraymisc/quantization.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/
+-rw-rw-rw-   0        0        0     2479 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/__init__.py
+-rw-rw-rw-   0        0        0     2051 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/alexnet.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/
+-rw-rw-rw-   0        0        0     1767 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/__init__.py
+-rw-rw-rw-   0        0        0     2582 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/activation.py
+-rw-rw-rw-   0        0        0     4806 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/context_block.py
+-rw-rw-rw-   0        0        0     1490 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv.py
+-rw-rw-rw-   0        0        0     2576 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-rw-rw-   0        0        0     8946 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv_module.py
+-rw-rw-rw-   0        0        0     5565 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv_ws.py
+-rw-rw-rw-   0        0        0     4238 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-rw-rw-   0        0        0     2217 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/drop.py
+-rw-rw-rw-   0        0        0    16408 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/generalized_attention.py
+-rw-rw-rw-   0        0        0     1592 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/hsigmoid.py
+-rw-rw-rw-   0        0        0      680 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/hswish.py
+-rw-rw-rw-   0        0        0    11318 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/non_local.py
+-rw-rw-rw-   0        0        0     5255 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/norm.py
+-rw-rw-rw-   0        0        0     1163 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/padding.py
+-rw-rw-rw-   0        0        0     2593 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/plugin.py
+-rw-rw-rw-   0        0        0      654 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/registry.py
+-rw-rw-rw-   0        0        0      598 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/scale.py
+-rw-rw-rw-   0        0        0      510 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/swish.py
+-rw-rw-rw-   0        0        0    38090 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/transformer.py
+-rw-rw-rw-   0        0        0     2962 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/upsample.py
+-rw-rw-rw-   0        0        0     7141 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/wrappers.py
+-rw-rw-rw-   0        0        0     1119 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/builder.py
+-rw-rw-rw-   0        0        0    10271 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/resnet.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/
+-rw-rw-rw-   0        0        0     1042 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/__init__.py
+-rw-rw-rw-   0        0        0    22678 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/flops_counter.py
+-rw-rw-rw-   0        0        0     1940 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-rw-rw-   0        0        0     2358 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/sync_bn.py
+-rw-rw-rw-   0        0        0    26645 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/weight_init.py
+-rw-rw-rw-   0        0        0     6228 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/cnn/vgg.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/engine/
+-rw-rw-rw-   0        0        0      274 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/engine/__init__.py
+-rw-rw-rw-   0        0        0     7350 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/engine/test.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/
+-rw-rw-rw-   0        0        0      489 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/__init__.py
+-rw-rw-rw-   0        0        0    43043 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/file_client.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/
+-rw-rw-rw-   0        0        0      285 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1023 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/base.py
+-rw-rw-rw-   0        0        0     1104 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/json_handler.py
+-rw-rw-rw-   0        0        0      845 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/pickle_handler.py
+-rw-rw-rw-   0        0        0      689 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/yaml_handler.py
+-rw-rw-rw-   0        0        0     5671 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/io.py
+-rw-rw-rw-   0        0        0     3555 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/fileio/parse.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/image/
+-rw-rw-rw-   0        0        0     1753 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/image/__init__.py
+-rw-rw-rw-   0        0        0    10197 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/image/colorspace.py
+-rw-rw-rw-   0        0        0    25898 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/image/geometric.py
+-rw-rw-rw-   0        0        0    11973 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/image/io.py
+-rw-rw-rw-   0        0        0     2000 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/image/misc.py
+-rw-rw-rw-   0        0        0    15427 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/image/photometric.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/
+-rw-rw-rw-   0        0        0      201 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/__init__.py
+-rw-rw-rw-   0        0        0      611 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/info.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/onnx_utils/
+-rw-rw-rw-   0        0        0       49 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/onnx_utils/__init__.py
+-rw-rw-rw-   0        0        0    11503 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/onnx_utils/symbolic_helper.py
+-rw-rw-rw-   0        0        0    19620 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/onnx/symbolic.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/
+-rw-rw-rw-   0        0        0     5108 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/__init__.py
+-rw-rw-rw-   0        0        0     2162 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/active_rotated_filter.py
+-rw-rw-rw-   0        0        0     4678 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/assign_score_withk.py
+-rw-rw-rw-   0        0        0     1775 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/ball_query.py
+-rw-rw-rw-   0        0        0     2665 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/bbox.py
+-rw-rw-rw-   0        0        0     3812 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/border_align.py
+-rw-rw-rw-   0        0        0     5319 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/box_iou_rotated.py
+-rw-rw-rw-   0        0        0    10187 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/carafe.py
+-rw-rw-rw-   0        0        0     3130 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/cc_attention.py
+-rw-rw-rw-   0        0        0     1843 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/contour_expand.py
+-rw-rw-rw-   0        0        0     1719 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/convex_iou.py
+-rw-rw-rw-   0        0        0     4920 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/corner_pool.py
+-rw-rw-rw-   0        0        0     6893 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/correlation.py
+-rw-rw-rw-   0        0        0    15999 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/deform_conv.py
+-rw-rw-rw-   0        0        0     7614 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/deform_roi_pool.py
+-rw-rw-rw-   0        0        0     1629 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/deprecated_wrappers.py
+-rw-rw-rw-   0        0        0     6794 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/focal_loss.py
+-rw-rw-rw-   0        0        0     2672 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/furthest_point_sample.py
+-rw-rw-rw-   0        0        0    10385 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/fused_bias_leakyrelu.py
+-rw-rw-rw-   0        0        0     1682 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/gather_points.py
+-rw-rw-rw-   0        0        0     8617 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/group_points.py
+-rw-rw-rw-   0        0        0      923 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/info.py
+-rw-rw-rw-   0        0        0     3227 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/iou3d.py
+-rw-rw-rw-   0        0        0     2692 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/knn.py
+-rw-rw-rw-   0        0        0     3870 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/masked_conv.py
+-rw-rw-rw-   0        0        0     5552 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/merge_cells.py
+-rw-rw-rw-   0        0        0      573 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/min_area_polygons.py
+-rw-rw-rw-   0        0        0    10872 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/modulated_deform_conv.py
+-rw-rw-rw-   0        0        0    15562 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/multi_scale_deform_attn.py
+-rw-rw-rw-   0        0        0    17688 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/nms.py
+-rw-rw-rw-   0        0        0     3214 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/pixel_group.py
+-rw-rw-rw-   0        0        0    12787 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/point_sample.py
+-rw-rw-rw-   0        0        0     5503 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/points_in_boxes.py
+-rw-rw-rw-   0        0        0     1506 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/points_in_polygons.py
+-rw-rw-rw-   0        0        0     6272 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/points_sampler.py
+-rw-rw-rw-   0        0        0     2865 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/psa_mask.py
+-rw-rw-rw-   0        0        0     4852 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/riroi_align_rotated.py
+-rw-rw-rw-   0        0        0     8742 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/roi_align.py
+-rw-rw-rw-   0        0        0     6611 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/roi_align_rotated.py
+-rw-rw-rw-   0        0        0     2603 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/roi_pool.py
+-rw-rw-rw-   0        0        0     4358 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/roiaware_pool3d.py
+-rw-rw-rw-   0        0        0     3085 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/roipoint_pool3d.py
+-rw-rw-rw-   0        0        0     2994 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/rotated_feature_align.py
+-rw-rw-rw-   0        0        0     5970 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/saconv.py
+-rw-rw-rw-   0        0        0     5563 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/scatter_points.py
+-rw-rw-rw-   0        0        0    11526 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/sync_bn.py
+-rw-rw-rw-   0        0        0     2315 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/three_interpolate.py
+-rw-rw-rw-   0        0        0     1590 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/three_nn.py
+-rw-rw-rw-   0        0        0     2279 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/tin_shift.py
+-rw-rw-rw-   0        0        0    12132 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/upfirdn2d.py
+-rw-rw-rw-   0        0        0     5875 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/ops/voxelize.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/
+-rw-rw-rw-   0        0        0      518 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/__init__.py
+-rw-rw-rw-   0        0        0     2775 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/_functions.py
+-rw-rw-rw-   0        0        0     3749 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/collate.py
+-rw-rw-rw-   0        0        0     2454 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/data_container.py
+-rw-rw-rw-   0        0        0     4588 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/data_parallel.py
+-rw-rw-rw-   0        0        0     4945 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/distributed.py
+-rw-rw-rw-   0        0        0     2887 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/distributed_deprecated.py
+-rw-rw-rw-   0        0        0      328 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/registry.py
+-rw-rw-rw-   0        0        0     2366 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/scatter_gather.py
+-rw-rw-rw-   0        0        0      728 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/parallel/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/
+-rw-rw-rw-   0        0        0     4385 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/__init__.py
+-rw-rw-rw-   0        0        0    14570 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/base_module.py
+-rw-rw-rw-   0        0        0    22884 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/base_runner.py
+-rw-rw-rw-   0        0        0      690 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/builder.py
+-rw-rw-rw-   0        0        0    33627 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/checkpoint.py
+-rw-rw-rw-   0        0        0     1952 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/default_constructor.py
+-rw-rw-rw-   0        0        0     5559 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/dist_utils.py
+-rw-rw-rw-   0        0        0    13655 2023-06-09 10:30:28.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/epoch_based_runner.py
+-rw-rw-rw-   0        0        0    16873 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/fp16_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/
+-rw-rw-rw-   0        0        0     2402 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/__init__.py
+-rw-rw-rw-   0        0        0    18943 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/checkpoint.py
+-rw-rw-rw-   0        0        0      280 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/closure.py
+-rw-rw-rw-   0        0        0     3674 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/ema.py
+-rw-rw-rw-   0        0        0    22909 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/evaluation.py
+-rw-rw-rw-   0        0        0     2841 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/hook.py
+-rw-rw-rw-   0        0        0      521 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/iter_timer.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/
+-rw-rw-rw-   0        0        0      537 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/__init__.py
+-rw-rw-rw-   0        0        0     6151 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/base.py
+-rw-rw-rw-   0        0        0     2294 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/dvclive.py
+-rw-rw-rw-   0        0        0     2995 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/mlflow.py
+-rw-rw-rw-   0        0        0     3338 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/neptune.py
+-rw-rw-rw-   0        0        0     5269 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/pavi.py
+-rw-rw-rw-   0        0        0     2739 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/tensorboard.py
+-rw-rw-rw-   0        0        0    11234 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/text.py
+-rw-rw-rw-   0        0        0     4009 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/wandb.py
+-rw-rw-rw-   0        0        0    27815 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/lr_updater.py
+-rw-rw-rw-   0        0        0      682 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/memory.py
+-rw-rw-rw-   0        0        0    23465 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/momentum_updater.py
+-rw-rw-rw-   0        0        0     1602 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/nni_hook.py
+-rw-rw-rw-   0        0        0    25296 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/optimizer.py
+-rw-rw-rw-   0        0        0     8221 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/profiler.py
+-rw-rw-rw-   0        0        0      867 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/sampler_seed.py
+-rw-rw-rw-   0        0        0      729 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/sync_buffer.py
+-rw-rw-rw-   0        0        0    11438 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/iter_based_runner.py
+-rw-rw-rw-   0        0        0     1880 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/log_buffer.py
+-rw-rw-rw-   0        0        0     1241 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/misc.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/optimizer/
+-rw-rw-rw-   0        0        0      379 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     1390 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/optimizer/builder.py
+-rw-rw-rw-   0        0        0    11971 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/optimizer/default_constructor.py
+-rw-rw-rw-   0        0        0     1658 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/priority.py
+-rw-rw-rw-   0        0        0    11163 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/record.py
+-rw-rw-rw-   0        0        0     3014 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/runner/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/tensorrt/
+-rw-rw-rw-   0        0        0      788 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/tensorrt/__init__.py
+-rw-rw-rw-   0        0        0      916 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/tensorrt/init_plugins.py
+-rw-rw-rw-   0        0        0     4459 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/tensorrt/preprocess.py
+-rw-rw-rw-   0        0        0     8417 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/tensorrt/tensorrt_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/
+-rw-rw-rw-   0        0        0     4027 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/__init__.py
+-rw-rw-rw-   0        0        0    27039 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/config.py
+-rw-rw-rw-   0        0        0     3407 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/env.py
+-rw-rw-rw-   0        0        0     2092 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/ext_loader.py
+-rw-rw-rw-   0        0        0     6167 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/hub.py
+-rw-rw-rw-   0        0        0    13394 2023-06-09 10:32:17.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/logging.py
+-rw-rw-rw-   0        0        0    11864 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/misc.py
+-rw-rw-rw-   0        0        0      940 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/parrots_jit.py
+-rw-rw-rw-   0        0        0     3643 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/parrots_wrapper.py
+-rw-rw-rw-   0        0        0     3516 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/path.py
+-rw-rw-rw-   0        0        0     7313 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/progressbar.py
+-rw-rw-rw-   0        0        0    11722 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/registry.py
+-rw-rw-rw-   0        0        0     4429 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/testing.py
+-rw-rw-rw-   0        0        0     3180 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/timer.py
+-rw-rw-rw-   0        0        0      806 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/trace.py
+-rw-rw-rw-   0        0        0     2763 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/utils/version_utils.py
+-rw-rw-rw-   0        0        0     1211 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/version.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/video/
+-rw-rw-rw-   0        0        0      581 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/video/__init__.py
+-rw-rw-rw-   0        0        0    10517 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/video/io.py
+-rw-rw-rw-   0        0        0     9942 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/video/optflow.py
+-rw-rw-rw-   0        0        0     5439 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/video/processing.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis/mmcv/visualization/
+-rw-rw-rw-   0        0        0      347 2022-10-04 08:46:06.000000 udl_vis-0.2b0/udl_vis/mmcv/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1420 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/visualization/color.py
+-rw-rw-rw-   0        0        0     5285 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/visualization/image.py
+-rw-rw-rw-   0        0        0     3477 2023-06-07 03:14:13.000000 udl_vis-0.2b0/udl_vis/mmcv/visualization/optflow.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis.egg-info/
+-rw-rw-rw-   0        0        0     5773 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7849 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 11:12:34.000000 udl_vis-0.2b0/udl_vis.egg-info/top_level.txt
```

### Comparing `udl_vis-0.2/LICENSE` & `udl_vis-0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/PKG-INFO` & `udl_vis-0.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udl_vis
-Version: 0.2
+Version: 0.2b0
 Summary: unified pytorch framework for vision task
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `udl_vis-0.2/README.md` & `udl_vis-0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/setup.py` & `udl_vis-0.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         name='udl_vis',
         description="unified pytorch framework for vision task",
         long_description=open("README.md", encoding='utf-8').read(),
         long_description_content_type="text/markdown",
         author="XiaoXiao-Woo",
         author_email="wxwsx1997@gmail.com",
         url='https://github.com/XiaoXiao-Woo/PanCollection',
-        version='0.2',
+        version='0.2b',
         packages=find_packages(),
         license='GPLv3',
         python_requires='>=3.7',
         install_requires=[
             "psutil",
             "opencv-python",
             "numpy",
```

### Comparing `udl_vis-0.2/udl_vis/AutoDL/trainer.py` & `udl_vis-0.2b0/udl_vis/AutoDL/trainer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/base.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/base.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/fp16_utils.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/__init__.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/__main__.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/__main__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/compute_flops.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/compute_flops.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/compute_madd.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/compute_madd.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/compute_memory.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/compute_memory.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/model_hook.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/model_hook.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/reporter.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/reporter.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/stat_tree.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/stat_tree.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/torchstat/statistics.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/torchstat/statistics.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/auxiliary/utils.py` & `udl_vis-0.2b0/udl_vis/Basis/auxiliary/utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/cal_ssim.py` & `udl_vis-0.2b0/udl_vis/Basis/cal_ssim.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/config.py` & `udl_vis-0.2b0/udl_vis/Basis/config.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/criterion_metrics.py` & `udl_vis-0.2b0/udl_vis/Basis/criterion_metrics.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/dist_utils.py` & `udl_vis-0.2b0/udl_vis/Basis/dist_utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/launch.py` & `udl_vis-0.2b0/udl_vis/Basis/launch.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/logger.py` & `udl_vis-0.2b0/udl_vis/Basis/logger.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/metrics.py` & `udl_vis-0.2b0/udl_vis/Basis/metrics.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/module.py` & `udl_vis-0.2b0/udl_vis/Basis/module.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/optim.py` & `udl_vis-0.2b0/udl_vis/Basis/optim.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/option.py` & `udl_vis-0.2b0/udl_vis/Basis/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os
 from udl_vis.Basis.python_sub_class import TaskDispatcher
 from udl_vis.Basis.config import Config
 import warnings
 
 def common_cfg():
     parser = argparse.ArgumentParser(description='PyTorch Training')
+
     # * Logger
     parser.add_argument('--use-log', default=True
                         , type=bool)
     parser.add_argument('--log-dir', metavar='DIR', default='logs',
                         help='path to save log')
     parser.add_argument('--tfb-dir', metavar='DIR', default=None,
                         help='useless in this script.')
@@ -65,15 +66,15 @@
     parser.add_argument('--mode', type=str, default=None,
                         help='dataset file extension')
     parser.add_argument('--task', type=str, default=None,
                         help='dataset file extension')
     parser.add_argument('--arch', type=str, default='',
                         help='dataset file extension')
 
-    args = parser.parse_args()
+    args = parser.parse_args(args=[])
     args.global_rank = 0
     args.once_epoch = False
     args.reset_lr = False
     args.amp_opt_level = 'O0' if args.amp == None else args.amp_opt_level
     args.save_top_k = 5
     args.start_epoch = 1
     assert args.accumulated_step > 0
```

### Comparing `udl_vis-0.2/udl_vis/Basis/postprocess.py` & `udl_vis-0.2b0/udl_vis/Basis/postprocess.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/python_sub_class.py` & `udl_vis-0.2b0/udl_vis/Basis/python_sub_class.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/Basis/variance_sacling_initializer.py` & `udl_vis-0.2b0/udl_vis/Basis/variance_sacling_initializer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/arraymisc/quantization.py` & `udl_vis-0.2b0/udl_vis/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/alexnet.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/activation.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/context_block.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv_module.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/conv_ws.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/drop.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/generalized_attention.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/hsigmoid.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/hswish.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/non_local.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/norm.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/padding.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/plugin.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/registry.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/scale.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/transformer.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/upsample.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/bricks/wrappers.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/builder.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/resnet.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/utils/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/utils/flops_counter.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/utils/fuse_conv_bn.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/utils/sync_bn.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/utils/weight_init.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/cnn/vgg.py` & `udl_vis-0.2b0/udl_vis/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/engine/test.py` & `udl_vis-0.2b0/udl_vis/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/file_client.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/handlers/base.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/handlers/json_handler.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/handlers/pickle_handler.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/handlers/yaml_handler.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/io.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/fileio/parse.py` & `udl_vis-0.2b0/udl_vis/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/image/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/image/colorspace.py` & `udl_vis-0.2b0/udl_vis/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/image/geometric.py` & `udl_vis-0.2b0/udl_vis/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/image/io.py` & `udl_vis-0.2b0/udl_vis/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/image/misc.py` & `udl_vis-0.2b0/udl_vis/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/image/photometric.py` & `udl_vis-0.2b0/udl_vis/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/onnx/info.py` & `udl_vis-0.2b0/udl_vis/mmcv/onnx/info.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/onnx/onnx_utils/symbolic_helper.py` & `udl_vis-0.2b0/udl_vis/mmcv/onnx/onnx_utils/symbolic_helper.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/onnx/symbolic.py` & `udl_vis-0.2b0/udl_vis/mmcv/onnx/symbolic.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/active_rotated_filter.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/active_rotated_filter.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/assign_score_withk.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/ball_query.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/bbox.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/border_align.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/box_iou_rotated.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/carafe.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/cc_attention.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/contour_expand.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/convex_iou.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/convex_iou.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/corner_pool.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/correlation.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/deform_conv.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/deform_roi_pool.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/deprecated_wrappers.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/focal_loss.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/furthest_point_sample.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/fused_bias_leakyrelu.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/gather_points.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/group_points.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/info.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/iou3d.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/knn.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/masked_conv.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/merge_cells.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/min_area_polygons.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/min_area_polygons.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/modulated_deform_conv.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/multi_scale_deform_attn.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/nms.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/pixel_group.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/point_sample.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/points_in_boxes.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/points_in_polygons.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/points_in_polygons.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/points_sampler.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/psa_mask.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/riroi_align_rotated.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/riroi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/roi_align.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/roi_align_rotated.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/roi_pool.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/roiaware_pool3d.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/roipoint_pool3d.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/rotated_feature_align.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/rotated_feature_align.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/saconv.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/scatter_points.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/sync_bn.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/three_interpolate.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/three_nn.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/tin_shift.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/upfirdn2d.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/ops/voxelize.py` & `udl_vis-0.2b0/udl_vis/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/_functions.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/collate.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/data_container.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/data_parallel.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/distributed.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/distributed_deprecated.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/scatter_gather.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/parallel/utils.py` & `udl_vis-0.2b0/udl_vis/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/base_module.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/base_runner.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/builder.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/checkpoint.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/default_constructor.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/dist_utils.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/epoch_based_runner.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/fp16_utils.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/checkpoint.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/ema.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/evaluation.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/hook.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/iter_timer.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/iter_timer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/base.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/dvclive.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/mlflow.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/neptune.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/pavi.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/tensorboard.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/text.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/logger/wandb.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/lr_updater.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/memory.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/momentum_updater.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/nni_hook.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/nni_hook.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/optimizer.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/profiler.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/sampler_seed.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/hooks/sync_buffer.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/iter_based_runner.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/log_buffer.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/misc.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/misc.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/optimizer/builder.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/optimizer/default_constructor.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/priority.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/record.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/record.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/runner/utils.py` & `udl_vis-0.2b0/udl_vis/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/tensorrt/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/tensorrt/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/tensorrt/init_plugins.py` & `udl_vis-0.2b0/udl_vis/mmcv/tensorrt/init_plugins.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/tensorrt/preprocess.py` & `udl_vis-0.2b0/udl_vis/mmcv/tensorrt/preprocess.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/tensorrt/tensorrt_utils.py` & `udl_vis-0.2b0/udl_vis/mmcv/tensorrt/tensorrt_utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/config.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/env.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/ext_loader.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/hub.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/hub.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/logging.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,25 +233,25 @@
 
     Returns:
         logging.Logger: The expected logger.
     """
     if name in logger_initialized:
         if cfg is None: # cfg.use_log
             return logging.getLogger(name)
-        else:
-            return None
+        # else:
+        #     return None
     # handle hierarchical names
     # e.g., logger "a" is initialized, then logger "a.b" will skip the
     # initialization since it is a child of "a".
-    for logger_name in logger_initialized:
-        if name.startswith(logger_name):
-            if cfg.use_log:
-                return logging.getLogger(name)
-            else:
-                return None
+    # for logger_name in logger_initialized:
+    #     if name.startswith(logger_name):
+    #         if cfg.use_log:
+    #             return logging.getLogger(name)
+    #         else:
+    #             return None
 
     logger = None
     tensorboard_log_dir = None
     root_output_dir = Path(cfg.out_dir)
     # set up logger in root_path
     if not root_output_dir.exists():
         # if not dist_print: #rank 0-N, 0 is False
@@ -293,15 +293,15 @@
             print_log('=> creating tfb logs {}'.format(tensorboard_log_dir))
             tensorboard_log_dir.mkdir(parents=True, exist_ok=True)
         logger = setup_logger(name, final_log_file)
 
     return logger, str(final_output_dir), str(model_save_dir), str(
         tensorboard_log_dir)  # logger,
 
-def print_log(msg, logger=None, level=logging.INFO):
+def print_log(msg, logger=None, level=logging.INFO, clear_logger=False):
     """Print a log message.
 
     Args:
         msg (str): The message to be logged.
         logger (logging.Logger | str | None): The logger to be used.
             Some special loggers are:
             - "silent": no message will be printed.
@@ -319,15 +319,16 @@
     elif isinstance(logger, str):
         _logger = get_logger(logger)
         _logger.log(level, msg)
     else:
         raise TypeError(
             'logger should be either a logging.Logger object, str, '
             f'"silent" or None, but got {type(logger)}')
-
+    if clear_logger:
+        logger_initialized = {}
 
 def load_json_log(json_log):
     """load and convert json_logs to log_dicts.
 
     Args:
         json_log (str): The path of the json log file.
```

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/misc.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/parrots_jit.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/parrots_wrapper.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/path.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/progressbar.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/registry.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/testing.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/timer.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/trace.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/utils/version_utils.py` & `udl_vis-0.2b0/udl_vis/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/version.py` & `udl_vis-0.2b0/udl_vis/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/video/__init__.py` & `udl_vis-0.2b0/udl_vis/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/video/io.py` & `udl_vis-0.2b0/udl_vis/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/video/optflow.py` & `udl_vis-0.2b0/udl_vis/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/video/processing.py` & `udl_vis-0.2b0/udl_vis/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/visualization/color.py` & `udl_vis-0.2b0/udl_vis/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/visualization/image.py` & `udl_vis-0.2b0/udl_vis/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis/mmcv/visualization/optflow.py` & `udl_vis-0.2b0/udl_vis/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `udl_vis-0.2/udl_vis.egg-info/PKG-INFO` & `udl_vis-0.2b0/udl_vis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udl-vis
-Version: 0.2
+Version: 0.2b0
 Summary: unified pytorch framework for vision task
 Home-page: https://github.com/XiaoXiao-Woo/PanCollection
 Author: XiaoXiao-Woo
 Author-email: wxwsx1997@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `udl_vis-0.2/udl_vis.egg-info/SOURCES.txt` & `udl_vis-0.2b0/udl_vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

