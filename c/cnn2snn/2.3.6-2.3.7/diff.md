# Comparing `tmp/cnn2snn-2.3.6.tar.gz` & `tmp/cnn2snn-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnn2snn-2.3.6.tar", last modified: Wed May 17 14:19:31 2023, max compression
+gzip compressed data, was "cnn2snn-2.3.7.tar", last modified: Fri Jun  9 15:01:59 2023, max compression
```

## Comparing `cnn2snn-2.3.6.tar` & `cnn2snn-2.3.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      520 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/akida_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/cnn2snn/calibration/
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16847 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/adaround.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)    12381 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/calibration.py
--rw-r--r--   0 root         (0) root         (0)    10739 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/cli.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/cnn2snn_objects.py
--rw-r--r--   0 root         (0) root         (0)    12382 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/converter.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/min_value_constraint.py
--rw-r--r--   0 root         (0) root         (0)    14077 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/model_generator.py
--rw-r--r--   0 root         (0) root         (0)    13749 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantization.py
--rw-r--r--   0 root         (0) root         (0)    26028 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantization_layers.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantization_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3962 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/activations.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/add.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/attention.py
--rw-r--r--   0 root         (0) root         (0)     5283 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/block_converter.py
--rw-r--r--   0 root         (0) root         (0)     9312 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13554 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/concatenate.py
--rw-r--r--   0 root         (0) root         (0)     6579 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/convolution.py
--rw-r--r--   0 root         (0) root         (0)    11957 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/dense.py
--rw-r--r--   0 root         (0) root         (0)     6272 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     6348 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/extract_token.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/input_data.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/layer_utils.py
--rw-r--r--   0 root         (0) root         (0)     4981 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/madnorm.py
--rw-r--r--   0 root         (0) root         (0)     6321 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/model_generator.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/outputs.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/padding.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/pooling.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     3083 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     7996 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/stem.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/cnn2snn/transforms/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/clone.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/equalization.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/reshape.py
--rw-r--r--   0 root         (0) root         (0)    14261 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/sequential.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/utils.py
--rw-r--r--   0 root         (0) root         (0)    11223 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/weights_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      520 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1798 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2023-05-17 14:19:24.000000 cnn2snn-2.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.619969 cnn2snn-2.3.7/cnn2snn/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/akida_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.619969 cnn2snn-2.3.7/cnn2snn/calibration/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16847 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/adaround.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    10739 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/cnn2snn_objects.py
+-rw-r--r--   0 root         (0) root         (0)    12382 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/min_value_constraint.py
+-rw-r--r--   0 root         (0) root         (0)    14077 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)    13749 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    26028 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantization_layers.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantization_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/cnn2snn/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/activations.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/add.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5283 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/block_converter.py
+-rw-r--r--   0 root         (0) root         (0)     9312 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    14915 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/concatenate.py
+-rw-r--r--   0 root         (0) root         (0)     6579 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/convolution.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/dense.py
+-rw-r--r--   0 root         (0) root         (0)     6272 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/extract_token.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/layer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4981 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/madnorm.py
+-rw-r--r--   0 root         (0) root         (0)     6214 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/padding.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     8660 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/stem.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/cnn2snn/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/clone.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/equalization.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/reshape.py
+-rw-r--r--   0 root         (0) root         (0)    14261 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/sequential.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/weights_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.619969 cnn2snn-2.3.7/cnn2snn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-06-09 15:01:53.000000 cnn2snn-2.3.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cnn2snn-2.3.6/LICENSE` & `cnn2snn-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/PKG-INFO` & `cnn2snn-2.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.6
+Version: 2.3.7
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.6/cnn2snn/__init__.py` & `cnn2snn-2.3.7/cnn2snn/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/akida_versions.py` & `cnn2snn-2.3.7/cnn2snn/akida_versions.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/calibration/__init__.py` & `cnn2snn-2.3.7/cnn2snn/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/calibration/adaround.py` & `cnn2snn-2.3.7/cnn2snn/calibration/adaround.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/calibration/bias_correction.py` & `cnn2snn-2.3.7/cnn2snn/calibration/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/calibration/calibration.py` & `cnn2snn-2.3.7/cnn2snn/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/cli.py` & `cnn2snn-2.3.7/cnn2snn/cli.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/cnn2snn_objects.py` & `cnn2snn-2.3.7/cnn2snn/cnn2snn_objects.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/compatibility_checks.py` & `cnn2snn-2.3.7/cnn2snn/compatibility_checks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/converter.py` & `cnn2snn-2.3.7/cnn2snn/converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/min_value_constraint.py` & `cnn2snn-2.3.7/cnn2snn/min_value_constraint.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/model_generator.py` & `cnn2snn-2.3.7/cnn2snn/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantization.py` & `cnn2snn-2.3.7/cnn2snn/quantization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantization_layers.py` & `cnn2snn-2.3.7/cnn2snn/quantization_layers.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantization_ops.py` & `cnn2snn-2.3.7/cnn2snn/quantization_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/__init__.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/activations.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/activations.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/add.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/add.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/attention.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/attention.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/batchnorm.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/batchnorm.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/block_converter.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/block_converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,26 +20,35 @@
 
 from ..akida_versions import AkidaVersion
 
 # Mapper to match layers block patterns with the right conversion method, populated thanks to
 # `register_conversion_patterns` function.
 _V2_PATTERN_CONVERTERS = {}
 _V1_PATTERN_CONVERTERS = {}
