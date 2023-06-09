# Comparing `tmp/optimum-intel-1.8.1.tar.gz` & `tmp/optimum-intel-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/optimum-intel-1.8.1.tar", last modified: Thu Jun  1 17:30:38 2023, max compression
+gzip compressed data, was "dist/optimum-intel-1.9.0.tar", last modified: Fri Jun  9 17:42:39 2023, max compression
```

## Comparing `optimum-intel-1.8.1.tar` & `optimum-intel-1.9.0.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9957 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.465065 optimum-intel-1.8.1/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.465065 optimum-intel-1.8.1/optimum/commands/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/commands/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/commands/neural_compressor/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/commands/neural_compressor/quantize.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/commands/register/register_inc.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     6003 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5717 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1063 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3744 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    27524 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    39213 2023-05-31 17:14:49.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10813 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3905 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     1514 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3014 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    22259 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15444 2023-05-31 17:19:54.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18165 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    19198 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    20602 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    19620 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13635 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38687 2023-05-31 17:19:54.000000 optimum-intel-1.8.1/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1278 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-01 17:28:46.000000 optimum-intel-1.8.1/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     1777 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      464 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2687 2023-05-31 17:19:02.000000 optimum-intel-1.8.1/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.014373 optimum-intel-1.9.0/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.004372 optimum-intel-1.9.0/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/intel/generation/
+-rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/generation/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/generation/modeling.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.034374 optimum-intel-1.9.0/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.034374 optimum-intel-1.9.0/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3730 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    27858 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38957 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.044374 optimum-intel-1.9.0/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15434 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18258 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    16811 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28970 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18032 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    14161 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-09 17:39:49.000000 optimum-intel-1.9.0/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-09 17:42:38.000000 optimum-intel-1.9.0/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      412 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2594 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/setup.py
```

### Comparing `optimum-intel-1.8.1/LICENSE` & `optimum-intel-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/MANIFEST.in` & `optimum-intel-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/PKG-INFO` & `optimum-intel-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.8.1
+Version: 1.9.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,57 +66,34 @@
 
 where `extras` can be one or more of `neural-compressor`, `openvino`, `nncf`.
 
 # Quick tour
 
 ## Neural Compressor
 
-#### Dynamic quantization:
+Dynamic quantization can be used through the Optimum command-line interface:
 
-Here is an example on how to apply dynamic quantization on a DistilBERT fine-tuned on the SQuAD1.0 dataset.
-Note that quantization is currently only supported for CPUs (only CPU backends are available), so we will not be utilizing GPUs / CUDA in this example.
-
-```python
-from transformers import AutoModelForQuestionAnswering
-from neural_compressor.config import PostTrainingQuantConfig
-from optimum.intel import INCQuantizer
-
-model_name = "distilbert-base-cased-distilled-squad"
-model = AutoModelForQuestionAnswering.from_pretrained(model_name)
-# The directory where the quantized model will be saved
-save_dir = "quantized_model"
-# Load the quantization configuration detailing the quantization we wish to apply
-quantization_config = PostTrainingQuantConfig(approach="dynamic")
-quantizer = INCQuantizer.from_pretrained(model)
-# Apply dynamic quantization and save the resulting model
-quantizer.quantize(quantization_config=quantization_config, save_directory=save_dir)
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
 ```
+Note that quantization is currently only supported for CPUs (only CPU backends are available), so we will not be utilizing GPUs / CUDA in this example.
 
 To load a quantized model hosted locally or on the 🤗 hub, you can do as follows :
 ```python
 from optimum.intel import INCModelForSequenceClassification
 
 # Load the PyTorch model hosted on the hub
 loaded_model_from_hub = INCModelForSequenceClassification.from_pretrained(
     "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
 )
 ```
 
