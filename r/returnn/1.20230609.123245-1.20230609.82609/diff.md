# Comparing `tmp/returnn-1.20230609.123245.tar.gz` & `tmp/returnn-1.20230609.82609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230609.123245.tar", last modified: Fri Jun  9 10:43:50 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230609.82609.tar", last modified: Fri Jun  9 06:52:10 2023, max compression
```

## Comparing `returnn-1.20230609.123245.tar` & `returnn-1.20230609.82609.tar`

### file list

```diff
@@ -1,448 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 10:43:28.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-09 10:43:31.000000 returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157757 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   150722 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   297063 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35124 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   552442 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:43:50.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-09 10:43:27.000000 returnn-1.20230609.123245/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 06:51:47.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157757 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150722 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   297063 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31004 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   552442 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230609.123245/.gitignore` & `returnn-1.20230609.82609/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/.gitmodules` & `returnn-1.20230609.82609/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/CHANGELOG.md` & `returnn-1.20230609.82609/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/CODEOWNERS` & `returnn-1.20230609.82609/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/CONTRIBUTING.md` & `returnn-1.20230609.82609/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/LICENSE` & `returnn-1.20230609.82609/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/MANIFEST.in` & `returnn-1.20230609.82609/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/PKG-INFO` & `returnn-1.20230609.82609/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230609.123245
+Version: 1.20230609.82609
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230609.123245/README.rst` & `returnn-1.20230609.82609/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/__init__.py` & `returnn-1.20230609.82609/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/12AX.cluster_map` & `returnn-1.20230609.82609/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-fwd.config` & `returnn-1.20230609.82609/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-horovod-mpi.py` & `returnn-1.20230609.82609/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230609.82609/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-hyper-param-tuning.config` & `returnn-1.20230609.82609/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-iter-dataset.py` & `returnn-1.20230609.82609/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-list-devices.py` & `returnn-1.20230609.82609/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-lua-torch-layer.config` & `returnn-1.20230609.82609/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230609.82609/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-returnn-as-framework.py` & `returnn-1.20230609.82609/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-rf.config` & `returnn-1.20230609.82609/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-rhn-enwik8.config` & `returnn-1.20230609.82609/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-sprint-interface.py` & `returnn-1.20230609.82609/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-att-copy.config` & `returnn-1.20230609.82609/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-attention.config` & `returnn-1.20230609.82609/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-enc-dec.config` & `returnn-1.20230609.82609/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230609.82609/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230609.82609/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230609.82609/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230609.82609/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-rec-self-att.config` & `returnn-1.20230609.82609/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230609.82609/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230609.82609/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230609.82609/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-torch.config` & `returnn-1.20230609.82609/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230609.82609/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/demo.sh` & `returnn-1.20230609.82609/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/README.txt` & `returnn-1.20230609.82609/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/config_demo` & `returnn-1.20230609.82609/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230609.82609/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/config_real` & `returnn-1.20230609.82609/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230609.82609/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/decode.py` & `returnn-1.20230609.82609/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230609.82609/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230609.82609/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230609.82609/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230609.82609/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230609.82609/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230609.82609/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230609.82609/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/__init__.py` & `returnn-1.20230609.82609/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/__main__.py` & `returnn-1.20230609.82609/returnn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,25 +330,14 @@
         OpMaker.log_stream = log.v3
         tf_util.debug_register_better_repr()
         if config.is_true("distributed_tf"):
             import returnn.tf.distributed
 
             returnn.tf.distributed.init_distributed_tf(config)
     elif BackendEngine.is_torch_selected():