+_V2_INPUT_PATTERN_CONVERTERS = {}
+_V1_INPUT_PATTERN_CONVERTERS = {}
 
 
-def register_conversion_patterns(version, patterns, converter):
+def register_conversion_patterns(version, patterns, converter, input_pattern=False):
     """Helper to populate the patterns_to_function dictionaries according to the right version.
 
     Args:
         version (AkidaVersion): the target Akida version.
         patterns (list): list of compatible quantized layers type patterns.
         converter (:obj:`BlockConverter`): the associated converter object.
+        input_pattern (bool, optional): boolean to specify if the pattern should match an Akida
+            input layer (such as a Stem or InputConv2D). Defaults to False.
     """
-
-    dict_ver = _V2_PATTERN_CONVERTERS if version == AkidaVersion.v2 else _V1_PATTERN_CONVERTERS
+    if input_pattern:
+        if version == AkidaVersion.v2:
+            dict_ver = _V2_INPUT_PATTERN_CONVERTERS
+        else:
+            dict_ver = _V1_INPUT_PATTERN_CONVERTERS
+    else:
+        dict_ver = _V2_PATTERN_CONVERTERS if version == AkidaVersion.v2 else _V1_PATTERN_CONVERTERS
     for pattern in patterns:
         dict_ver.update({pattern: converter})
 
 
 class BlockConverter:
     """This represents the main class that allows the conversion of a block of quantized layers with
     quantizeml into their Akida layer equivalent.
```

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/blocks.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/blocks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/compatibility_checks.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/compatibility_checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from keras import layers
 from quantizeml import layers as qlayers
 
 from .blocks import split_model_into_blocks
 from .padding import check_same_valid_compatibility
 from ..transforms.sequential import _check_layers_data_format, _check_layer_inbounds
 from ..akida_versions import get_akida_version, AkidaVersion
-from .block_converter import _V1_PATTERN_CONVERTERS, _V2_PATTERN_CONVERTERS
+from .block_converter import (_V1_PATTERN_CONVERTERS, _V2_PATTERN_CONVERTERS,
+                              _V1_INPUT_PATTERN_CONVERTERS, _V2_INPUT_PATTERN_CONVERTERS)
 
 neural_layers = (qlayers.QuantizedConv2D, qlayers.QuantizedSeparableConv2D,
                  qlayers.QuantizedDense, qlayers.QuantizedDepthwiseConv2D,
                  qlayers.QuantizedConv2DTranspose, qlayers.QuantizedDepthwiseConv2DTranspose)
 skippable_layers = (layers.InputLayer, layers.Rescaling, layers.Activation, layers.Softmax,
                     layers.Dropout)
 pooling_layers = (qlayers.QuantizedGlobalAveragePooling2D, qlayers.QuantizedMaxPool2D)
@@ -115,26 +116,43 @@
         block_converter = _V1_PATTERN_CONVERTERS.get(pattern, None)
     else:
         block_converter = _V2_PATTERN_CONVERTERS.get(pattern, None)
 
     return block_converter
 
 
-def check_model_compatibility(model):
+def _get_input_block_converter(block):
+    """Helper to get the BlockConverter of an input block of layers.
+
+    Args:
+        block (list): list of quantized quantizeml layers.
+
+    Returns:
+        (:obj:`BlockConverter`): the BlockConverter corresponding to the block of layers or None.
+    """
+    pattern = _block_pattern(block)
+
+    if get_akida_version() == AkidaVersion.v1:
+        return _V1_INPUT_PATTERN_CONVERTERS.get(pattern, None)
+    return _V2_INPUT_PATTERN_CONVERTERS.get(pattern, None)
+
+
+def check_model_compatibility(model, input_is_image):
     r"""Checks if a QuantizeML model is compatible for Akida conversion.
 
     This function does NOT:
 
     - convert the QuantizeML model to an Akida model,
     - check if the model is compatible with Akida hardware
 
     It ONLY checks if the model design is compatible with Akida.
 
     Args:
         model (:obj:`tf.keras.Model`): the model to check.