-#### Apply dynamic quantization on your model using the CLI
-
-Dynamic quantization can be used through the Optimum Intel command-line:
-
-```bash
-optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
-```
-
 You can load many more quantized models hosted on the hub under the Intel organization [`here`](https://huggingface.co/Intel).
 
-
-For more details, please refer to this [guide](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc#apply-quantization-using-the-cli).
+For more details on the supported compression techniques, please refer to the [documentation](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc).
 
 
 ## OpenVINO
 
 Below are the examples of how to use OpenVINO and its [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html) framework to accelerate inference.
 
 #### Inference:
```

### Comparing `optimum-intel-1.8.1/README.md` & `optimum-intel-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,57 +37,34 @@
 
 where `extras` can be one or more of `neural-compressor`, `openvino`, `nncf`.
 
 # Quick tour
 
 ## Neural Compressor
 
-#### Dynamic quantization:
+Dynamic quantization can be used through the Optimum command-line interface:
 
-Here is an example on how to apply dynamic quantization on a DistilBERT fine-tuned on the SQuAD1.0 dataset.
-Note that quantization is currently only supported for CPUs (only CPU backends are available), so we will not be utilizing GPUs / CUDA in this example.
-
-```python
-from transformers import AutoModelForQuestionAnswering
-from neural_compressor.config import PostTrainingQuantConfig
-from optimum.intel import INCQuantizer
-
-model_name = "distilbert-base-cased-distilled-squad"
-model = AutoModelForQuestionAnswering.from_pretrained(model_name)
-# The directory where the quantized model will be saved
-save_dir = "quantized_model"
-# Load the quantization configuration detailing the quantization we wish to apply
-quantization_config = PostTrainingQuantConfig(approach="dynamic")
-quantizer = INCQuantizer.from_pretrained(model)
-# Apply dynamic quantization and save the resulting model
-quantizer.quantize(quantization_config=quantization_config, save_directory=save_dir)
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
 ```
+Note that quantization is currently only supported for CPUs (only CPU backends are available), so we will not be utilizing GPUs / CUDA in this example.
 
 To load a quantized model hosted locally or on the 🤗 hub, you can do as follows :
 ```python
 from optimum.intel import INCModelForSequenceClassification
 
 # Load the PyTorch model hosted on the hub
 loaded_model_from_hub = INCModelForSequenceClassification.from_pretrained(
     "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
 )
 ```
 
-#### Apply dynamic quantization on your model using the CLI
-
-Dynamic quantization can be used through the Optimum Intel command-line:
-
-```bash
-optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
-```
-
 You can load many more quantized models hosted on the hub under the Intel organization [`here`](https://huggingface.co/Intel).
 
-
-For more details, please refer to this [guide](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc#apply-quantization-using-the-cli).
+For more details on the supported compression techniques, please refer to the [documentation](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc).
 
 
 ## OpenVINO
 
 Below are the examples of how to use OpenVINO and its [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html) framework to accelerate inference.
 
 #### Inference:
```

### Comparing `optimum-intel-1.8.1/optimum/commands/neural_compressor/base.py` & `optimum-intel-1.9.0/optimum/commands/neural_compressor/base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/commands/neural_compressor/quantize.py` & `optimum-intel-1.9.0/optimum/commands/neural_compressor/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/commands/register/register_inc.py` & `optimum-intel-1.9.0/optimum/commands/register/register_inc.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/__init__.py` & `optimum-intel-1.9.0/optimum/intel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         "OVQuantizer",
         "OVTrainer",
         "OVTrainingArguments",
     ]
 else:
     _import_structure["openvino"].extend(["OVConfig", "OVQuantizer", "OVTrainer", "OVTrainingArguments"])
 
-
 try:
     if not (is_openvino_available() and is_diffusers_available()):
         raise OptionalDependencyNotAvailable()
 except OptionalDependencyNotAvailable:
     _import_structure["utils.dummy_openvino_and_diffusers_objects"] = ["OVStableDiffusionPipeline"]
 else:
     _import_structure["openvino"].append("OVStableDiffusionPipeline")
@@ -105,14 +104,21 @@
         "INCModelForSequenceClassification",
         "INCModelForTokenClassification",
         "INCModelForVision2Seq",
         "INCQuantizer",
         "INCSeq2SeqTrainer",
         "INCTrainer",
     ]
+try:
+    if not (is_neural_compressor_available() and is_diffusers_available()):
+        raise OptionalDependencyNotAvailable()
+except OptionalDependencyNotAvailable:
+    _import_structure["utils.dummy_neural_compressor_and_diffusers_objects"] = ["INCStableDiffusionPipeline"]
+else:
+    _import_structure["neural_compressor"].append("INCStableDiffusionPipeline")
 
 
 if TYPE_CHECKING:
     try:
         if not is_ipex_available():
             raise OptionalDependencyNotAvailable()
     except OptionalDependencyNotAvailable:
@@ -171,11 +177,20 @@
             INCModelForSequenceClassification,
             INCModelForTokenClassification,
             INCModelForVision2Seq,
             INCQuantizer,
             INCSeq2SeqTrainer,
             INCTrainer,
         )
+
+    try:
+        if not (is_neural_compressor_available() and is_diffusers_available()):
+            raise OptionalDependencyNotAvailable()
+    except OptionalDependencyNotAvailable:
+        from .utils.dummy_neural_compressor_and_diffusers_objects import INCStableDiffusionPipeline
+    else:
+        from .neural_compressor import INCStableDiffusionPipeline
+
 else:
     import sys
 
     sys.modules[__name__] = _LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `optimum-intel-1.8.1/optimum/intel/ipex/inference.py` & `optimum-intel-1.9.0/optimum/intel/ipex/inference.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import torch
 from torch import nn
 from transformers import add_start_docstrings
 from transformers.pipelines import Pipeline
 from transformers.utils import is_ipex_available
 
+from ..generation.modeling import TSModelForCausalLM, jit_trace
+
 
 logger = logging.getLogger(__name__)
 
 IPEX_NOT_AVAILABLE_ERROR_MSG = (
     "Intel PyTorch Extensions was not found."
     "please make sure you've installed the package or run "
     "pip install intel_extension_for_pytorch"
@@ -36,99 +38,119 @@
     def __getattr__(self, item):
         if not item.startswith("__"):
             return getattr(self._default, item)
         else:
             return self.item
 
 
+class _ModelGenerationWrapper(_ModelFallbackWrapper):
+    def __getattr__(self, item):
+        if not item.startswith("__"):
+            try:
+                return getattr(self._optimized, item)
+            except Exception:
+                return getattr(self._default, item)
+        else:
+            return self.item
+
+
 @add_start_docstrings(
     """
     inference_mode is an Intel specific context-manager analogous to PyTorch's inference_mode to use for inference
     workload on Intel CPUs, especially Intel Xeon Scalable CPUs.
     """,
 )
 class inference_mode:
     __slots__ = ("_model", "_dtype", "_graph_mode", "_verbose", "_original", "_jit")
 
     def __init__(
         self,
         model: Union[nn.Module, Pipeline],
         dtype: torch.dtype = torch.float32,
-        verbose: bool = False,
         jit: bool = False,
+        **kwargs,
     ):
         """
         Args:
             model (`torch.nn.Module` or `transformers.Pipeline`):
                 The model or pipeline instance to optimize.
             dtype (`torch.dtype = torch.float32`), *optional*):
                 The data type used to do the computation.
                 Acceptable type are `torch.float32` (default) and `torch.bfloat16`.
                 Please note `torch.bfloat16` requires `avx512_bf16` instructions set as present on
                 4th Generation of Intel Xeon Scalable CPUs (Sapphire Rapids).
-            verbose (`boolean = False`, *optional*):
-                Enable IPEx verbose output to see the kernels and optimizations applied.
+            jit (`boolean = False`, *optional*):
+                Enable jit to accelerate inference speed
         """
         if not is_ipex_available():
             raise ImportError(IPEX_NOT_AVAILABLE_ERROR_MSG)
 
         self._model = model
-        self._verbose = ipex.utils.verbose.VERBOSE_ON if verbose else ipex.utils.verbose.VERBOSE_OFF
         self._dtype = dtype
         self._graph_mode = False  # Let's keep for future use when it doesn't hang anymore
         self._original = None
         self._jit = jit
 
     def __enter__(self):
         if self._model.framework == "pt":
             with torch.inference_mode():
                 try:
-                    with ipex.verbose(self._verbose):
-                        ipex.enable_onednn_fusion(True)
-                        if isinstance(self._model, Pipeline):
-                            self._original = self._model.model
-
-                            model = ipex.optimize(
-                                self._model.model,
-                                dtype=self._dtype,
-                                graph_mode=self._graph_mode,
-                                level="O1",
-                                auto_kernel_selection=True,
-                            )
-
-                            # Enable automatic mixed precision (AMP) if we are going to target `bfloat16`
-                            with torch.cpu.amp.autocast(enabled=(self._dtype == torch.bfloat16)), torch.no_grad():
-                                if self._model.tokenizer is not None and self._jit:
-                                    try:
-                                        jit_inputs = []
-                                        dummy_input = self._model.tokenizer("")
-                                        for key in dummy_input:
-                                            jit_inputs.append(torch.ones((1, len(dummy_input[key])), dtype=torch.long))
-                                        model = torch.jit.trace(model, jit_inputs, strict=False)
-                                        model = torch.jit.freeze(model)
-                                        model(*jit_inputs)
-                                        model(*jit_inputs)
-                                    except Exception as e:
-                                        logger.warning(f"failed to use PyTorch jit mode due to: {e}.")
+                    ipex.enable_onednn_fusion(True)
+                    if isinstance(self._model, Pipeline):
+                        self._original = self._model.model
+
+                        model = ipex.optimize(
+                            self._model.model,
+                            dtype=self._dtype,
+                            graph_mode=self._graph_mode,
+                            level="O1",
+                            auto_kernel_selection=True,
+                        )
+
+                        # Enable automatic mixed precision (AMP) if we are going to target `bfloat16`
+                        with torch.cpu.amp.autocast(
+                            enabled=(self._dtype == torch.bfloat16 and self._original.dtype != torch.bfloat16)
+                        ), torch.no_grad():
+                            if self._jit:
+                                try:
+                                    use_cache = False
+                                    if hasattr(self._original.config, "use_cache") and self._original.config.use_cache:
+                                        use_cache = True
+                                    model = jit_trace(
+                                        model=model,
+                                        task=self._model.task,
+                                        use_cache=use_cache,
+                                    )
+                                    if self._model.task == "text-generation":
+                                        model = TSModelForCausalLM(
+                                            model=model,
+                                            config=self._original.config,
+                                            use_cache=use_cache,
+                                            model_dtype=self._original.dtype,
+                                        )
+                                except Exception as e:
+                                    logger.warning(f"failed to use PyTorch jit mode due to: {e}.")
                                 # Patching model with the new one
-                                self._model.model = _ModelFallbackWrapper(model, self._original)
-                                return self._model
-                        else:
-                            self._original = self._model
-                            model = ipex.optimize(
-                                self._model,
-                                dtype=self._dtype,
-                                graph_mode=self._graph_mode,
-                                level="O1",
-                                auto_kernel_selection=True,
-                            )
-
-                            # Enable automatic mixed precision (AMP) if we are going to target `bfloat16`
-                            with torch.cpu.amp.autocast(enabled=(self._dtype == torch.bfloat16)):
-                                return model
+                            self._model.model = _ModelGenerationWrapper(model, self._original)
+                            return self._model
+                    else:
+                        self._original = self._model
+                        model = ipex.optimize(
+                            self._model,
+                            dtype=self._dtype,
+                            graph_mode=self._graph_mode,
+                            level="O1",
+                            auto_kernel_selection=True,
+                        )
+
+                        # Enable automatic mixed precision (AMP) if we are going to target `bfloat16`
+                        with torch.cpu.amp.autocast(
+                            enabled=(self._dtype == torch.bfloat16 and self._original.dtype != torch.bfloat16)
+                        ):
+                            return model
                 except RuntimeError:
                     return self._model
         else:
             return self._model
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._model = self._original
```

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/__init__.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from ..utils.import_utils import is_diffusers_available
 from .configuration import INCConfig
 from .quantization import (
     INCModel,
     INCModelForCausalLM,
     INCModelForMaskedLM,
     INCModelForMultipleChoice,
     INCModelForQuestionAnswering,
@@ -24,7 +25,11 @@
     INCModelForTokenClassification,
     INCModelForVision2Seq,
     INCQuantizationMode,
     INCQuantizer,
 )
 from .trainer import INCTrainer
 from .trainer_seq2seq import INCSeq2SeqTrainer
+
+
+if is_diffusers_available():
+    from .modeling_diffusion import INCStableDiffusionPipeline
```

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/configuration.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Dict, Optional, Union
 
-from neural_compressor.conf.pythonic_config import DistillationConfig, WeightPruningConfig, _BaseQuantizationConfig
+from neural_compressor.config import DistillationConfig, WeightPruningConfig, _BaseQuantizationConfig
 
 from optimum.configuration_utils import BaseConfig
 
 from ..utils.import_utils import _neural_compressor_version, _torch_version
 
 
 _quantization_model = {
```

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 import inspect
 import logging
 import os
 import warnings
 from enum import Enum
 from itertools import chain
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, ClassVar, Dict, Optional, Union
+from typing import Callable, ClassVar, Dict, Optional, Union
 
 import torch
 from datasets import Dataset, load_dataset
 from huggingface_hub import HfApi, hf_hub_download
 from neural_compressor.adaptor.pytorch import PyTorch_FXAdaptor, _cfg_to_qconfig, _propagate_qconfig
+from neural_compressor.config import PostTrainingQuantConfig
 from neural_compressor.experimental.export import torch_to_int8_onnx
 from neural_compressor.model.torch_model import IPEXModel, PyTorchModel
 from neural_compressor.quantization import fit
 from neural_compressor.utils.pytorch import load
 from torch.utils.data import DataLoader, RandomSampler
 from transformers import (
     AutoConfig,
@@ -53,27 +54,23 @@
 from transformers.utils import TRANSFORMERS_CACHE, is_offline_mode
 from transformers.utils.generic import ContextManagers
 
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
 from optimum.quantization_base import OptimumQuantizer
 
-from ..utils.constant import _TASK_ALIASES
+from ..utils.constant import _TASK_ALIASES, MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, WEIGHTS_NAME
 from ..utils.import_utils import (
     _neural_compressor_version,
     _torch_version,
     is_neural_compressor_version,
     is_torch_version,
 )
 from .configuration import INCConfig
-from .utils import MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, WEIGHTS_NAME, INCDataLoader, _cfgs_to_fx_cfgs
-
-
-if TYPE_CHECKING:
-    from neural_compressor.config import PostTrainingQuantConfig
+from .utils import INCDataLoader, _cfgs_to_fx_cfgs
 
 
 logger = logging.getLogger(__name__)
 
 NEURAL_COMPRESSOR_MINIMUM_VERSION = "2.1.0"
 
 if is_neural_compressor_version("<", NEURAL_COMPRESSOR_MINIMUM_VERSION):
@@ -137,14 +134,15 @@
         self,
         quantization_config: "PostTrainingQuantConfig",
         save_directory: Union[str, Path],
         calibration_dataset: Dataset = None,
         batch_size: int = 8,
         data_collator: Optional[DataCollator] = None,
         remove_unused_columns: bool = True,
+        file_name: str = None,
         **kwargs,
     ):
         """
         Quantize a model given the optimization specifications defined in `quantization_config`.
 
         Args:
             quantization_config (`PostTrainingQuantConfig`):
@@ -159,28 +157,33 @@
                 The function to use to form a batch from a list of elements of the calibration dataset.
             remove_unused_columns (`bool`, defaults to `True`):
                 Whether or not to remove the columns unused by the model forward method.
         """
         save_directory = Path(save_directory)
         save_directory.mkdir(parents=True, exist_ok=True)
         save_onnx_model = kwargs.pop("save_onnx_model", False)
-        output_path = save_directory.joinpath(WEIGHTS_NAME)
+        output_path = save_directory.joinpath(file_name or WEIGHTS_NAME)
         calibration_dataloader = None
 
         if INCQuantizationMode(quantization_config.approach) == INCQuantizationMode.STATIC:
+            # Since PyTorch fx trace does not really require an example_inputs, only need calibration_dataset or calibration_fn here.
+            if calibration_dataset is None and self.calibration_fn is None:
+                raise ValueError(
+                    "Post-training static quantization needs a calibration dataset or a calibration_function."
+                )
             if calibration_dataset is None:
-                raise ValueError("Post-training static quantization needs a calibration dataset.")
-
-            quantization_config.calibration_sampling_size = len(calibration_dataset)
-            calibration_dataloader = self._get_calibration_dataloader(
-                calibration_dataset=calibration_dataset,
-                batch_size=batch_size,
-                remove_unused_columns=remove_unused_columns,
-                data_collator=data_collator,
-            )
+                calibration_dataloader = None
+            else:
+                quantization_config.calibration_sampling_size = len(calibration_dataset)
+                calibration_dataloader = self._get_calibration_dataloader(
+                    calibration_dataset=calibration_dataset,
+                    batch_size=batch_size,
+                    remove_unused_columns=remove_unused_columns,
+                    data_collator=data_collator,
+                )
 
         if isinstance(self._original_model.config, PretrainedConfig):
             self._original_model.config.backend = quantization_config.backend
 
         compressed_model = fit(
             self._original_model,
             conf=quantization_config,
@@ -191,15 +194,18 @@
 
         if not hasattr(compressed_model, "_model") or compressed_model._model is None:
             raise RuntimeError(
                 "The maximum number of trials specified has been reached and no quantized model meeting the specified"
                 " accuracy tolerance has been found. Either the tolerance or the number of trials need to be increased."
             )
         if isinstance(self._original_model.config, PretrainedConfig):
+            original_dtype = self._original_model.config.torch_dtype
+            self._original_model.config.torch_dtype = "int8"
             self._original_model.config.save_pretrained(save_directory)
+            self._original_model.config.torch_dtype = original_dtype
 
         self._quantized_model = compressed_model._model
 
         if save_onnx_model:
             self._set_task()
             model_type = self._original_model.config.model_type.replace("_", "-")
             model_name = getattr(self._original_model, "name", None)
@@ -224,14 +230,15 @@
     @staticmethod
     def _save_pretrained(model: Union[PyTorchModel, IPEXModel], output_path: str):
         if isinstance(model, IPEXModel):
             model._model.save(output_path)
             logger.info(f"Model weights saved to {output_path}")
             return
         state_dict = model._model.state_dict()
+
         if hasattr(model, "q_config"):
             state_dict["best_configure"] = model.q_config
         torch.save(state_dict, output_path)
         logger.info(f"Model weights saved to {output_path}")
 
     def _onnx_export(
         self,
@@ -646,15 +653,7 @@
 
 class IncQuantizedModelForXLNetLM(IncQuantizedModel):
     TRANSFORMERS_AUTO_CLASS = XLNetLMHeadModel
 
 
 class IncQuantizedModelForVision2Seq(IncQuantizedModel):
     TRANSFORMERS_AUTO_CLASS = AutoModelForVision2Seq
-
-
-class IncQuantizer(INCQuantizer):
-    # Warning at import time
-    warnings.warn(
-        "The class `IncQuantizer` has been depreciated and will be removed in optimum-intel v1.7, please use "
-        "`INCQuantizer` instead.",
-    )
```

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #  limitations under the License.
 
 import copy
 import math
 import os
 import sys
 import time
-import warnings
 from collections.abc import Mapping
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import datasets
 import torch
 import torch.distributed as dist
@@ -60,18 +59,17 @@
     speed_metrics,
 )
 from transformers.training_args import TrainingArguments
 from transformers.utils import is_apex_available, is_sagemaker_mp_enabled, logging
 
 from optimum.exporters import TasksManager
 
-from ..utils.constant import _TASK_ALIASES
+from ..utils.constant import _TASK_ALIASES, MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, TRAINING_ARGS_NAME
 from ..utils.import_utils import is_neural_compressor_version
 from .configuration import INCConfig
-from .utils import MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, TRAINING_ARGS_NAME
 
 
 if is_apex_available():
     from apex import amp
 
 if is_sagemaker_mp_enabled():
     import smdistributed.modelparallel.torch as smp
@@ -157,18 +155,18 @@
 
         if len(inc_config) >= 1 and self.args.do_train:
             inc_config = inc_config if len(inc_config) > 1 else inc_config.pop()
             self._compression_manager = training.prepare_compression(self.model, confs=inc_config)
             self.model = self._compression_manager.model.model
             self.model_wrapped = self.model
 
-        for callback in self._compression_manager.callbacks.callbacks_list:
-            if isinstance(callback, DistillationCallbacks):
-                self.distillation_callback = callback
-                break
+            for callback in self._compression_manager.callbacks.callbacks_list:
+                if isinstance(callback, DistillationCallbacks):
+                    self.distillation_callback = callback
+                    break
 
         self.inc_config = INCConfig(
             quantization=self.quantization_config,
             pruning=self.pruning_config,
             distillation=self.distillation_config,
             save_onnx_model=save_onnx_model,
         )
@@ -808,15 +806,7 @@
         return super().predict(*args, **kwargs)
 
     def get_model_sparsity(self):
         sparsity = 0.0
         if self._compression_manager is not None:
             sparsity = self._compression_manager.model.report_sparsity()[-1]
         return sparsity
-
-
-class IncTrainer(INCTrainer):
-    # Warning at import time
-    warnings.warn(
-        "The class `IncTrainer` has been depreciated and will be removed in optimum-intel v1.7, please use "
-        "`INCTrainer` instead.",
-    )
```

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
             )
 
         has_labels = "labels" in inputs
         inputs = self._prepare_inputs(inputs)
 
         # XXX: adapt synced_gpus for fairscale as well
         gen_kwargs = {
-            "max_length": self._max_length if self._max_length is not None else self.config.max_length,
-            "num_beams": self._num_beams if self._num_beams is not None else self.config.num_beams,
+            "max_length": self._max_length if self._max_length is not None else self.model.config.max_length,
+            "num_beams": self._num_beams if self._num_beams is not None else self.model.config.num_beams,
             "synced_gpus": True if is_deepspeed_zero3_enabled() else False,
         }
 
         if "attention_mask" in inputs:
             gen_kwargs["attention_mask"] = inputs.get("attention_mask", None)
         if "global_attention_mask" in inputs:
             gen_kwargs["global_attention_mask"] = inputs.get("global_attention_mask", None)
@@ -206,16 +206,16 @@
     def _pad_tensors_to_max_len(self, tensor, max_length):
         if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
             # If PAD token is not defined at least EOS token has to be defined
             pad_token_id = (
                 self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
             )
         else:
-            if self.config.pad_token_id is not None:
-                pad_token_id = self.config.pad_token_id
+            if self.model.config.pad_token_id is not None:
+                pad_token_id = self.model.config.pad_token_id
             else:
                 raise ValueError("Pad_token_id must be set in the configuration of the model, in order to pad tensors")
 
         padded_tensor = pad_token_id * torch.ones(
             (tensor.shape[0], max_length), dtype=tensor.dtype, device=tensor.device
         )
         padded_tensor[:, : tensor.shape[-1]] = tensor
```

### Comparing `optimum-intel-1.8.1/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.9.0/optimum/intel/neural_compressor/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,42 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import os
+import warnings
 from collections import UserDict
 from typing import Dict
 
 import torch
 from neural_compressor.utils.pytorch import load
 from packaging import version
 from torch.utils.data import DataLoader
 
+from ..utils.constant import WEIGHTS_NAME
+
 
 logger = logging.getLogger(__name__)
 
 
 CONFIG_NAME = "best_configure.yaml"
-WEIGHTS_NAME = "pytorch_model.bin"
-TRAINING_ARGS_NAME = "training_args.bin"
-ONNX_WEIGHTS_NAME = "model.onnx"
-MIN_QDQ_ONNX_OPSET = 14
+
+_HEAD_TO_AUTOMODELS = {
+    "fill-mask": "INCModelForMaskedLM",
+    "text-generation": "INCModelForCausalLM",
+    "text2text-generation": "INCModelForSeq2SeqLM",
+    "text-classification": "INCModelForSequenceClassification",
+    "token-classification": "INCModelForTokenClassification",
+    "question-answering": "INCModelForQuestionAnswering",
+    "multiple-choice": "INCModelForMultipleChoice",
+    "stable-diffusion": "INCStableDiffusionPipeline",
+}
+
 
 parsed_torch_version_base = version.parse(version.parse(torch.__version__).base_version)
 is_torch_less_than_1_13 = parsed_torch_version_base < version.parse("1.13.0")
 
 
 class INCDataLoader(DataLoader):
     @classmethod
@@ -98,13 +109,14 @@
 
     Arguments:
         checkpoint_dir_or_file (`str`):
             The path to the model checkpoint containing the quantization information.
         model (`torch.nn.Module`):
             The original FP32 model.
     """
+    warnings.warn("This function has been depreciated and will be removed in optimum-intel v1.9.")
     if os.path.isdir(checkpoint_dir_or_file):
         checkpoint_dir_or_file = os.path.join(
             os.path.abspath(os.path.expanduser(checkpoint_dir_or_file)), WEIGHTS_NAME
         )
 
     return load(checkpoint_dir_or_file, model, **kwargs)
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/__init__.py` & `optimum-intel-1.9.0/optimum/intel/openvino/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import logging
 
 from ..utils.import_utils import is_diffusers_available, is_nncf_available
 from .utils import OV_DECODER_NAME, OV_DECODER_WITH_PAST_NAME, OV_ENCODER_NAME, OV_XML_FILE_NAME
 
 
 if is_nncf_available():
+    import nncf
+
+    # Suppress version mismatch logging
+    nncf.set_log_level(logging.ERROR)
     from nncf.torch import patch_torch_operators
 
+    nncf.set_log_level(logging.INFO)
+
     patch_torch_operators()
 
     from .configuration import OVConfig
     from .quantization import OVQuantizer
     from .trainer import OVTrainer
     from .training_args import OVTrainingArguments
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/configuration.py` & `optimum-intel-1.9.0/optimum/intel/openvino/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,18 +52,18 @@
         super().__init__()
         self.compression = compression or DEFAULT_QUANTIZATION_CONFIG
         self.input_info = input_info
         self.save_onnx_model = save_onnx_model
         self._enable_standard_onnx_export_option()
         self.optimum_version = kwargs.pop("optimum_version", None)
 
-    def add_input_info(self, model_inputs: Dict):
+    def add_input_info(self, model_inputs: Dict, force_batch_one: bool = False):
         self.input_info = [
             {
-                "sample_size": list(value.shape),
+                "sample_size": [1] + list(value.shape[1:]) if force_batch_one else list(value.shape),
                 "type": "long" if value.dtype is torch.int64 else "float",
                 "keyword": name,
             }
             for name, value in model_inputs.items()
         ]
 
     def _enable_standard_onnx_export_option(self):
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/modeling.py` & `optimum-intel-1.9.0/optimum/intel/openvino/modeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,16 +174,15 @@
         }
 
         # Add the token_type_ids when needed
         if "token_type_ids" in self.input_names:
             inputs["token_type_ids"] = token_type_ids
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
+        outputs = self.request(inputs)
         logits = torch.from_numpy(outputs["logits"]).to(self.device) if not np_inputs else outputs["logits"]
         return SequenceClassifierOutput(logits=logits)
 
 
 QUESTION_ANSWERING_EXAMPLE = r"""
     Example of question answering using `transformers.pipeline`:
     ```python
@@ -241,16 +240,15 @@
         }
 
         # Add the token_type_ids when needed
         if "token_type_ids" in self.input_names:
             inputs["token_type_ids"] = token_type_ids
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
+        outputs = self.request(inputs)
         start_logits = (
             torch.from_numpy(outputs["start_logits"]).to(self.device) if not np_inputs else outputs["start_logits"]
         )
         end_logits = (
             torch.from_numpy(outputs["end_logits"]).to(self.device) if not np_inputs else outputs["end_logits"]
         )
         return QuestionAnsweringModelOutput(start_logits=start_logits, end_logits=end_logits)
@@ -312,16 +310,15 @@
         }
 
         # Add the token_type_ids when needed
         if "token_type_ids" in self.input_names:
             inputs["token_type_ids"] = token_type_ids
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
+        outputs = self.request(inputs)
         logits = torch.from_numpy(outputs["logits"]).to(self.device) if not np_inputs else outputs["logits"]
         return TokenClassifierOutput(logits=logits)
 
 
 FEATURE_EXTRACTION_EXAMPLE = r"""
     Example of feature extraction using `transformers.pipelines`:
     ```python
@@ -378,21 +375,20 @@
         }
 
         # Add the token_type_ids when needed
         if "token_type_ids" in self.input_names:
             inputs["token_type_ids"] = token_type_ids
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
-
-        last_hidden_state = outputs["last_hidden_state"]
-        if not np_inputs:
-            last_hidden_state = torch.from_numpy(last_hidden_state).to(self.device)
-
+        outputs = self.request(inputs)
+        last_hidden_state = (
+            torch.from_numpy(outputs["last_hidden_state"]).to(self.device)
+            if not np_inputs
+            else outputs["last_hidden_state"]
+        )
         return BaseModelOutput(last_hidden_state=last_hidden_state)
 
 
 MASKED_LM_EXAMPLE = r"""
     Example of masked language modeling using `transformers.pipelines`:
     ```python
     >>> from transformers import {processor_class}, pipeline
@@ -449,16 +445,15 @@
         }
 
         # Add the token_type_ids when needed
         if "token_type_ids" in self.input_names:
             inputs["token_type_ids"] = token_type_ids
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
+        outputs = self.request(inputs)
         logits = torch.from_numpy(outputs["logits"]).to(self.device) if not np_inputs else outputs["logits"]
         return MaskedLMOutput(logits=logits)
 
 
 IMAGE_CLASSIFICATION_EXAMPLE = r"""
     Example of image classification using `transformers.pipelines`:
     ```python
@@ -508,16 +503,15 @@
             pixel_values = np.array(pixel_values)
 
         inputs = {
             "pixel_values": pixel_values,
         }
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
+        outputs = self.request(inputs)
         logits = torch.from_numpy(outputs["logits"]).to(self.device) if not np_inputs else outputs["logits"]
         return ImageClassifierOutput(logits=logits)
 
 
 AUDIO_CLASSIFICATION_EXAMPLE = r"""
     Example of audio classification using `transformers.pipelines`:
     ```python
@@ -574,11 +568,10 @@
         }
 
         # Add the attention_mask when needed
         if "attention_mask" in self.input_names:
             inputs["attention_mask"] = attention_mask
 
         # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
