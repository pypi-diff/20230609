# Comparing `tmp/xGPR-0.1.1.5.tar.gz` & `tmp/xGPR-0.1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xGPR-0.1.1.5.tar", last modified: Tue Jun  6 04:21:54 2023, max compression
+gzip compressed data, was "xGPR-0.1.1.6.tar", last modified: Thu Jun  8 22:04:04 2023, max compression
```

## Comparing `xGPR-0.1.1.5.tar` & `xGPR-0.1.1.6.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/LICENSE
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/README.md
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/setup.cfg
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.1.5/setup.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-06 04:20:02.000000 xGPR-0.1.1.5/xGPR/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/cg_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/cg_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/cg_toolkit/cg_linear_operators.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/cg_toolkit/cg_tools.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/cg_toolkit/cuda_cg_linear_operators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/constants/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/constants/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/constants/constants.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/data_handling/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/data_handling/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/data_handling/data_handling_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12408 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/data_handling/dataset_builder.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/data_handling/minibatch_data_handler.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/data_handling/offline_data_handling.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6583 2023-06-06 03:33:02.000000 xGPR-0.1.1.5/xGPR/data_handling/online_data_handling.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/fitting_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/fitting_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/fitting_toolkit/ams_grad_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/fitting_toolkit/cg_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.1.5/xGPR/fitting_toolkit/exact_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/kernels/
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/kernels/ARD_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/kernels/ARD_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13106 2023-05-25 01:08:51.000000 xGPR-0.1.1.5/xGPR/kernels/ARD_kernels/mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-05-25 15:24:30.000000 xGPR-0.1.1.5/xGPR/kernels/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/matern.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6970 2023-05-25 01:05:26.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/polynomial.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7948 2023-05-25 01:09:48.000000 xGPR-0.1.1.5/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8337 2023-05-25 01:05:52.000000 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10322 2023-05-25 01:06:23.000000 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/fht_conv1d.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7551 2023-05-25 15:40:52.000000 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/graph_arccos.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7065 2023-05-25 01:07:22.000000 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/graph_polysum.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-05-25 13:27:31.000000 xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/graph_rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.1.5/xGPR/kernels/kernel_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.1.5/xGPR/kernels/srht_compressor.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR/optimizers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/optimizers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/optimizers/bayes_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/optimizers/crude_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/optimizers/lb_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/optimizers/map_loss_bayes_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/optimizers/pure_bayes_optimizer.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/preconditioners/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/preconditioners/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.1.5/xGPR/preconditioners/inter_device_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/preconditioners/rand_nys_constructors.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/preconditioners/rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/preconditioners/tuning_preconditioners.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20803 2023-06-02 19:55:34.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12509 2023-05-25 00:59:46.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14218 2023-06-06 03:20:50.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23069 2023-06-02 19:55:30.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14619 2023-06-06 02:32:10.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
--rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.996810 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.1.5/xGPR/regression_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/xGPR/scoring_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/scoring_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/scoring_toolkit/approximate_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/scoring_toolkit/cho_solvers.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/scoring_toolkit/exact_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/scoring_toolkit/nmll_gradient_tools.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/scoring_toolkit/probe_generators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/xGPR/static_layers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/static_layers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.1.5/xGPR/static_layers/fast_conv.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/xGPR/tuning_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/tuning_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/tuning_toolkit/direct_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/tuning_toolkit/hparam_scoring.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:54.000810 xGPR-0.1.1.5/xGPR/visualization_tools/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.1.5/xGPR/visualization_tools/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.1.5/xGPR/visualization_tools/kernel_xpca.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-06 04:07:57.000000 xGPR-0.1.1.5/xGPR/xGP_Regression.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-06 04:21:53.992810 xGPR-0.1.1.5/xGPR.egg-info/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-06 04:21:53.000000 xGPR-0.1.1.5/xGPR.egg-info/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6956 2023-06-06 04:21:53.000000 xGPR-0.1.1.5/xGPR.egg-info/SOURCES.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-06 04:21:53.000000 xGPR-0.1.1.5/xGPR.egg-info/dependency_links.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-06 04:21:53.000000 xGPR-0.1.1.5/xGPR.egg-info/requires.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-06 04:21:53.000000 xGPR-0.1.1.5/xGPR.egg-info/top_level.txt
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/LICENSE
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/README.md
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/setup.cfg
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.1.6/setup.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.051120 xGPR-0.1.1.6/xGPR/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-08 22:03:12.000000 xGPR-0.1.1.6/xGPR/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.063120 xGPR-0.1.1.6/xGPR/cg_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/cg_linear_operators.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/cg_tools.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.063120 xGPR-0.1.1.6/xGPR/constants/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/constants/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/constants/constants.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.075120 xGPR-0.1.1.6/xGPR/data_handling/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/data_handling_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13221 2023-06-07 22:51:35.000000 xGPR-0.1.1.6/xGPR/data_handling/dataset_builder.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/minibatch_data_handler.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/data_handling/offline_data_handling.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.1.6/xGPR/data_handling/online_data_handling.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.079120 xGPR-0.1.1.6/xGPR/fitting_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/ams_grad_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.079120 xGPR-0.1.1.6/xGPR/kernels/
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.103120 xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13106 2023-05-25 01:08:51.000000 xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-05-25 15:24:30.000000 xGPR-0.1.1.6/xGPR/kernels/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.119120 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/matern.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6970 2023-05-25 01:05:26.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/polynomial.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf_linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7948 2023-05-25 01:09:48.000000 xGPR-0.1.1.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.163120 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8337 2023-05-25 01:05:52.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10322 2023-05-25 01:06:23.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/fht_conv1d.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7551 2023-05-25 15:40:52.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_arccos.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7065 2023-05-25 01:07:22.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_polysum.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-05-25 13:27:31.000000 xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.1.6/xGPR/kernels/kernel_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.1.6/xGPR/kernels/srht_compressor.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.207120 xGPR-0.1.1.6/xGPR/optimizers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/bayes_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/crude_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/lb_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/optimizers/map_loss_bayes_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/optimizers/pure_bayes_optimizer.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.239120 xGPR-0.1.1.6/xGPR/preconditioners/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.1.6/xGPR/preconditioners/inter_device_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_constructors.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/preconditioners/tuning_preconditioners.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.239120 xGPR-0.1.1.6/xGPR/random_feature_generation/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.243120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.243120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.247120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20803 2023-06-02 19:55:34.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12509 2023-05-25 00:59:46.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14218 2023-06-06 03:20:50.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.247120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.247120 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.251120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.251120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.255120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23069 2023-06-02 19:55:30.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14619 2023-06-06 02:32:10.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
+-rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.255120 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.1.6/xGPR/regression_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.259120 xGPR-0.1.1.6/xGPR/scoring_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/cho_solvers.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/exact_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/nmll_gradient_tools.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/scoring_toolkit/probe_generators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.259120 xGPR-0.1.1.6/xGPR/static_layers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/static_layers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.1.6/xGPR/static_layers/fast_conv.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/xGPR/tuning_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/tuning_toolkit/hparam_scoring.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.299120 xGPR-0.1.1.6/xGPR/visualization_tools/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.1.6/xGPR/visualization_tools/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.1.6/xGPR/visualization_tools/kernel_xpca.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-06 04:07:57.000000 xGPR-0.1.1.6/xGPR/xGP_Regression.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-08 22:04:04.051120 xGPR-0.1.1.6/xGPR.egg-info/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6956 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/requires.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-08 22:04:03.000000 xGPR-0.1.1.6/xGPR.egg-info/top_level.txt
```

### Comparing `xGPR-0.1.1.5/LICENSE` & `xGPR-0.1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/PKG-INFO` & `xGPR-0.1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.1.5
+Version: 0.1.1.6
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.1.5/README.md` & `xGPR-0.1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/setup.py` & `xGPR-0.1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/cg_toolkit/cg_linear_operators.py` & `xGPR-0.1.1.6/xGPR/cg_toolkit/cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/cg_toolkit/cg_tools.pyx` & `xGPR-0.1.1.6/xGPR/cg_toolkit/cg_tools.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/cg_toolkit/cuda_cg_linear_operators.py` & `xGPR-0.1.1.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/constants/constants.py` & `xGPR-0.1.1.6/xGPR/constants/constants.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/data_handling/data_handling_baseclass.py` & `xGPR-0.1.1.6/xGPR/data_handling/data_handling_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/data_handling/dataset_builder.py` & `xGPR-0.1.1.6/xGPR/data_handling/dataset_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 """
 import numpy as np
 
 from .online_data_handling import OnlineDataset
 from .offline_data_handling import OfflineDataset
 
 
-def build_online_dataset(xdata, ydata, chunk_size = 2000):
+def build_online_dataset(xdata, ydata, chunk_size = 2000,
+        normalize_y = True):
     """build_online_dataset constructs an OnlineDataset
     object for data stored in memory, after first checking
     that some validity requirements are satisfied.
 
     Args:
         xdata (np.ndarray): A numpy array containing the x-values.
         ydata (np.ndarray): A numpy array containing the y-values.
         chunk_size (int): The maximum size of data chunks that
             will be returned to callers. Limits memory consumption.
             Defaults to 2000.