+        input_is_image (bool): True if input is an 8-bit unsigned tensors (like images).
 
     Returns:
         list: a list of sequences of the non_skippable layers ('blocks').
     """
     # Check general rules about model in three steps:
     # 1. Check if model has only one input and one output,
     # 2. Check right data format and
@@ -147,19 +165,23 @@
     # Split model into theirs blocks:
     blocks = split_model_into_blocks(model)
 
     # This list will contains either a block converter instance,
     # or a list of non-skippable layers.
     straight_blocks = []
     # Evaluate block-by-block integrity
-    for block in blocks:
+    for id, block in enumerate(blocks):
         # Split blocks into skippable and none skippable blocks
         _, non_skippable = _extract_skippable_layers(block)
         # Get the corresponding BlockConverter of the layers block if available.
-        block_converter = _get_block_converter(non_skippable)
+        if id == 0 and input_is_image and not any(isinstance(layer, qlayers.QuantizedDense)
+                                                  for layer in block):
+            block_converter = _get_input_block_converter(non_skippable)
+        else:
+            block_converter = _get_block_converter(non_skippable)
         if block_converter:
             straight_blocks.append(block_converter(non_skippable))
             continue
         # TODO: remove this part once all conversion uses BlockConverter classes
         # Check pooling layers
         _check_pooling_compatibility(non_skippable)
         # Check other rules
@@ -307,14 +329,23 @@
     Returns:
         tuple: list of skippable and non skippable layers
     """
     skippable, non_skippable = [], []
     for layer in block:
         if isinstance(layer, skippable_layers):
             skippable.append(layer)
+        elif isinstance(layer, qlayers.QuantizedReshape):
+            in_shape = layer.input_shape
+            out_shape = layer.output_shape
+            in_dims = [x for x in in_shape if x != 1]
+            out_dims = [x for x in out_shape if x != 1]
+            if in_dims != out_dims:
+                non_skippable.append(layer)
+            else:
+                skippable.append(layer)
         else:
             non_skippable.append(layer)
     return skippable, non_skippable
 
 
 def _check_pooling_compatibility(block):
     """Asserts pooling layer is compatible for conversion.
```

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/concatenate.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/concatenate.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/conv2d_transpose.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/convolution.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/dense.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/dense.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d_transpose.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/dequantizer.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/dequantizer.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/extract_token.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/extract_token.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/input_data.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/input_data.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/layer_utils.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/layer_utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/madnorm.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/madnorm.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/model_generator.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/model_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 from .depthwise_conv2d import convert_depthwise_conv_block
 from .depthwise_conv2d_transpose import convert_depthwise_conv2d_transpose_block
 from .add import convert_quantized_add
 from .input_data import convert_input
 from .shiftmax import convert_quantized_shiftmax
 from .attention import convert_quantized_attention
 from .madnorm import convert_quantized_madnorm
-from .stem import convert_quantized_stem_layers
 from .concatenate import convert_quantized_concatenate
 from .convolution import convert_conv_block
 from .separable_convolution import convert_sepconv_block
 from .batchnorm import convert_batchnorm_block
 from .extract_token import convert_extract_token
 from .conv2d_transpose import convert_conv_transpose_block
 from .dequantizer import convert_dequantizer
 from ..akida_versions import AkidaVersion, get_akida_version
 from .compatibility_checks import check_model_compatibility
 from .block_converter import BlockConverter
+from .stem import StemBlockConverter
 
 
 def _raise_block_error(block):
     """ Raise error due to non convertible layers block"""
     block_layers_name = ""
     block_layers_type = ""
     for layer in block:
@@ -63,31 +63,28 @@
         model (:obj:`tf.keras.Model`): a Keras model to convert.
         input_is_image (bool): True if input is an 8-bit unsigned tensors (like images).
 
     Returns:
         :obj:`akida.Model`: the generated Akida model.
     """
     # Check if input model is convertible and extract its layers blocks