+        outputs = self.request(inputs)
         logits = torch.from_numpy(outputs["logits"]).to(self.device) if not np_inputs else outputs["logits"]
         return SequenceClassifierOutput(logits=logits)
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.9.0/optimum/intel/openvino/modeling_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,15 @@
         use_auth_token: Optional[Union[bool, str]] = None,
         revision: Optional[str] = None,
         force_download: bool = False,
         cache_dir: Optional[str] = None,
         subfolder: str = "",
         local_files_only: bool = False,
         task: Optional[str] = None,
+        trust_remote_code: bool = False,
         **kwargs,
     ):
         """
         Export a vanilla Transformers model into an ONNX model using `transformers.onnx.export_onnx`.
 
         Arguments:
             model_id (`str` or `Path`):
@@ -268,14 +269,15 @@
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
             "cache_dir": cache_dir,
             "subfolder": subfolder,
             "local_files_only": local_files_only,
             "force_download": force_download,
+            "trust_remote_code": trust_remote_code,
         }
 
         model = TasksManager.get_model_from_task(task, model_id, **model_kwargs)
 
         model_type = model.config.model_type.replace("_", "-")
         onnx_config_class = TasksManager.get_exporter_config_constructor(
             exporter="onnx",
@@ -307,19 +309,18 @@
             cache_dir=cache_dir,
             local_files_only=local_files_only,
             **kwargs,
         )
 
     def compile(self):
         if self.request is None:
-            logger.info("Compiling the model and creating the inference request ...")
+            logger.info("Compiling the model...")
             cache_dir = Path(self.model_save_dir).joinpath("model_cache")
             ov_config = {**self.ov_config, "CACHE_DIR": str(cache_dir)}
-            compiled_model = core.compile_model(self.model, self._device, ov_config)
-            self.request = compiled_model.create_infer_request()
+            self.request = core.compile_model(self.model, self._device, ov_config)
 
     def _reshape(
         self,
         model: openvino.runtime.Model,
         batch_size: int,
         sequence_length: int,
         height: int = None,
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.9.0/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,15 @@
         revision: Optional[str] = None,
         force_download: bool = False,
         cache_dir: Optional[str] = None,
         subfolder: str = "",
         local_files_only: bool = False,
         task: Optional[str] = None,
         use_cache: bool = True,
+        trust_remote_code: bool = False,
         **kwargs,
     ):
         """
         Export a vanilla Transformers model into an ONNX model using `transformers.onnx.export_onnx`.
 
         Arguments:
             model_id (`str` or `Path`):
@@ -306,14 +307,15 @@
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
             "cache_dir": cache_dir,
             "subfolder": subfolder,
             "local_files_only": local_files_only,
             "force_download": force_download,
+            "trust_remote_code": trust_remote_code,
         }
 
         model = TasksManager.get_model_from_task(task, model_id, **model_kwargs)
         onnx_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="onnx", task=task)
         onnx_config = onnx_config_constructor(model.config, use_past=use_cache)
         models_and_onnx_configs = get_encoder_decoder_models_for_export(model, onnx_config)
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/modeling_decoder.py` & `optimum-intel-1.9.0/optimum/intel/openvino/modeling_decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from tempfile import TemporaryDirectory
 from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 import openvino
 import torch
 from openvino.runtime import Core, Tensor
-from transformers import AutoConfig, AutoModelForCausalLM, PretrainedConfig
+from transformers import AutoModelForCausalLM, PretrainedConfig
 from transformers.file_utils import add_start_docstrings, add_start_docstrings_to_model_forward
 from transformers.modeling_outputs import CausalLMOutputWithPast
 
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import export
-from optimum.utils import NormalizedConfig, NormalizedConfigManager
+from optimum.utils import NormalizedConfigManager
 
 from ..utils.import_utils import is_transformers_version
-from .modeling import _TOKENIZER_FOR_DOC, INPUTS_DOCSTRING, MODEL_START_DOCSTRING
-from .modeling_base import OVBaseModel
+from ..utils.modeling_utils import _prepare_attn_mask, _prepare_decoder_attention_mask
+from .modeling import _TOKENIZER_FOR_DOC, INPUTS_DOCSTRING, MODEL_START_DOCSTRING, OVModel
 from .utils import ONNX_WEIGHTS_NAME
 
 
 if is_transformers_version("<", "4.25.0"):
     from transformers.generation_utils import GenerationMixin
 else:
     from transformers.generation import GenerationMixin