+        normalize_y (bool): If True, y values are normalized. Generally a
+            good idea, unless you have already selected hyperparameters based
+            on prior knowledge.
 
     Returns:
         dataset (OnlineDataset): An object of class OnlineDataset
             that can be passed to the hyperparameter tuning
             and fitting routines of the model classes.
 
     Raises:
@@ -42,20 +46,21 @@
         raise ValueError("Different number of datapoints in x and y.")
     if np.sum(np.isnan(xdata)) > 0:
         raise ValueError("One or more elements in x is nan!")
     if np.max(xdata) > 1e15 or np.min(xdata) < -1e15:
         raise ValueError("Values > 1e15 or < -1e15 encountered. "
                     "Please rescale your data and check for np.inf.")
 
-    dataset = OnlineDataset(xdata, ydata, chunk_size = chunk_size)
+    dataset = OnlineDataset(xdata, ydata, chunk_size = chunk_size,
+            normalize_y = normalize_y)
     return dataset
 
 
 def build_offline_fixed_vector_dataset(xlist, ylist, chunk_size = 2000,
-        skip_safety_checks = False):
+        normalize_y = True, skip_safety_checks = False):
     """Constructs an OfflineDataset
     object for data stored on disk, after first checking
     that some validity requirements are satisfied. This is
     intended for data that comes in fixed-vector form
     (e.g. tabular data or a sequence alignment).
 
     Args:
@@ -65,14 +70,17 @@
         ylist (list): A list of valid filepaths to .npy numpy
             arrays containing the y-data. These must all be 1d
             arrays. The number of datapoints in each should
             match the corresponding element of xlist.
         chunk_size (int): The maximum size of data chunks that
             will be returned to callers. Limits memory consumption.
             Defaults to 2000.
+        normalize_y (bool): If True, y values are normalized. Generally a
+            good idea, unless you have already selected hyperparameters based
+            on prior knowledge.
         skip_safety_checks (bool): If False, the builder will check
             each input array to make sure it does not contain
             infinite values or nan and that all the input arrays are 2d
             This is important -- if there are unexpected 3d arrays, np.nan,
             etc., this can lead to weird and unexpected results during
             fitting. On the other hand,
             this is a slow step and for a large dataset can take some
@@ -128,22 +136,25 @@
     else:
         xdim = [0,-1]
         for xfile in xlist:
             xshape = _get_array_file_shape(xfile)
             xdim[1] = xshape[1]
             xdim[0] += xshape[0]
 
-    trainy_mean, trainy_std = _get_offline_scaling_factors(ylist)
+    if normalize_y:
+        trainy_mean, trainy_std = _get_offline_scaling_factors(ylist)
+    else:
+        trainy_mean, trainy_std = 0.0, 1.0
     dataset = OfflineDataset(xlist, ylist, tuple(xdim),
                 trainy_mean, trainy_std, chunk_size = chunk_size)
     return dataset
 
 
 def build_offline_sequence_dataset(xlist, ylist, chunk_size = 2000,
-        skip_safety_checks = False):
+        normalize_y = True, skip_safety_checks = False):
     """Constructs an OfflineDataset
     object for data stored on disk, after first checking
     that some validity requirements are satisfied. This is
     intended for data like time series or sequences.
 
     Args:
         xlist (list): A list of valid filepaths to .npy numpy