-    blocks = check_model_compatibility(model)
+    blocks = check_model_compatibility(model, input_is_image)
     # First store necessary variables for conversion
     record_quantization_variables(model)
 
     model_ak = Model()
 
-    # Identify the input block
-    ak_version = get_akida_version()
     # Flag to identify if the current block has been converted
     converted = False
-    if not isinstance(blocks[0], BlockConverter) and input_is_image:
-        if ak_version == AkidaVersion.v2:
-            # Convert the akida 2.0 stem block layer if the keras model has one.
-            converted = convert_quantized_stem_layers(model_ak, blocks[0])
-        if not converted:
-            # Look for an input convolution layer
-            converted = convert_conv_block(model_ak, blocks[0])
+    # Stem conversion is handled with the associated StemBlockConverter
+    if isinstance(blocks[0], StemBlockConverter):
+        converted = blocks[0].convert(model_ak)
+    if not converted and not isinstance(blocks[0], BlockConverter) and input_is_image:
+        # Look for an input convolution layer
+        converted = convert_conv_block(model_ak, blocks[0])
     if not converted:
         # Convert the keras InputLayer into an InputData layer
         convert_input(model_ak, model.layers[0], input_is_image)
     else:
         blocks.pop(0)
 
     for block in blocks:
```

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/outputs.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/outputs.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/padding.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/padding.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/pooling.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/pooling.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/separable_convolution.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/separable_convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/shiftmax.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/shiftmax.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/stem.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/stem.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,44 +18,59 @@
 Those layers are:
     - The Embedding layer
     - The Reshape layer
     - The ClassToken (+ the DistToken for distilled models) layer(s)
     - The AddPosEmbedding layer
 """
 from akida import LayerType, Stem
-import quantizeml.layers as qlayers
+from quantizeml.layers import (QuantizedConv2D, QuantizedReshape,
+                               QuantizedClassToken, QuantizedAddPositionEmbs, OutputQuantizer)
 import numpy as np
 from .blocks import get_block_out_quantizer
 from .outputs import set_output_v2_variables
 from .weights import broadcast_and_set_variables
+from .block_converter import BlockConverter, register_conversion_patterns
+from ..akida_versions import AkidaVersion
 
+_PATTERNS = [(QuantizedConv2D, QuantizedReshape, QuantizedClassToken, QuantizedAddPositionEmbs),
+             (QuantizedConv2D, QuantizedReshape, QuantizedAddPositionEmbs),
+             (QuantizedConv2D, QuantizedReshape, QuantizedClassToken, QuantizedClassToken,
+              QuantizedAddPositionEmbs)]
 
-def _set_stem_variables(ak_layer, layers):
+
+def _get_cls_layers(block):
+    """Helper that returns the QuantizedClassToken layers of a stem block.
+
+    Args:
+        block (list): the quantizeml quantized layers of the Stem to convert.
+
+    Returns:
+        list: Returns a list of the QuantizedClassToken layers of a stem block.
+    """
+
+    return [layer for layer in block if isinstance(layer, QuantizedClassToken)]
+
+
+def _set_stem_variables(ak_layer, block):
     """Computes and sets the variables for an Akida Stem layer.
 
     This function converts the variables of a Keras layers and sets them into
     the corresponding variables of the equivalent Akida layer.
 
     Args:
         ak_layer (:obj:`akida.Layer`): the targeted akida layer.
-        layers (list): list of the source quantized layers.
+        block (list): list of the source quantized layers block.
     """
     assert ak_layer.parameters.layer_type == LayerType.Stem
 
-    embedding_layer = layers[0]
+    embedding_layer = block[0]
 
-    cls_layers = []
-    add_pos_emb_layer = None
-    # Get the QuantizedClassToken layer(s) and the optional
-    # QuantizedAddPositionEmbs layer
-    for layer in layers:
-        if isinstance(layer, qlayers.QuantizedClassToken):
-            cls_layers.append(layer)
-        elif isinstance(layer, qlayers.QuantizedAddPositionEmbs):
-            add_pos_emb_layer = layer
+    # Get the optional QuantizedClassToken layer(s) and the QuantizedAddPositionEmbs layer
+    cls_layers = _get_cls_layers(block)
+    add_pos_emb_layer = block[-1]
 
     # Prepare a dict for akida variables
     variables_ak = {}
 
     # get the Embedding weights
     weights_ak = embedding_layer.weight_quantizer.qweights.value.fp.values.numpy()
 
@@ -77,130 +92,120 @@
             # Insert the token value at the first position. This allows us to match
             # the model concatenation order.
             tokens_ak.insert(0, np.squeeze(token_ak))
             shifts_tokens_ak.insert(0, token_shift)
         variables_ak["tokens"] = np.stack(tokens_ak)
         variables_ak["tokens_shift"] = np.concatenate(shifts_tokens_ak)
 
-    if add_pos_emb_layer:
-        # get the positional embedding matrix
-        pos_emb_quantizer = add_pos_emb_layer.pe_quantizer
-        pos_emb = pos_emb_quantizer.qweights.value.values.numpy().astype(np.int32)
-        pos_emb_shift = pos_emb_quantizer.shift.value.numpy().astype(np.uint8)
-        pos_emb_ak = pos_emb >> pos_emb_shift
-        variables_ak["pos_embedding"] = pos_emb_ak
-        # Get the QuantizedAddPositionEmbs layer shifts
-        variables_ak["pos_embs_shift"] = pos_emb_shift
+    # get the positional embedding matrix
+    pos_emb_quantizer = add_pos_emb_layer.pe_quantizer
+    pos_emb = pos_emb_quantizer.qweights.value.values.numpy().astype(np.int32)
+    pos_emb_shift = pos_emb_quantizer.shift.value.numpy().astype(np.uint8)
+    pos_emb_ak = pos_emb >> pos_emb_shift
+    variables_ak["pos_embedding"] = pos_emb_ak
+    # Get the QuantizedAddPositionEmbs layer shifts
+    variables_ak["pos_embs_shift"] = pos_emb_shift
 
     variables_ak["weights"] = weights_ak.astype(np.int8)
     variables_ak["bias"] = bias_ak
     # Get the Embedding layer shifts
     variables_ak["bias_shift"] = bias_shift.astype(np.uint8)
 
     broadcast_and_set_variables(ak_layer, variables_ak)
 
 
-def _parse_embedding(layer):
-    """Parses the quantizeml.QuantizedConv2D embedding layer parameters.
-
-    Args:
-        layer (:obj:`tf.keras.Layer`): the layer to parse.
-
-    Returns:
-        dict: the corresponding akida parameters.
-    """
-    # Remove batch dimension to get input shape
-    input_shape = layer.input_shape[1:]
-    filters = layer.filters
-    kernel_size = layer.kernel_size[0]
-    # In quantizeml one reserves automatically one bit for the sign, but in akida
-    # this is rather checked during the clipping operations.
-    buffer_bits = layer.buffer_bitwidth + 1
-    name = layer.name
-
-    embedding_params = dict(input_shape=input_shape,
-                            filters=filters,
-                            kernel_size=kernel_size,
-                            buffer_bits=buffer_bits,
-                            name=name)
-    return embedding_params
-
-
-def _parse_additional_layers(layers):
+def _parse_stem_block_layers(block):
     """Parses the quantizeml quantized additional layers of the Stem block and returns the
     params to create the corresponding Akida Stem layer.
 
     Args:
         layers (list): the quantizeml quantized layers of the Stem to convert.
 
     Returns:
         dict: the corresponding akida parameters.
     """
+    # Extract neural layer of the block
+    embedding = block[0]
 
-    cls_layers = []
-    add_pos_emb_layer = None
-    # Get the QuantizedClassToken layer(s) and the optional
-    # QuantizedAddPositionEmbs layer
-    for layer in layers:
-        if isinstance(layer, qlayers.QuantizedClassToken):
-            cls_layers.append(layer)
-        elif isinstance(layer, qlayers.QuantizedAddPositionEmbs):
-            add_pos_emb_layer = layer
-
-    # A block of layers always end with an output Quantizer. Extract it.
-    out_quantizer = getattr(layers[-1], "out_quantizer", False)
-    assert isinstance(out_quantizer, qlayers.OutputQuantizer)
-    output_bits = out_quantizer.bitwidth
+    # Get the QuantizedClassToken layer(s)
+    cls_layers = _get_cls_layers(block)
 
-    num_non_patch_tokens = len(cls_layers)
+    # A block of layers always end with an OutputQuantizer. Extract it.
+    out_quantizer = get_block_out_quantizer(block)
+    assert isinstance(out_quantizer, OutputQuantizer)
 
-    return dict(output_bits=output_bits,
+    return dict(input_shape=embedding.input_shape[1:],
+                filters=embedding.filters,
+                kernel_size=embedding.kernel_size[0],
+                buffer_bits=embedding.buffer_bitwidth + 1,
+                output_bits=out_quantizer.bitwidth,
                 collapse_spatial_dims=True,
-                num_non_patch_tokens=num_non_patch_tokens,
-                add_pos_embs_available=add_pos_emb_layer is not None)
+                num_non_patch_tokens=len(cls_layers),
+                add_pos_embs_available=True,
+                name=embedding.name)
 
 
 def convert_quantized_stem_layers(model_ak, block):
-    """Converts QuantizedDense layer and its variables and adds it to the
+    """Converts stem block layers and their variables and adds them to the
     Akida's model.
 
     Args:
         model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
         block (list): the quantizeml quantized layers of the Stem to convert.
 
     Returns:
-        bool: return False if conversion fails, True otherwise.
+        bool: Returns True for a successful conversion.
     """
-    # Extract neural layer of the block
-    embedding_layer = block[0]
-    # Stem block has at least one embedding layer and an additional layer (QuantizedClassToken
-    # and/or QuantizedAddPosEmbedding). Stem can only be the first layer of the Akida model.
-    if len(block) == 1 or not isinstance(embedding_layer, qlayers.QuantizedConv2D) \
-            or len(model_ak.layers) != 0:
-        return False
-
-    # The embedding layer should be followed by a QuantizedReshape in the Stem
-    next_layer = embedding_layer.outbound_nodes[0].outbound_layer
-    if not isinstance(next_layer, qlayers.QuantizedReshape):
-        return False
-
-    # Parse the Stem embedding layer parameters
-    stem_params = _parse_embedding(embedding_layer)
-    # Stem can handle only 3D or 1D inputs
-    if stem_params["input_shape"][-1] not in [1, 3]:
-        return False
-
-    # Parse additional layers of the Stem
-    additional_params = _parse_additional_layers(block[1:])
-    stem_params.update(additional_params)
+    # Parse the Stem block layers parameters
+    stem_params = _parse_stem_block_layers(block)
 
     layer_ak = Stem(**stem_params)
     model_ak.add(layer_ak)
     _set_stem_variables(layer_ak, block)
     # Get out_quantizer of the block.
     out_quantizer = get_block_out_quantizer(block)
-    # OutputQuantizer is mandatory at the end of the block
-    assert isinstance(out_quantizer, qlayers.OutputQuantizer)
-
     set_output_v2_variables(layer_ak, out_quantizer)
 
     return True
+
+
+class StemBlockConverter(BlockConverter):
+    """Main class that should be used to check if the stem block is compatible to an Akida v2
+    conversion and provides a method to convert it in an equivalent Akida stem layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def __init__(self, block):
+        super().__init__(block)
+        self._stem_additional_checks()
+
+    def convert(self, model_ak):
+        assert len(model_ak.layers) == 0, "Stem layer should be the first model layer."
+        return convert_quantized_stem_layers(model_ak, self._block)
+
+    def _stem_additional_checks(self):
+        embedding = self._block[0]
+        # Get embedding layer input shape without the batch size.
+        input_shape = embedding.input_shape[1:]
+        # Stem handles only square inputs
+        if (input_shape[0] != input_shape[1]):
+            raise ValueError("input should have square spatial dimensions. Receives: "
+                             f"x_size={input_shape[0]} and y_size={input_shape[1]}")
+        # Stem handles only image-like inputs (1-D or 3-D uint8 inputs)
+        if input_shape[-1] not in (1, 3):
+            raise ValueError("Stem layer can only handle image like inputs (i.e 3-D or 1-D input "
+                             f"shape). Received: {embedding.input_shape[1:]}.")
+        # Get the kernel size
+        kernel_size = embedding.kernel_size
+        # Stem handles only square kernels.
+        if (kernel_size[0] != kernel_size[1]):
+            raise ValueError("input should have square kernels. Receives: "
+                             f"k_x={kernel_size[0]} and k_y={kernel_size[1]}")
+        # Stem input size must be a multiple of kernel size.
+        if (input_shape[0] % kernel_size[0] != 0):
+            raise ValueError("Input spatial dimension size must be a multiple of kernel size")
+
+
+# Register the valid stem block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, StemBlockConverter, input_pattern=True)
```

