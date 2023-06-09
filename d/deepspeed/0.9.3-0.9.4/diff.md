# Comparing `tmp/deepspeed-0.9.3.tar.gz` & `tmp/deepspeed-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepspeed-0.9.3.tar", last modified: Fri Jun  2 22:12:58 2023, max compression
+gzip compressed data, was "deepspeed-0.9.4.tar", last modified: Fri Jun  9 18:43:47 2023, max compression
```

## Comparing `deepspeed-0.9.3.tar` & `deepspeed-0.9.4.tar`

### file list

```diff
@@ -1,638 +1,638 @@
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.3/LICENSE
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.3/MANIFEST.in
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27468 2023-06-02 22:12:58.850620 deepspeed-0.9.3/PKG-INFO
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26538 2023-05-03 17:31:31.000000 deepspeed-0.9.3/README.md
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.490620 deepspeed-0.9.3/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.3/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/cpu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/npu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6385 2023-06-02 22:08:07.000000 deepspeed-0.9.3/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.490620 deepspeed-0.9.3/bin/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/deepspeed
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/deepspeed.pt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/ds
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.3/bin/ds_bench
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.3/bin/ds_elastic
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/ds_report
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/ds_ssh
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.3/bin/dsr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:57.000000 deepspeed-0.9.3/build.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.490620 deepspeed-0.9.3/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.500620 deepspeed-0.9.3/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.500620 deepspeed-0.9.3/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.510620 deepspeed-0.9.3/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.520620 deepspeed-0.9.3/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/cpu/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.520620 deepspeed-0.9.3/csrc/cpu/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/cpu/comm/ccl.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.550620 deepspeed-0.9.3/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.3/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.550620 deepspeed-0.9.3/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.560620 deepspeed-0.9.3/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.580620 deepspeed-0.9.3/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.3/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.3/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.470620 deepspeed-0.9.3/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.580620 deepspeed-0.9.3/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/pointwise_ops.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/rms_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.3/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/deepspeed/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.600620 deepspeed-0.9.3/deepspeed/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/cpu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/npu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6385 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.610620 deepspeed-0.9.3/deepspeed/autotuning/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54184 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/autotuner.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.610620 deepspeed-0.9.3/deepspeed/autotuning/config_templates/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero0.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero1.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero2.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.3/deepspeed/autotuning/config_templates/template_zero3.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5943 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.610620 deepspeed-0.9.3/deepspeed/autotuning/tuner/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2754 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/base_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/cost_model.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/index_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/model_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/autotuning/tuner/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15053 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/autotuning/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.620620 deepspeed-0.9.3/deepspeed/checkpoint/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/checkpoint/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12012 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/checkpoint/deepspeed_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/reshape_3d_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/reshape_meg_2d.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/reshape_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/universal_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2534 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/checkpoint/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/checkpoint/zero_checkpoint.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.630620 deepspeed-0.9.3/deepspeed/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/comm/backend.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2248 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/ccl.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27788 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/comm/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1276 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      259 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/comm/reduce_op.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13128 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/comm/torch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/comm/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.630620 deepspeed-0.9.3/deepspeed/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36033 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11886 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/compress.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25067 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5569 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14637 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8161 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7818 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/compression/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/elasticity/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4703 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/elasticity/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2454 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/elasticity/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/elastic_agent.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/elasticity.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/elasticity/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4804 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/env_report.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/git_version_info.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed/git_version_info_installed.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9501 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/inference/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    31552 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/inference/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/launcher/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/launcher/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      375 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14601 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/launch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16568 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/multinode_runner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24125 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/launcher/runner.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/model_implementations/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/diffusers/vae.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.640620 deepspeed-0.9.3/deepspeed/model_implementations/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/features/cuda_graph.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.650620 deepspeed-0.9.3/deepspeed/model_implementations/transformers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/clip_encoder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8247 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.660620 deepspeed-0.9.3/deepspeed/module_inject/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4998 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/auto_tp.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.670620 deepspeed-0.9.3/deepspeed/module_inject/containers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      893 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12798 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/base_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3690 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5289 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2822 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/clip.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3109 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/distil_bert.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.670620 deepspeed-0.9.3/deepspeed/module_inject/containers/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      275 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4788 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/gated_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7273 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4129 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1200 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2930 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/meta_tensor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7120 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/features/split_qkv.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2221 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gpt2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4768 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gptj.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5002 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gptneo.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5571 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/gptneox.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5797 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/llama.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5017 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3936 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6599 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/containers/vae.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/inject.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4592 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/layers.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14597 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/load_checkpoint.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/module_inject/module_quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8259 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    44312 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/replace_module.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      989 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/replace_policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1762 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/module_inject/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.670620 deepspeed-0.9.3/deepspeed/moe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/experts.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/mappings.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/sharded_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/moe/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/monitor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2485 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/monitor/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/csv_monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/tensorboard.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/monitor/wandb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/nebula/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/nebula/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/nebula/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/nebula/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/ops/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.680620 deepspeed-0.9.3/deepspeed/ops/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adagrad/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adagrad/cpu_adagrad.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/adam/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adam/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8544 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/adam/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8767 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/adam/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/adam/multi_tensor_apply.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/aio/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/aio/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.690620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.700620 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_test/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_test/single_process_config.json
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.700620 deepspeed-0.9.3/deepspeed/ops/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/cpu/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.700620 deepspeed-0.9.3/deepspeed/ops/csrc/cpu/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/cpu/comm/ccl.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.710620 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.480620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.720620 deepspeed-0.9.3/deepspeed/ops/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/lamb/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/lamb/fused_lamb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.730620 deepspeed-0.9.3/deepspeed/ops/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29590 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/builder.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1238 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/no_impl.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/quantizer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/quantizer/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/quantizer/quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/random_ltd/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4902 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/random_ltd/dropping_utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.740620 deepspeed-0.9.3/deepspeed/ops/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/matmul.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_attention_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_self_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42463 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparsity_config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.750620 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/matmul.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.750620 deepspeed-0.9.3/deepspeed/ops/transformer/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.750620 deepspeed-0.9.3/deepspeed/ops/transformer/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/bias_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5725 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9830 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4853 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13853 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6212 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18454 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/moe_inference.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      536 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1496 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1404 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4472 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3129 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2660 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/residual_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2460 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2131 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1447 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/inference/triton_ops.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/ops/transformer/transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/pipe/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/profiling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/profiling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1959 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/profiling/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1243 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/profiling/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.760620 deepspeed-0.9.3/deepspeed/profiling/flops_profiler/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/profiling/flops_profiler/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47248 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/profiling/flops_profiler/profiler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.780620 deepspeed-0.9.3/deepspeed/runtime/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.780620 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/checkpointing.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.3/deepspeed/runtime/bf16_optimizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.780620 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      653 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4981 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.790620 deepspeed-0.9.3/deepspeed/runtime/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/coalesced_collectives.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/mpi.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/comm/nccl.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.790620 deepspeed-0.9.3/deepspeed/runtime/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/compression/cupy.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39863 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/config_utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12971 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.790620 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25023 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/dataloader.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/eigenvalue.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   155145 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/fp16/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/fused_optimizer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11492 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/loss_scaler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.800620 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/zoadam.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/fp16/unfused_optimizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21045 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/hybrid_engine.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/lr_schedules.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.810620 deepspeed-0.9.3/deepspeed/runtime/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56845 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/module.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/p2p.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/schedule.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/pipe/topology.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/progressive_layer_drop.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/sparse_tensor.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/state_dict_factory.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.820620 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/aio_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/async_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/optimizer_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/swap_tensor/utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35805 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/weight_quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.830620 deepspeed-0.9.3/deepspeed/runtime/zero/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/contiguous_memory_allocator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/linear.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21571 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/mics.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/mics_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/offload_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22194 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/parameter_offload.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    72665 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/partition_parameters.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22356 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/partitioned_param_coordinator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   114250 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/stage3.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110843 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/runtime/zero/stage_1_and_2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/test.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/runtime/zero/tiling.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/runtime/zero/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.840620 deepspeed-0.9.3/deepspeed/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      751 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/comms_logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/debug.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/exceptions.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/groups.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/init_on_device.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/mixed_precision_linkage.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5158 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/numa.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/nvtx.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.3/deepspeed/utils/tensor_fragment.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     9477 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/timer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      434 2023-06-02 22:08:07.000000 deepspeed-0.9.3/deepspeed/utils/types.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.3/deepspeed/utils/zero_to_fp32.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.590620 deepspeed-0.9.3/deepspeed.egg-info/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27468 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/PKG-INFO
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21258 2023-06-02 22:12:58.000000 deepspeed-0.9.3/deepspeed.egg-info/SOURCES.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/dependency_links.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/entry_points.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1146 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/requires.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-06-02 22:12:57.000000 deepspeed-0.9.3/deepspeed.egg-info/top_level.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29590 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/builder.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/op_builder/cpu/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1238 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/cpu/no_impl.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.3/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.3/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.3/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-02 22:12:58.850620 deepspeed-0.9.3/requirements/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-1bit-mpi.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-autotuning-ml.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-autotuning.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       28 2023-06-02 22:08:07.000000 deepspeed-0.9.3/requirements/requirements-cpu.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.3/requirements/requirements-dev.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.3/requirements/requirements-inf.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.3/requirements/requirements-readthedocs.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.3/requirements/requirements-sd.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.3/requirements/requirements-sparse_attn.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       25 2023-06-02 22:08:07.000000 deepspeed-0.9.3/requirements/requirements-sparse_pruning.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.3/requirements/requirements.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-06-02 22:12:58.850620 deepspeed-0.9.3/setup.cfg
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11424 2023-06-02 22:08:07.000000 deepspeed-0.9.3/setup.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-05-03 17:31:59.000000 deepspeed-0.9.3/version.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.806864 deepspeed-0.9.4/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.4/LICENSE
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.4/MANIFEST.in
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27751 2023-06-09 18:43:47.806864 deepspeed-0.9.4/PKG-INFO
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26821 2023-06-09 18:33:23.000000 deepspeed-0.9.4/README.md
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.4/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/cpu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/npu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6791 2023-06-09 18:33:23.000000 deepspeed-0.9.4/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/bin/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/deepspeed
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/deepspeed.pt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/ds
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.4/bin/ds_bench
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.4/bin/ds_elastic
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/ds_report
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/ds_ssh
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/dsr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:46.000000 deepspeed-0.9.4/build.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.254364 deepspeed-0.9.4/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.286864 deepspeed-0.9.4/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.297697 deepspeed-0.9.4/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.297697 deepspeed-0.9.4/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/cpu/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.297697 deepspeed-0.9.4/csrc/cpu/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/cpu/comm/ccl.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.330197 deepspeed-0.9.4/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.4/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.341030 deepspeed-0.9.4/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.341030 deepspeed-0.9.4/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.373530 deepspeed-0.9.4/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.384364 deepspeed-0.9.4/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/pointwise_ops.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/rms_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/deepspeed/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/deepspeed/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/cpu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/npu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6791 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.406030 deepspeed-0.9.4/deepspeed/autotuning/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54184 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/autotuner.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.406030 deepspeed-0.9.4/deepspeed/autotuning/config_templates/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero0.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero1.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero2.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero3.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5943 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.416864 deepspeed-0.9.4/deepspeed/autotuning/tuner/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2754 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/base_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/cost_model.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/index_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/model_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15053 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.427697 deepspeed-0.9.4/deepspeed/checkpoint/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/checkpoint/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12012 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/checkpoint/deepspeed_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/reshape_3d_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/reshape_meg_2d.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/reshape_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/universal_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2534 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/checkpoint/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/zero_checkpoint.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.438530 deepspeed-0.9.4/deepspeed/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/comm/backend.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2248 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/ccl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27788 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/comm/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1276 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      259 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/reduce_op.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13416 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/comm/torch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/comm/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.460197 deepspeed-0.9.4/deepspeed/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36033 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11886 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/compress.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25067 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5569 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14637 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8161 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7818 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.460197 deepspeed-0.9.4/deepspeed/elasticity/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4703 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/elasticity/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2454 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/elasticity/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/elastic_agent.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/elasticity.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4804 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/env_report.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/git_version_info.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed/git_version_info_installed.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.471030 deepspeed-0.9.4/deepspeed/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9501 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/inference/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    31552 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/inference/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.471030 deepspeed-0.9.4/deepspeed/launcher/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/launcher/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      375 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/launcher/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14654 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/launcher/launch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16568 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/launcher/multinode_runner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24146 2023-06-09 18:38:25.000000 deepspeed-0.9.4/deepspeed/launcher/runner.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.471030 deepspeed-0.9.4/deepspeed/model_implementations/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.481864 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/vae.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.481864 deepspeed-0.9.4/deepspeed/model_implementations/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/features/cuda_graph.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.492697 deepspeed-0.9.4/deepspeed/model_implementations/transformers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/clip_encoder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8247 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.503530 deepspeed-0.9.4/deepspeed/module_inject/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4998 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/auto_tp.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.514364 deepspeed-0.9.4/deepspeed/module_inject/containers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      893 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13091 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/base_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3690 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5289 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2822 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/clip.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3109 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/distil_bert.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.525197 deepspeed-0.9.4/deepspeed/module_inject/containers/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      275 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4788 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/gated_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7273 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4129 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1200 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2930 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/meta_tensor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7136 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/split_qkv.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2221 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gpt2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4768 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gptj.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5002 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gptneo.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5571 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gptneox.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5797 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/llama.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5017 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3936 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6599 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/vae.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/inject.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4592 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/layers.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14597 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/load_checkpoint.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/module_quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8259 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    44312 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/replace_module.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      989 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/replace_policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1762 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.525197 deepspeed-0.9.4/deepspeed/moe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/experts.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/mappings.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/sharded_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.525197 deepspeed-0.9.4/deepspeed/monitor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2485 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/monitor/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/csv_monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/tensorboard.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/wandb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.536030 deepspeed-0.9.4/deepspeed/nebula/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/nebula/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/nebula/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/nebula/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.536030 deepspeed-0.9.4/deepspeed/ops/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.536030 deepspeed-0.9.4/deepspeed/ops/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adagrad/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adagrad/cpu_adagrad.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/adam/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adam/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8544 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/adam/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8767 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/adam/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adam/multi_tensor_apply.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/aio/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/aio/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_test/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_test/single_process_config.json
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/cpu/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/cpu/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/cpu/comm/ccl.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.568530 deepspeed-0.9.4/deepspeed/ops/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.568530 deepspeed-0.9.4/deepspeed/ops/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.590197 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.590197 deepspeed-0.9.4/deepspeed/ops/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.590197 deepspeed-0.9.4/deepspeed/ops/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/lamb/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/lamb/fused_lamb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.601030 deepspeed-0.9.4/deepspeed/ops/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29637 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/builder.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.611864 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1224 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/no_impl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.611864 deepspeed-0.9.4/deepspeed/ops/quantizer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/quantizer/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/quantizer/quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.611864 deepspeed-0.9.4/deepspeed/ops/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/random_ltd/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4902 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/random_ltd/dropping_utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.622697 deepspeed-0.9.4/deepspeed/ops/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/matmul.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_attention_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_self_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42463 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparsity_config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.633530 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/matmul.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.633530 deepspeed-0.9.4/deepspeed/ops/transformer/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.644364 deepspeed-0.9.4/deepspeed/ops/transformer/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/bias_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5725 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9830 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4853 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13853 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6212 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18454 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/moe_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      536 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1496 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1404 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/linear.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4472 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3129 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2660 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/residual_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2460 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2131 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1447 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/triton_ops.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/pipe/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/profiling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/profiling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1959 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/profiling/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1243 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/profiling/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/profiling/flops_profiler/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/profiling/flops_profiler/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47248 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/profiling/flops_profiler/profiler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.687697 deepspeed-0.9.4/deepspeed/runtime/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.698530 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/checkpointing.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/runtime/bf16_optimizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.698530 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      653 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4975 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.709364 deepspeed-0.9.4/deepspeed/runtime/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/coalesced_collectives.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/mpi.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/nccl.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.709364 deepspeed-0.9.4/deepspeed/runtime/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/compression/cupy.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39863 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/config_utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12971 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.709364 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.720197 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.720197 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25023 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/dataloader.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/eigenvalue.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   155219 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.731030 deepspeed-0.9.4/deepspeed/runtime/fp16/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/fused_optimizer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11492 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/loss_scaler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.741864 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/zoadam.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/unfused_optimizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21045 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/hybrid_engine.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/lr_schedules.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.752697 deepspeed-0.9.4/deepspeed/runtime/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56845 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/module.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/p2p.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/schedule.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/topology.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/progressive_layer_drop.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/sparse_tensor.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/state_dict_factory.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.763530 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/aio_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/async_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/optimizer_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35805 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/weight_quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.785197 deepspeed-0.9.4/deepspeed/runtime/zero/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/contiguous_memory_allocator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/linear.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21984 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/mics.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/mics_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/offload_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22194 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/zero/parameter_offload.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    73213 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/partition_parameters.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22674 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/partitioned_param_coordinator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   115761 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/stage3.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110843 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/zero/stage_1_and_2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/test.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/tiling.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.796030 deepspeed-0.9.4/deepspeed/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      751 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/comms_logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/debug.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/exceptions.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/groups.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/init_on_device.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/mixed_precision_linkage.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5158 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/numa.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/nvtx.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/tensor_fragment.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     9477 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/timer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      434 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/types.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/utils/zero_to_fp32.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/deepspeed.egg-info/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27751 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/PKG-INFO
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21258 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/entry_points.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1146 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/requires.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/top_level.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.796030 deepspeed-0.9.4/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29637 2023-06-09 18:33:23.000000 deepspeed-0.9.4/op_builder/builder.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.796030 deepspeed-0.9.4/op_builder/cpu/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/cpu/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1224 2023-06-09 18:33:23.000000 deepspeed-0.9.4/op_builder/cpu/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/cpu/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/cpu/no_impl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.4/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.806864 deepspeed-0.9.4/requirements/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-1bit-mpi.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-autotuning-ml.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-autotuning.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       28 2023-06-02 22:08:07.000000 deepspeed-0.9.4/requirements/requirements-cpu.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.4/requirements/requirements-dev.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.4/requirements/requirements-inf.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.4/requirements/requirements-readthedocs.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.4/requirements/requirements-sd.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-sparse_attn.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       25 2023-06-02 22:08:07.000000 deepspeed-0.9.4/requirements/requirements-sparse_pruning.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.4/requirements/requirements.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-06-09 18:43:47.806864 deepspeed-0.9.4/setup.cfg
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11424 2023-06-02 22:08:07.000000 deepspeed-0.9.4/setup.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-06-02 22:13:07.000000 deepspeed-0.9.4/version.txt
```

### Comparing `deepspeed-0.9.3/LICENSE` & `deepspeed-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/PKG-INFO` & `deepspeed-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.3
+Version: 0.9.4
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -249,14 +249,15 @@
 14. Reza Yazdani Aminabadi, Samyam Rajbhandari, Minjia Zhang, Ammar Ahmad Awan, Cheng Li, Du Li, Elton Zheng, Jeff Rasley, Shaden Smith, Olatunji Ruwase, Yuxiong He. (2022) DeepSpeed Inference: Enabling Efficient Inference of Transformer Models at Unprecedented Scale. [arXiv:2207.00032](https://arxiv.org/abs/2207.00032) and [SC 2022](https://dl.acm.org/doi/abs/10.5555/3571885.3571946).
 15. Zhewei Yao, Xiaoxia Wu, Conglong Li, Connor Holmes, Minjia Zhang, Cheng Li, Yuxiong He. (2022) Random-LTD: Random and Layerwise Token Dropping Brings Efficient Training for Large-scale Transformers. [arXiv:2211.11586](https://arxiv.org/abs/2211.11586).
 16. Conglong Li, Zhewei Yao, Xiaoxia Wu, Minjia Zhang, Yuxiong He. (2022) DeepSpeed Data Efficiency: Improving Deep Learning Model Quality and Training Efficiency via Efficient Data Sampling and Routing. [arXiv:2212.03597](https://arxiv.org/abs/2212.03597).
 17. Xiaoxia Wu, Cheng Li, Reza Yazdani Aminabadi, Zhewei Yao, Yuxiong He. (2023) Understanding INT4 Quantization for Transformer Models: Latency Speedup, Composability, and Failure Cases. [arXiv:2301.12017](https://arxiv.org/abs/2301.12017).
 18. Syed Zawad, Cheng Li, Zhewei Yao, Elton Zheng, Yuxiong He, Feng Yan. (2023) DySR: Adaptive Super-Resolution via Algorithm and System Co-design. [ICLR:2023](https://openreview.net/forum?id=Pgtn4l6eKjv).
 19. Sheng Shen, Zhewei Yao, Chunyuan Li, Trevor Darrell, Kurt Keutzer, Yuxiong He. (2023) Scaling Vision-Language Models with Sparse Mixture of Experts. [arXiv:2303.07226](https://arxiv.org/abs/2303.07226).
 20. Quentin Anthony, Ammar Ahmad Awan, Jeff Rasley, Yuxiong He, Aamir Shafi, Mustafa Abduljabbar, Hari Subramoni, Dhabaleswar Panda. (2023) MCR-DL: Mix-and-Match Communication Runtime for Deep Learning [arXiv:2303.08374](https://arxiv.org/abs/2303.08374) and will appear at IPDPS 2023.
+21. Siddharth Singh, Olatunji Ruwase, Ammar Ahmad Awan, Samyam Rajbhandari, Yuxiong He, Abhinav Bhatele. (2023) A Hybrid Tensor-Expert-Data Parallelism Approach to Optimize Mixture-of-Experts Training [arXiv:2303.06318](https://arxiv.org/abs/2303.06318) and will appear at ICS 2023.
 
 
 # Videos
 1. DeepSpeed KDD 2020 Tutorial
     1. [Overview](https://www.youtube.com/watch?v=CaseqC45DNc&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=29)
     2. [ZeRO + large model training](https://www.youtube.com/watch?v=y4_bCiAsIAk&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=28)
     3. [17B T-NLG demo](https://www.youtube.com/watch?v=9V-ZbP92drg&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=27)
```

### Comparing `deepspeed-0.9.3/README.md` & `deepspeed-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
 14. Reza Yazdani Aminabadi, Samyam Rajbhandari, Minjia Zhang, Ammar Ahmad Awan, Cheng Li, Du Li, Elton Zheng, Jeff Rasley, Shaden Smith, Olatunji Ruwase, Yuxiong He. (2022) DeepSpeed Inference: Enabling Efficient Inference of Transformer Models at Unprecedented Scale. [arXiv:2207.00032](https://arxiv.org/abs/2207.00032) and [SC 2022](https://dl.acm.org/doi/abs/10.5555/3571885.3571946).
 15. Zhewei Yao, Xiaoxia Wu, Conglong Li, Connor Holmes, Minjia Zhang, Cheng Li, Yuxiong He. (2022) Random-LTD: Random and Layerwise Token Dropping Brings Efficient Training for Large-scale Transformers. [arXiv:2211.11586](https://arxiv.org/abs/2211.11586).
 16. Conglong Li, Zhewei Yao, Xiaoxia Wu, Minjia Zhang, Yuxiong He. (2022) DeepSpeed Data Efficiency: Improving Deep Learning Model Quality and Training Efficiency via Efficient Data Sampling and Routing. [arXiv:2212.03597](https://arxiv.org/abs/2212.03597).
 17. Xiaoxia Wu, Cheng Li, Reza Yazdani Aminabadi, Zhewei Yao, Yuxiong He. (2023) Understanding INT4 Quantization for Transformer Models: Latency Speedup, Composability, and Failure Cases. [arXiv:2301.12017](https://arxiv.org/abs/2301.12017).
 18. Syed Zawad, Cheng Li, Zhewei Yao, Elton Zheng, Yuxiong He, Feng Yan. (2023) DySR: Adaptive Super-Resolution via Algorithm and System Co-design. [ICLR:2023](https://openreview.net/forum?id=Pgtn4l6eKjv).
 19. Sheng Shen, Zhewei Yao, Chunyuan Li, Trevor Darrell, Kurt Keutzer, Yuxiong He. (2023) Scaling Vision-Language Models with Sparse Mixture of Experts. [arXiv:2303.07226](https://arxiv.org/abs/2303.07226).
 20. Quentin Anthony, Ammar Ahmad Awan, Jeff Rasley, Yuxiong He, Aamir Shafi, Mustafa Abduljabbar, Hari Subramoni, Dhabaleswar Panda. (2023) MCR-DL: Mix-and-Match Communication Runtime for Deep Learning [arXiv:2303.08374](https://arxiv.org/abs/2303.08374) and will appear at IPDPS 2023.
+21. Siddharth Singh, Olatunji Ruwase, Ammar Ahmad Awan, Samyam Rajbhandari, Yuxiong He, Abhinav Bhatele. (2023) A Hybrid Tensor-Expert-Data Parallelism Approach to Optimize Mixture-of-Experts Training [arXiv:2303.06318](https://arxiv.org/abs/2303.06318) and will appear at ICS 2023.
 
 
 # Videos
 1. DeepSpeed KDD 2020 Tutorial
     1. [Overview](https://www.youtube.com/watch?v=CaseqC45DNc&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=29)
     2. [ZeRO + large model training](https://www.youtube.com/watch?v=y4_bCiAsIAk&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=28)
     3. [17B T-NLG demo](https://www.youtube.com/watch?v=9V-ZbP92drg&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=27)
```

### Comparing `deepspeed-0.9.3/accelerator/abstract_accelerator.py` & `deepspeed-0.9.4/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/accelerator/cpu_accelerator.py` & `deepspeed-0.9.4/accelerator/cpu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/accelerator/cuda_accelerator.py` & `deepspeed-0.9.4/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/accelerator/npu_accelerator.py` & `deepspeed-0.9.4/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/accelerator/real_accelerator.py` & `deepspeed-0.9.4/accelerator/real_accelerator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 import os
 
 try:
+    # Importing logger currently requires that torch is installed, hence the try...except
+    # TODO: Remove logger dependency on torch.
+    from deepspeed.utils import logger as accel_logger
+except ImportError as e:
+    accel_logger = None
+
+try:
     from accelerator.abstract_accelerator import DeepSpeedAccelerator as dsa1
 except ImportError as e:
     dsa1 = None
 try:
     from deepspeed.accelerator.abstract_accelerator import DeepSpeedAccelerator as dsa2
 except ImportError as e:
     dsa2 = None
@@ -68,20 +75,20 @@
     # 2. If no override, detect which accelerator to use automatically
     if accelerator_name == None:
         try:
             from intel_extension_for_deepspeed import XPU_Accelerator  # noqa: F401,F811
             accelerator_name = 'xpu'
         except ImportError as e:
             # We need a way to choose between CUDA_Accelerator and CPU_Accelerator
-            # Currently we detect whether intel_etension_for_pytorch is installed
-            # in the environment and use CPU_Accelerator if the answewr is True.
+            # Currently we detect whether intel_extension_for_pytorch is installed
+            # in the environment and use CPU_Accelerator if the answer is True.
             # An alternative might be detect whether CUDA device is installed on
             # the system but this comes with two pitfalls:
             # 1. the system may not have torch pre-installed, so
-            #    get_accelerator().is_avaiable() may not work.
+            #    get_accelerator().is_available() may not work.
             # 2. Some scenario like install on login node (without CUDA device)
             #    and run on compute node (with CUDA device) may cause mismatch
             #    between installation time and runtime.
             try:
                 import intel_extension_for_pytorch  # noqa: F401,F811
                 accelerator_name = 'cpu'
             except ImportError as e:
@@ -95,56 +102,58 @@
     elif accelerator_name == 'cpu':
         from .cpu_accelerator import CPU_Accelerator
         ds_accelerator = CPU_Accelerator()
     elif accelerator_name == 'xpu':
         # XPU_Accelerator is already imported in detection stage
         ds_accelerator = XPU_Accelerator()
     _validate_accelerator(ds_accelerator)
-    print(f"Setting ds_accelerator to {ds_accelerator._name} ({ds_set_method})")
+    if accel_logger is not None:
+        accel_logger.info(f"Setting ds_accelerator to {ds_accelerator._name} ({ds_set_method})")
     return ds_accelerator
 
 
 def set_accelerator(accel_obj):
     global ds_accelerator
     _validate_accelerator(accel_obj)
-    print(f"Setting ds_accelerator to {accel_obj._name} (model specified)")
+    if accel_logger is not None:
+        accel_logger.info(f"Setting ds_accelerator to {accel_obj._name} (model specified)")
     ds_accelerator = accel_obj
 
 
 '''
 -----------[code] test_get.py -----------
 from deepspeed.accelerator import get_accelerator
 my_accelerator = get_accelerator()
-print(f'{my_accelerator._name=}')
-print(f'{my_accelerator._communication_backend=}')
-print(f'{my_accelerator.HalfTensor().device=}')
-print(f'{my_accelerator.total_memory()=}')
+logger.info(f'{my_accelerator._name=}')
+logger.info(f'{my_accelerator._communication_backend=}')
+logger.info(f'{my_accelerator.HalfTensor().device=}')
+logger.info(f'{my_accelerator.total_memory()=}')
 -----------[code] test_get.py -----------
 
 ---[output] python test_get.py---------
 my_accelerator.name()='cuda'
 my_accelerator.communication_backend='nccl'
 my_accelerator.HalfTensor().device=device(type='cuda', index=0)
 my_accelerator.total_memory()=34089730048
 ---[output] python test_get.py---------
 
 **************************************************************************
 -----------[code] test_set.py -----------
 from deepspeed.accelerator.cuda_accelerator import CUDA_Accelerator
 cu_accel = CUDA_Accelerator()
-print(f'{id(cu_accel)=}')
+logger.info(f'{id(cu_accel)=}')
 from deepspeed.accelerator import set_accelerator, get_accelerator
 set_accelerator(cu_accel)
 
 my_accelerator = get_accelerator()
-print(f'{id(my_accelerator)=}')
-print(f'{my_accelerator._name=}')
-print(f'{my_accelerator._communication_backend=}')
-print(f'{my_accelerator.HalfTensor().device=}')
-print(f'{my_accelerator.total_memory()=}')
+logger.info(f'{id(my_accelerator)=}')
+logger.info(f'{my_accelerator._name=}')
+logger.info(f'{my_accelerator._communication_backend=}')
+logger.info(f'{my_accelerator.HalfTensor().device=}')
+logger.info(f'{my_accelerator.total_memory()=}')
 -----------[code] test_set.py -----------
 
 
 ---[output] python test_set.py---------
 id(cu_accel)=139648165478304
 my_accelerator=<deepspeed.accelerator.cuda_accelerator.CUDA_Accelerator object at 0x7f025f4bffa0>
 my_accelerator.name='cuda'
```

### Comparing `deepspeed-0.9.3/bin/ds_bench` & `deepspeed-0.9.4/bin/ds_bench`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/bin/ds_elastic` & `deepspeed-0.9.4/bin/ds_elastic`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/bin/ds_ssh` & `deepspeed-0.9.4/bin/ds_ssh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.4/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.4/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.4/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.4/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.4/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.4/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.4/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/cpu/comm/ccl.cpp` & `deepspeed-0.9.4/csrc/cpu/comm/ccl.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/StopWatch.h` & `deepspeed-0.9.4/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/Timer.h` & `deepspeed-0.9.4/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/context.h` & `deepspeed-0.9.4/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/conversion_utils.h` & `deepspeed-0.9.4/csrc/includes/conversion_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.4/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/cpu_adam.h` & `deepspeed-0.9.4/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.4/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.4/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.4/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/dropout.h` & `deepspeed-0.9.4/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.4/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.4/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/feed_forward.h` & `deepspeed-0.9.4/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/gelu.h` & `deepspeed-0.9.4/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/gemm_test.h` & `deepspeed-0.9.4/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/general_kernels.h` & `deepspeed-0.9.4/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.4/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/normalize_layer.h` & `deepspeed-0.9.4/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/quantization.h` & `deepspeed-0.9.4/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/quantization_utils.h` & `deepspeed-0.9.4/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/reduction_utils.h` & `deepspeed-0.9.4/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/simd.h` & `deepspeed-0.9.4/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/softmax.h` & `deepspeed-0.9.4/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.4/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/includes/type_shim.h` & `deepspeed-0.9.4/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/quantization/dequantize.cu` & `deepspeed-0.9.4/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.4/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.4/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/quantization/quantize.cu` & `deepspeed-0.9.4/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.4/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.4/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.4/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.4/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.4/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.4/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.4/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.4/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.4/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.4/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.4/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.4/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.4/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/dequantize.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/pointwise_ops.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/pointwise_ops.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/relu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/rms_norm.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/softmax.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.4/csrc/transformer/inference/csrc/transform.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.4/csrc/transformer/inference/includes/inference_context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.4/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.4/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.4/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.4/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/__init__.py` & `deepspeed-0.9.4/deepspeed/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/accelerator/abstract_accelerator.py` & `deepspeed-0.9.4/deepspeed/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/accelerator/cpu_accelerator.py` & `deepspeed-0.9.4/deepspeed/accelerator/cpu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/accelerator/cuda_accelerator.py` & `deepspeed-0.9.4/deepspeed/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/accelerator/npu_accelerator.py` & `deepspeed-0.9.4/deepspeed/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/accelerator/real_accelerator.py` & `deepspeed-0.9.4/deepspeed/accelerator/real_accelerator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 import os
 
 try:
+    # Importing logger currently requires that torch is installed, hence the try...except
+    # TODO: Remove logger dependency on torch.
+    from deepspeed.utils import logger as accel_logger
+except ImportError as e:
+    accel_logger = None
+
+try:
     from accelerator.abstract_accelerator import DeepSpeedAccelerator as dsa1
 except ImportError as e:
     dsa1 = None
 try:
     from deepspeed.accelerator.abstract_accelerator import DeepSpeedAccelerator as dsa2
 except ImportError as e:
     dsa2 = None
@@ -68,20 +75,20 @@
     # 2. If no override, detect which accelerator to use automatically
     if accelerator_name == None:
         try:
             from intel_extension_for_deepspeed import XPU_Accelerator  # noqa: F401,F811
             accelerator_name = 'xpu'
         except ImportError as e:
             # We need a way to choose between CUDA_Accelerator and CPU_Accelerator
-            # Currently we detect whether intel_etension_for_pytorch is installed
-            # in the environment and use CPU_Accelerator if the answewr is True.
+            # Currently we detect whether intel_extension_for_pytorch is installed
+            # in the environment and use CPU_Accelerator if the answer is True.
             # An alternative might be detect whether CUDA device is installed on
             # the system but this comes with two pitfalls:
             # 1. the system may not have torch pre-installed, so
-            #    get_accelerator().is_avaiable() may not work.
+            #    get_accelerator().is_available() may not work.
             # 2. Some scenario like install on login node (without CUDA device)
             #    and run on compute node (with CUDA device) may cause mismatch
             #    between installation time and runtime.
             try:
                 import intel_extension_for_pytorch  # noqa: F401,F811
                 accelerator_name = 'cpu'
             except ImportError as e:
@@ -95,56 +102,58 @@
     elif accelerator_name == 'cpu':
         from .cpu_accelerator import CPU_Accelerator
         ds_accelerator = CPU_Accelerator()
     elif accelerator_name == 'xpu':
         # XPU_Accelerator is already imported in detection stage
         ds_accelerator = XPU_Accelerator()
     _validate_accelerator(ds_accelerator)
-    print(f"Setting ds_accelerator to {ds_accelerator._name} ({ds_set_method})")
+    if accel_logger is not None:
+        accel_logger.info(f"Setting ds_accelerator to {ds_accelerator._name} ({ds_set_method})")
     return ds_accelerator
 
 
 def set_accelerator(accel_obj):
     global ds_accelerator
     _validate_accelerator(accel_obj)
-    print(f"Setting ds_accelerator to {accel_obj._name} (model specified)")
+    if accel_logger is not None:
+        accel_logger.info(f"Setting ds_accelerator to {accel_obj._name} (model specified)")
     ds_accelerator = accel_obj
 
 
 '''
 -----------[code] test_get.py -----------
 from deepspeed.accelerator import get_accelerator
 my_accelerator = get_accelerator()
-print(f'{my_accelerator._name=}')
-print(f'{my_accelerator._communication_backend=}')
-print(f'{my_accelerator.HalfTensor().device=}')
-print(f'{my_accelerator.total_memory()=}')
+logger.info(f'{my_accelerator._name=}')
+logger.info(f'{my_accelerator._communication_backend=}')
+logger.info(f'{my_accelerator.HalfTensor().device=}')
+logger.info(f'{my_accelerator.total_memory()=}')
 -----------[code] test_get.py -----------
 
 ---[output] python test_get.py---------
 my_accelerator.name()='cuda'
 my_accelerator.communication_backend='nccl'
 my_accelerator.HalfTensor().device=device(type='cuda', index=0)
 my_accelerator.total_memory()=34089730048
 ---[output] python test_get.py---------
 
 **************************************************************************
 -----------[code] test_set.py -----------
 from deepspeed.accelerator.cuda_accelerator import CUDA_Accelerator
 cu_accel = CUDA_Accelerator()
-print(f'{id(cu_accel)=}')
+logger.info(f'{id(cu_accel)=}')
 from deepspeed.accelerator import set_accelerator, get_accelerator
 set_accelerator(cu_accel)
 
 my_accelerator = get_accelerator()
-print(f'{id(my_accelerator)=}')
-print(f'{my_accelerator._name=}')
-print(f'{my_accelerator._communication_backend=}')
-print(f'{my_accelerator.HalfTensor().device=}')
-print(f'{my_accelerator.total_memory()=}')
+logger.info(f'{id(my_accelerator)=}')
+logger.info(f'{my_accelerator._name=}')
+logger.info(f'{my_accelerator._communication_backend=}')
+logger.info(f'{my_accelerator.HalfTensor().device=}')
+logger.info(f'{my_accelerator.total_memory()=}')
 -----------[code] test_set.py -----------
 
 
 ---[output] python test_set.py---------
 id(cu_accel)=139648165478304
 my_accelerator=<deepspeed.accelerator.cuda_accelerator.CUDA_Accelerator object at 0x7f025f4bffa0>
 my_accelerator.name='cuda'
```

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/autotuner.py` & `deepspeed-0.9.4/deepspeed/autotuning/autotuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/config.py` & `deepspeed-0.9.4/deepspeed/autotuning/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/constants.py` & `deepspeed-0.9.4/deepspeed/autotuning/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/scheduler.py` & `deepspeed-0.9.4/deepspeed/autotuning/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/tuner/base_tuner.py` & `deepspeed-0.9.4/deepspeed/autotuning/tuner/base_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/tuner/cost_model.py` & `deepspeed-0.9.4/deepspeed/autotuning/tuner/cost_model.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/tuner/index_based_tuner.py` & `deepspeed-0.9.4/deepspeed/autotuning/tuner/index_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/tuner/model_based_tuner.py` & `deepspeed-0.9.4/deepspeed/autotuning/tuner/model_based_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 INIT_NUM = 2
 
 
 class ModelBasedTuner(BaseTuner):
     """Exploring the search space with a cost model"""
 
-    def __init__(self, exps: list, resource_manager, metric, tuning_sapce):
+    def __init__(self, exps: list, resource_manager, metric, tuning_space):
         super().__init__(exps, resource_manager, metric)
-        self.tuning_space = tuning_sapce
+        self.tuning_space = tuning_space
         self.best_iter = 0
 
         self.all_configs = [e['ds_config'] for e in exps]
         self.num_all_configs = len(self.all_configs)
 
         self.dims = dict_to_dims(self.tuning_space)
```

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/tuner/utils.py` & `deepspeed-0.9.4/deepspeed/autotuning/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/autotuning/utils.py` & `deepspeed-0.9.4/deepspeed/autotuning/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/__init__.py` & `deepspeed-0.9.4/deepspeed/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/constants.py` & `deepspeed-0.9.4/deepspeed/checkpoint/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/deepspeed_checkpoint.py` & `deepspeed-0.9.4/deepspeed/checkpoint/deepspeed_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/reshape_3d_utils.py` & `deepspeed-0.9.4/deepspeed/checkpoint/reshape_3d_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/reshape_meg_2d.py` & `deepspeed-0.9.4/deepspeed/checkpoint/reshape_meg_2d.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/reshape_utils.py` & `deepspeed-0.9.4/deepspeed/checkpoint/reshape_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/universal_checkpoint.py` & `deepspeed-0.9.4/deepspeed/checkpoint/universal_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/utils.py` & `deepspeed-0.9.4/deepspeed/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/checkpoint/zero_checkpoint.py` & `deepspeed-0.9.4/deepspeed/checkpoint/zero_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/comm/backend.py` & `deepspeed-0.9.4/deepspeed/comm/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 class Backend(object):
 
     def __init__(self, name='backend', rank=0, size=1):
         self.name = name
         # The world size and rank of the world process group
         self.world_group = None
-        self.world_size = rank
-        self.world_rank = size
+        self.world_size = size
+        self.world_rank = rank
         # Single process group (pg) implementation for now but keep a list for future
         self.process_groups = []
         self.initialized = False
 
     def is_initialized(self):
         return self.initialized
```

### Comparing `deepspeed-0.9.3/deepspeed/comm/ccl.py` & `deepspeed-0.9.4/deepspeed/comm/ccl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/comm/comm.py` & `deepspeed-0.9.4/deepspeed/comm/comm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/comm/config.py` & `deepspeed-0.9.4/deepspeed/comm/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/comm/constants.py` & `deepspeed-0.9.4/deepspeed/comm/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/comm/torch.py` & `deepspeed-0.9.4/deepspeed/comm/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,32 @@
     TORCH_MAJOR = int(torch.__version__.split('.')[0])
     if TORCH_MAJOR >= 2:
         return True
     else:
         return False
 
 
+def torch_ver_ge_1_13():
+    if is_torch_two():
+        return True
+    else:
+        TORCH_MAJOR = int(torch.__version__.split('.')[0])
+        assert TORCH_MAJOR == 1
+
+        TORCH_MINOR = int(torch.__version__.split('.')[1])
+        return TORCH_MINOR >= 13
+
+
 def has_coalescing_manager():
     has_c10d = hasattr(torch.distributed, 'distributed_c10d')
     return has_c10d and hasattr(torch.distributed.distributed_c10d, '_coalescing_manager')
 
 
 def has_all_reduce_coalesced():
-    return hasattr(torch.distributed, "all_reduce_coalesced")
+    return hasattr(torch.distributed, "all_reduce_coalesced") and torch_ver_ge_1_13()
 
 
 def get_coalescing_manager(group, device, reqs):
     if is_torch_two():
         return torch.distributed.distributed_c10d._coalescing_manager(group, device=device, reqs=reqs)
     else:
         return torch.distributed.distributed_c10d._coalescing_manager(group, reqs)
```

### Comparing `deepspeed-0.9.3/deepspeed/comm/utils.py` & `deepspeed-0.9.4/deepspeed/comm/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/basic_layer.py` & `deepspeed-0.9.4/deepspeed/compression/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/compress.py` & `deepspeed-0.9.4/deepspeed/compression/compress.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/config.py` & `deepspeed-0.9.4/deepspeed/compression/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/constants.py` & `deepspeed-0.9.4/deepspeed/compression/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/helper.py` & `deepspeed-0.9.4/deepspeed/compression/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/scheduler.py` & `deepspeed-0.9.4/deepspeed/compression/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/compression/utils.py` & `deepspeed-0.9.4/deepspeed/compression/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/constants.py` & `deepspeed-0.9.4/deepspeed/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/elasticity/config.py` & `deepspeed-0.9.4/deepspeed/elasticity/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/elasticity/constants.py` & `deepspeed-0.9.4/deepspeed/elasticity/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/elasticity/elastic_agent.py` & `deepspeed-0.9.4/deepspeed/elasticity/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/elasticity/elasticity.py` & `deepspeed-0.9.4/deepspeed/elasticity/elasticity.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/env_report.py` & `deepspeed-0.9.4/deepspeed/env_report.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/git_version_info.py` & `deepspeed-0.9.4/deepspeed/git_version_info.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/git_version_info_installed.py` & `deepspeed-0.9.4/deepspeed/git_version_info_installed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-version='0.9.3'
+version='0.9.4'
 git_hash='unknown'
 git_branch='unknown'
 installed_ops={'async_io': False, 'cpu_adagrad': False, 'cpu_adam': False, 'fused_adam': False, 'fused_lamb': False, 'quantizer': False, 'random_ltd': False, 'sparse_attn': False, 'spatial_inference': False, 'transformer': False, 'stochastic_transformer': False, 'transformer_inference': False, 'utils': False}
 compatible_ops={'async_io': False, 'cpu_adagrad': True, 'cpu_adam': True, 'fused_adam': True, 'fused_lamb': True, 'quantizer': True, 'random_ltd': True, 'sparse_attn': False, 'spatial_inference': True, 'transformer': True, 'stochastic_transformer': True, 'transformer_inference': True, 'utils': True}
 torch_info={'version': '1.9', 'bf16_support': False, 'cuda_version': '10.2', 'nccl_version': '2.7', 'hip_version': '0.0'}
```

### Comparing `deepspeed-0.9.3/deepspeed/inference/config.py` & `deepspeed-0.9.4/deepspeed/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/inference/engine.py` & `deepspeed-0.9.4/deepspeed/inference/engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/launcher/launch.py` & `deepspeed-0.9.4/deepspeed/launcher/launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,17 +211,18 @@
                 try:
                     os.makedirs(args.enable_each_rank_log)
                 except Exception as e:
                     print(e)
                     raise ValueError(f"unable to create directory {args.enable_each_rank_log} for each rank log.")
             log_name_prefix = time.strftime("%Y%m%d%H%M%S", time.localtime())
 
-        for local_rank in range(0, num_local_procs):
+        for local_proc in range(0, num_local_procs):
             # each process's rank
-            dist_rank = global_rank_mapping[local_node][local_rank]
+            dist_rank = global_rank_mapping[local_node][local_proc]
+            local_rank = dist_rank % num_local_procs
             current_env["RANK"] = str(dist_rank)
             current_env["LOCAL_RANK"] = str(local_rank)
 
             # spawn the processes
             cmd = []
             if args.bind_cores_to_rank:
                 cores_per_rank, numactl_cmd = get_numactl_cmd(args.bind_core_list, num_local_procs, local_rank)
```

### Comparing `deepspeed-0.9.3/deepspeed/launcher/multinode_runner.py` & `deepspeed-0.9.4/deepspeed/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/launcher/runner.py` & `deepspeed-0.9.4/deepspeed/launcher/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             num_slots = int(match.group(2))
             if host in resource_pool:
                 logger.error(f"Bad hostfile text: {hostfile_lines}")
                 raise ValueError(f"Hostfile contains multiple entries for {host}, unable to proceed with launching")
             resource_pool[host] = num_slots
         else:
             logger.error(f"Bad hostfile text: {hostfile_lines}")
-            raise ValueError("Hostfile contains a bad entry: {line}, unable to proceed with launching")
+            raise ValueError(f"Hostfile contains a bad entry: {line}, unable to proceed with launching")
 
     if len(resource_pool) == 0:
         logger.error(f"Bad hostfile text: {hostfile_lines}")
         raise ValueError("Hostfile is empty or not formatted correctly, unable to proceed with launching.")
 
     return resource_pool
 
@@ -560,15 +560,15 @@
         time.sleep(0.1)
         result.send_signal(signal.SIGTERM)
         result_kill = subprocess.Popen(kill_cmd, env=env)
         result_kill.wait()
         time.sleep(1)
         sys.exit(1)
 
-    if args.launcher == PDSH_LAUNCHER:
+    if args.launcher == PDSH_LAUNCHER and multi_node_exec:
         signal.signal(signal.SIGINT, sigkill_handler)
 
     result.wait()
 
     # In case of failure must propagate the error-condition back to the caller (usually shell). The
     # actual error and traceback should have been printed in the subprocess, so in order to avoid
     # unnecessary noise we just quietly exit here with the same code as the subprocess
```

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/diffusers/unet.py` & `deepspeed-0.9.4/deepspeed/model_implementations/diffusers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/diffusers/vae.py` & `deepspeed-0.9.4/deepspeed/model_implementations/diffusers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/features/cuda_graph.py` & `deepspeed-0.9.4/deepspeed/model_implementations/features/cuda_graph.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/clip_encoder.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bert.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_bloom.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_gpt.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_megatron_gpt.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_opt.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/model_implementations/transformers/ds_transformer.py` & `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/auto_tp.py` & `deepspeed-0.9.4/deepspeed/module_inject/auto_tp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/__init__.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/base.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,25 +245,29 @@
         self.module.mlp.output_w = mp_replace.copy(self.module.mlp.output_w, self._4hh_w, int8=reversed_dim)
         self.module.mlp.output_b = mp_replace.copy(self.module.mlp.output_b,
                                                    self._4hh_b,
                                                    int8=reversed_dim,
                                                    allocate_tensor=reversed_dim)
 
     def copy_data_to_new_module(self):
-        params = {
-            self.module.mlp.attn_nw: self.attn_nw,
-            self.module.mlp.attn_nb: self.attn_nb,
-            self.module.norm_w: self.input_nw,
-            self.module.norm_b: self.input_nb
-        }
-        for dst, src in params.items():
-            if src is None:
-                dst = src
+        params = {'attn_nw': self.attn_nw, 'attn_nb': self.attn_nb}
+        for key in params:
+            if params[key] is None:
+                setattr(self.module.mlp, key, None)
             else:
-                dst.data.copy_(src.to(get_accelerator().current_device_name()))
+                setattr(self.module.mlp, key,
+                        torch.nn.parameter.Parameter(params[key].to(get_accelerator().current_device_name())))
+
+        params = {'norm_w': self.input_nw, 'norm_b': self.input_nb}
+        for key in params:
+            if params[key] is None:
+                setattr(self.module, key, None)
+            else:
+                setattr(self.module, key,
+                        torch.nn.parameter.Parameter(params[key].to(get_accelerator().current_device_name())))
 
     def transpose(self):
         self.transpose_attention()
         self.transpose_mlp()
 
     def transpose_attention(self):
         if self.attn_linear_layer:
```

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/base_moe.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/base_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/bert.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/bloom.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/clip.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/clip.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/distil_bert.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/distil_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/features/gated_mlp.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/features/gated_mlp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_engine.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/features/hybrid_megatron.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_megatron.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/features/megatron.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/features/megatron.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/features/meta_tensor.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/features/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/features/split_qkv.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/features/split_qkv.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,22 +119,22 @@
         self.kb.data = self.module.attention.attn_qkvb.data[self.qw.shape[0]:2 * self.qw.shape[0]]
         self.vw.data = self.module.attention.attn_qkvw.data[2 * self.qw.shape[0]:]
         self.vb.data = self.module.attention.attn_qkvb.data[2 * self.qw.shape[0]:]
 
         for data in qkv_data:
             del data
 
-    def set_attn_parameters_wo_copy(self, Z3_enabled=False):
+    def set_attn_params_wo_copy(self, Z3_enabled=False):
         self.module.attention.attn_ow = self.dense_w
         self.module.attention.attn_ob = self.dense_b
         if not Z3_enabled:
             # In initialize_tensors, we create a fused qkvw with the appropriate shape
             # and copy the qw, qb, kw, kb, vw, vb into it
-            self.module.attn_qkvw = self.qkvw
-            self.module.attn_qkvb = self.qkvb
+            self.module.attention.attn_qkvw = self.qkvw
+            self.module.attention.attn_qkvb = self.qkvb
 
             # We reset the data for qw (which is the original model parameter) to point
             # to the fused weight matrix we have created here
             self.qw.data = self.qkvw[:self.qw.shape[0], :]
             self.kw.data = self.qkvw[self.qw.shape[0]:2 * self.qw.shape[0], :]
             self.vw.data = self.qkvw[self.qw.shape[0] * 2:, :]
```

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/gpt2.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/gpt2.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/gptj.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/gptj.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/gptneo.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/gptneo.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/gptneox.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/gptneox.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/llama.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/llama.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/megatron_gpt_moe.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/opt.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/unet.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/containers/vae.py` & `deepspeed-0.9.4/deepspeed/module_inject/containers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/inject.py` & `deepspeed-0.9.4/deepspeed/module_inject/inject.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/layers.py` & `deepspeed-0.9.4/deepspeed/module_inject/layers.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/load_checkpoint.py` & `deepspeed-0.9.4/deepspeed/module_inject/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/module_quantize.py` & `deepspeed-0.9.4/deepspeed/module_inject/module_quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/policy.py` & `deepspeed-0.9.4/deepspeed/module_inject/policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/replace_module.py` & `deepspeed-0.9.4/deepspeed/module_inject/replace_module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/replace_policy.py` & `deepspeed-0.9.4/deepspeed/module_inject/replace_policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/module_inject/utils.py` & `deepspeed-0.9.4/deepspeed/module_inject/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/moe/experts.py` & `deepspeed-0.9.4/deepspeed/moe/experts.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/moe/layer.py` & `deepspeed-0.9.4/deepspeed/moe/layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/moe/mappings.py` & `deepspeed-0.9.4/deepspeed/moe/mappings.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/moe/sharded_moe.py` & `deepspeed-0.9.4/deepspeed/moe/sharded_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/moe/utils.py` & `deepspeed-0.9.4/deepspeed/moe/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/monitor/config.py` & `deepspeed-0.9.4/deepspeed/monitor/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/monitor/csv_monitor.py` & `deepspeed-0.9.4/deepspeed/monitor/csv_monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/monitor/monitor.py` & `deepspeed-0.9.4/deepspeed/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/monitor/tensorboard.py` & `deepspeed-0.9.4/deepspeed/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/monitor/utils.py` & `deepspeed-0.9.4/deepspeed/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/monitor/wandb.py` & `deepspeed-0.9.4/deepspeed/monitor/wandb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/nebula/config.py` & `deepspeed-0.9.4/deepspeed/nebula/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/nebula/constants.py` & `deepspeed-0.9.4/deepspeed/nebula/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/adagrad/cpu_adagrad.py` & `deepspeed-0.9.4/deepspeed/ops/adagrad/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/adam/cpu_adam.py` & `deepspeed-0.9.4/deepspeed/ops/adam/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/adam/fused_adam.py` & `deepspeed-0.9.4/deepspeed/ops/adam/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/cpu/comm/ccl.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/cpu/comm/ccl.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/StopWatch.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/Timer.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/context.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/conversion_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/conversion_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/cpu_adam.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/dropout.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/feed_forward.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/gelu.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/gemm_test.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/general_kernels.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/normalize_layer.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/quantization_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/reduction_utils.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/simd.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/softmax.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/includes/type_shim.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/dequantize.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/quantization/quantize.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.4/deepspeed/ops/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/lamb/fused_lamb.py` & `deepspeed-0.9.4/deepspeed/ops/lamb/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/__init__.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/all_ops.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/async_io.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/builder.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,16 @@
         return version_ge_1_1 + version_ge_1_3 + version_ge_1_5
 
     def is_compatible(self, verbose=True):
         return super().is_compatible(verbose)
 
     def builder(self):
         try:
-            assert_no_cuda_mismatch(self.name)
+            if not self.is_rocm_pytorch():
+                assert_no_cuda_mismatch(self.name)
             self.build_for_cpu = False
         except BaseException:
             self.build_for_cpu = True
 
         if self.build_for_cpu:
             from torch.utils.cpp_extension import CppExtension as ExtensionBuilder
         else:
```

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/builder.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,11 @@
                                    include_dirs=self.strip_empty_entries(self.include_paths()),
                                    libraries=self.strip_empty_entries(self.libraries_args()),
                                    extra_compile_args=compile_args)
 
         return cpp_ext
 
     def cxx_args(self):
-        return ['-O3', '-std=c++14', '-g', '-Wno-reorder']
+        return ['-O3', '-g', '-Wno-reorder']
 
     def libraries_args(self):
         return []
```

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/comm.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/comm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu/no_impl.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/no_impl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adagrad.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/cpu_adam.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/fused_adam.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/fused_lamb.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/quantizer.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/random_ltd.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/sparse_attn.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/spatial_inference.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/stochastic_transformer.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/transformer.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/op_builder/transformer_inference.py` & `deepspeed-0.9.4/deepspeed/ops/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/quantizer/quantizer.py` & `deepspeed-0.9.4/deepspeed/ops/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/random_ltd/dropping_utils.py` & `deepspeed-0.9.4/deepspeed/ops/random_ltd/dropping_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/matmul.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/softmax.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_attention_utils.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_attention_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparse_self_attention.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/sparsity_config.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparsity_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/__init__.py` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/matmul.tr` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/matmul.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr` & `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/bias_add.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/bias_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/config.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_attention.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/diffusers_transformer_block.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_transformer_block.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_attention.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/ds_mlp.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_mlp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/moe_inference.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/moe_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/base.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/base.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/linear.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/residual_add.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/residual_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/softmax_context.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax_context.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/inference/triton_ops.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/inference/triton_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/ops/transformer/transformer.py` & `deepspeed-0.9.4/deepspeed/ops/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/profiling/config.py` & `deepspeed-0.9.4/deepspeed/profiling/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/profiling/constants.py` & `deepspeed-0.9.4/deepspeed/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/profiling/flops_profiler/profiler.py` & `deepspeed-0.9.4/deepspeed/profiling/flops_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/checkpointing.py` & `deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/checkpointing.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/activation_checkpointing/config.py` & `deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/bf16_optimizer.py` & `deepspeed-0.9.4/deepspeed/runtime/bf16_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py` & `deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py` & `deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,31 +42,31 @@
         self.checkpoint = torch_nebula.Checkpoint(tag, -2)
 
     def save(self, state_dict, path: str):
         log_dist(f"[Nebula] Create dummy files for loading.")
         torch.save("", path)
 
         tag = _get_tag_from_path(path)
-        partititon_name = os.path.basename(path)
-        logger.info(f"[Nebula] Saving {partititon_name} under tag {tag}...")
-        self.checkpoint.save(partititon_name, state_dict)
-        logger.info(f"[Nebula] Saved {partititon_name} under tag {tag}.")
+        partition_name = os.path.basename(path)
+        logger.info(f"[Nebula] Saving {partition_name} under tag {tag}...")
+        self.checkpoint.save(partition_name, state_dict)
+        logger.info(f"[Nebula] Saved {partition_name} under tag {tag}.")
         return None
 
     def load(self, path: str, map_location=None):
         tag = _get_tag_from_path(path)
         first_load_flag = self.tag_flag is None or self.tag_flag == tag
         if not self.enable_nebula_load and first_load_flag:
             self.tag_flag = tag
             logger.info(f"[Nebula] Disable nebula load. Loading checkpoint from {path} ...")
             partition = torch.load(path, map_location=map_location)
             logger.info(f"[Nebula] Disable nebula load. Loaded checkpoint from {path} .")
             return partition
 
-        partititon_name = os.path.basename(path)
+        partition_name = os.path.basename(path)
         logger.info(f"[Nebula] Loading {path} under tag {tag} from nebula path {self.nebula_load_path}...")
 
         checkpoint = None
         if tag in (None, 'latest', 'latest_universal'):
             # In some cases, there is the inconsistent tag between deepspeed metadata (latest file)
             # and nebula metadata, will lead to the failure on loading with deepspeed tag. Then we
             # will try to load the valid latest checkpoint from nebula(tier3 > tier1). So, in summary
@@ -89,15 +89,15 @@
                 # nebula tier1 latest
                 checkpoint = torch_nebula.get_latest_checkpoint()
                 logger.warning(f"Unable to find valid checkpoint from Nebula under tag:{tag}.")
                 return None
 
         tag = checkpoint.tag
         self.tag_flag = -1
-        partition = checkpoint.load(partititon_name, map_location=map_location)
+        partition = checkpoint.load(partition_name, map_location=map_location)
         logger.info(f"[Nebula] Loaded {path} under tag {tag} from {self.nebula_load_path}.")
         return partition
 
     def commit(self, tag):
         # nebula commit will be call when all files under give tag are ready to be persisted in the async way.
         logger.info(f"[Nebula] all files for {tag} are saved in tier1. It is ready to start persisting")
         commit_rls = self.checkpoint.commit()
```

### Comparing `deepspeed-0.9.3/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py` & `deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/comm/coalesced_collectives.py` & `deepspeed-0.9.4/deepspeed/runtime/comm/coalesced_collectives.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/comm/mpi.py` & `deepspeed-0.9.4/deepspeed/runtime/comm/mpi.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/comm/nccl.py` & `deepspeed-0.9.4/deepspeed/runtime/comm/nccl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/compression/cupy.py` & `deepspeed-0.9.4/deepspeed/runtime/compression/cupy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/config.py` & `deepspeed-0.9.4/deepspeed/runtime/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/config_utils.py` & `deepspeed-0.9.4/deepspeed/runtime/config_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/constants.py` & `deepspeed-0.9.4/deepspeed/runtime/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/config.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/constants.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/curriculum_scheduler.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/curriculum_scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/helper.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/scheduler.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_routing/utils.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/data_pipeline/data_sampling/utils.py` & `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/dataloader.py` & `deepspeed-0.9.4/deepspeed/runtime/dataloader.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/eigenvalue.py` & `deepspeed-0.9.4/deepspeed/runtime/eigenvalue.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/engine.py` & `deepspeed-0.9.4/deepspeed/runtime/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -3053,19 +3053,19 @@
             return False
 
         return True
 
     def _create_zero_checkpoint_files(self, save_dir, tag):
         success = True
         # zero checkpoint files are created sequentially
-        for rank in range(self.world_size):
+        for rank in range(dist.get_world_size(self.optimizer.dp_process_group)):
             if rank == self.global_rank:
                 success = self._create_checkpoint_file(save_dir, tag, True)
 
-            dist.barrier()
+            dist.barrier(group=self.optimizer.dp_process_group)
 
         return success
 
     def _save_checkpoint(self, save_dir, tag, client_state={}):
 
         save_path = self._get_ckpt_name(save_dir, tag)
```

### Comparing `deepspeed-0.9.3/deepspeed/runtime/fp16/fused_optimizer.py` & `deepspeed-0.9.4/deepspeed/runtime/fp16/fused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/fp16/loss_scaler.py` & `deepspeed-0.9.4/deepspeed/runtime/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/adam.py` & `deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/lamb.py` & `deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/fp16/onebit/zoadam.py` & `deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/zoadam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/fp16/unfused_optimizer.py` & `deepspeed-0.9.4/deepspeed/runtime/fp16/unfused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/hybrid_engine.py` & `deepspeed-0.9.4/deepspeed/runtime/hybrid_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/lr_schedules.py` & `deepspeed-0.9.4/deepspeed/runtime/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/pipe/engine.py` & `deepspeed-0.9.4/deepspeed/runtime/pipe/engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/pipe/module.py` & `deepspeed-0.9.4/deepspeed/runtime/pipe/module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/pipe/p2p.py` & `deepspeed-0.9.4/deepspeed/runtime/pipe/p2p.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/pipe/schedule.py` & `deepspeed-0.9.4/deepspeed/runtime/pipe/schedule.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/pipe/topology.py` & `deepspeed-0.9.4/deepspeed/runtime/pipe/topology.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/progressive_layer_drop.py` & `deepspeed-0.9.4/deepspeed/runtime/progressive_layer_drop.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/quantize.py` & `deepspeed-0.9.4/deepspeed/runtime/quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/sparse_tensor.py` & `deepspeed-0.9.4/deepspeed/runtime/sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/state_dict_factory.py` & `deepspeed-0.9.4/deepspeed/runtime/state_dict_factory.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/aio_config.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/aio_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/async_swapper.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/async_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/constants.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/optimizer_utils.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/swap_tensor/utils.py` & `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/utils.py` & `deepspeed-0.9.4/deepspeed/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/weight_quantizer.py` & `deepspeed-0.9.4/deepspeed/runtime/weight_quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/config.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/contiguous_memory_allocator.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/contiguous_memory_allocator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/linear.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/mics.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/mics.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,23 +389,28 @@
                          max_reuse_distance, max_live_parameters, param_persistence_threshold,
                          model_persistence_threshold, dp_process_group, reduce_scatter, overlap_comm,
                          offload_optimizer_config, offload_param_config, sub_group_size, mpu, clip_grad,
                          communication_data_type, postscale_gradients, gradient_predivide_factor,
                          gradient_accumulation_steps, elastic_checkpoint, aio_config)
         first_param = next(module.parameters())
         # overload the dp_process_group and partition_count
+        assert hasattr(first_param, "comm"), " ".join([
+            "Sharded parameters don't have the MiCS_CommGroups attached.",
+            "Might due to the use of deepspeed.zero.Init context for initializing the weights.",
+            "To use MiCS sharding, please use deepspeed.zero.MiCS_Init instead for initializing parameter."
+        ])
         self.dp_process_group = first_param.comm.param_shard_group
         self.partition_count = first_param.comm.param_shard_size
 
     def initialize_ds_offload(self, module, timers, ds_config, overlap_comm, prefetch_bucket_size, max_reuse_distance,
                               max_live_parameters, param_persistence_threshold, model_persistence_threshold,
-                              offload_optimizer_config, mpu):
+                              offload_param_config, mpu):
         return MiCS_Offload(module, timers, ds_config, overlap_comm, prefetch_bucket_size, max_reuse_distance,
                             max_live_parameters, param_persistence_threshold, model_persistence_threshold,
-                            offload_optimizer_config, mpu)
+                            offload_param_config, mpu)
 
     def partition_grads(self, params_to_release: List[Parameter], grad_partitions: List[Tensor]) -> None:
         grad_buffers = super().partition_grads(params_to_release, grad_partitions)
         # perform all-reduce among replication groups
         # the function will perform accumulation boundary check
         self.allreduce_mics_shard_grads(params_to_release, grad_buffers)
 
@@ -436,18 +441,17 @@
             aggregated_buffer.div_(param_repli_size)
             dist.all_reduce(aggregated_buffer, group=param_repli_group)
             offset = 0
             for grad_buff in partitioned_grads_buffers:
                 grad_buff.view(-1).copy_(aggregated_buffer.narrow(0, offset, grad_buff.numel()))
                 offset += grad_buff.numel()
 
-    # TODO: Support different/changing load/save DP degree.
     def load_state_dict(self,
                         state_dict_list,
                         load_optimizer_states=True,
                         load_from_fp32_weights=False,
                         checkpoint_folder=None):
-        r""" Loading the MiCS checkpoints
-
-        TODO: move the implementation from zhen/merged_ds_master branch
+        r""" Loading the ZeRO-3/MiCS partitioned checkpoints
+        Because the self.dp_process_group is replaced with the communicator for
+        partition group we can call the load_state_dict logic from ZeRO-3.
         """
-        raise NotImplementedError("Not implemented for loading MiCS checkpoints")
+        super().load_state_dict(state_dict_list, load_optimizer_states, load_from_fp32_weights, checkpoint_folder)
```

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/mics_utils.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/mics_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/offload_config.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/offload_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/parameter_offload.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/parameter_offload.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/partition_parameters.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/partition_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import types
 from typing import Callable, Iterable
 from enum import Enum
 import functools
 import itertools
 from typing import List
+import logging
 import torch
 from torch import Tensor
 from deepspeed import comm as dist
 from torch.nn import Module
 from torch.nn import Parameter
 
 from .linear import zero3_linear_wrap
@@ -215,14 +216,16 @@
     INFLIGHT = 3
 
 
 _orig_torch_empty = torch.empty
 _orig_torch_zeros = torch.zeros
 _orig_torch_ones = torch.ones
 _orig_torch_full = torch.full
+_orig_torch_arange = torch.arange
+_orig_torch_eye = torch.eye
 
 
 def zero_wrapper_for_fp_tensor_constructor(fn: Callable, target_fp_dtype: torch.dtype) -> Callable:
 
     def wrapped_fn(*args, **kwargs) -> Tensor:
         if kwargs.get("device", None) is None:
             kwargs['device'] = torch.device(get_accelerator().device_name(os.environ["LOCAL_RANK"]))
@@ -419,19 +422,15 @@
             torch.nn.modules.module.Module._old_apply = torch.nn.modules.module.Module.apply
             torch.Tensor.__old_new__ = torch.Tensor.__new__
 
             # Replace .__init__() for future subclasses of torch.nn.Module
             torch.nn.modules.module.Module.__init_subclass__ = classmethod(_init_subclass)
             torch.nn.modules.module.Module.apply = apply_with_gather(torch.nn.modules.module.Module._old_apply)
 
-            torch.Tensor.__new__ = get_new_tensor_fn_for_dtype(self.dtype)
-            torch.empty = zero_wrapper_for_fp_tensor_constructor(_orig_torch_empty, self.dtype)
-            torch.zeros = zero_wrapper_for_fp_tensor_constructor(_orig_torch_zeros, self.dtype)
-            torch.ones = zero_wrapper_for_fp_tensor_constructor(_orig_torch_ones, self.dtype)
-            torch.full = zero_wrapper_for_fp_tensor_constructor(_orig_torch_full, self.dtype)
+            self._add_tensor_creation_wrappers()
 
             if self.mem_efficient_linear:
                 print_rank_0(
                     "nn.functional.linear has been overridden with a more memory efficient version. This will persist unless manually reset.",
                     force=False)
                 self.linear_bk = torch.nn.functional.linear
                 torch.nn.functional.linear = zero3_linear_wrap
@@ -471,14 +470,32 @@
             elif ds_config.fp16_enabled:
                 self.dtype = torch.half
             else:
                 self.dtype = torch.float
         else:
             self.dtype = dtype or torch.half
 
+    def _add_tensor_creation_wrappers(self):
+        torch.Tensor.__new__ = get_new_tensor_fn_for_dtype(self.dtype)
+        torch.empty = zero_wrapper_for_fp_tensor_constructor(_orig_torch_empty, self.dtype)
+        torch.zeros = zero_wrapper_for_fp_tensor_constructor(_orig_torch_zeros, self.dtype)
+        torch.ones = zero_wrapper_for_fp_tensor_constructor(_orig_torch_ones, self.dtype)
+        torch.full = zero_wrapper_for_fp_tensor_constructor(_orig_torch_full, self.dtype)
+        torch.arange = zero_wrapper_for_fp_tensor_constructor(_orig_torch_arange, self.dtype)
+        torch.eye = zero_wrapper_for_fp_tensor_constructor(_orig_torch_eye, self.dtype)
+
+    def _remove_tensor_creation_wrappers(self):
+        torch.Tensor.__new__ = torch.Tensor.__old_new__
+        torch.empty = _orig_torch_empty
+        torch.zeros = _orig_torch_zeros
+        torch.ones = _orig_torch_ones
+        torch.full = _orig_torch_full
+        torch.arange = _orig_torch_arange
+        torch.eye = _orig_torch_eye
+
     def remove_wrappers(self):
 
         def _disable_class(cls):
             cls.__init__ = cls._old_init
 
         for subclass in self.wrapped_cls:
             _disable_class(subclass)
@@ -486,19 +503,15 @@
 
         # This context is the top level of nested Init
         if self.nest_level == 0 and self.torch_func_wrapped:
             # putting methods back the way we found them
             torch.nn.modules.module.Module.__init_subclass__ = torch.nn.modules.module.Module._old_init_subclass
             torch.nn.modules.module.Module.apply = torch.nn.modules.module.Module._old_apply
 
-            torch.Tensor.__new__ = torch.Tensor.__old_new__
-            torch.empty = _orig_torch_empty
-            torch.zeros = _orig_torch_zeros
-            torch.ones = _orig_torch_ones
-            torch.full = _orig_torch_full
+            self._remove_tensor_creation_wrappers()
 
             # un doing it here will undo it during training
             # if self.mem_efficient_linear:
             #    torch.nn.functional.linear = self.linear_bk
             #        if self.mem_efficient_linear:
             #            torch.nn.functional.linear = self.linear_bk
 
@@ -894,15 +907,16 @@
             # is done by flattening the parameter list into a single tensor that
             # can be allgathered in a single call - this means that if each rank
             # gives a list of the same parameters in a different order we will
             # silently get incorrect parameter values, and have very difficult
             # to debug correctness issues.
             params = sorted(params, key=lambda p: p.ds_id)
 
-            debug_rank0(f"-allgather_coalesced: {[p.ds_id for p in params]}")
+            if logger.isEnabledFor(logging.DEBUG):
+                debug_rank0(f"-allgather_coalesced: {[p.ds_id for p in params]}")
 
             if safe_mode:
                 # ensure that same list (with same ordering) of parameters are
                 # being allgathered across all ranks, otherwise could mix
                 # data between tensors.
                 assert_ints_same_as_other_ranks([p.ds_id for p in params])
                 # ensure that tensors from each rank agree on the same ds_numel
```

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/partitioned_param_coordinator.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/partitioned_param_coordinator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from deepspeed import comm as dist
 from deepspeed.utils.logging import logger
 from deepspeed.runtime.zero.offload_config import OffloadDeviceEnum
 from deepspeed.runtime.zero.partition_parameters import *
 from deepspeed.runtime.swap_tensor.partitioned_param_swapper import PartitionedParamStatus
 from deepspeed.utils.debug import debug_module2name_id, debug_param2name_id
 from deepspeed.accelerator import get_accelerator
+import logging
 
 
 def debug_rank0(message: str) -> None:
     if dist.get_rank() == 0:
         logger.debug(message)
 
 
@@ -231,33 +232,36 @@
     @torch.no_grad()
     def fetch_sub_module(self, current_submodule: Module) -> None:
         """This method does the following (in order):
         1. kick off fetch for parameters in immediately required sub module
         2. kick off fetch for next few parameters we will need later (prefetch)
         3. block on parameters in immediately required sub module
         """
-        debug_rank0(
-            f"{self.__step_id}: M{current_submodule.id}({type(current_submodule).__name__}) P{[p.ds_id for p in iter_params(current_submodule)]} "
-            + str({
-                "avail": f"{self.__n_available_params:.1e}",
-                "queue_sz": f"{len(self.__param_queue or [])}",
-                "inflight": [p.ds_id for p in self.__inflight_param_registry],
-            }))
+        if logger.isEnabledFor(logging.DEBUG):
+            debug_rank0(
+                f"{self.__step_id}: M{current_submodule.id}({type(current_submodule).__name__}) P{[p.ds_id for p in iter_params(current_submodule)]} "
+                + str({
+                    "avail": f"{self.__n_available_params:.1e}",
+                    "queue_sz": f"{len(self.__param_queue or [])}",
+                    "inflight": [p.ds_id for p in self.__inflight_param_registry],
+                }))
 
         params_to_fetch = frozenset(iter_params(current_submodule))
 
         # kick off all gather for params in the immediately required submodule
-        for param in params_to_fetch:
-            debug_rank0(f"-fetch: {param.ds_summary()}")
+        if logger.isEnabledFor(logging.DEBUG):
+            for param in params_to_fetch:
+                debug_rank0(f"-fetch: {param.ds_summary()}")
         self.__all_gather_params(params_to_fetch)
 
         # wait for parameters in the immediately needed submodule to become available
         for param in params_to_fetch:
             param.ds_active_sub_modules.add(current_submodule.id)
-            debug_rank0(f"-wait: {param.ds_summary()}")
+            if logger.isEnabledFor(logging.DEBUG):
+                debug_rank0(f"-wait: {param.ds_summary()}")
             if param in self.__inflight_param_registry:
                 with get_accelerator().stream(self.__allgather_stream):
                     while self.__ongoing_fetch_events and self.__ongoing_fetch_events[0].query():
                         self.__ongoing_fetch_events.popleft()
                     if len(self.__ongoing_fetch_events) > self.__max_ongoing_fetch_events:
                         self.__ongoing_fetch_events.popleft().synchronize()
 
@@ -324,16 +328,17 @@
                         max(self.__most_recent_step_id_param_fetched_for[param_in_trace.param],
                             param_in_trace.step_id_last_used_at)
 
                     if do_prefetch:
                         params_to_prefetch.add(param_in_trace.param)
                         numel_prefetching += param_in_trace.param.ds_numel
 
-                for param in params_to_prefetch:
-                    debug_rank0(f"-prefetch: {param.ds_summary()}")
+                if logger.isEnabledFor(logging.DEBUG):
+                    for param in params_to_prefetch:
+                        debug_rank0(f"-prefetch: {param.ds_summary()}")
                 self.__all_gather_params(params_to_prefetch)
 
                 if self.__prefetch_nvme:
                     self.__prefetch_nvme_param_partitions()
 
         self.__step_id += 1
 
@@ -390,15 +395,16 @@
             ]
             if swap_persisted_params:
                 swap_persisted_params[0].nvme_swapper.remove_partition_and_release_buffers(swap_persisted_params)
 
     @instrument_w_nvtx
     def __release_param(self, param: Parameter) -> None:
         if param.ds_status == ZeroParamStatus.AVAILABLE and not param.ds_active_sub_modules:
-            debug_rank0(f"-release: {param.ds_summary()}")
+            if logger.isEnabledFor(logging.DEBUG):
+                debug_rank0(f"-release: {param.ds_summary()}")
             param.partition()
             self.__n_available_params -= param.ds_numel
 
     @instrument_w_nvtx
     @functools.lru_cache(maxsize=None)
     def __params_to_release(self, submodule_to_release: Module, step_id: int) -> Set[int]:
         if not self.is_complete_trace():
```

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/stage3.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/stage3.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,14 @@
         num_fp16_subgroups = len(self.fp16_partitioned_groups_flat)
         see_memory_usage(f"After creating fp16 partitions: {num_fp16_subgroups}", force=True)
 
         # Optimizer tensor swapping
         if self.swap_optimizer:
             self._configure_tensor_swapping(offload_optimizer_config, aio_config)
 
-        self.params_in_ipg_bucket = []
         self.is_gradient_accumulation_boundary: bool = True
 
         self.param_reduce_events: Deque[get_accelerator().Event] = collections.deque()
         # TODO. make this configurable via JSON
         self.max_param_reduce_events: int = 2
 
         self.param_dict = {}
@@ -273,29 +272,27 @@
         # map between param_id and bool to specify if a param is in this partition
         self.is_param_in_current_partition = {}
 
         self.extra_large_param_to_reduce = None
         self.grads_in_ipg_bucket = []
         self.params_in_ipg_bucket = []
 
-        self.params_already_reduced = []
         self.is_gradient_accumulation_boundary = True
         self._release_ipg_buffers()
         self.previous_reduced_grads = None
 
         # simplified param id
         self.param_id = {}
 
         count = 0
         for i, params_group in enumerate(self.fp16_groups):
             for param in params_group:
                 unique_id = id(param)
                 self.param_id[unique_id] = count
                 self.param_dict[count] = param
-                self.params_already_reduced.append(False)
                 count = count + 1
 
         #Largest partitioned param
         largest_partitioned_param_numel = max([
             max([max(tensor.numel(), tensor.ds_numel) for tensor in fp16_partitioned_group])
             for fp16_partitioned_group in self.fp16_partitioned_groups
         ])
@@ -303,15 +300,14 @@
 
         self._setup_for_real_optimizer()
         self.grad_position = {}
         self.set_grad_positions()
 
         if self.offload_optimizer:
             self.norm_for_param_grads = {}
-            self.local_overflow = False
 
         # stores if a partition has been reduced in this step
         self.is_partition_reduced = {}
 
         # stores if a grad in a partition has been computed or not
         self.is_grad_computed = {}
 
@@ -393,28 +389,28 @@
 
         # IPG
         if self.contiguous_gradients:
             self.__ipg_bucket_flat_buffer: Tensor = torch.empty(self.reduce_bucket_size,
                                                                 dtype=self.dtype,
                                                                 device=get_accelerator().current_device_name())
 
-        grad_partitions_flat_buffer = None
+        self.grad_partitions_flat_buffer = None
         self.__param_id_to_grad_partition: Dict[int, Tensor] = {}
 
         all_params = list(itertools.chain.from_iterable(self.fp16_groups))
 
-        grad_partitions_flat_buffer: Tensor = torch.zeros(sum(p.partition_numel() for p in all_params),
-                                                          dtype=self.dtype,
-                                                          device=self.device)
+        self.grad_partitions_flat_buffer: Tensor = torch.zeros(sum(p.partition_numel() for p in all_params),
+                                                               dtype=self.dtype,
+                                                               device=self.device)
         if self.offload_optimizer_pin_memory:
-            grad_partitions_flat_buffer = get_accelerator().pin_memory(grad_partitions_flat_buffer)
+            self.grad_partitions_flat_buffer = get_accelerator().pin_memory(self.grad_partitions_flat_buffer)
 
         offset = 0
         for param in all_params:
-            self.__param_id_to_grad_partition[param.ds_id] = grad_partitions_flat_buffer.narrow(
+            self.__param_id_to_grad_partition[param.ds_id] = self.grad_partitions_flat_buffer.narrow(
                 0, offset, param.partition_numel())
             offset += param.partition_numel()
 
     def _link_all_hp_params(self):
         for p in self.module.parameters():
             p._z3_optimizer = self
 
@@ -962,19 +958,14 @@
     def independent_gradient_partition_epilogue(self):
         self.report_ipg_memory_usage(f"In ipg_epilogue before reduce_ipg_grads", 0)
         self.__reduce_and_partition_ipg_grads()
         self.report_ipg_memory_usage(f"In ipg_epilogue after reduce_ipg_grads", 0)
 
         self.reduce_and_partition_stream.synchronize()
 
-        # if dist.get_rank() == 0:
-        #    logger.info("Params already reduced %s", self.params_already_reduced)
-        for i in range(len(self.params_already_reduced)):
-            self.params_already_reduced[i] = False
-
         #in case of cpu offload, averaged gradients are already in fp32_partitioned_groups_flat.grad
         #TODO: use a similar code path for both cpu_offload and non-cpu offload
         if not self.offload_optimizer:
             for i, sub_group in enumerate(self.fp16_groups):
                 self.averaged_gradients[i] = [
                     self.__param_id_to_grad_partition[param.ds_id]
                     if param.requires_grad else torch.zeros_like(param.ds_tensor) for param in sub_group
@@ -1041,26 +1032,19 @@
         #print_rank_0(f"Inside reduce ipg buckets. {debug_param2name_id_shape(param)}, ipg elements {self.elements_in_ipg_bucket}, reduce bucket size {self.reduce_bucket_size}", force=True)
 
         # Because the ipg bucket is initialized with a random place holder tensor, we must
         # explicitly check that the bucket has any real data in it (self.elements_in_ipg_bucket >
         # 0). Otherwise if the incoming param.ds_numel is large, this branch may get triggered on a
         # garbage data and `self.average_tensor()` will crash because its params_to_reduce will be
         # empty, while reduction_list will have that garbage data.
-        if self.elements_in_ipg_bucket > 0 and self.elements_in_ipg_bucket + param.ds_numel > self.reduce_bucket_size:
+        if self.elements_in_ipg_bucket + param.ds_numel > self.reduce_bucket_size and self.elements_in_ipg_bucket > 0:
             self.report_ipg_memory_usage("In ipg_remove_grads before reduce_ipg_grads", param.ds_numel)
 
             self.__reduce_and_partition_ipg_grads()
 
-        param_id = self.get_param_id(param)
-
-        assert self.params_already_reduced[param_id] == False, \
-            f"The parameter {param_id} has already been reduced. \
-            Gradient computed twice for this partition. \
-            Multiple gradient reduction is currently not supported"
-
         self.__add_grad_to_ipg_bucket(param)
 
     @instrument_w_nvtx
     @torch.no_grad()
     def __add_grad_to_ipg_bucket(self, param: Parameter) -> None:
         self.reduce_and_partition_stream.wait_stream(get_accelerator().default_stream())
 
@@ -1083,37 +1067,82 @@
             return
 
         for param in self.params_in_ipg_bucket:
             if param.grad.numel() != param.ds_numel:
                 raise RuntimeError(f"{param.grad.numel()} != {param.ds_numel} Cannot reduce scatter "
                                    f"gradients whose size is not same as the params")
 
-        self.params_in_ipg_bucket.sort(key=lambda p: p.ds_id)
-
         assert len(set(p.ds_id for p in self.params_in_ipg_bucket)) == len(self.params_in_ipg_bucket)
 
         while self.param_reduce_events and self.param_reduce_events[0].query():
             self.param_reduce_events.popleft()
         if len(self.param_reduce_events) > self.max_param_reduce_events:
             self.param_reduce_events.popleft().synchronize()
 
         with get_accelerator().stream(self.reduce_and_partition_stream):
             if safe_mode:
                 assert_ints_same_as_other_ranks([p.ds_id for p in self.params_in_ipg_bucket])
 
-            grad_partitions = self.__avg_scatter_grads(self.params_in_ipg_bucket)
+            if self.contiguous_gradients and not self.reduce_scatter:
+                grad_bucket = self.__ipg_bucket_flat_buffer.narrow(0, 0, self.elements_in_ipg_bucket)
+                grad_partitions = self.__avg_scatter_contiguous_grads(grad_bucket)
+            else:
+                self.params_in_ipg_bucket.sort(key=lambda p: p.ds_id)
+                grad_partitions = self.__avg_scatter_grads(self.params_in_ipg_bucket)
+
             self.partition_grads(self.params_in_ipg_bucket, grad_partitions)
 
             self.params_in_ipg_bucket.clear()
 
             event = get_accelerator().Event()
             event.record()
             self.param_reduce_events.append(event)
 
     @instrument_w_nvtx
+    def __avg_scatter_contiguous_grads(self, buffer_to_reduce: Tensor) -> List[Tensor]:
+        dtype = buffer_to_reduce.dtype
+        if self.communication_data_type == self.dtype:
+            buffer_to_reduce = buffer_to_reduce.to(self.communication_data_type)
+        if self.postscale_gradients and self.gradient_predivide_factor != 1.0:
+            buffer_to_reduce = buffer_to_reduce.div_(self.gradient_predivide_factor)
+
+        world_sz = dist.get_world_size(self.dp_process_group)
+        rank = dist.get_rank(self.dp_process_group)
+        buffer_to_reduce.div_(world_sz)
+
+        dist.all_reduce(buffer_to_reduce, group=self.dp_process_group)
+
+        if self.postscale_gradients and self.gradient_predivide_factor != world_sz:
+            buffer_to_reduce = buffer_to_reduce.mul(self.gradient_predivide_factor)
+
+        if self.communication_data_type != self.dtype:
+            buffer_to_reduce = buffer_to_reduce.to(self.dtype)
+
+        grad_partitions = []
+        grad_offset_in_buffer = 0
+        for param in self.params_in_ipg_bucket:
+            grad = param.grad
+            chunk_sz = math.ceil(grad.numel() / world_sz)
+
+            start_offset = grad_offset_in_buffer + min(rank * chunk_sz, grad.numel())
+            end_offset = grad_offset_in_buffer + min(rank * chunk_sz + chunk_sz, grad.numel())
+
+            partition = buffer_to_reduce[start_offset:end_offset]
+            if param.partition_numel() != partition.numel():
+                padded_partition = torch.empty(param.partition_numel(), device=grad.device, dtype=grad.dtype)
+                if partition.numel() > 0:
+                    padded_partition[:partition.numel()] = partition
+                grad_partitions.append(padded_partition)
+            else:
+                grad_partitions.append(partition)
+            grad_offset_in_buffer += grad.numel()
+
+        return grad_partitions
+
+    @instrument_w_nvtx
     def __avg_scatter_grads(self, params_to_reduce: List[Parameter]) -> List[Tensor]:
         """average gradients and scatter partitions across ranks"""
 
         full_grads_for_rank = [p.grad for p in params_to_reduce]
         if self.communication_data_type != self.dtype:
             full_grads_for_rank = [g.to(self.communication_data_type) for g in full_grads_for_rank]
 
@@ -1219,23 +1248,14 @@
                 cuda_grad_buffer = grad_buffer.to(grad_partition.device, non_blocking=True)
                 cuda_grad_buffer.add_(grad_partition)
                 grad_buffer.copy_(cuda_grad_buffer, non_blocking=True)
                 # ensure grad buffer is a CUDA buffer to speed up the next few
                 # operations and so it can be used asynchronously
                 grad_buffer = cuda_grad_buffer
 
-            if hasattr(self.inf_or_nan_tracker, "logical_or_"):
-                self.inf_or_nan_tracker.logical_or_(torch.isinf(grad_buffer).any())
-                self.inf_or_nan_tracker.logical_or_(torch.isnan(grad_buffer).any())
-            else:
-                # logical_or_ not available in older versions of pytorch
-                self.inf_or_nan_tracker += torch.isinf(grad_buffer).any()
-                self.inf_or_nan_tracker += torch.isnan(grad_buffer).any()
-                self.inf_or_nan_tracker = self.inf_or_nan_tracker > 0
-
             # offload the gradient partition if applicable
             if self.offload_optimizer:
                 i, dest_offset, _ = self.grad_position[self.get_param_id(param)]
 
                 if self.is_gradient_accumulation_boundary:
                     self.norm_for_param_grads[self.get_param_id(param)] = self._constant_buffered_norm2(grad_buffer)
 
@@ -1563,15 +1583,14 @@
 
     def free_grad_in_param_list(self, param_list):
         for p in param_list:
             p.grad = None
 
     def reset_cpu_buffers(self):
         self.norm_for_param_grads = {}
-        self.local_overflow = False
 
     def log_timers(self, timer_names):
         if self.timers is None:
             return
 
         self.timers.log(names=list(timer_names))
 
@@ -1897,20 +1916,27 @@
                     return True
         return False
 
     @instrument_w_nvtx
     def has_overflow(self, partition_gradients=True):
         if partition_gradients:
             with get_accelerator().stream(self.reduce_and_partition_stream):
-                self.local_overflow = bool(self.inf_or_nan_tracker.item())
+                if hasattr(self.inf_or_nan_tracker, "logical_or_"):
+                    self.inf_or_nan_tracker.logical_or_(torch.isinf(self.grad_partitions_flat_buffer).any())
+                    self.inf_or_nan_tracker.logical_or_(torch.isnan(self.grad_partitions_flat_buffer).any())
+                else:
+                    # logical_or_ not available in older versions of pytorch
+                    self.inf_or_nan_tracker += torch.isinf(self.grad_partitions_flat_buffer).any()
+                    self.inf_or_nan_tracker += torch.isnan(self.grad_partitions_flat_buffer).any()
+                    self.inf_or_nan_tracker = self.inf_or_nan_tracker > 0
+
+                overflow_gpu = self.inf_or_nan_tracker.clone().to(torch.uint8)
                 self.inf_or_nan_tracker.zero_()
 
-            overflow = self.local_overflow
-            #overflow = self.has_overflow_partitioned_grads_serial()
-            overflow_gpu = get_accelerator().ByteTensor([overflow])
+            get_accelerator().default_stream().wait_stream(self.reduce_and_partition_stream)
             dist.all_reduce(overflow_gpu, op=dist.ReduceOp.MAX, group=self.dp_process_group)
 
         else:
             params = []
             for group in self.fp16_groups:
                 for param in group:
                     params.append(param)
```

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/stage_1_and_2.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/stage_1_and_2.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/test.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/test.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/tiling.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/tiling.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/runtime/zero/utils.py` & `deepspeed-0.9.4/deepspeed/runtime/zero/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/__init__.py` & `deepspeed-0.9.4/deepspeed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/comms_logging.py` & `deepspeed-0.9.4/deepspeed/utils/comms_logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/debug.py` & `deepspeed-0.9.4/deepspeed/utils/debug.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/groups.py` & `deepspeed-0.9.4/deepspeed/utils/groups.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/init_on_device.py` & `deepspeed-0.9.4/deepspeed/utils/init_on_device.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/logging.py` & `deepspeed-0.9.4/deepspeed/utils/logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/mixed_precision_linkage.py` & `deepspeed-0.9.4/deepspeed/utils/mixed_precision_linkage.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/numa.py` & `deepspeed-0.9.4/deepspeed/utils/numa.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/tensor_fragment.py` & `deepspeed-0.9.4/deepspeed/utils/tensor_fragment.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/timer.py` & `deepspeed-0.9.4/deepspeed/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed/utils/zero_to_fp32.py` & `deepspeed-0.9.4/deepspeed/utils/zero_to_fp32.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed.egg-info/PKG-INFO` & `deepspeed-0.9.4/deepspeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.3
+Version: 0.9.4
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -249,14 +249,15 @@
 14. Reza Yazdani Aminabadi, Samyam Rajbhandari, Minjia Zhang, Ammar Ahmad Awan, Cheng Li, Du Li, Elton Zheng, Jeff Rasley, Shaden Smith, Olatunji Ruwase, Yuxiong He. (2022) DeepSpeed Inference: Enabling Efficient Inference of Transformer Models at Unprecedented Scale. [arXiv:2207.00032](https://arxiv.org/abs/2207.00032) and [SC 2022](https://dl.acm.org/doi/abs/10.5555/3571885.3571946).
 15. Zhewei Yao, Xiaoxia Wu, Conglong Li, Connor Holmes, Minjia Zhang, Cheng Li, Yuxiong He. (2022) Random-LTD: Random and Layerwise Token Dropping Brings Efficient Training for Large-scale Transformers. [arXiv:2211.11586](https://arxiv.org/abs/2211.11586).
 16. Conglong Li, Zhewei Yao, Xiaoxia Wu, Minjia Zhang, Yuxiong He. (2022) DeepSpeed Data Efficiency: Improving Deep Learning Model Quality and Training Efficiency via Efficient Data Sampling and Routing. [arXiv:2212.03597](https://arxiv.org/abs/2212.03597).
 17. Xiaoxia Wu, Cheng Li, Reza Yazdani Aminabadi, Zhewei Yao, Yuxiong He. (2023) Understanding INT4 Quantization for Transformer Models: Latency Speedup, Composability, and Failure Cases. [arXiv:2301.12017](https://arxiv.org/abs/2301.12017).
 18. Syed Zawad, Cheng Li, Zhewei Yao, Elton Zheng, Yuxiong He, Feng Yan. (2023) DySR: Adaptive Super-Resolution via Algorithm and System Co-design. [ICLR:2023](https://openreview.net/forum?id=Pgtn4l6eKjv).
 19. Sheng Shen, Zhewei Yao, Chunyuan Li, Trevor Darrell, Kurt Keutzer, Yuxiong He. (2023) Scaling Vision-Language Models with Sparse Mixture of Experts. [arXiv:2303.07226](https://arxiv.org/abs/2303.07226).
 20. Quentin Anthony, Ammar Ahmad Awan, Jeff Rasley, Yuxiong He, Aamir Shafi, Mustafa Abduljabbar, Hari Subramoni, Dhabaleswar Panda. (2023) MCR-DL: Mix-and-Match Communication Runtime for Deep Learning [arXiv:2303.08374](https://arxiv.org/abs/2303.08374) and will appear at IPDPS 2023.
+21. Siddharth Singh, Olatunji Ruwase, Ammar Ahmad Awan, Samyam Rajbhandari, Yuxiong He, Abhinav Bhatele. (2023) A Hybrid Tensor-Expert-Data Parallelism Approach to Optimize Mixture-of-Experts Training [arXiv:2303.06318](https://arxiv.org/abs/2303.06318) and will appear at ICS 2023.
 
 
 # Videos
 1. DeepSpeed KDD 2020 Tutorial
     1. [Overview](https://www.youtube.com/watch?v=CaseqC45DNc&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=29)
     2. [ZeRO + large model training](https://www.youtube.com/watch?v=y4_bCiAsIAk&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=28)
     3. [17B T-NLG demo](https://www.youtube.com/watch?v=9V-ZbP92drg&list=PLa85ZdUjfWS21mgibJ2vCvLziprjpKoW0&index=27)
```

### Comparing `deepspeed-0.9.3/deepspeed.egg-info/SOURCES.txt` & `deepspeed-0.9.4/deepspeed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/deepspeed.egg-info/requires.txt` & `deepspeed-0.9.4/deepspeed.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -10,49 +10,49 @@
 
 [1bit]
 
 [1bit_mpi]
 mpi4py
 
 [all]
-packaging
-neural-compressor==2.1.0
-tensorboard
-torchvision
 mpi4py
-transformers
-pytest-forked
-protobuf
-xgboost
-pytest
-triton==1.0.0
 transformers[sentencepiece]
 tabulate
-clang-format==16.0.2
+sphinx
+sphinx-rtd-theme
+future
+autodoc_pydantic<2.0.0
+diffusers
+transformers
+pytest-xdist
+torch
 docutils<0.18
+pytest-forked
+tensorboard
 psutil
+xgboost
 py-cpuinfo
+tqdm
 triton==2.0.0.dev20221202
+clang-format==16.0.2
+importlib-metadata>=4
+pytest-randomly
+protobuf
+lm-eval==0.3.0
 pre-commit>=2.20.0
-sphinx-rtd-theme
-sphinx
-autodoc_pydantic<2.0.0
 wandb
+packaging
+pytest
 pydantic<2.0.0
-pytest-xdist
-importlib-metadata>=4
-hjson
+triton==1.0.0
 google
+neural-compressor==2.1.0
+hjson
 recommonmark
-tqdm
-torch
-lm-eval==0.3.0
-future
-diffusers
-pytest-randomly
+torchvision
 
 [autotuning]
 tabulate
 
 [autotuning_ml]
 hjson
 tabulate
```

### Comparing `deepspeed-0.9.3/op_builder/__init__.py` & `deepspeed-0.9.4/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/all_ops.py` & `deepspeed-0.9.4/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/async_io.py` & `deepspeed-0.9.4/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/builder.py` & `deepspeed-0.9.4/op_builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,16 @@
         return version_ge_1_1 + version_ge_1_3 + version_ge_1_5
 
     def is_compatible(self, verbose=True):
         return super().is_compatible(verbose)
 
     def builder(self):
         try:
-            assert_no_cuda_mismatch(self.name)
+            if not self.is_rocm_pytorch():
+                assert_no_cuda_mismatch(self.name)
             self.build_for_cpu = False
         except BaseException:
             self.build_for_cpu = True
 
         if self.build_for_cpu:
             from torch.utils.cpp_extension import CppExtension as ExtensionBuilder
         else:
```

### Comparing `deepspeed-0.9.3/op_builder/cpu/builder.py` & `deepspeed-0.9.4/op_builder/cpu/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,11 @@
                                    include_dirs=self.strip_empty_entries(self.include_paths()),
                                    libraries=self.strip_empty_entries(self.libraries_args()),
                                    extra_compile_args=compile_args)
 
         return cpp_ext
 
     def cxx_args(self):
-        return ['-O3', '-std=c++14', '-g', '-Wno-reorder']
+        return ['-O3', '-g', '-Wno-reorder']
 
     def libraries_args(self):
         return []
```

### Comparing `deepspeed-0.9.3/op_builder/cpu/comm.py` & `deepspeed-0.9.4/op_builder/cpu/comm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/cpu/no_impl.py` & `deepspeed-0.9.4/op_builder/cpu/no_impl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/cpu_adagrad.py` & `deepspeed-0.9.4/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/cpu_adam.py` & `deepspeed-0.9.4/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/fused_adam.py` & `deepspeed-0.9.4/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/fused_lamb.py` & `deepspeed-0.9.4/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/quantizer.py` & `deepspeed-0.9.4/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/random_ltd.py` & `deepspeed-0.9.4/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/sparse_attn.py` & `deepspeed-0.9.4/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/spatial_inference.py` & `deepspeed-0.9.4/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/stochastic_transformer.py` & `deepspeed-0.9.4/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/transformer.py` & `deepspeed-0.9.4/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/op_builder/transformer_inference.py` & `deepspeed-0.9.4/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.3/setup.py` & `deepspeed-0.9.4/setup.py`

 * *Files identical despite different names*