@@ -68,92 +68,76 @@
     >>> gen_pipeline = pipeline("text-generation", model=model, tokenizer=tokenizer)
     >>> text = "I love this story because"
     >>> gen = gen_pipeline(text)
     ```
 """
 
 
-def _contiguous_helper(tensor: np.ndarray) -> np.ndarray:
-    return tensor if tensor.flags["C_CONTIGUOUS"] else np.ascontiguousarray(tensor)
-
-
 @add_start_docstrings(
     """
     Base OVBaseDecoderModel class.
     """,
 )
-class OVBaseDecoderModel(OVBaseModel):
+class OVBaseDecoderModel(OVModel):
     def __init__(
         self,
         model: openvino.runtime.Model,
         config: PretrainedConfig = None,
         device: str = "CPU",
         dynamic_shapes: bool = True,
         ov_config: Optional[Dict[str, str]] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         **kwargs,
     ):
-        self.config = config
-        self.use_cache = any("past_key_values" in key.get_any_name() for key in model.inputs)
-        self.model_save_dir = model_save_dir
-        self._device = device.upper()
-        self.is_dynamic = True
-        self.ov_config = ov_config if ov_config is not None else {}
-        self.preprocessors = kwargs.get("preprocessors", [])
-        self.model = self._reshape(model, -1, -1)
-        self.device = torch.device("cpu")
-        self.main_input_name = "input_ids"
-        enable_compilation = kwargs.get("compile", True)
-        normalized_config = NormalizedConfigManager.get_normalized_config_class(config.model_type)(config)
-        self.decoder = OVDecoder(self.model, self._device, self.use_cache, self.ov_config, normalized_config)
-
-        if enable_compilation:
-            self.compile()
-
-        if is_transformers_version("<=", "4.25.1"):
-            self.generation_config = None
-        else:
-            from transformers import GenerationConfig
-
-            self.generation_config = GenerationConfig.from_model_config(config)
+        if not dynamic_shapes:
+            raise ValueError(
+                "`dynamic_shapes` was set to `False` but static shapes are not supported for causal language model. Please set `dynamic_shapes=True`."
+            )
 
-        # Avoid warnings when creating a transformers pipeline
-        AutoConfig.register(self.base_model_prefix, AutoConfig)
-        self.auto_model_class.register(AutoConfig, self.__class__)
+        super().__init__(
+            model,
+            config,
+            device=device,
+            dynamic_shapes=True,
+            ov_config=ov_config,
+            model_save_dir=model_save_dir,
+            **kwargs,
+        )
 
         use_cache = kwargs.pop("use_cache", True)
+        self.use_cache = any("past_key_values" in key.get_any_name() for key in model.inputs)
+        self.main_input_name = "input_ids"
+        self.num_pkv = 2
+        self.normalized_config = NormalizedConfigManager.get_normalized_config_class(config.model_type)(config)
+        self.output_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.outputs)}
+        self.key_value_input_names = [key for key in self.input_names if "key_values" in key]
+        self.key_value_output_names = [key for key in self.output_names if "present" in key]
+
         if use_cache ^ self.use_cache:
             raise ValueError(
                 f"`use_cache` was set to `{use_cache}` but the loaded model only supports `use_cache={self.use_cache}`. "
                 f"Please load your current model with `use_cache={self.use_cache}` or export the original model "
                 f"once again with `use_cache={use_cache}` when calling the `from_pretrained` method. "
                 "To export your model, simply set `export=True`."
             )
 
-        if not dynamic_shapes:
-            logger.warning(
-                "`dynamic_shapes` was set to `False` but static shapes are not supported for causal language model and will be ignored."
-            )
-
-    def compile(self):
-        self.decoder._create_inference_request()
-
     @classmethod
     def _from_transformers(
         cls,
         model_id: str,
         config: PretrainedConfig,
         use_auth_token: Optional[Union[bool, str]] = None,
         revision: Optional[str] = None,
         force_download: bool = False,
         cache_dir: Optional[str] = None,
         subfolder: str = "",
         local_files_only: bool = False,
         task: Optional[str] = None,
         use_cache: bool = True,
+        trust_remote_code: bool = False,
         **kwargs,
     ):
         model_file_name = ONNX_WEIGHTS_NAME
 
         if task is None:
             task = cls._auto_model_to_task(cls.auto_model_class)
 
@@ -162,19 +146,27 @@
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
             "cache_dir": cache_dir,
             "subfolder": subfolder,
             "local_files_only": local_files_only,
             "force_download": force_download,
+            "trust_remote_code": trust_remote_code,
         }
         model = TasksManager.get_model_from_task(task, model_id, **model_kwargs)
         onnx_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="onnx", task=task)
         onnx_config = onnx_config_constructor(model.config, use_past=use_cache)
 
+        # TODO : create ModelPatcher to patch each architecture
+        if model.config.model_type == "bloom":
+            model.transformer._prepare_attn_mask = _prepare_attn_mask
+
+        if model.config.model_type == "llama":
+            model.model._prepare_decoder_attention_mask = _prepare_decoder_attention_mask
+
         # Export the model to the ONNX format
         export(model=model, config=onnx_config, output=save_dir_path / model_file_name)
 
         return cls._from_pretrained(
             model_id=save_dir_path,
             config=config,
             from_onnx=True,
@@ -184,15 +176,28 @@
             cache_dir=cache_dir,
             file_name=model_file_name,
             local_files_only=local_files_only,
             use_cache=use_cache,
             **kwargs,
         )
 
-    def _reshape(self, model: openvino.runtime.Model, batch_size: int, sequence_length: int, is_decoder=True):
+    def _reshape(
+        self,
+        model: openvino.runtime.Model,
+        batch_size: int,
+        sequence_length: int,
+        height: int = None,
+        width: int = None,
+    ):
+        if height is not None:
+            logger.warning(f"`height` set to `{height}` will be ignored during reshaping operation.")
+
+        if width is not None:
+            logger.warning(f"`width` set to `{width}` will be ignored during reshaping operation.")
+
         shapes = {}
         for inputs in model.inputs:
             shapes[inputs] = inputs.get_partial_shape()
             shapes[inputs][0] = -1
             input_name = inputs.get_any_name()
             if input_name.startswith("past_key_values"):
                 if len(inputs.partial_shape) == 3 and input_name.endswith("value"):
@@ -204,27 +209,14 @@
         model.reshape(shapes)
         return model
 
     def reshape(self, batch_size: int, sequence_length: int):
         logger.warning("Static shapes are not supported for causal language model.")
         return self
 
-    def to(self, device: str):
-        """
-        Use the specified `device` for inference. For example: "cpu" or "gpu". `device` can
-        be in upper or lower case. To speed up first inference, call `.compile()` after `.to()`.
-        """
-        self._device = device.upper()
-        self.decoder._device = device.upper()
-        self.decoder.request = None
-        return self
-
-    def forward(self, *args, **kwargs):
-        raise NotImplementedError
-
 
 @add_start_docstrings(
     """
     OpenVINO Model with a causal language modeling head on top (linear layer with weights tied to the input
     embeddings).
     """,
     MODEL_START_DOCSTRING,
@@ -239,28 +231,73 @@
             processor_class=_TOKENIZER_FOR_DOC,
             model_class="OVModelForCausalLM",
             checkpoint="gpt2",
         )
     )
     def forward(
         self,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
+        input_ids: torch.LongTensor,
+        attention_mask: Optional[torch.LongTensor] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
         **kwargs,
     ) -> CausalLMOutputWithPast:
+        self.compile()
+
         if self.use_cache and past_key_values is not None:
             input_ids = input_ids[:, -1:]
 
-        outputs = self.decoder(
-            input_ids=input_ids,
-            past_key_values=past_key_values,
-            attention_mask=attention_mask,
-        )
-        return CausalLMOutputWithPast(logits=outputs.logits, past_key_values=outputs.past_key_values)
+        inputs = {}
+        if past_key_values is not None:
+            # Flatten the past_key_values
+            past_key_values = tuple(
+                np.array(past_key_value) for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer
+            )
+            # Add the past_key_values to the decoder inputs
+            inputs = dict(zip(self.key_value_input_names, past_key_values))
+
+        # Create empty past_key_values for decoder_with_past first generation step
+        elif self.use_cache:
+            shape_input_ids = input_ids.shape
+            num_attention_heads = (
+                self.normalized_config.num_attention_heads if self.config.model_type == "bloom" else 1
+            )
+            for input_name in self.key_value_input_names:
+                model_inputs = self.model.input(input_name)
+                shape = model_inputs.get_partial_shape()
+                shape[0] = shape_input_ids[0] * num_attention_heads
+                if shape[2].is_dynamic:
+                    shape[2] = 0
+                if shape[1].is_dynamic:
+                    shape[1] = 0
+                inputs[input_name] = Tensor(model_inputs.get_element_type(), shape.get_shape())
+
+        inputs["input_ids"] = np.array(input_ids)
+
+        # Add the attention_mask inputs when needed
+        if "attention_mask" in self.input_names and attention_mask is not None:
+            inputs["attention_mask"] = np.array(attention_mask)
+
+        # Run inference
+        outputs = self.request(inputs, shared_memory=True)
+
+        logits = torch.from_numpy(outputs["logits"]).to(self.device)
+
+        if self.use_cache:
+            # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the self-attention layer)
+            past_key_values = tuple(
+                torch.from_numpy(outputs[key]).to(self.device) for key in self.key_value_output_names
+            )
+            # Tuple of tuple of length `n_layers`, with each tuple of length equal to 2 (k/v of self-attention)
+            past_key_values = tuple(
+                past_key_values[i : i + self.num_pkv] for i in range(0, len(past_key_values), self.num_pkv)
+            )
+        else:
+            past_key_values = None
+
+        return CausalLMOutputWithPast(logits=logits, past_key_values=past_key_values)
 
     # Adapted from transformers.models.gpt2.modeling_gpt2.GPT2LMHeadModel.prepare_inputs_for_generation
     def prepare_inputs_for_generation(self, input_ids, past_key_values=None, **kwargs):
         past_key_values = past_key_values or kwargs.get("past", None)
 
         # `past_key_values` may be in the stardard format (e.g. in contrastive search), converts to bloom's format if needed
         if past_key_values is not None and self.config.model_type == "bloom":
@@ -358,99 +395,7 @@
             )
             for layer_past in past_key_value
         )
 
     def can_generate(self):
         """Returns True to validate the check that the model using `GenerationMixin.generate()` can indeed generate."""
         return True
-
-
-class OVDecoder:
-    def __init__(
-        self, model: openvino.runtime.Model, device: str, use_cache: bool, ov_config: Dict, config: NormalizedConfig
-    ):
-        self.model = model
-        self._device = device
-        self.device = torch.device("cpu")
-        self.input_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.inputs)}
-        self.output_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.outputs)}
-        self.key_value_input_names = [key for key in self.input_names if "key_values" in key]
-        self.key_value_output_names = [key for key in self.output_names if "present" in key]
-        self.use_cache = use_cache
-        self.num_pkv = 2
-        self.ov_config = ov_config
-        self.config = config
-        self.request = None
-
-    def forward(
-        self,
-        input_ids: torch.LongTensor,
-        attention_mask: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
-    ) -> CausalLMOutputWithPast:
-        self._create_inference_request()
-
-        inputs = {}
-        if past_key_values is not None:
-            # Flatten the past_key_values
-            past_key_values = tuple(
-                _contiguous_helper(np.array(past_key_value))
-                for pkv_per_layer in past_key_values
-                for past_key_value in pkv_per_layer
-            )
-            # Add the past_key_values to the decoder inputs
-            inputs = {
-                input_name: Tensor(past_key_value, shared_memory=True)
-                for input_name, past_key_value in zip(self.key_value_input_names, past_key_values)
-            }
-
-        # Create empty past_key_values for decoder_with_past first generation step
-        elif self.use_cache:
-            shape_input_ids = input_ids.shape
-            num_attention_heads = self.config.num_attention_heads if self.config.config.model_type == "bloom" else 1
-            for input_name in self.key_value_input_names:
-                model_inputs = self.model.input(input_name)
-                shape = model_inputs.get_partial_shape()
-                shape[0] = shape_input_ids[0] * num_attention_heads
-                if shape[2].is_dynamic:
-                    shape[2] = 0
-                if shape[1].is_dynamic:
-                    shape[1] = 0
-                inputs[input_name] = Tensor(model_inputs.get_element_type(), shape.get_shape())
-
-        inputs["input_ids"] = np.array(input_ids)
-
-        # Add the attention_mask inputs when needed
-        if "attention_mask" in self.input_names and attention_mask is not None:
-            inputs["attention_mask"] = np.array(attention_mask)
-
-        # Run inference
-        self.request.start_async(inputs)
-        self.request.wait()
-
-        outputs = {
-            key.get_any_name(): value.data for key, value in zip(self.request.model_outputs, self.request.outputs)
-        }
-        logits = torch.from_numpy(outputs["logits"]).to(self.device)
-
-        if self.use_cache:
-            # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the self-attention layer)
-            past_key_values = tuple(
-                torch.from_numpy(outputs[key]).to(self.device) for key in self.key_value_output_names
-            )
-            # Tuple of tuple of length `n_layers`, with each tuple of length equal to 2 (k/v of self-attention)
-            past_key_values = tuple(
-                past_key_values[i : i + self.num_pkv] for i in range(0, len(past_key_values), self.num_pkv)
-            )
-        else:
-            past_key_values = None
-
-        return CausalLMOutputWithPast(logits=logits, past_key_values=past_key_values)
-
-    def __call__(self, *args, **kwargs):
-        return self.forward(*args, **kwargs)
-
-    def _create_inference_request(self):
-        if self.request is None:
-            logger.info("Compiling the decoder and creating the inference request ...")
-            compiled_model = core.compile_model(self.model, self._device, self.ov_config)
-            self.request = compiled_model.create_infer_request()
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.9.0/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,496 +8,428 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import importlib
 import logging
-import os
 from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Any, Dict, Optional, Union
+from typing import Dict, Optional, Tuple
 
-import numpy as np
 import openvino
-from diffusers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler, StableDiffusionPipeline
-from diffusers.schedulers.scheduling_utils import SCHEDULER_CONFIG_NAME
-from diffusers.utils import CONFIG_NAME
-from huggingface_hub import snapshot_download
-from openvino._offline_transformations import compress_model_transformation
+import torch
+import transformers
 from openvino.runtime import Core
-from transformers import CLIPFeatureExtractor, CLIPTokenizer
+from transformers import AutoConfig, AutoModelForSeq2SeqLM
+from transformers.file_utils import add_start_docstrings, add_start_docstrings_to_model_forward
+from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
+
+from ..utils.import_utils import is_transformers_version
+from .modeling_base_seq2seq import OVBaseModelForSeq2SeqLM
 
-from optimum.exporters import TasksManager
-from optimum.exporters.onnx import export_models, get_stable_diffusion_models_for_export
-from optimum.pipelines.diffusers.pipeline_stable_diffusion import StableDiffusionPipelineMixin
-from optimum.utils import (
-    DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER,
-    DIFFUSION_MODEL_UNET_SUBFOLDER,
-    DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER,
-    DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER,
-)
-
-from .modeling_base import OVBaseModel
-from .utils import ONNX_WEIGHTS_NAME, OV_TO_NP_TYPE, OV_XML_FILE_NAME
 
+if is_transformers_version("<", "4.25.0"):
+    from transformers.generation_utils import GenerationMixin
+else:
+    from transformers.generation import GenerationMixin
 
 core = Core()
 
 logger = logging.getLogger(__name__)
 
+_TOKENIZER_FOR_DOC = "AutoTokenizer"
 
-class OVStableDiffusionPipeline(OVBaseModel, StableDiffusionPipelineMixin):
-    auto_model_class = StableDiffusionPipeline
-    config_name = "model_index.json"
-    export_feature = "stable-diffusion"
+INPUTS_DOCSTRING = r"""
+    Arguments:
+        encoder (`openvino.runtime.Model`):
+            The OpenVINO Runtime model associated to the encoder.
+        decoder (`openvino.runtime.Model`):
+            The OpenVINO Runtime model associated to the decoder.
+        decoder_with_past (`openvino.runtime.Model`):
+            The OpenVINO Runtime model associated  to the decoder with past key values.
+        config (`transformers.PretrainedConfig`):
+            [PretrainedConfig](https://huggingface.co/docs/transformers/main_classes/configuration#transformers.PretrainedConfig)
+            is an instance of the configuration associated to the model. Initializing with a config file does
+            not load the weights associated with the model, only the configuration.
+"""
+
+ENCODER_INPUTS_DOCSTRING = r"""
+    Arguments:
+        input_ids (`torch.LongTensor`):
+            Indices of input sequence tokens in the vocabulary of shape `(batch_size, encoder_sequence_length)`.
+        attention_mask (`torch.LongTensor`):
+            Mask to avoid performing attention on padding token indices, of shape
+            `(batch_size, encoder_sequence_length)`. Mask values selected in `[0, 1]`.
+"""
+
+
+DECODER_INPUTS_DOCSTRING = r"""
+    Arguments:
+        input_ids (`torch.LongTensor`):
+            Indices of decoder input sequence tokens in the vocabulary of shape `(batch_size, decoder_sequence_length)`.
+        encoder_hidden_states (`torch.FloatTensor`):
+            The encoder `last_hidden_state` of shape `(batch_size, encoder_sequence_length, hidden_size)`.
+        encoder_attention_mask (`torch.LongTensor`, *optional*):
+            Mask to avoid performing cross-attention on padding tokens indices of encoder `input_ids`.
+        past_key_values (`tuple(tuple(torch.FloatTensor), *optional*)`
+            Contains the precomputed key and value hidden states of the attention blocks used to speed up decoding.
+            The tuple is of length `config.n_layers` with each tuple having 2 tensors of shape
+            `(batch_size, num_heads, decoder_sequence_length, embed_size_per_head)` and 2 additional tensors of shape
+            `(batch_size, num_heads, encoder_sequence_length, embed_size_per_head)`.
+"""
+
+SEQ2SEQ_MODEL_DOCSTRING = r"""
+    Arguments:
+        input_ids (`torch.LongTensor`):
+            Indices of input sequence tokens in the vocabulary of shape `(batch_size, encoder_sequence_length)`.
+        attention_mask (`torch.LongTensor`):
+            Mask to avoid performing attention on padding token indices, of shape
+            `(batch_size, encoder_sequence_length)`. Mask values selected in `[0, 1]`.
+        decoder_input_ids (`torch.LongTensor`):
+            Indices of decoder input sequence tokens in the vocabulary of shape `(batch_size, decoder_sequence_length)`.
+        encoder_outputs (`torch.FloatTensor`):
+            The encoder `last_hidden_state` of shape `(batch_size, encoder_sequence_length, hidden_size)`.
+        past_key_values (`tuple(tuple(torch.FloatTensor), *optional*)`
+            Contains the precomputed key and value hidden states of the attention blocks used to speed up decoding.
+            The tuple is of length `config.n_layers` with each tuple having 2 tensors of shape
+            `(batch_size, num_heads, decoder_sequence_length, embed_size_per_head)` and 2 additional tensors of shape
+            `(batch_size, num_heads, encoder_sequence_length, embed_size_per_head)`.
+"""
+
+
+TRANSLATION_EXAMPLE = r"""
+    Example of text generation:
+    ```python
+    >>> from transformers import {processor_class}
+    >>> from optimum.intel import {model_class}
+
+    >>> tokenizer = {processor_class}.from_pretrained("{checkpoint}")
+    >>> model = {model_class}.from_pretrained("{checkpoint}")
+    >>> text = "He never went out without a book under his arm, and he often came back with two."
+    >>> inputs = tokenizer(text, return_tensors="pt")
+    >>> gen_tokens = model.generate(**inputs)
+    >>> outputs = tokenizer.batch_decode(gen_tokens)
+    ```
+
+    Example using `transformers.pipeline`:
+    ```python
+    >>> from transformers import {processor_class}, pipeline
+    >>> from optimum.intel import {model_class}
+
+    >>> tokenizer = {processor_class}.from_pretrained("{checkpoint}")
+    >>> model = {model_class}.from_pretrained("{checkpoint}")
+    >>> pipe = pipeline("translation_en_to_fr", model=model, tokenizer=tokenizer)
+    >>> text = "He never went out without a book under his arm, and he often came back with two."
+    >>> outputs = pipe(text)
+    ```
+"""
+
+
+@add_start_docstrings(
+    """
+    Sequence-to-sequence model with a language modeling head for OpenVINO inference.
+    """,
+    INPUTS_DOCSTRING,
+)
+class OVModelForSeq2SeqLM(OVBaseModelForSeq2SeqLM, GenerationMixin):
+    auto_model_class = AutoModelForSeq2SeqLM
 
     def __init__(
         self,
-        vae_decoder: openvino.runtime.Model,
-        text_encoder: openvino.runtime.Model,
-        unet: openvino.runtime.Model,
-        config: Dict[str, Any],
-        tokenizer: "CLIPTokenizer",
-        scheduler: Union["DDIMScheduler", "PNDMScheduler", "LMSDiscreteScheduler"],
-        feature_extractor: Optional["CLIPFeatureExtractor"] = None,
-        vae_encoder: Optional[openvino.runtime.Model] = None,
-        device: str = "CPU",
-        dynamic_shapes: bool = True,
-        compile: bool = True,
-        ov_config: Optional[Dict[str, str]] = None,
-        model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
+        encoder: openvino.runtime.Model,
+        decoder: openvino.runtime.Model,
+        decoder_with_past: openvino.runtime.Model = None,
+        config: transformers.PretrainedConfig = None,
         **kwargs,
     ):
-        self._internal_dict = config
-        self._device = device.upper()
-        self.is_dynamic = dynamic_shapes
-        self.ov_config = ov_config if ov_config is not None else {}
-        model_save_dir = model_save_dir.name if isinstance(model_save_dir, TemporaryDirectory) else model_save_dir
-
-        self.vae_decoder = OVModelVaeDecoder(
-            vae_decoder,
-            self,
-            {**self.ov_config, "CACHE_DIR": os.path.join(model_save_dir, DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER)},
-        )
-        self.text_encoder = OVModelTextEncoder(
-            text_encoder,
-            self,
-            {**self.ov_config, "CACHE_DIR": os.path.join(model_save_dir, DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER)},
-        )
-        self.unet = OVModelUnet(
-            unet,
-            self,
-            {**self.ov_config, "CACHE_DIR": os.path.join(model_save_dir, DIFFUSION_MODEL_UNET_SUBFOLDER)},
+        super().__init__(
+            encoder=encoder, decoder=decoder, decoder_with_past=decoder_with_past, config=config, **kwargs
         )
-        vae_ov_config = {
-            **self.ov_config,
-            "CACHE_DIR": os.path.join(model_save_dir, DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER),
-        }
-        self.vae_encoder = OVModelVaeEncoder(vae_encoder, self, vae_ov_config) if vae_encoder is not None else None
-        self.tokenizer = tokenizer
-        self.scheduler = scheduler
-        self.feature_extractor = feature_extractor
-        self.safety_checker = None
-        self.preprocessors = []
-
-        if self.is_dynamic:
-            self.reshape(batch_size=-1, height=-1, width=-1, num_images_per_prompt=-1)
-
-        if compile:
+        self.device = torch.device("cpu")
+        self.main_input_name = "input_ids"
+        self.decoder_with_past = None
+        enable_compilation = kwargs.get("compile", True)
+        encoder_cache_dir = Path(self.model_save_dir).joinpath("encoder_cache")
+        encoder_cache_dir.mkdir(parents=True, exist_ok=True)
+        ov_encoder_config = {**self.ov_config, "CACHE_DIR": str(encoder_cache_dir)}
+        self.encoder = OVEncoder(self.encoder_model, self._device, ov_encoder_config)
+        decoder_cache_dir = Path(self.model_save_dir).joinpath("decoder_cache")
+        decoder_cache_dir.mkdir(parents=True, exist_ok=True)
+        ov_decoder_config = {**self.ov_config, "CACHE_DIR": str(decoder_cache_dir)}
+        self.decoder = OVDecoder(self.decoder_model, self._device, ov_decoder_config)
+        if self.use_cache:
+            decoder_past_cache_dir = Path(self.model_save_dir).joinpath("decoder_past_cache")
+            decoder_past_cache_dir.mkdir(parents=True, exist_ok=True)
+            ov_decoder_past_config = {**self.ov_config, "CACHE_DIR": str(decoder_past_cache_dir)}
+            self.decoder_with_past = OVDecoder(self.decoder_with_past_model, self._device, ov_decoder_past_config)
+        if enable_compilation:
             self.compile()
 
-        sub_models = {
-            DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER: self.text_encoder,
-            DIFFUSION_MODEL_UNET_SUBFOLDER: self.unet,
-            DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER: self.vae_decoder,
-            DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER: self.vae_encoder,
-        }
-        for name in sub_models.keys():
-            self._internal_dict[name] = (
-                ("optimum", sub_models[name].__class__.__name__) if sub_models[name] is not None else (None, None)
-            )
+        # Avoid warnings when creating a transformers pipeline
+        AutoConfig.register(self.base_model_prefix, AutoConfig)
+        self.auto_model_class.register(AutoConfig, self.__class__)
 
-        self._internal_dict.pop("vae", None)
+    def to(self, device: str):
+        self._device = device.upper()
+        self.encoder._device = self._device
+        self.decoder._device = self._device
+        if self.use_cache:
+            self.decoder_with_past._device = self._device
+        self.clear_requests()
+        return self
 
-    def _save_pretrained(
+    @add_start_docstrings_to_model_forward(
+        SEQ2SEQ_MODEL_DOCSTRING.format("batch_size, sequence_length")
+        + TRANSLATION_EXAMPLE.format(
+            processor_class=_TOKENIZER_FOR_DOC,
+            model_class="OVModelForSeq2SeqLM",
+            checkpoint="echarlaix/t5-small-openvino",
+        )
+    )
+    def forward(
         self,
-        save_directory: Union[str, Path],
-        vae_decoder_file_name: str = OV_XML_FILE_NAME,
-        text_encoder_file_name: str = OV_XML_FILE_NAME,
-        unet_file_name: str = OV_XML_FILE_NAME,
-        vae_encoder_file_name: str = OV_XML_FILE_NAME,
-        **kwargs,
-    ):
-        """
-        Saves the model to the OpenVINO IR format so that it can be re-loaded using the
-        [`~optimum.intel.openvino.modeling.OVModel.from_pretrained`] class method.
-
-        Arguments:
-            save_directory (`str` or `Path`):
-                The directory where to save the model files.
-            vae_decoder_file_name (`str`, defaults to `optimum.intel.openvino.utils.OV_XML_FILE_NAME`):
-                The VAE decoder model file name. Overwrites the default file name and allows one to save the VAE decoder model
-                with a different name.
-            text_encoder_file_name (`str`, defaults to `optimum.intel.openvino.utils.OV_XML_FILE_NAME`):
-                The text encoder model file name. Overwrites the default file name and allows one to save the text encoder model
-                with a different name.
-            unet_file_name (`str`, defaults to `optimum.intel.openvino.utils.OV_XML_FILE_NAME`):
-                The U-NET model file name. Overwrites the default file name and allows one to save the U-NET model
-                with a different name.
-            vae_encoder_file_name (`str`, defaults to `optimum.intel.openvino.utils.OV_XML_FILE_NAME`):
-                The VAE encoder model file name. Overwrites the default file name and allows one to save the VAE decoder model
-                with a different name.
-        """
-        save_directory = Path(save_directory)
-        src_to_dst_file = {
-            self.vae_decoder.model: save_directory / DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER / vae_decoder_file_name,
-            self.text_encoder.model: save_directory / DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER / text_encoder_file_name,
-            self.unet.model: save_directory / DIFFUSION_MODEL_UNET_SUBFOLDER / unet_file_name,
-        }
-        if self.vae_encoder is not None:
-            src_to_dst_file[self.vae_encoder.model] = (
-                save_directory / DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER / vae_encoder_file_name
-            )
-
-        for src_file, dst_path in src_to_dst_file.items():
-            dst_path.parent.mkdir(parents=True, exist_ok=True)
-            openvino.runtime.serialize(src_file, str(dst_path), str(dst_path.with_suffix(".bin")))
-
-        self.tokenizer.save_pretrained(save_directory.joinpath("tokenizer"))
-        self.scheduler.save_pretrained(save_directory.joinpath("scheduler"))
-        if self.feature_extractor is not None:
-            self.feature_extractor.save_pretrained(save_directory.joinpath("feature_extractor"))
-
-    @classmethod
-    def _from_pretrained(
-        cls,
-        model_id: Union[str, Path],
-        config: Dict[str, Any],
-        use_auth_token: Optional[Union[bool, str]] = None,
-        revision: Optional[str] = None,
-        cache_dir: Optional[str] = None,
-        vae_decoder_file_name: Optional[str] = None,
-        text_encoder_file_name: Optional[str] = None,
-        unet_file_name: Optional[str] = None,
-        vae_encoder_file_name: Optional[str] = None,
-        local_files_only: bool = False,
-        from_onnx: bool = False,
-        model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
+        input_ids: torch.LongTensor = None,
+        attention_mask: Optional[torch.FloatTensor] = None,
+        decoder_input_ids: Optional[torch.LongTensor] = None,
+        encoder_outputs: Optional[Tuple[Tuple[torch.Tensor]]] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
         **kwargs,
-    ):
-        default_file_name = ONNX_WEIGHTS_NAME if from_onnx else OV_XML_FILE_NAME
-        vae_decoder_file_name = vae_decoder_file_name or default_file_name
-        text_encoder_file_name = text_encoder_file_name or default_file_name
-        unet_file_name = unet_file_name or default_file_name
-        vae_encoder_file_name = vae_encoder_file_name or default_file_name
-        model_id = str(model_id)
-        sub_models_to_load, _, _ = cls.extract_init_dict(config)
-        sub_models_names = set(sub_models_to_load.keys()).intersection({"feature_extractor", "tokenizer", "scheduler"})
-
-        if not os.path.isdir(model_id):
-            patterns = set(config.keys())
-            patterns.update({"vae_encoder", "vae_decoder"})
-            allow_patterns = {os.path.join(k, "*") for k in patterns if not k.startswith("_")}
-            allow_patterns.update(
-                {
-                    vae_decoder_file_name,
-                    text_encoder_file_name,
-                    unet_file_name,
-                    vae_encoder_file_name,
-                    vae_decoder_file_name.replace(".xml", ".bin"),
-                    text_encoder_file_name.replace(".xml", ".bin"),
-                    unet_file_name.replace(".xml", ".bin"),
-                    vae_encoder_file_name.replace(".xml", ".bin"),
-                    SCHEDULER_CONFIG_NAME,
-                    CONFIG_NAME,
-                    cls.config_name,
-                }
+    ) -> Seq2SeqLMOutput:
+        # Encode if needed : first prediction pass
+        if encoder_outputs is None:
+            encoder_outputs = self.encoder(input_ids=input_ids, attention_mask=attention_mask)
+
+        # Decode
+        if past_key_values is None or self.decoder_with_past is None:
+            decoder_outputs = self.decoder(
+                input_ids=decoder_input_ids,
+                encoder_hidden_states=encoder_outputs.last_hidden_state,
+                encoder_attention_mask=attention_mask,
             )
-            # Downloads all repo's files matching the allowed patterns
-            model_id = snapshot_download(
-                model_id,
-                cache_dir=cache_dir,
-                local_files_only=local_files_only,
-                use_auth_token=use_auth_token,
-                revision=revision,
-                allow_patterns=allow_patterns,
-                ignore_patterns=["*.msgpack", "*.safetensors", "*pytorch_model.bin"],
+        else:
+            decoder_outputs = self.decoder_with_past(
+                input_ids=decoder_input_ids[:, -1:],  # Cut decoder_input_ids if past is used
+                past_key_values=past_key_values,
+                encoder_hidden_states=encoder_outputs.last_hidden_state,
+                encoder_attention_mask=attention_mask,
             )
-        new_model_save_dir = Path(model_id)
 
-        for name in sub_models_names:
-            # Check if the subcomponent needs to be loaded
-            if kwargs.get(name, None) is not None:
-                continue
-            library_name, library_classes = sub_models_to_load[name]
-            if library_classes is not None:
-                library = importlib.import_module(library_name)
-                class_obj = getattr(library, library_classes)
-                load_method = getattr(class_obj, "from_pretrained")
-                # Check if the module is in a subdirectory
-                if (new_model_save_dir / name).is_dir():
-                    kwargs[name] = load_method(new_model_save_dir / name)
-                else:
-                    kwargs[name] = load_method(new_model_save_dir)
+        return Seq2SeqLMOutput(logits=decoder_outputs.logits, past_key_values=decoder_outputs.past_key_values)
 
-        vae_decoder = cls.load_model(
-            new_model_save_dir / DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER / vae_decoder_file_name
-        )
-        text_encoder = cls.load_model(
-            new_model_save_dir / DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER / text_encoder_file_name
-        )
-        unet = cls.load_model(new_model_save_dir / DIFFUSION_MODEL_UNET_SUBFOLDER / unet_file_name)
-        vae_encoder_path = new_model_save_dir / DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER / vae_encoder_file_name
-        vae_encoder = cls.load_model(vae_encoder_path) if vae_encoder_path.is_file() else None
-
-        if model_save_dir is None:
-            model_save_dir = new_model_save_dir
-
-        return cls(
-            vae_decoder=vae_decoder,
-            text_encoder=text_encoder,
-            unet=unet,
-            config=config,
-            tokenizer=kwargs.pop("tokenizer"),
-            scheduler=kwargs.pop("scheduler"),
-            feature_extractor=kwargs.pop("feature_extractor", None),
-            vae_encoder=vae_encoder,
-            model_save_dir=model_save_dir,
-            **kwargs,
-        )
-
-    @classmethod
-    def _from_transformers(
-        cls,
-        model_id: str,
-        config: Dict[str, Any],
-        use_auth_token: Optional[Union[bool, str]] = None,
-        revision: Optional[str] = None,
-        force_download: bool = False,
-        cache_dir: Optional[str] = None,
-        local_files_only: bool = False,
-        task: Optional[str] = None,
-        tokenizer: "CLIPTokenizer" = None,
-        scheduler: Union["DDIMScheduler", "PNDMScheduler", "LMSDiscreteScheduler"] = None,
-        feature_extractor: Optional["CLIPFeatureExtractor"] = None,
+    def prepare_inputs_for_generation(
+        self,
+        input_ids,
+        past_key_values=None,
+        attention_mask=None,
+        head_mask=None,
+        decoder_head_mask=None,
+        cross_attn_head_mask=None,
+        use_cache=None,
+        encoder_outputs=None,
         **kwargs,
-    ):
-        if task is None:
-            task = cls._auto_model_to_task(cls.auto_model_class)
-        save_dir = TemporaryDirectory()
-        save_dir_path = Path(save_dir.name)
-
-        model_kwargs = {
-            "revision": revision,
-            "use_auth_token": use_auth_token,
-            "cache_dir": cache_dir,
-            "local_files_only": local_files_only,
-            "force_download": force_download,
-            "config": config,
+    ) -> Dict:
+        return {
+            "decoder_input_ids": input_ids,
+            "past_key_values": past_key_values or kwargs.get("past", None),
+            "encoder_outputs": encoder_outputs,
+            "attention_mask": attention_mask,
+            "head_mask": head_mask,
+            "decoder_head_mask": decoder_head_mask,
+            "cross_attn_head_mask": cross_attn_head_mask,
+            "use_cache": use_cache,
         }
-        model = TasksManager.get_model_from_task(task, model_id, **model_kwargs)
-
-        output_names = [
-            os.path.join(DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER, ONNX_WEIGHTS_NAME),
-            os.path.join(DIFFUSION_MODEL_UNET_SUBFOLDER, ONNX_WEIGHTS_NAME),
-            os.path.join(DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER, ONNX_WEIGHTS_NAME),
-            os.path.join(DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER, ONNX_WEIGHTS_NAME),
-        ]
-        models_and_onnx_configs = get_stable_diffusion_models_for_export(model)
-        model.save_config(save_dir_path)
-        export_models(
-            models_and_onnx_configs=models_and_onnx_configs,
-            output_dir=save_dir_path,
-            output_names=output_names,
-        )
-
-        return cls._from_pretrained(
-            model_id=save_dir_path,
-            config=config,
-            from_onnx=True,
-            use_auth_token=use_auth_token,
-            revision=revision,
-            force_download=force_download,
-            cache_dir=cache_dir,
-            local_files_only=local_files_only,
-            model_save_dir=save_dir,
-            tokenizer=tokenizer or model.tokenizer,
-            scheduler=scheduler or model.scheduler,
-            feature_extractor=feature_extractor or model.feature_extractor,
-            **kwargs,
-        )
-
-    def to(self, device: str):
-        self._device = device.upper()
-        self.clear_requests()
-        return self
 
-    @property
-    def device(self) -> str:
-        return self._device.lower()
+    def get_encoder(self):
+        return self.encoder
 
-    def _reshape_unet(
-        self,
-        model: openvino.runtime.Model,
-        batch_size: int = -1,
-        height: int = -1,
-        width: int = -1,
-        num_images_per_prompt: int = -1,
-    ):
-        if batch_size == -1 or num_images_per_prompt == -1:
-            batch_size = -1
-        else:
-            # The factor of 2 comes from the guidance scale > 1
-            batch_size = 2 * batch_size * num_images_per_prompt
+    # Copied from transformers.models.bart.modeling_bart.BartForConditionalGeneration._reorder_cache
+    @staticmethod
+    def _reorder_cache(past, beam_idx) -> Tuple[Tuple[torch.FloatTensor]]:
+        reordered_past = ()
+        for layer_past in past:
+            # Cached cross_attention states don't have to be reordered -> they are always the same
+            reordered_past += (
+                tuple(past_state.index_select(0, beam_idx) for past_state in layer_past[:2]) + layer_past[2:],
+            )
+        return reordered_past
 
-        height = height // 8 if height > 0 else height
-        width = width // 8 if width > 0 else width
-        shapes = {}
-        for inputs in model.inputs:
-            shapes[inputs] = inputs.get_partial_shape()
-            if inputs.get_any_name().startswith("timestep"):
-                shapes[inputs][0] = 1
-            elif inputs.get_any_name().startswith("sample"):
-                shapes[inputs] = [batch_size, 4, height, width]
-            else:
-                shapes[inputs][0] = batch_size
-                shapes[inputs][1] = self.tokenizer.model_max_length
-        model.reshape(shapes)
-        return model
-
-    def _reshape_text_encoder(self, model: openvino.runtime.Model, batch_size: int = -1):
-        if batch_size != -1:
-            shapes = {model.inputs[0]: [batch_size, self.tokenizer.model_max_length]}
-            model.reshape(shapes)
-        return model
-
-    def _reshape_vae_decoder(self, model: openvino.runtime.Model, height: int = -1, width: int = -1):
-        height = height // 8 if height > -1 else height
-        width = width // 8 if width > -1 else width
-        shapes = {model.inputs[0]: [1, 4, height, width]}
-        model.reshape(shapes)
-        return model
+    def reshape(self, batch_size: int, sequence_length: int):
+        """
+        Propagates the given input shapes on the model's layers, fixing the inputs shapes of the model.
 
-    def reshape(
-        self,
-        batch_size: int,
-        height: int,
-        width: int,
-        num_images_per_prompt: int = -1,
-    ):
-        self.is_dynamic = -1 in {batch_size, height, width, num_images_per_prompt}
-        self.text_encoder.model = self._reshape_text_encoder(self.text_encoder.model, batch_size)
-        self.vae_decoder.model = self._reshape_vae_decoder(self.vae_decoder.model, height, width)
-        self.unet.model = self._reshape_unet(self.unet.model, batch_size, height, width, num_images_per_prompt)
+        Arguments:
+            batch_size (`int`):
+                The batch size.
+            sequence_length (`int`):
+                The sequence length.
+        """
+        super().reshape(batch_size, sequence_length)
         self.clear_requests()
         return self
 
     def half(self):
         """
         Converts all the model weights to FP16 for more efficient inference on GPU.
         """
-        compress_model_transformation(self.vae_decoder.model)
-        compress_model_transformation(self.text_encoder.model)
-        compress_model_transformation(self.unet.model)
+        super().half()
         self.clear_requests()
         return self
 
     def clear_requests(self):
-        self.text_encoder.request = None
-        self.vae_decoder.request = None
-        self.unet.request = None
+        self.encoder.request = None
+        self.decoder.request = None
+        if self.use_cache:
+            self.decoder_with_past.request = None
 
     def compile(self):
-        self.text_encoder._create_inference_request()
-        self.vae_decoder._create_inference_request()
-        self.unet._create_inference_request()
+        self.encoder._compile()
+        self.decoder._compile()
+        if self.use_cache:
+            self.decoder_with_past._compile()
+
+
+class OVEncoder:
+    """
+    Encoder model for OpenVINO inference.
+
+    Arguments:
+        request (`openvino.runtime.ie_api.InferRequest`):
+            The OpenVINO inference request associated to the encoder.
+    """
 
-    def __call__(self, *args, **kwargs):
-        guidance_scale = kwargs.get("guidance_scale", None)
-        if guidance_scale is not None and guidance_scale <= 1 and not self.is_dynamic:
-            raise ValueError(
-                f"`guidance_scale` was set to {guidance_scale}, static shapes are only supported for `guidance_scale` > 1, "
-                "please set `dynamic_shapes` to `True` when loading the model."
-            )
-        return StableDiffusionPipelineMixin.__call__(self, *args, **kwargs)
+    def __init__(self, model: openvino.runtime.Model, device: str, ov_config: Dict):
+        self.model = model
+        self._device = device
+        self.device = torch.device("cpu")
+        self.input_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.inputs)}
+        self.main_input_name = "input_ids"
+        self.ov_config = ov_config
+        self.request = None
 
-    @classmethod
-    def _load_config(cls, config_name_or_path: Union[str, os.PathLike], **kwargs):
-        return cls.load_config(config_name_or_path, **kwargs)
+    @add_start_docstrings_to_model_forward(ENCODER_INPUTS_DOCSTRING)
+    def forward(
+        self,
+        input_ids: torch.LongTensor,
+        attention_mask: torch.LongTensor = None,
+        **kwargs,
+    ) -> BaseModelOutput:
+        self._compile()
 
-    def _save_config(self, save_directory):
-        self.save_config(save_directory)
+        # Model inputs
+        inputs = {"input_ids": input_ids}
 
+        # Add the attention_mask inputs when needed
+        if "attention_mask" in self.input_names:
+            inputs["attention_mask"] = attention_mask
+
+        # Run inference
+        last_hidden_state = torch.from_numpy(self.request(inputs, shared_memory=True)["last_hidden_state"]).to(
+            self.device
+        )
 
-class OVModelPart:
-    def __init__(
-        self, model: openvino.runtime.Model, parent_model: OVBaseModel, ov_config: Optional[Dict[str, str]] = None
-    ):
-        self.model = model
-        self.parent_model = parent_model
-        self.input_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.inputs)}
-        self.input_dtype = {
-            inputs.get_any_name(): OV_TO_NP_TYPE[inputs.get_element_type().get_type_name()]
-            for inputs in self.model.inputs
-        }
-        self.ov_config = ov_config or self.parent_model.ov_config
-        self.request = None
+        return BaseModelOutput(last_hidden_state=last_hidden_state)
 
-    def _create_inference_request(self):
+    def __call__(self, *args, **kwargs):
+        return self.forward(*args, **kwargs)
+
+    def _compile(self):
         if self.request is None:
-            logger.info("Compiling the encoder and creating the inference request ...")
-            compiled_model = core.compile_model(self.model, self.device, self.ov_config)
-            self.request = compiled_model.create_infer_request()
+            logger.info("Compiling the encoder...")
+            self.request = core.compile_model(self.model, self._device, self.ov_config)
 
-    @property
-    def device(self):
-        return self.parent_model._device
 
+class OVDecoder:
+    """
+    Decoder model for OpenVINO inference.
+
+    Arguments:
+        request (`openvino.runtime.ie_api.InferRequest`):
+            The OpenVINO inference request associated to the decoder.
+        device (`torch.device`):
+            The device type used by this process.
+    """
 
-class OVModelTextEncoder(OVModelPart):
-    def __call__(self, input_ids: np.ndarray):
-        self._create_inference_request()
+    def __init__(self, model: openvino.runtime.Model, device: str, ov_config: Dict):
+        self.model = model
+        self._device = device
+        self.device = torch.device("cpu")
+        self.input_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.inputs)}
+        self.key_value_input_names = [key for key in self.input_names if "key_values" in key]
+        is_legacy = any("past_key_values" in key.get_any_name() for key in self.model.outputs)
 
-        inputs = {
-            "input_ids": input_ids,
-        }
-        outputs = self.request.infer(inputs)
-        return list(outputs.values())
+        if len(self.key_value_input_names) > 0 and not is_legacy:
+            self.use_past = True
+            self.num_pkv = 2
+        else:
+            self.use_past = False
+            self.num_pkv = 4
 
+        self.ov_config = ov_config
+        self.request = None
 
-class OVModelUnet(OVModelPart):
-    def __call__(self, sample: np.ndarray, timestep: np.ndarray, encoder_hidden_states: np.ndarray):
-        self._create_inference_request()
-
-        inputs = {
-            "sample": sample,
-            "timestep": timestep,
-            "encoder_hidden_states": encoder_hidden_states,
-        }
+    @add_start_docstrings_to_model_forward(DECODER_INPUTS_DOCSTRING)
+    def forward(
+        self,
+        input_ids: torch.LongTensor,
+        encoder_hidden_states: torch.FloatTensor,
+        encoder_attention_mask: Optional[torch.LongTensor] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+    ) -> Seq2SeqLMOutput:
+        self._compile()
+        # Model inputs
+        inputs = {}
+
+        if past_key_values is not None:
+            # Flatten the past_key_values
+            past_key_values = tuple(
+                past_key_value for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer
+            )
 
-        outputs = self.request.infer(inputs)
-        return list(outputs.values())
+            # Add the past_key_values to the decoder inputs
+            inputs = dict(zip(self.key_value_input_names, past_key_values))
 
+        inputs["input_ids"] = input_ids
 
-class OVModelVaeDecoder(OVModelPart):
-    def __call__(self, latent_sample: np.ndarray):
-        self._create_inference_request()
+        # Add the encoder_attention_mask inputs when needed
+        if "encoder_attention_mask" in self.input_names and encoder_attention_mask is not None:
+            inputs["encoder_attention_mask"] = encoder_attention_mask
+
+        # Add the encoder_hidden_states inputs when needed
+        if "encoder_hidden_states" in self.input_names and encoder_hidden_states is not None:
+            inputs["encoder_hidden_states"] = encoder_hidden_states
+
+        # Run inference
+        outputs = self.request(inputs, shared_memory=True)
+        logits = torch.from_numpy(outputs["logits"]).to(self.device)
+
+        # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the
+        # self-attention layer and 2 to the cross-attention layer)
+        out_past_key_values = tuple(
+            torch.from_numpy(outputs[next(iter(key))]).to(self.device)
+            for key in outputs.names()
+            if ("key_values" in next(iter(key)) or "present" in next(iter(key)))
+        )
 
-        inputs = {
-            "latent_sample": latent_sample,
-        }
-        outputs = self.request.infer(inputs)
-        return list(outputs.values())
+        # Tuple of tuple of length `n_layers`, with each tuple of length equal to:
+        # * 4 for the decoder without cache (k/v of self-attention + k/v of cross-attention)
+        # * 2 for the decoder with cache (k/v of self-attention as cross-attention cache is constant)
+        if self.use_past is False:
+            out_past_key_values = tuple(
+                out_past_key_values[i : i + self.num_pkv] for i in range(0, len(out_past_key_values), self.num_pkv)
+            )
+        else:
+            # grab the cross attention key/values from the inputs
+            out_past_key_values = tuple(
+                out_past_key_values[i : i + self.num_pkv] + past_key_values[2 * i + 2 : 2 * i + 2 + self.num_pkv]
+                for i in range(0, len(out_past_key_values), self.num_pkv)
+            )
 
+        return Seq2SeqLMOutput(logits=logits, past_key_values=out_past_key_values)
 
-class OVModelVaeEncoder(OVModelPart):
-    def __call__(self, sample: np.ndarray):
-        self._create_inference_request()
+    def __call__(self, *args, **kwargs):
+        return self.forward(*args, **kwargs)
 
-        inputs = {
-            "sample": sample,
-        }
-        outputs = self.request.infer(inputs)
-        return list(outputs.values())
+    def _compile(self):
+        if self.request is None:
+            logger.info("Compiling the decoder...")
+            self.request = core.compile_model(self.model, self._device, self.ov_config)
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/quantization.py` & `optimum-intel-1.9.0/optimum/intel/openvino/quantization.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from nncf.torch import create_compressed_model, register_default_init_args
 from nncf.torch.dynamic_graph.io_handling import wrap_nncf_model_inputs_with_objwalk
 from nncf.torch.initialization import PTInitializingDataLoader
 from nncf.torch.nncf_network import NNCFNetwork
 from openvino._offline_transformations import compress_quantize_weights_transformation
 from openvino.runtime import Core
 from torch.onnx import export as onnx_export
+from torch.utils._pytree import tree_map
 from torch.utils.data import DataLoader, RandomSampler
 from transformers import DataCollator, PreTrainedModel, default_data_collator
 
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
 from optimum.quantization_base import OptimumQuantizer
 
@@ -167,62 +168,40 @@
         model_type = self.model.config.model_type.replace("_", "-")
         onnx_config_class = TasksManager.get_exporter_config_constructor(
             exporter="onnx",
             model=self.model,
             task=self.task,
             model_type=model_type,
         )
-        onnx_config = onnx_config_class(self.model.config)
+
+        if self.task == "text-generation":
+            onnx_config = onnx_config_class(self.model.config, use_past=self.model.config.use_cache)
+        else:
+            onnx_config = onnx_config_class(self.model.config)
+
         compressed_model.eval()
         num_parameters = compressed_model.num_parameters()
         save_as_external_data = use_external_data_format(num_parameters) or quantization_config.save_onnx_model
         f = io.BytesIO() if not save_as_external_data else save_directory / ONNX_WEIGHTS_NAME
 
         # Export the compressed model to the ONNX format
-        self._onnx_export(compressed_model, onnx_config, model_inputs, quantization_config, f)
+        opset = min(onnx_config.DEFAULT_ONNX_OPSET, MAX_ONNX_OPSET)
+        opset = opset if not quantization_config.save_onnx_model else max(opset, MIN_ONNX_QDQ_OPSET)
+        _onnx_export_nncf_model(compressed_model, onnx_config, f, opset)
 
         # Load and save the compressed model
         model = core.read_model(f) if save_as_external_data else core.read_model(f.getvalue(), b"")
         self._save_pretrained(model, output_path)
         quantization_config.save_pretrained(save_directory)
 
     @staticmethod
     def _save_pretrained(model: openvino.runtime.Model, output_path: str):
         compress_quantize_weights_transformation(model)
         openvino.runtime.serialize(model, output_path, output_path.replace(".xml", ".bin"))
 
-    def _onnx_export(
-        self,
-        model: NNCFNetwork,
-        config: OnnxConfig,
-        model_inputs: Dict,
-        ov_config: OVConfig,
-        f: Union[str, io.BytesIO],
-    ):
-        opset = min(config.DEFAULT_ONNX_OPSET, MAX_ONNX_OPSET)
-        opset = opset if not ov_config.save_onnx_model else max(opset, MIN_ONNX_QDQ_OPSET)
-        model_inputs = {k: v.to(model.device) for k, v in model_inputs.items()}
-        # Create ordered inputs for the ONNX export of NNCFNetwork as keyword arguments are currently not supported
-        inputs = tuple([model_inputs.pop(key, None) for key in self._export_input_names if len(model_inputs) != 0])
-
-        with torch.no_grad():
-            # Disable node additions to be exported in the graph
-            model.disable_dynamic_graph_building()
-            onnx_export(
-                model,
-                inputs,
-                f=f,
-                input_names=list(config.inputs.keys()),
-                output_names=list(config.outputs.keys()),
-                dynamic_axes=dict(chain(config.inputs.items(), config.outputs.items())),
-                do_constant_folding=True,
-                opset_version=opset,
-            )
-            model.enable_dynamic_graph_building()
-
     def _set_task(self):
         if self.task is None:
             self.task = HfApi().model_info(self.model.config._name_or_path).pipeline_tag
             if self.task is None:
                 raise ValueError(
                     "The task defining the model topology could not be extracted and needs to be specified for the ONNX export."
                 )
@@ -295,7 +274,40 @@
             calibration_dataset, batch_size=batch_size, sampler=sampler, collate_fn=data_collator, drop_last=False
         )
         return OVDataLoader(calibration_dataloader)
 
     def _remove_unused_columns(self, dataset: Dataset):
         ignored_columns = list(set(dataset.column_names) - set(self._signature_columns))
         return dataset.remove_columns(ignored_columns)
+
+
+def _onnx_export_nncf_model(model: NNCFNetwork, config: OnnxConfig, output: Union[str, io.BytesIO], opset: int = None):
+    signature = inspect.signature(model.forward)
+    signature = list(signature.parameters.keys())
+    opset = opset or config.DEFAULT_ONNX_OPSET
+    model_inputs = config.generate_dummy_inputs(framework="pt")
+    # Create ordered inputs for the ONNX export of NNCFNetwork as keyword arguments are currently not supported
+    model_inputs = tuple(model_inputs.pop(key, None) for key in signature if len(model_inputs) != 0)
+    device = model.device
+
+    def remap(value):
+        if isinstance(value, torch.Tensor):
+            value = value.to(device)
+        return value
+
+    with config.patch_model_for_export(model):
+        model_inputs = tree_map(remap, model_inputs)
+        with torch.no_grad():
+            model.eval()
+            # Disable node additions to be exported in the graph
+            model.disable_dynamic_graph_building()
+            onnx_export(
+                model,
+                model_inputs,
+                f=output,
+                input_names=list(config.inputs.keys()),
+                output_names=list(config.outputs.keys()),
+                dynamic_axes=dict(chain(config.inputs.items(), config.outputs.items())),
+                do_constant_folding=True,
+                opset_version=opset,
+            )
+            model.enable_dynamic_graph_building()
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/trainer.py` & `optimum-intel-1.9.0/optimum/intel/openvino/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import inspect
 import io
 import math
 import os
 import sys
 import time
 from collections import defaultdict
-from itertools import chain
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 
 import openvino
 import openvino.runtime
 import torch
 import torch.distributed as dist
@@ -33,24 +32,22 @@
 from nncf.common.utils.tensorboard import prepare_for_tensorboard
 from nncf.config.structures import BNAdaptationInitArgs, QuantizationRangeInitArgs
 from nncf.experimental.torch.sparsity.movement.algo import MovementSparsityController
 from nncf.experimental.torch.sparsity.movement.scheduler import MovementSchedulerStage
 from nncf.torch import create_compressed_model
 from nncf.torch.composite_compression import PTCompositeCompressionAlgorithmController
 from nncf.torch.compression_method_api import PTCompressionAlgorithmController
-from nncf.torch.nncf_network import NNCFNetwork
 from nncf.torch.quantization.algo import QuantizationController
 from openvino._offline_transformations import compress_quantize_weights_transformation
 from openvino.runtime import Core, PartialShape, serialize
 from openvino.tools.mo.back.offline_transformations import (
     apply_fused_names_cleanup,
     apply_moc_transformations,
     apply_user_transformations,
 )
-from torch.onnx import export as onnx_export
 from torch.utils.data import DataLoader, Dataset, RandomSampler
 from torch.utils.data.distributed import DistributedSampler
 from tqdm.auto import tqdm
 from transformers import Trainer
 from transformers.data.data_collator import DataCollator
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
 from transformers.deepspeed import deepspeed_init
@@ -74,20 +71,19 @@
     is_apex_available,
     is_sagemaker_mp_enabled,
     is_torch_tpu_available,
     logging,
 )
 
 from optimum.exporters import TasksManager
-from optimum.exporters.onnx import OnnxConfig
 
 from ..utils.constant import _TASK_ALIASES
 from ..utils.import_utils import is_transformers_version
 from .configuration import OVConfig
-from .quantization import OVDataLoader
+from .quantization import OVDataLoader, _onnx_export_nncf_model
 from .training_args import OVTrainingArguments
 from .utils import (
     MAX_ONNX_OPSET,
     MIN_ONNX_QDQ_OPSET,
     ONNX_WEIGHTS_NAME,
     OV_XML_FILE_NAME,
     use_external_data_format,
@@ -168,15 +164,16 @@
 
         if self.ov_config is not None and self.args.do_train:
             self._set_task()
             train_dataloader = self.get_train_dataloader()
             model_inputs = next(iter(train_dataloader))
             for label_name in self.label_names:
                 model_inputs.pop(label_name)
-            self.ov_config.add_input_info(model_inputs)
+            force_batch_one = self._is_pruning_enabled()
+            self.ov_config.add_input_info(model_inputs, force_batch_one)
             nncf_config = NNCFConfig.from_dict(self.ov_config.__dict__)
             nncf_config.register_extra_structs(
                 [
                     QuantizationRangeInitArgs(OVDataLoader(train_dataloader)),
                     BNAdaptationInitArgs(OVDataLoader(train_dataloader)),
                 ]
             )
@@ -196,18 +193,15 @@
             self.model_wrapped = self.model
             # TODO : To deprecate once support transformers > 4.30.0
             self.deepspeed = None
 
     def _set_signature_columns_if_needed(self):
         if self._signature_columns is None:
             # Inspect model forward signature to keep only the arguments it accepts.
-            if isinstance(self.model, NNCFNetwork):
-                signature = inspect.signature(self.model.get_nncf_wrapped_model().forward)
-            else:
-                signature = inspect.signature(self.model.forward)
+            signature = inspect.signature(self.model.forward)
             self._signature_columns = list(signature.parameters.keys())
             # Labels may be named label or label_ids, the default data collator handles that.
             self._signature_columns += list(set(["label", "label_ids"] + self.label_names))
 
     def _inner_training_loop(
         self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
     ):
@@ -664,16 +658,14 @@
         os.makedirs(output_dir, exist_ok=True)
         logger.info(f"Saving model checkpoint to {output_dir}")
         # Save a trained model and configuration using `save_pretrained()`.
         # They can then be reloaded using `from_pretrained()`
 
         if not isinstance(self.model, PreTrainedModel):
             unwrapped_model = unwrap_model(self.model)
-            if isinstance(unwrapped_model, NNCFNetwork):
-                unwrapped_model = unwrapped_model.get_nncf_wrapped_model()
             is_pretrained_model = isinstance(unwrapped_model, PreTrainedModel)
             if state_dict is None:
                 state_dict = self.model.state_dict()
             if is_pretrained_model:
                 unwrapped_model.save_pretrained(output_dir, state_dict=state_dict)
             else:
                 logger.info("Trainer.model is not a `PreTrainedModel`, only saving its state dict.")
@@ -698,19 +690,26 @@
             onnx_config_class = TasksManager.get_exporter_config_constructor(
                 exporter="onnx",
                 model=self.model,
                 task=self.task,
                 model_type=model_type,
             )
 
-            onnx_config = onnx_config_class(self.model.config)
+            if self.task == "text-generation":
+                onnx_config = onnx_config_class(self.model.config, use_past=self.model.config.use_cache)
+            else:
+                onnx_config = onnx_config_class(self.model.config)
+
             num_parameters = self.model.num_parameters()
             save_as_external_data = use_external_data_format(num_parameters) or self.ov_config.save_onnx_model
             f = io.BytesIO() if not save_as_external_data else os.path.join(output_dir, ONNX_WEIGHTS_NAME)
-            self._onnx_export(self.model, onnx_config, self.ov_config, f)
+
+            opset = min(onnx_config.DEFAULT_ONNX_OPSET, MAX_ONNX_OPSET)
+            opset = opset if not self.ov_config.save_onnx_model else max(opset, MIN_ONNX_QDQ_OPSET)
+            _onnx_export_nncf_model(self.model, onnx_config, f, opset)
             ov_model = core.read_model(f) if save_as_external_data else core.read_model(f.getvalue(), b"")
 
             # Prune IR if structured pruning is conducted on the model
             if self._should_apply_pruning_transform():
                 try:
                     # OpenVINO IR pruning requires static-shaped input
                     ov_model = self._reshape_ir(ov_model, static_shape=True)
@@ -769,32 +768,15 @@
         return ov_model
 
     def _set_task(self):
         if self.task is None:
             raise ValueError("The model task defining the model topology needs to be specified for the ONNX export.")
         self.task = _TASK_ALIASES.get(self.task, self.task)
 
-    def _onnx_export(self, model: NNCFNetwork, config: OnnxConfig, ov_config: OVConfig, f: Union[str, io.BytesIO]):
-        opset = min(config.DEFAULT_ONNX_OPSET, MAX_ONNX_OPSET)
-        opset = opset if not ov_config.save_onnx_model else max(opset, MIN_ONNX_QDQ_OPSET)
-        model_inputs = config.generate_dummy_inputs(framework="pt")
-        device = model.device
-        model_inputs = {k: v.to(device) for k, v in model_inputs.items()}
-        self._set_signature_columns_if_needed()  # find model input names needed in ONNX export
-        # Create ordered inputs for the ONNX export of NNCFNetwork as keyword arguments are currently not supported
-        inputs = tuple([model_inputs.pop(key, None) for key in self._signature_columns if len(model_inputs) != 0])
-
-        with torch.no_grad():
-            model.eval()
-            # Disable node additions to be exported in the graph
-            model.disable_dynamic_graph_building()
-            onnx_export(
-                model,
-                inputs,
-                f=f,
-                input_names=list(config.inputs.keys()),
-                output_names=list(config.outputs.keys()),
-                dynamic_axes=dict(chain(config.inputs.items(), config.outputs.items())),
-                do_constant_folding=True,
-                opset_version=opset,
-            )
-            model.enable_dynamic_graph_building()
+    def _is_pruning_enabled(compression: Union[Dict, List, None]):
+        if isinstance(compression, dict) and compression["algorithm"] == "movement_pruning":
+            return True
+        if isinstance(compression, list):
+            for algo_config in compression:
+                if algo_config["algorithm"] == "movement_pruning":
+                    return True
+        return False
```

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/training_args.py` & `optimum-intel-1.9.0/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/openvino/utils.py` & `optimum-intel-1.9.0/optimum/intel/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/__init__.py` & `optimum-intel-1.9.0/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.9.0/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/utils/import_utils.py` & `optimum-intel-1.9.0/optimum/intel/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/optimum/intel/version.py` & `optimum-intel-1.9.0/optimum/intel/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.8.1"
+__version__ = "1.9.0"
```

### Comparing `optimum-intel-1.8.1/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.9.0/optimum_intel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.8.1
+Version: 1.9.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,57 +66,34 @@
 
 where `extras` can be one or more of `neural-compressor`, `openvino`, `nncf`.
 
 # Quick tour
 
 ## Neural Compressor
 