@@ -154,14 +165,17 @@
         ylist (list): A list of valid filepaths to .npy numpy
             arrays containing the y-data. These must all be 1d
             arrays. The number of datapoints in each should
             match the corresponding element of xlist.
         chunk_size (int): The maximum size of data chunks that
             will be returned to callers. Limits memory consumption.
             Defaults to 2000.
+        normalize_y (bool): If True, y values are normalized. Generally a
+            good idea, unless you have already selected hyperparameters based
+            on prior knowledge.
         skip_safety_checks (bool): If False, the builder will check
             each input array to make sure it does not contain
             infinite values or nan and that all the input arrays are 3d
             This is important -- if there are unexpected 2d arrays, np.nan,
             etc., this can lead to weird and unexpected results during
             fitting. On the other hand,
             this is a slow step and for a large dataset can take some
@@ -219,15 +233,18 @@
         xdim = [0,-1,-1]
         for xfile in xlist:
             xshape = _get_array_file_shape(xfile)
             xdim[1] = xshape[1]
             xdim[2] = xshape[2]
             xdim[0] += xshape[0]
 
-    trainy_mean, trainy_std = _get_offline_scaling_factors(ylist)
+    if normalize_y:
+        trainy_mean, trainy_std = _get_offline_scaling_factors(ylist)
+    else:
+        trainy_mean, trainy_std = 0.0, 1.0
     dataset = OfflineDataset(xlist, ylist, xdim,
                 trainy_mean, trainy_std, chunk_size = chunk_size)
     return dataset
 
 
 def _get_offline_scaling_factors(yfiles):
     """Gets scaling factors (mean and standard deviation)
```

### Comparing `xGPR-0.1.1.5/xGPR/data_handling/minibatch_data_handler.py` & `xGPR-0.1.1.6/xGPR/data_handling/minibatch_data_handler.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/data_handling/offline_data_handling.py` & `xGPR-0.1.1.6/xGPR/data_handling/offline_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/data_handling/online_data_handling.py` & `xGPR-0.1.1.6/xGPR/data_handling/online_data_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,22 @@
             are of size chunk_size. This limits memory consumption
             (by avoiding situations where we try to featurize
             too many datapoints at once).
         pretransformed_ (bool): If True, the data has already been
             "featurized" or transformed and the xfiles do not
             need to be run through the kernel. This can save time
             during fitting if an SSD is available. Default is False.
+        normalize_y (bool): If True, the y-values are normalized.
+            Generally a good idea.
     """
     def __init__(self, xdata, ydata,
                        device = "cpu",
                        chunk_size = 2000,
-                       pretransformed = False):
+                       pretransformed = False,
+                       normalize_y = True):
         """Constructor for the OnlineDataset class.
 
         Args:
             xdata (array): A numpy array containing the x data.
             ydata (array): A numpy array containing the y data.
             device (str): The current device. Must be in ["cpu", "gpu"].
             chunk_size (int): When returning chunks of data, the chunks
@@ -63,17 +66,20 @@
                 during fitting if an SSD is available. Default is False.
         """
         super().__init__(pretransformed, xdata.shape, device, chunk_size)
         if pretransformed:
             raise ValueError("Only offline datasets can be pretransformed.")
         self.xdata_ = xdata
         self.ydata_ = ydata