### Comparing `cnn2snn-2.3.6/cnn2snn/quantizeml/weights.py` & `cnn2snn-2.3.7/cnn2snn/quantizeml/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/transforms/__init__.py` & `cnn2snn-2.3.7/cnn2snn/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/transforms/batch_normalization.py` & `cnn2snn-2.3.7/cnn2snn/transforms/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/transforms/clone.py` & `cnn2snn-2.3.7/cnn2snn/transforms/clone.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/transforms/equalization.py` & `cnn2snn-2.3.7/cnn2snn/transforms/equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/transforms/reshape.py` & `cnn2snn-2.3.7/cnn2snn/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/transforms/sequential.py` & `cnn2snn-2.3.7/cnn2snn/transforms/sequential.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/utils.py` & `cnn2snn-2.3.7/cnn2snn/utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn/weights_ops.py` & `cnn2snn-2.3.7/cnn2snn/weights_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/cnn2snn.egg-info/PKG-INFO` & `cnn2snn-2.3.7/cnn2snn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.6
+Version: 2.3.7
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.6/cnn2snn.egg-info/SOURCES.txt` & `cnn2snn-2.3.7/cnn2snn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.6/setup.py` & `cnn2snn-2.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 def get_tf_dep():
   platform_string = platform()
   if 'macOS' in platform_string and 'arm64' in platform_string:
     tf_name = 'tensorflow-macos'
   else:
     tf_name = 'tensorflow'
-  return tf_name + '>=2.10.0'
+  return tf_name + '~=2.10.0'
 
 
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cnn2snn',
-    version='2.3.6',
+    version='2.3.7',
     description='Keras to Akida CNN Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alvaro Moran',
     author_email='amoran@brainchip.com',
     url='https://doc.brainchipinc.com',
     license='Apache 2.0',
     packages=['cnn2snn', 'cnn2snn.transforms', 'cnn2snn.calibration', 'cnn2snn.quantizeml'],
     entry_points={
         'console_scripts': [ 'cnn2snn = cnn2snn.cli:main' ]
     },
     install_requires=[get_tf_dep(), 'keras~=2.10.0',
-        'akida==2.3.6', 'quantizeml~=0.4.1'],
+        'akida==2.3.7', 'quantizeml~=0.4.1'],
 )
```