-#### Dynamic quantization:
+Dynamic quantization can be used through the Optimum command-line interface:
 
-Here is an example on how to apply dynamic quantization on a DistilBERT fine-tuned on the SQuAD1.0 dataset.
-Note that quantization is currently only supported for CPUs (only CPU backends are available), so we will not be utilizing GPUs / CUDA in this example.
-
-```python
-from transformers import AutoModelForQuestionAnswering
-from neural_compressor.config import PostTrainingQuantConfig
-from optimum.intel import INCQuantizer
-
-model_name = "distilbert-base-cased-distilled-squad"
-model = AutoModelForQuestionAnswering.from_pretrained(model_name)
-# The directory where the quantized model will be saved
-save_dir = "quantized_model"
-# Load the quantization configuration detailing the quantization we wish to apply
-quantization_config = PostTrainingQuantConfig(approach="dynamic")
-quantizer = INCQuantizer.from_pretrained(model)
-# Apply dynamic quantization and save the resulting model
-quantizer.quantize(quantization_config=quantization_config, save_directory=save_dir)
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
 ```
+Note that quantization is currently only supported for CPUs (only CPU backends are available), so we will not be utilizing GPUs / CUDA in this example.
 
 To load a quantized model hosted locally or on the 🤗 hub, you can do as follows :
 ```python
 from optimum.intel import INCModelForSequenceClassification
 
 # Load the PyTorch model hosted on the hub
 loaded_model_from_hub = INCModelForSequenceClassification.from_pretrained(
     "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
 )
 ```
 