-        if config.typed_value("torch_distributed") is not None:
-            import socket
-            import returnn.torch.distributed
-
-            torch_distributed = returnn.torch.distributed.get_ctx(config=config)
-            print(
-                "Torch: Hostname %s, pid %i, using GPU %s."
-                % (socket.gethostname(), os.getpid(), str(torch_distributed.local_rank())),
-                file=log.v3,
-            )
-
         print("PyTorch:", util.describe_torch_version(), file=log.v3)
     else:
         raise NotImplementedError
 
 
 def init(config_filename=None, command_line_options=(), config_updates=None, extra_greeting=None):
     """
@@ -393,19 +382,14 @@
     if engine:
         if BackendEngine.is_tensorflow_selected():
             engine.finalize(error_occurred=error_occurred)
             if config.is_true("use_horovod"):
                 import horovod.tensorflow as hvd  # noqa
 
                 hvd.shutdown()
-        elif BackendEngine.is_torch_selected():
-            if config.typed_value("torch_distributed") is not None:
-                from torch.distributed import destroy_process_group
-
-                destroy_process_group()
 
 
 def need_data():
     """
     :return: whether we need to init the data (call :func:`init_data`) for the current task (:func:`execute_main_task`)
     :rtype: bool
     """
```

### Comparing `returnn-1.20230609.123245/returnn/__old_mod_loader__.py` & `returnn-1.20230609.82609/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/__setup__.py` & `returnn-1.20230609.82609/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/config.py` & `returnn-1.20230609.82609/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/audio.py` & `returnn-1.20230609.82609/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/basic.py` & `returnn-1.20230609.82609/returnn/datasets/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,19 +241,14 @@
         if not config:
             return 0
         if config.is_true("use_horovod"):
             import returnn.tf.horovod
 
             if returnn.tf.horovod.get_ctx().is_dataset_distribution_random_seed_offset():
                 return returnn.tf.horovod.get_ctx().rank() * 16127
-
-        if config.typed_value("torch_distributed") is not None:
-            import returnn.torch.distributed
-
-            return returnn.torch.distributed.get_ctx().rank() * 16127
         return 0
 
     @staticmethod
     def _parse_chunking(chunking):
         """
         :param None|str|int|(int,int)|dict|(dict,dict)|(NumbersDict,NumbersDict)|function chunking:
           as it comes from the config / from the user
```

### Comparing `returnn-1.20230609.123245/returnn/datasets/bundle_file.py` & `returnn-1.20230609.82609/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/cached.py` & `returnn-1.20230609.82609/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/cached2.py` & `returnn-1.20230609.82609/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/generating.py` & `returnn-1.20230609.82609/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/hdf.py` & `returnn-1.20230609.82609/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/lm.py` & `returnn-1.20230609.82609/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/map.py` & `returnn-1.20230609.82609/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/meta.py` & `returnn-1.20230609.82609/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/multi_proc.py` & `returnn-1.20230609.82609/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/normalization_data.py` & `returnn-1.20230609.82609/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/numpy_dump.py` & `returnn-1.20230609.82609/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/raw_wav.py` & `returnn-1.20230609.82609/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/sprint.py` & `returnn-1.20230609.82609/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/stereo.py` & `returnn-1.20230609.82609/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230609.82609/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/datasets/util/vocabulary.py` & `returnn-1.20230609.82609/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/engine/base.py` & `returnn-1.20230609.82609/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/engine/batch.py` & `returnn-1.20230609.82609/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/edit.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/select.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/transform.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/extern/graph_editor/util.py` & `returnn-1.20230609.82609/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/forward_iface.py` & `returnn-1.20230609.82609/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/__init__.py` & `returnn-1.20230609.82609/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/_backend.py` & `returnn-1.20230609.82609/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/_numpy_backend.py` & `returnn-1.20230609.82609/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/_utils.py` & `returnn-1.20230609.82609/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/array_.py` & `returnn-1.20230609.82609/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/attention.py` & `returnn-1.20230609.82609/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/cond.py` & `returnn-1.20230609.82609/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/const.py` & `returnn-1.20230609.82609/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/container.py` & `returnn-1.20230609.82609/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/conv.py` & `returnn-1.20230609.82609/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/device.py` & `returnn-1.20230609.82609/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/dims.py` & `returnn-1.20230609.82609/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/dropout.py` & `returnn-1.20230609.82609/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/dtype.py` & `returnn-1.20230609.82609/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/encoder/base.py` & `returnn-1.20230609.82609/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/encoder/conformer.py` & `returnn-1.20230609.82609/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/init.py` & `returnn-1.20230609.82609/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/linear.py` & `returnn-1.20230609.82609/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/loop.py` & `returnn-1.20230609.82609/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/loss.py` & `returnn-1.20230609.82609/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/math_.py` & `returnn-1.20230609.82609/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/matmul.py` & `returnn-1.20230609.82609/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/module.py` & `returnn-1.20230609.82609/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/normalization.py` & `returnn-1.20230609.82609/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/parameter.py` & `returnn-1.20230609.82609/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/rand.py` & `returnn-1.20230609.82609/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/rec.py` & `returnn-1.20230609.82609/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/reduce.py` & `returnn-1.20230609.82609/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/run_ctx.py` & `returnn-1.20230609.82609/returnn/frontend/run_ctx.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,14 @@
             # The expected output usually comes from `model_outputs` from the user config.
             # The dimensions of `expected_output` and `tensor` should match,
             # but we can't directly check for expected_output.dims == tensor.dims
             # because not all dims can be known in advance in `expected_output`,
             # e.g. dynamic dims.
             # Thus, we allow undefined dims in the expected output,
             # and ignore them when checking for equality.