-        self.trainy_mean_ = np.mean(ydata)
-        self.trainy_std_ = np.std(ydata)
-
+        if normalize_y:
+            self.trainy_mean_ = np.mean(ydata)
+            self.trainy_std_ = np.std(ydata)
+        else:
+            self.trainy_mean_ = 1.0
+            self.trainy_std_ = 1.0
 
     def get_chunked_data(self):
         """A generator that returns the stored data in chunks
         of size chunk_size."""
         for i in range(0, self.xdim_[0], self.chunk_size):
             cutoff = min(i + self.chunk_size, self.xdim_[0])
             xchunk = self.xdata_[i:cutoff,...]
```

### Comparing `xGPR-0.1.1.5/xGPR/fitting_toolkit/ams_grad_toolkit.py` & `xGPR-0.1.1.6/xGPR/fitting_toolkit/ams_grad_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/fitting_toolkit/cg_fitting_toolkit.py` & `xGPR-0.1.1.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/fitting_toolkit/exact_fitting_toolkit.py` & `xGPR-0.1.1.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py` & `xGPR-0.1.1.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/fitting_toolkit/sgd_fitting_toolkit.py` & `xGPR-0.1.1.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/ARD_kernels/mini_ard.py` & `xGPR-0.1.1.6/xGPR/kernels/ARD_kernels/mini_ard.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/__init__.py` & `xGPR-0.1.1.6/xGPR/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/basic_kernels/linear.py` & `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/basic_kernels/matern.py` & `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/matern.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/basic_kernels/polynomial.py` & `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/polynomial.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/basic_kernels/rbf.py` & `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/basic_kernels/rbf_linear.py` & `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/rbf_linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py` & `xGPR-0.1.1.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/conv_feature_extractor.py` & `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/fht_conv1d.py` & `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/fht_conv1d.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/graph_arccos.py` & `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_arccos.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/graph_polysum.py` & `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_polysum.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/convolution_kernels/graph_rbf.py` & `xGPR-0.1.1.6/xGPR/kernels/convolution_kernels/graph_rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/kernel_baseclass.py` & `xGPR-0.1.1.6/xGPR/kernels/kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/kernels/srht_compressor.py` & `xGPR-0.1.1.6/xGPR/kernels/srht_compressor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/optimizers/bayes_grid_optimizer.py` & `xGPR-0.1.1.6/xGPR/optimizers/bayes_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/optimizers/crude_grid_optimizer.py` & `xGPR-0.1.1.6/xGPR/optimizers/crude_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/optimizers/lb_optimizer.py` & `xGPR-0.1.1.6/xGPR/optimizers/lb_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/optimizers/map_loss_bayes_optimizer.py` & `xGPR-0.1.1.6/xGPR/optimizers/map_loss_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/optimizers/pure_bayes_optimizer.py` & `xGPR-0.1.1.6/xGPR/optimizers/pure_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/preconditioners/cuda_rand_nys_preconditioners.py` & `xGPR-0.1.1.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/preconditioners/inter_device_preconditioners.py` & `xGPR-0.1.1.6/xGPR/preconditioners/inter_device_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/preconditioners/rand_nys_constructors.py` & `xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_constructors.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/preconditioners/rand_nys_preconditioners.py` & `xGPR-0.1.1.6/xGPR/preconditioners/rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/preconditioners/tuning_preconditioners.py` & `xGPR-0.1.1.6/xGPR/preconditioners/tuning_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.1.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/regression_baseclass.py` & `xGPR-0.1.1.6/xGPR/regression_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/scoring_toolkit/approximate_nmll_calcs.py` & `xGPR-0.1.1.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/scoring_toolkit/cho_solvers.py` & `xGPR-0.1.1.6/xGPR/scoring_toolkit/cho_solvers.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/scoring_toolkit/exact_nmll_calcs.py` & `xGPR-0.1.1.6/xGPR/scoring_toolkit/exact_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/scoring_toolkit/nmll_gradient_tools.py` & `xGPR-0.1.1.6/xGPR/scoring_toolkit/nmll_gradient_tools.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/scoring_toolkit/probe_generators.py` & `xGPR-0.1.1.6/xGPR/scoring_toolkit/probe_generators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/static_layers/fast_conv.py` & `xGPR-0.1.1.6/xGPR/static_layers/fast_conv.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py` & `xGPR-0.1.1.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/tuning_toolkit/direct_fitting_optimizer.py` & `xGPR-0.1.1.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/tuning_toolkit/hparam_scoring.py` & `xGPR-0.1.1.6/xGPR/tuning_toolkit/hparam_scoring.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/visualization_tools/kernel_xpca.py` & `xGPR-0.1.1.6/xGPR/visualization_tools/kernel_xpca.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR/xGP_Regression.py` & `xGPR-0.1.1.6/xGPR/xGP_Regression.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.1.5/xGPR.egg-info/PKG-INFO` & `xGPR-0.1.1.6/xGPR.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.1.5
+Version: 0.1.1.6
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.1.5/xGPR.egg-info/SOURCES.txt` & `xGPR-0.1.1.6/xGPR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