-#### Apply dynamic quantization on your model using the CLI
-
-Dynamic quantization can be used through the Optimum Intel command-line:
-
-```bash
-optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
-```
-
 You can load many more quantized models hosted on the hub under the Intel organization [`here`](https://huggingface.co/Intel).
 
-
-For more details, please refer to this [guide](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc#apply-quantization-using-the-cli).
+For more details on the supported compression techniques, please refer to the [documentation](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc).
 
 
 ## OpenVINO
 
 Below are the examples of how to use OpenVINO and its [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html) framework to accelerate inference.
 
 #### Inference:
```

### Comparing `optimum-intel-1.8.1/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.9.0/optimum_intel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 setup.cfg
 setup.py
 optimum/commands/neural_compressor/base.py
 optimum/commands/neural_compressor/quantize.py
 optimum/commands/register/register_inc.py
 optimum/intel/__init__.py
 optimum/intel/version.py
+optimum/intel/generation/__init__.py
+optimum/intel/generation/modeling.py
 optimum/intel/ipex/__init__.py
 optimum/intel/ipex/inference.py
 optimum/intel/neural_compressor/__init__.py
 optimum/intel/neural_compressor/configuration.py
 optimum/intel/neural_compressor/launcher.py
+optimum/intel/neural_compressor/modeling_diffusion.py
 optimum/intel/neural_compressor/neural_coder_adaptor.py
 optimum/intel/neural_compressor/quantization.py
 optimum/intel/neural_compressor/trainer.py
 optimum/intel/neural_compressor/trainer_seq2seq.py
 optimum/intel/neural_compressor/utils.py
 optimum/intel/openvino/__init__.py
 optimum/intel/openvino/configuration.py
@@ -30,19 +33,21 @@
 optimum/intel/openvino/quantization.py
 optimum/intel/openvino/trainer.py
 optimum/intel/openvino/training_args.py
 optimum/intel/openvino/utils.py
 optimum/intel/utils/__init__.py
 optimum/intel/utils/constant.py
 optimum/intel/utils/dummy_ipex_objects.py
+optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
 optimum/intel/utils/dummy_neural_compressor_objects.py
 optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
 optimum/intel/utils/dummy_openvino_and_nncf_objects.py
 optimum/intel/utils/dummy_openvino_objects.py
 optimum/intel/utils/import_utils.py
+optimum/intel/utils/modeling_utils.py
 optimum_intel.egg-info/PKG-INFO
 optimum_intel.egg-info/SOURCES.txt
 optimum_intel.egg-info/dependency_links.txt
 optimum_intel.egg-info/entry_points.txt
 optimum_intel.egg-info/not-zip-safe
 optimum_intel.egg-info/requires.txt
 optimum_intel.egg-info/top_level.txt
```

### Comparing `optimum-intel-1.8.1/pyproject.toml` & `optimum-intel-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/setup.cfg` & `optimum-intel-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.1/setup.py` & `optimum-intel-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,25 @@
 
 INSTALL_REQUIRE = [
     "optimum>=1.8.0",
     "transformers>=4.20.0",
     "datasets>=1.4.0",
     "sentencepiece",
     "scipy",
+    "accelerate",  # transformers 4.29 require accelerate for PyTorch
 ]
 
 TESTS_REQUIRE = ["pytest", "parameterized", "Pillow", "evaluate", "diffusers", "py-cpuinfo"]
 
 QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241"]
 
 EXTRAS_REQUIRE = {
-    "neural-compressor": [
-        "neural-compressor>=2.1.0",
-        "onnx",
-        "onnxruntime",
-        "torch<2.0.0",  # remove after neural-compressor next release
-        "intel-extension-for-pytorch<2.0.0",
-    ],
-    "openvino": ["openvino>=2023.0.0.dev20230217", "onnx", "onnxruntime"],
-    "nncf": ["nncf>=2.4.0", "openvino-dev>=2023.0.0.dev20230217"],
+    "neural-compressor": ["neural-compressor>=2.1.1", "onnx", "onnxruntime<1.15.0"],
+    "openvino": ["openvino>=2023.0.0", "onnx", "onnxruntime"],
+    "nncf": ["nncf>=2.5.0", "openvino-dev>=2023.0.0"],
     "ipex": ["intel-extension-for-pytorch", "onnx"],
     "diffusers": ["diffusers"],
     "quality": QUALITY_REQUIRE,
     "tests": TESTS_REQUIRE,
 }
 
 setup(
```