-            # The most important thing for the user is to define what dims are dynamic and what dims are static.
-            # This is also necessary for ONNX export.
             assert len(expected_output.dims) == len(tensor.dims), (
                 f"mark_as_output: lengths of expected output {expected_output.dims}"
                 f" and actual output {tensor.dims} don't match."
             )
             for expected_dim, actual_dim in zip(expected_output.dims, tensor.dims):
                 expected_dim: Dim
                 actual_dim: Dim
@@ -233,20 +231,18 @@
                     )
                 elif expected_dim.is_dynamic():
                     assert actual_dim.is_dynamic(), (
                         f"mark_as_output: expected dim {expected_dim} is dynamic."
                         f" Matching actual dim assumed to be dynamic, but got non-dynamic dim {actual_dim}."
                     )
                 elif expected_dim.is_static():
-                    assert expected_dim.is_static() and actual_dim.dimension == expected_dim.dimension, (
+                    assert actual_dim is expected_dim, (
                         f"mark_as_output: expected dim {expected_dim} is static."
-                        f" Matching actual dim assumed to be the same static dim value, but got {actual_dim}."
+                        f" Matching actual dim assumed to be the same static dim, but got {actual_dim}."
                     )
-                else:
-                    assert False, f"mark_as_output: unexpected expected dim {expected_dim}."
             assert expected_output.dtype == tensor.dtype, (
                 f"mark_as_output: {name!r} dtype mismatch from expected output,"
                 f" given {tensor.dtype}, expected {expected_output.dtype}"
             )
             assert expected_output.sparse_dim == tensor.sparse_dim, (
                 f"mark_as_output: {name!r} sparse_dim mismatch from expected output,"
                 f" given {tensor.sparse_dim}, expected {expected_output.sparse_dim}"
```

### Comparing `returnn-1.20230609.123245/returnn/frontend/signal.py` & `returnn-1.20230609.82609/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/state.py` & `returnn-1.20230609.82609/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/tensor_array.py` & `returnn-1.20230609.82609/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/frontend/types.py` & `returnn-1.20230609.82609/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/import_/common.py` & `returnn-1.20230609.82609/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/import_/git.py` & `returnn-1.20230609.82609/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/import_/import_.py` & `returnn-1.20230609.82609/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/learning_rate_control.py` & `returnn-1.20230609.82609/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/log.py` & `returnn-1.20230609.82609/returnn/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,26 +188,14 @@
             hvd = returnn.tf.horovod.get_ctx(config=config)
             new_logs = []
             for fn in logs:
                 fn_prefix, fn_ext = os.path.splitext(fn)
                 fn_ext = ".horovod-%i-%i%s" % (hvd.rank(), hvd.size(), fn_ext)
                 new_logs.append(fn_prefix + fn_ext)
             logs = new_logs
-
-        if config.typed_value("torch_distributed") is not None:
-            import returnn.torch.distributed
-
-            torch_distributed = returnn.torch.distributed.get_ctx(config=config)
-            new_logs = []
-            for fn in logs:
-                fn_prefix, fn_ext = os.path.splitext(fn)
-                fn_ext = ".torch-distrib-%i-%i%s" % (torch_distributed.rank(), torch_distributed.size(), fn_ext)
-                new_logs.append(fn_prefix + fn_ext)
-            logs = new_logs
-
         self.initialize(logs=logs, verbosity=log_verbosity, formatter=log_format)
 
     def print_warning(self, text, prefix_text="WARNING:", extra_text=None):
         """
         Write a warning to log.v2. Does not write repeated warnings.
 
         :param str text:
```

### Comparing `returnn-1.20230609.123245/returnn/native_op.cpp` & `returnn-1.20230609.82609/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/native_op.py` & `returnn-1.20230609.82609/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/pretrain.py` & `returnn-1.20230609.82609/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/sprint/cache.py` & `returnn-1.20230609.82609/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/sprint/control.py` & `returnn-1.20230609.82609/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/sprint/error_signals.py` & `returnn-1.20230609.82609/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/sprint/extern_interface.py` & `returnn-1.20230609.82609/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/sprint/interface.py` & `returnn-1.20230609.82609/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/_dim_extra.py` & `returnn-1.20230609.82609/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/_tensor_extra.py` & `returnn-1.20230609.82609/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230609.82609/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230609.82609/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230609.82609/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/dim.py` & `returnn-1.20230609.82609/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/marked_dim.py` & `returnn-1.20230609.82609/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/tensor.py` & `returnn-1.20230609.82609/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/tensor_dict.py` & `returnn-1.20230609.82609/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tensor/utils.py` & `returnn-1.20230609.82609/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/compat.py` & `returnn-1.20230609.82609/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/data_pipeline.py` & `returnn-1.20230609.82609/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/distributed.py` & `returnn-1.20230609.82609/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/engine.py` & `returnn-1.20230609.82609/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230609.82609/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230609.82609/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/horovod.py` & `returnn-1.20230609.82609/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230609.82609/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/layers/base.py` & `returnn-1.20230609.82609/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/layers/basic.py` & `returnn-1.20230609.82609/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/layers/rec.py` & `returnn-1.20230609.82609/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/layers/segmental_model.py` & `returnn-1.20230609.82609/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/layers/signal_processing.py` & `returnn-1.20230609.82609/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/layers/variable.py` & `returnn-1.20230609.82609/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/native_op.py` & `returnn-1.20230609.82609/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/network.py` & `returnn-1.20230609.82609/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/sprint.py` & `returnn-1.20230609.82609/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/updater.py` & `returnn-1.20230609.82609/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/util/basic.py` & `returnn-1.20230609.82609/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/util/data.py` & `returnn-1.20230609.82609/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/util/ken_lm.py` & `returnn-1.20230609.82609/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/tf/util/open_fst.py` & `returnn-1.20230609.82609/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/torch/data/pipeline.py` & `returnn-1.20230609.82609/returnn/torch/data/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,18 +104,14 @@
         """
         chunking_data_keys = list(self._chunk_size.keys())
 
         for data_dict in self._dataset:
 
             if not chunking_data_keys:
                 chunking_data_keys = list(data_dict.keys())  # use all if not configured separately
-                chunking_data_key_black_list = ["seq_tag"]
-                for key in chunking_data_key_black_list:
-                    if key in chunking_data_keys:
-                        chunking_data_keys.remove(key)
                 assert chunking_data_keys, "Dataset produced sequence without any data."
 
             data_chunks = {}
             num_chunks = None
 
             for data_key in chunking_data_keys:
                 chunk_size = self._chunk_size[data_key]
```

### Comparing `returnn-1.20230609.123245/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230609.82609/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/torch/data/tensor_utils.py` & `returnn-1.20230609.82609/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/torch/engine.py` & `returnn-1.20230609.82609/returnn/torch/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,29 @@
 from __future__ import annotations
 from typing import Optional, Union, Callable, Dict
 from contextlib import nullcontext
 
 import os
 import numpy
 import torch
-import time
-from torch.distributed import init_process_group
-from torch.nn.parallel import DistributedDataParallel
 import torch.utils.data.datapipes as dp
 from torch import autocast
 from torch.cuda import amp
 from torchdata.dataloader2 import DataLoader2
 from random import random
 
 from returnn.config import Config
 from returnn.log import log
 from returnn.engine.base import EngineBase
 import returnn.frontend as rf
 from returnn.tensor import TensorDict, Tensor, Dim
 from returnn.datasets.basic import init_dataset, Dataset
 from returnn.util import basic as util
 from returnn.util import NumbersDict
-from returnn.util.basic import hms, NotSpecified
+from returnn.util.basic import NotSpecified
 from returnn.forward_iface import ForwardCallbackIface
 
 from .updater import Updater
 from .data import pipeline as data_pipeline
 from .data import returnn_dataset_wrapper
 from .frontend.bridge import rf_module_to_pt_module
 
@@ -71,26 +68,14 @@
         self._use_autocast = False
         self._autocast_dtype = None  # type: Optional[str]
         self._grad_scaler = None  # type: Optional[amp.GradScaler]
 
         self._device = _get_device_from_config(config)
         print("Using device:", self._device, file=log.v2)
 
-        self._use_torch_distributed = False
-        self._torch_distributed_class = None  # type: Optional[Callable]
-        self._torch_distributed_options = None  # type: Optional[dict]
-        self._ddp_pt_model = None  # type: Optional[torch.nn.Module]
-        self._accum_grad_multiple_step = config.int("accum_grad_multiple_step", 1)
-
-        torch_distributed = config.typed_value("torch_distributed")
-        if torch_distributed is not None:
-            self._use_torch_distributed = True
-            self._torch_distributed_class = torch_distributed.get("class", None)
-            self._torch_distributed_options = torch_distributed.get("options", None)
-
         amp_options = self.config.typed_value("torch_amp")
         grad_scaler_opts = self.config.typed_value("grad_scaler", NotSpecified)
         if amp_options is not None:
             self._use_autocast = True
             if isinstance(amp_options, dict):
                 amp_options = util.CollectionReadCheckCovered(amp_options)
                 dtype = amp_options.get("dtype", None)
@@ -141,22 +126,14 @@
         :param train_data:
         :param dev_data:
         :param eval_data:
         """
         assert config is self.config or not config
         super().init_train_from_config(config=config)
 
-        if self._use_torch_distributed:
-            import returnn.torch.distributed
-
-            torch_distributed = returnn.torch.distributed.get_ctx(config=config)
-            local_rank = torch_distributed.local_rank()
-            print(f"Start running torch distributed training on local rank {local_rank}.", file=log.v2)
-            self._device = f"cuda:{local_rank}"
-
         self.train_dataset = train_data
         self.eval_datasets.clear()
         if dev_data:
             self.eval_datasets["dev"] = dev_data
         if eval_data:
             self.eval_datasets["eval"] = eval_data
         if config.has("eval_datasets"):
@@ -170,21 +147,14 @@
         self._start_epoch = self.get_train_start_epoch(self.config)
         self._final_epoch = self.config_get_final_epoch(self.config)
 
         self.init_network_from_config(config=config)
 
         self._save_model_epoch_interval = config.int("save_interval", 1)
 
-        if self._use_torch_distributed:
-            from returnn.torch.distributed import get_device_ids
-
-            # wrap the model use torch distributed class
-            self._ddp_pt_model = self._torch_distributed_class(
-                self._pt_model, device_ids=get_device_ids(), **self._torch_distributed_options
-            )
         self._updater = Updater(self.config, self._pt_model, self.learning_rate)
         self._updater.create_optimizer()
         if self._start_epoch > 1:
             self._load_optimizer()
 
         self._train_step_func = self.config.typed_value("train_step")
         assert self._train_step_func, "train_step not defined"
@@ -228,114 +198,67 @@
         print("start", self.get_epoch_str(), "with learning rate", self.learning_rate, "...", file=log.v4)
 
         self._pt_model.train()
 
         accumulated_losses_dict = NumbersDict()
         accumulated_inv_norm_factors_dict = NumbersDict()
         step_idx = 0
-        epoch_start_time = time.time()
-
-        data_iter = iter(self._train_dataloader)
-        elapsed_computation_time = 0
-
-        while True:
-            extern_data_raw = next(data_iter, None)
-            # WARNING: torch.distributed works only for the registered device,
-            # as it uses only one mechanism for communication, like NCCL.
-            # This is suboptimal here as we have the roundtrip CPU -> GPU -> NCCL -> GPU -> CPU.
-            # TODO: Use more direct CPU -> Ethernet -> CPU communication.
-            _has_data = torch.tensor([extern_data_raw is not None], dtype=torch.int8).to(self._device)
-
-            if self._use_torch_distributed:
-                # use all reduce to check if all workers have data, if at least one worker does not have data,
-                # all workers finish this epoch
-                torch.distributed.all_reduce(_has_data, op=torch.distributed.ReduceOp.MIN)
-            if not _has_data[0]:
-                break
-
-            # clear the gradients when every gradient accumulation loop starts
-            if step_idx % self._accum_grad_multiple_step == 0:
-                self._updater.get_optimizer().zero_grad()
-
-            step_begin_time = time.time()
-
+        for extern_data_raw in self._train_dataloader:
+            self._updater.get_optimizer().zero_grad()
             extern_data = _raw_dict_to_extern_data(
                 extern_data_raw, extern_data_template=self.extern_data, device=self._device
             )
-            self._run_step(extern_data, train_flag=True, train_func=True)
+            self._run_step(extern_data, train_func=True, train_flag=True)
 
             train_ctx = rf.get_run_ctx()
-
-            # scale the loss to account for gradient accumulation
-            if self._accum_grad_multiple_step > 1:
-                for loss_name in train_ctx.losses.keys():
-                    train_ctx.losses[loss_name].loss /= self._accum_grad_multiple_step
-
             total_loss = train_ctx.total_loss()
             losses_dict = NumbersDict(
                 {
                     name: float(loss.get_summed_loss().raw_tensor.detach().cpu().numpy())
                     for name, loss in train_ctx.losses.items()
                 }
             )
             inv_norm_factors_dict = NumbersDict(
                 {name: float(_to_raw(loss.get_inv_norm_factor())) for name, loss in train_ctx.losses.items()}
             )
 
-            with self._ddp_pt_model.no_sync() if self._use_torch_distributed and (
-                step_idx % self._accum_grad_multiple_step
-            ) != (self._accum_grad_multiple_step - 1) else nullcontext():
-                if self._grad_scaler is not None:
-                    self._grad_scaler.scale(total_loss).backward()
-                else:
-                    total_loss.raw_tensor.backward()
-
-            # only update the weights when every gradient accumulation loop ends
-            if (step_idx % self._accum_grad_multiple_step) == (self._accum_grad_multiple_step - 1):
-                if self._grad_scaler is not None:
-                    self._grad_scaler.step(self._updater.get_optimizer())
-                    self._grad_scaler.update()
-                else:
-                    self._updater.get_optimizer().step()
-
-            elapsed_computation_time += time.time() - step_begin_time
+            if self._grad_scaler is not None:
+                self._grad_scaler.scale(total_loss).backward()
+                self._grad_scaler.step(self._updater.get_optimizer())
+                self._grad_scaler.update()
+            else:
+                total_loss.raw_tensor.backward()
+                self._updater.get_optimizer().step()
 
             accumulated_losses_dict += losses_dict
             accumulated_inv_norm_factors_dict += inv_norm_factors_dict
             _print_process(
                 f"ep {self.epoch} train",
                 step=step_idx,
                 eval_info=dict(losses_dict / inv_norm_factors_dict),
             )
 
             step_idx += 1
             self.global_train_step += 1
 
-        elapsed = time.time() - epoch_start_time
-        elapsed_computation_percentage = elapsed_computation_time / elapsed
-        print(
-            "Trained %i steps, %s elapsed (%.1f%% computing time)"
-            % (step_idx, hms(elapsed), (elapsed_computation_percentage * 100.0)),
-            file=log.v3,
-        )
+        print("Trained %i steps" % step_idx)
 
-        if (not self._use_torch_distributed) or (self._use_torch_distributed and torch.distributed.get_rank() == 0):
-            accumulated_losses_dict = accumulated_losses_dict / accumulated_inv_norm_factors_dict
-            self.learning_rate_control.set_epoch_error(
-                self.epoch, {f"train_loss_{k}": v for k, v in accumulated_losses_dict.items()}
-            )
-            self.learning_rate_control.save()
+        accumulated_losses_dict = accumulated_losses_dict / accumulated_inv_norm_factors_dict
+        self.learning_rate_control.set_epoch_error(
+            self.epoch, {f"train_loss_{k}": v for k, v in accumulated_losses_dict.items()}
+        )
+        self.learning_rate_control.save()
 
-            print(f"Total train loss:", _format_score(dict(accumulated_losses_dict)), file=log.v3)
+        print(f"Total train loss:", _format_score(dict(accumulated_losses_dict)), file=log.v3)
 
-            if self.epoch % self._save_model_epoch_interval == 0 or self.epoch == self._final_epoch:
-                self._save_model()
-                self._save_optimizer()
+        if self.epoch % self._save_model_epoch_interval == 0 or self.epoch == self._final_epoch:
+            self._save_model()
+            self._save_optimizer()
 
-            self.eval_model()
+        self.eval_model()
 
     def eval_model(self):
         """
         Runs model on all eval datasets and calculates the loss.
         """
         self._pt_model.eval()
 
@@ -443,21 +366,15 @@
         if train_func:
             assert self._train_step_func is not None
             rf.init_train_step_run_ctx(train_flag=train_flag)
         else:
             assert self._forward_step_func is not None, "define forward_step in the config"
             rf.init_forward_step_run_ctx(expected_outputs=self._forward_step_expected_outputs)
 
-        from returnn.torch.distributed import ddp_train_forward_ctx
-
-        with autocast(
-            device_type=self._device, dtype=self._autocast_dtype
-        ) if self._use_autocast else nullcontext(), ddp_train_forward_ctx(pt_model=self._ddp_pt_model) if isinstance(
-            self._ddp_pt_model, DistributedDataParallel
-        ) else nullcontext():
+        with autocast(device_type=self._device, dtype=self._autocast_dtype) if self._use_autocast else nullcontext():
             sentinel_kw = {"__fwd_compatible_random_arg_%i" % int(random() * 100): None}
             if train_func:
                 self._train_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
             else:
                 self._forward_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
 
     def _load_model(self):
```

### Comparing `returnn-1.20230609.123245/returnn/torch/frontend/_backend.py` & `returnn-1.20230609.82609/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/torch/frontend/_rand.py` & `returnn-1.20230609.82609/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/torch/frontend/bridge.py` & `returnn-1.20230609.82609/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/torch/updater.py` & `returnn-1.20230609.82609/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/basic.py` & `returnn-1.20230609.82609/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/better_exchook.py` & `returnn-1.20230609.82609/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/bpe.py` & `returnn-1.20230609.82609/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/debug.py` & `returnn-1.20230609.82609/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/debug_helpers.py` & `returnn-1.20230609.82609/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/fsa.py` & `returnn-1.20230609.82609/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230609.82609/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/pprint.py` & `returnn-1.20230609.82609/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/py-to-pickle.cpp` & `returnn-1.20230609.82609/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/sig_proc.py` & `returnn-1.20230609.82609/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn/util/task_system.py` & `returnn-1.20230609.82609/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/returnn.egg-info/PKG-INFO` & `returnn-1.20230609.82609/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230609.123245
+Version: 1.20230609.82609
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230609.123245/returnn.egg-info/SOURCES.txt` & `returnn-1.20230609.82609/returnn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,14 @@
 returnn/tf/util/__init__.py
 returnn/tf/util/basic.py
 returnn/tf/util/data.py
 returnn/tf/util/ken_lm.py
 returnn/tf/util/open_fst.py
 returnn/torch/README.md
 returnn/torch/__init__.py
-returnn/torch/distributed.py
 returnn/torch/engine.py
 returnn/torch/updater.py
 returnn/torch/data/__init__.py
 returnn/torch/data/pipeline.py
 returnn/torch/data/returnn_dataset_wrapper.py
 returnn/torch/data/tensor_utils.py
 returnn/torch/frontend/__init__.py
```

### Comparing `returnn-1.20230609.123245/setup.py` & `returnn-1.20230609.82609/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/DummySprintExec.py` & `returnn-1.20230609.82609/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230609.82609/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230609.82609/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/_set_num_threads1.py` & `returnn-1.20230609.82609/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/_setup_test_env.py` & `returnn-1.20230609.82609/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/bpe-unicode-demo.codes` & `returnn-1.20230609.82609/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/bpe-unicode-demo.vocab` & `returnn-1.20230609.82609/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/lexicon_opt.isyms` & `returnn-1.20230609.82609/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/lexicon_opt.jpg` & `returnn-1.20230609.82609/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/lint_common.py` & `returnn-1.20230609.82609/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/pycharm-inspect.py` & `returnn-1.20230609.82609/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/pylint.py` & `returnn-1.20230609.82609/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/returnn-as-framework.py` & `returnn-1.20230609.82609/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/rf_utils.py` & `returnn-1.20230609.82609/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/spelling.dic` & `returnn-1.20230609.82609/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_Config.py` & `returnn-1.20230609.82609/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_Dataset.py` & `returnn-1.20230609.82609/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_Fsa.py` & `returnn-1.20230609.82609/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_GeneratingDataset.py` & `returnn-1.20230609.82609/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_HDFDataset.py` & `returnn-1.20230609.82609/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_LearningRateControl.py` & `returnn-1.20230609.82609/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_Log.py` & `returnn-1.20230609.82609/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_MultiProcDataset.py` & `returnn-1.20230609.82609/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_PTDataset.py` & `returnn-1.20230609.82609/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_Pretrain.py` & `returnn-1.20230609.82609/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_ResNet.py` & `returnn-1.20230609.82609/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_SprintDataset.py` & `returnn-1.20230609.82609/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_SprintInterface.py` & `returnn-1.20230609.82609/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFEngine.py` & `returnn-1.20230609.82609/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFNativeOp.py` & `returnn-1.20230609.82609/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFNetworkLayer.py` & `returnn-1.20230609.82609/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230609.82609/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230609.82609/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFUpdater.py` & `returnn-1.20230609.82609/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TFUtil.py` & `returnn-1.20230609.82609/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TF_determinism.py` & `returnn-1.20230609.82609/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TaskSystem.py` & `returnn-1.20230609.82609/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230609.82609/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_TranslationDataset.py` & `returnn-1.20230609.82609/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_Util.py` & `returnn-1.20230609.82609/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_demos.py` & `returnn-1.20230609.82609/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_fork_exec.py` & `returnn-1.20230609.82609/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_hdf_dump.py` & `returnn-1.20230609.82609/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_array.py` & `returnn-1.20230609.82609/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_attention.py` & `returnn-1.20230609.82609/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_base.py` & `returnn-1.20230609.82609/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_cond.py` & `returnn-1.20230609.82609/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_container.py` & `returnn-1.20230609.82609/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_conv.py` & `returnn-1.20230609.82609/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_encoder_conformer.py` & `returnn-1.20230609.82609/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_loop.py` & `returnn-1.20230609.82609/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_math.py` & `returnn-1.20230609.82609/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_normalization.py` & `returnn-1.20230609.82609/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_rec.py` & `returnn-1.20230609.82609/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_reduce.py` & `returnn-1.20230609.82609/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_rf_signal.py` & `returnn-1.20230609.82609/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_tensor.py` & `returnn-1.20230609.82609/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_tools.py` & `returnn-1.20230609.82609/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_torch_engine.py` & `returnn-1.20230609.82609/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_torch_frontend.py` & `returnn-1.20230609.82609/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tests/test_torch_internal_frontend.py` & `returnn-1.20230609.82609/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/analyze-dataset-batches.py` & `returnn-1.20230609.82609/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/bliss-collect-seq-lens.py` & `returnn-1.20230609.82609/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/bliss-dump-text.py` & `returnn-1.20230609.82609/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/bliss-get-segment-names.py` & `returnn-1.20230609.82609/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/bliss-to-ogg-zip.py` & `returnn-1.20230609.82609/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/bpe-create-lexicon.py` & `returnn-1.20230609.82609/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/calculate-word-error-rate.py` & `returnn-1.20230609.82609/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/cleanup-old-models.py` & `returnn-1.20230609.82609/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/collect-orth-symbols.py` & `returnn-1.20230609.82609/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/collect-words.py` & `returnn-1.20230609.82609/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/compile_native_op.py` & `returnn-1.20230609.82609/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/compile_tf_graph.py` & `returnn-1.20230609.82609/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/debug-dump-search-scores.py` & `returnn-1.20230609.82609/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/debug-plot-search-scores.py` & `returnn-1.20230609.82609/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/dump-dataset-raw-strings.py` & `returnn-1.20230609.82609/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/dump-dataset.py` & `returnn-1.20230609.82609/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/dump-forward-stats.py` & `returnn-1.20230609.82609/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/dump-forward.py` & `returnn-1.20230609.82609/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/dump-network-json.py` & `returnn-1.20230609.82609/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/dump-pickle.py` & `returnn-1.20230609.82609/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230609.82609/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/get-attention-weights.py` & `returnn-1.20230609.82609/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/get-best-model-epoch.py` & `returnn-1.20230609.82609/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/hdf_dump.py` & `returnn-1.20230609.82609/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230609.82609/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/import-blocks-mt-model.py` & `returnn-1.20230609.82609/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/import-t2t-mt-model.py` & `returnn-1.20230609.82609/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/Makefile` & `returnn-1.20230609.82609/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/README.md` & `returnn-1.20230609.82609/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/example/README.md` & `returnn-1.20230609.82609/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230609.82609/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/file.h` & `returnn-1.20230609.82609/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/main.cc` & `returnn-1.20230609.82609/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230609.82609/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/tf_avg_checkpoints.py` & `returnn-1.20230609.82609/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/tf_inspect_checkpoint.py` & `returnn-1.20230609.82609/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/tf_inspect_summary_log.py` & `returnn-1.20230609.82609/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.123245/tools/torch_export_to_onnx.py` & `returnn-1.20230609.82609/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

